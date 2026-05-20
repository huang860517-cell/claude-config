---
name: markitdown
description: Convert various document formats (PDF, Word, Excel, PowerPoint, HTML, images, etc.) to Markdown using Microsoft's MarkItDown library
---

# MarkItDown

Convert files to Markdown for easier processing by language models.

## Usage

To convert a file to Markdown:

```bash
python -m markitdown input-file.pdf > output.md
```

Or use the `markitdown` command directly if in PATH:

```bash
markitdown input-file.docx -o output.md
```

## Supported Formats

- PDF (.pdf)
- Word (.docx)
- Excel (.xlsx)
- PowerPoint (.pptx)
- Images (EXIF metadata, OCR via magika)
- HTML
- CSV, JSON, XML
- ZIP files (iterates over contents)
- EPUB
- And more via plugins (Azure AI Document Intelligence, etc.)

## Examples

```bash
# Convert PDF to stdout
python -m markitdown document.pdf

# Convert to file
python -m markitdown document.docx -o output.md

# Use Azure Document Intelligence for better PDF parsing
python -m markitdown --use-document-intelligence document.pdf

# Pipe from stdin
cat document.html | python -m markitdown
```
