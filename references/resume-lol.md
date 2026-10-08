# Editing a resume hosted on resume.lol

The editor is Markdown plus CSS rendered by paged.js inside a preview iframe, with Monaco as the editor. Models are named `<id>-resume.md`, `<id>-resume.css` and `<id>-settings.css`.

## Safety first

- **Never leave two editor tabs open on the same resume.** A stale tab autosaves over newer edits. Reload before editing, close the tab when done.
- The user may be editing at the same time. Re-read the current text immediately before applying edits, and skip any edit whose find string no longer matches rather than forcing it.

## Targeted edits

```js
const m = monaco.editor.getModels().find(x => x.uri.toString().endsWith('resume.md'));
const hits = m.findMatches(oldText, false, false, true, null, false);  // expect exactly 1
editor.pushUndoStop();
editor.executeEdits('label', hits.map(h => ({ range: h.range, text: newText })));
editor.pushUndoStop();
```

Verify after reload, not before: paged.js pagination is stale until the page reloads. Check `document.querySelectorAll('.pagedjs_page').length` inside the preview iframe, and take a screenshot if the preview has not rendered yet.

## Orphan check

A last word alone on its own line wastes a line and looks careless. Per-character `Range.getClientRects()` inside the iframe finds where each line breaks, which also confirms whether the win really lands in the first half of the first line.

## Duplicating a resume

There is no duplicate button. Copy all three models into localStorage, create a new resume through the dialog using the native input value setter plus an `input` event, switch editor tabs by dispatching pointer and mouse events, then write the content with `executeEdits`. Clear the localStorage keys afterwards.

## Exporting

"Download .zip" gives the Markdown and CSS. "Export PDF" opens the browser's own print dialog, which automation cannot drive. To produce a PDF headlessly: serialize the preview iframe's document, save it through a Blob download, then print that file with headless Chrome:

```bash
"/Applications/Google Chrome.app/Contents/MacOS/Google Chrome" --headless=new \
  --no-pdf-header-footer --virtual-time-budget=8000 \
  --print-to-pdf=out.pdf "file://$PWD/render.html"
```

Open the result and look at it before handing it over.

## Reading content back

Browser JavaScript tools may refuse to return page text containing contact details. Return counts, or strip contact lines and URLs, rather than trying to return the raw document.
