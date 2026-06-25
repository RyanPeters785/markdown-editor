# Markdown Editor

A single-file, browser-based Markdown editor. No install, no server, no account. Open `markdown-editor.html` in Chrome and point it at a folder of `.md` files.

---

## Who it's for

Anyone who keeps notes, docs, or wikis as plain Markdown files and wants a clean way to read and edit them without leaving the browser — or without touching a code editor.

Good fits:

- Personal knowledge bases and note collections
- Team wikis stored in a shared folder or repo
- Project documentation you want to read rendered without a build step
- Meeting notes, journals, or any folder of `.md` files

---

## How it works

1. Open `markdown-editor.html` in Chrome
2. Click **Open folder** and pick any folder on your computer that contains `.md` files
3. Chrome remembers that folder — future visits reopen it automatically with no extra clicks

From there, click any file in the sidebar to read it rendered. Switch between **Preview**, **Split** (side-by-side source and preview), and **Edit** (raw Markdown) using the toolbar.

---

## What you can do

**Read**
Files render with full Markdown support — headings, tables, code blocks, images, and links. Links to other `.md` files in the same folder open directly in the editor.

**Edit**
The editor autosaves changes back to the original file on disk as you type. No manual save needed (though Ctrl/Cmd+S works too, and autosave can be toggled off).

**Search**
Full-text search across every file in the folder, powered by BM25 ranking. Results show a snippet with the matching terms highlighted. Click a result to jump straight to that file with the matches highlighted in the preview.

**Multiple files at once**
Each file you open gets its own tab. Switch between them freely; unsaved changes are tracked per-tab.

**Images**
Paste or drag an image directly into the editor. You'll be prompted to name it, then it's saved into an `images/` folder next to the current file and inserted as a Markdown image tag automatically. Images in the preview can be resized by dragging.

**Links**
Right-click any selected text in the editor or preview to bring up a link picker — search your open files and insert a relative Markdown link in one click.

**Undo / Redo**
Full undo history per file, with Ctrl/Cmd+Z and Ctrl/Cmd+Shift+Z. Fast typing is coalesced into single steps; discrete actions (bold, link insert) each get their own step.

**Keyboard shortcuts**
- `Ctrl/Cmd+S` — save
- `Ctrl/Cmd+B` — bold selected text
- `Ctrl/Cmd+F` — focus search
- `Tab` / `Shift+Tab` — indent / outdent (list-aware)
- `Enter` on a list item — continues the list; Enter on an empty item exits it

---

## Requirements

- **Chrome** (or any Chromium-based browser that supports the File System Access API)
- No internet connection required after the file is downloaded
- Works on Mac, Windows, and Linux

Firefox and Safari do not support the File System Access API, so saving back to disk won't work in those browsers. The editor will fall back to a download-on-save mode, or you can use **Open files** to load individual `.md` files in read-only mode.

---

## Privacy

Everything stays on your machine. No data is sent anywhere. The editor reads and writes files directly through the browser's local file system API.
