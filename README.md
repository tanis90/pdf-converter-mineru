# pdf-converter

A Claude Code skill for converting PDFs and documents using [MinerU](https://mineru.net).

## What it does

Converts PDF, images, and Office documents to Markdown, Word, HTML, LaTeX, or plain text. Also handles OCR for scanned documents and supports 80+ languages.

## Install

```bash
npx skills add tanis90/pdf-converter-mineru
```

## Usage

Just talk to Claude naturally:

- "帮我把这个PDF转成markdown"
- "What does this paper say?"
- "Extract the tables from this PDF"
- "Convert report.pdf to Word"

Claude will automatically use `mineru-open-api` to extract the document and help you with what you need.

## Two modes

| Mode | When to use | Limits |
|---|---|---|
| `flash-extract` | Quick reads, no auth needed | 10 MB / 20 pages |
| `extract` | Full fidelity, images, batch | 200 MB / 600 pages |

`flash-extract` is used by default. Run `mineru-open-api auth` to unlock `extract` mode.

## Output formats

`md`, `docx`, `html`, `latex`, `json` — specify with `-f md,docx`

## Powered by

[MinerU Open API](https://mineru.net/ecosystem?tab=cli) by [OpenDataLab](https://github.com/opendatalab/MinerU) (Shanghai AI Lab)
