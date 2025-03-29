# Obsidian-workflow-docs
Documentation repository for Obsidian-workflow.<sup>[Codeberg](https://codeberg.org/portellam/Obsidian-workflow) | [GitHub](https://github.com/portellam/Obsidian-workflow)</sup>

## Requirements
- Python
- [MkDocs](https://www.mkdocs.org/) with the [Material theme](https://squidfunk.github.io/mkdocs-material/).
  - It has a wonderful documentation and is very customizable.

## Installation
- Run the following in a *Bash* terminal:
  - **If running on Linux,** you may need to prefix with the command `sudo`.
```bash
pip install mkdocs
pip install mkdocs-material
```

## Usage
*MkDocs* includes a live preview server, so you may preview changes as documentation is written.
The server will automatically rebuild the site upon saving.

To start the server, run:
```bash
mkdocs serve
```

When editing is complete, a static site may be built from Markdown files. To do so, run:
```bash
mkdocs build
```