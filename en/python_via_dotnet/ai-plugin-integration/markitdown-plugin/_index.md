---
title: Aspose.Words for MarkItDown plugin
second_title: Aspose.Words for MarkItDown plugin
articleTitle: Aspose.Words for MarkItDown plugin
linktitle: Aspose.Words for MarkItDown plugin
description: "Use Aspose.Words for MarkItDown plugin for better document convertion"
type: docs
weight: 40
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /python-net/markitdown-plugin/
aliases: [/python/markitdown-plugin/]
timestamp: 2025-12-19-11-09-00
---

**Aspose.Words for MarkItDown** is a free plugin for [MarkItDown](https://github.com/microsoft/markitdown) based on [Aspose.Words for Python via .Net](https://products.aspose.com/words/python-net/) commercial library.  
The plugin is designed for parsing multiple document formats and converting them into Markdown suitable for AI processing.  
The project is located in the [GitHub repository](https://github.com/aspose-words/Aspose.Words-for-MarkItDown).  

## Features

Aspose.Words for MarkItDown supports the following features:

- Parsing new `.doc`, `.rtf`, `.odt`, `.mhtml`, `.mobi` and `.azw3` formats
- Improved conversion of `.docx`, `.pdf`, `.html`, `.epub` and `.txt` documents
- Support all document components, including paragraphs, tables, images, headers, and footers
- Fully integrated with MarkItDown tool. You don't need to change your code to use the Aspose.Words plugin

## Requirements

- [MarkItDown](https://github.com/microsoft/markitdown) version 0.1.0 or higher
- [Aspose.Words for Python via .Net](https://products.aspose.com/words/python-net/). This library is a [commercial product](https://purchase.aspose.com/buy/words/python)

You'll need to obtain valid license for Aspose.Words. The package will install this dependency, but you're responsible for complying with Aspose's licensing terms.

## How to Install Aspose.Words for MarkItDown

To install Aspose.Words MCP Server via pip, run the following:

```bash
pip install aspose-words-markitdown
```

## How to Use Aspose.Words for MarkItDown

1. Make sure the plugin is installed correctly:
  - List MarkItDown plugins with the command: `markitdown --list-plugins`
  - Check the plugin is installed:
  ```
  Installed MarkItDown 3rd-party Plugins:
    * aspose_words_markitdown  (package: aspose_words_markitdown)
  ```

2. Use the original `markitdown` CLI in the common way. Just add the `--use-plugins` option to enable the plugin.

3. Convert a Single File:
  ```bash
  markitdown test.doc -o out.md --use-plugins
  ```

4. Use Python API: 
  {{< highlight python >}}  
  from markitdown import MarkItDown  

  md = MarkItDown(enable_plugins=True) # Set to True to enable the plugin  
  result = md.convert("test.doc")  
  print(result.text_content)  
  {{< /highlight >}}  

## Aspose.Words License

{{% alert color="primary" %}}

This package is licensed under the MIT License. However, it depends on Aspose.Words for Python via .Net library, which is proprietary, closed-source library.

You must obtain valid license for Aspose.Words for Python via .Net library. This repository does not include or distribute any proprietary components.

{{% /alert %}}

To activate your Aspose.Words for Python license, set the corresponding environment variable.

Refer to the OS-specific instructions below:

**Unix-based (Linux/macOS):**
```
export ASPOSE_WORDS_LICENSE_PATH="/path/to/license/aspose.words.lic"
```

**Windows-based:**
```
set ASPOSE_WORDS_LICENSE_PATH=c:\path\to\license\aspose.words.lic
```

**Python API:**
{{< highlight python >}}  
from aspose_words_markitdown import LicenseManager

LicenseManager().apply_license("/path/to/license/aspose.words.lic")  
{{< /highlight >}}  

## How to Run Tests

To run unit tests for **Aspose.Words for MarkItDown**, follow these steps:

1. Navigate to the package directory:
  From the root of the repository, change into the package directory:
  ```bash
  cd /packages/aspose-words-markitdown/tests
  ```

2. Install test dependencies:
  Make sure `pytest` is installed:
  ```bash
  pip install pytest
  ```

3. Run all the tests using `pytest`:
  ```bash
  pytest
  ```