# Resume Helper (Google Docs Apps Script)

Replace the text of a single bullet point in a Google Doc while preserving the bullet/numbering, indentation, and paragraph formatting. Includes a simple sanitizer to convert pasted text into clean, single-line plain text suitable for resumes.

This README explains how to add the script to your own Google Doc and use it for resume editing or any bulleted list.

---

## What it does

- Adds a custom menu: **Resume Helper → Replace Selected Bullet…**
- Lets you place the cursor inside any bulleted or numbered line and replace only that line’s text.
- Preserves list formatting (bullet/number, indent level).
- Cleans pasted input (removes HTML, bullet glyphs, emojis, smart quotes, extra whitespace, and quotes).

---

## Prerequisites

- A Google account with access to Google Docs.
- Permission to run Apps Script in your Docs (standard for personal accounts).

No Google Cloud Project is required for the basic, bound-script usage below.

---

## Installation (Bound Script)

1. Open your target Google Doc (e.g., your resume).
2. Go to **Extensions → Apps Script** to open the Script Editor.
3. Replace any starter code with your script (see the “Code” section below).
4. Click **Save**.
5. Reload the Google Doc (or run `onOpen` once from the Script Editor to authorize).
6. You should now see a **Resume Helper** menu at the top of the Doc.

---

## Usage

1. Place your text cursor anywhere inside the bullet you want to change.
2. Click **Resume Helper → Replace Selected Bullet…**
3. A dialog shows the current bullet and asks for the new text.
4. Paste or type your replacement line and click **OK**.
5. The existing line’s text is replaced; bullet/numbering and indent are preserved.

---

## Purpose

When using ChatGPT or other generative tools to refine or optimize your resume, the output often requires additional cleanup before it can be pasted into Google Docs. Formatting issues such as unwanted quotation marks, bullet symbols, emojis, or extra whitespace can disrupt the consistency of your document. This add-on streamlines that process by allowing you to quickly replace a selected bullet point with sanitized text, ensuring your resume maintains a professional, uniform format with minimal manual editing.
