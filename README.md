# KM HTML Converter

A lightweight browser-based tool that converts copied Microsoft Word content into cleaner, Salesforce Knowledge-ready HTML.

This project was built as an internal workflow support tool for Knowledge Management writers who regularly migrate or prepare documentation for Salesforce Knowledge. It helps reduce repetitive formatting cleanup by converting pasted Word content into structured HTML that can be reviewed, edited, copied, and pasted into a Salesforce Knowledge source editor.

## Why I built this

Our KM workflow often involves moving drafted or reviewed article content from Microsoft Word into Salesforce Knowledge. Copying directly from Word can bring unnecessary styling, inconsistent spacing, messy table formatting, and Word-specific markup.

This tool was created to make that handoff cleaner and faster for writers by giving them a simple way to:

* Paste copied Word content
* Convert it into cleaner HTML
* Preview the rendered output
* Review warnings for tables, images, code blocks, and formatting issues
* Edit the HTML before copying
* Copy the final HTML for Salesforce Knowledge

## What it does

* Captures rich content pasted from Microsoft Word
* Removes Word-specific styling and metadata
* Converts headings, paragraphs, lists, links, tables, notes, warnings, and code-like content into cleaner HTML
* Preserves table structures, including merged cells where possible
* Detects images and replaces them with manual insertion placeholders
* Provides a rendered preview beside the generated HTML
* Allows manual marking of selected text as code
* Shows warnings and informational messages for items that need review
* Provides a copy button for the final HTML output

## Key features

### Word-to-HTML cleanup

The converter removes unnecessary Word-generated markup and outputs cleaner HTML with consistent inline styling.

### Salesforce Knowledge-ready output

The generated HTML uses simple formatting intended for Salesforce Knowledge source code, including Arial font styling, table borders, heading hierarchy, and readable paragraph formatting.

### Table handling

The tool preserves common table structures, including header rows, empty cells, uneven rows, nested tables, and merged cells where possible.

### Warning panel

The warning panel helps writers catch items that need manual review, such as images, nested tables, uneven tables, unsafe links, or possible code blocks.

### Manual code marking

Writers can select pasted text and mark it as code before conversion, which outputs the selection as a `<pre><code>` block.

## Tech stack

* HTML
* CSS
* Vanilla JavaScript

No framework, build tool, package manager, or backend is required.

## How to use

1. Open `index.html` in a browser.
2. Copy content from Microsoft Word.
3. Paste the content into the paste area.
4. Click **Convert to HTML**.
5. Review the rendered preview.
6. Check the warnings panel for items that need manual review.
7. Edit the HTML output if needed.
8. Click **Copy HTML**.
9. Paste the HTML into the Salesforce Knowledge source editor.

## Project scope

This is a small internal productivity tool, not a full publishing system. It is designed to support a specific KM workflow: preparing cleaner HTML from Word-based article drafts for Salesforce Knowledge.

## Portfolio note

This project demonstrates practical workflow automation, documentation operations thinking, and the ability to build small tools that reduce repetitive cleanup work for a content or KM team.
