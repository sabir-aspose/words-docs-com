---
title: Aspose.Words MCP Server
second_title: Aspose.Words for Python via .NET
articleTitle: Aspose.Words MCP Server
linktitle: Aspose.Words MCP Server
description: "A Model Context Protocol (MCP) server that exposes Aspose.Words for Python via .NET features as callable tools for AI/assistant clients."
type: docs
weight: 70
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /python-net/aspose-words-mcp-server/
aliases: [/python/aspose-words-mcp-server/]
timestamp: 2025-12-17-21-09-00
---

Aspose.Words MCP Server is an MCP (Model Context Protocol) server built on top of [Aspose.Words for Python via .NET](/words/python-net/). It automates Microsoft Word document creation and editing and exposes operations as MCP tools that any MCP‑compatible client can call.

Repository: https://github.com/aspose-words/Aspose.Words-MCP-Server

Supported transports: `stdio`, `streamable-http`, `sse`.

### Features

- Create documents; read/write text, headings, and paragraphs
- Text formatting (font, size, style, color, underline)
- Page and section breaks; page setup (margins, orientation, paper size, columns)
- Lists (bulleted/numbered)
- Tables: create, auto-fit, merge cells, alignment, shading, paddings, column widths, header styling
- Footnotes and endnotes: add, convert, anchor-based operations, validation
- Comments: get by author, by paragraph, all comments
- Document properties: read/write (title, author, subject, keywords)
- Protection: protect/unprotect, partial editing restrictions
- Bookmarks, hyperlinks
- Watermarks (text/image)
- Export as Base64 (DOCX, PDF, etc.), advanced export options
- Render page to image (PNG, etc.)
- In-memory document management: copy, save as, list, delete, merge

### Installation

```bash
pip install aspose-words-mcp
```

From source:

```bash
git clone https://github.com/aspose-words/Aspose.Words-MCP-Server
cd Aspose.Words-MCP-Server
pip install -r requirements.txt
```

### Running the Server

CLI command after installation:

```bash
aspose-words-mcp
```

Run without installation:

```bash
python mcp_server.py
```

By default, the server runs with the `stdio` transport.

Supported transports and environment variables:

- `MCP_TRANSPORT` — `stdio` | `streamable-http` | `sse` (default `stdio`)
- `MCP_HOST` — host address (default `0.0.0.0`)
- `MCP_PORT` — port (default `8080`)
- `MCP_PATH` — HTTP path for `streamable-http` (default `/mcp`)
- `MCP_SSE_PATH` — events path for `sse` (default `/sse`)
- `LOG_LEVEL` — logging level (`INFO`, `DEBUG`, ...)

HTTP/SSE example:

```bash
export MCP_TRANSPORT=streamable-http   # or sse
export MCP_HOST=0.0.0.0
export MCP_PORT=8080
export MCP_PATH=/mcp                   # for streamable-http
export MCP_SSE_PATH=/sse               # for sse
aspose-words-mcp
```

On start, the server prints the listening address.

### Aspose.Words License

The Aspose.Words license is applied on server startup. The path is resolved with the following precedence:

1) `license_path` argument of `run_server(..., license_path=None)`
2) `ASPOSE_WORDS_LICENSE_PATH` environment variable

If no license is provided or the file is not accessible, the server runs in Evaluation mode.

Example:

```bash
export ASPOSE_WORDS_LICENSE_PATH='/path/to/aspose.words.lic'
```

### Tools Overview

Tool categories exposed by the server include:

- Content/reading: create document, insert/delete/read text, headings, lists, HTML/Markdown
- Layout: pages, breaks, columns, headers/footers, page numbering
- Tables: create and format tables
- Watermarks: text and image watermarks
- Links/bookmarks: hyperlinks and bookmarks
- Properties: document properties
- Protection: protection and restrictions
- Comments/notes: comments, footnotes/endnotes
- Export/render: export to formats and page rendering

For signatures and details, see the server source and tests in the repository (`mcp_server.py`, `tests/features/*`).

### Integration

- Claude Desktop MCP: add this server with `streamable-http` or `sse` transport and the URL printed by the server at startup.
- Any MCP (JSON) clients — configure the matching transport and path.

### Licensing Notes

This package is MIT‑licensed, but it depends on Aspose.Words for Python via .NET, which is a proprietary product. You must obtain a valid Aspose.Words license to use it beyond evaluation limitations. See [Aspose.Words for Python via .NET](/words/python-net/) and [purchase options](https://purchase.aspose.com/buy/words/python).
