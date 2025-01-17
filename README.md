# Typst Companion

A VS Code extension that adds Markdown-like editing niceties **on top of and in addition to** to Nathan Varner's [Typst LSP](https://github.com/nvarner/typst-lsp).

## Features

- Intuitive handling of Ordered and Unordered lists in `.typ` files.
  - `Enter` while in a list context (either ordered or unordered) continues the existing list at the current level of indentation (with correct numbering, if ordered).
  - `Tab` and `Shift+Tab` while in a list context (either ordered or unordered) indents and out-dents bullets intuitively (and re-numbers ordered lists if appropriate).
  - Reordering lines inside an ordered list automatically updates the list numbers accordingly.
- Keyboard Shortcuts for:
  - Toggle Bold, Italics, and Underline (`ctrl/cmd + b|i|u`)
  - Increase and decrease header level (`ctrl/cmd + shift + ]|[`)
  - Insert a page break (`ctrl/cmd + enter`, when not in a list context)

## Requirements

I *strongly* encourage installing Nathan Varner's [Typst LSP](https://github.com/nvarner/typst-lsp) in addition to this extension for syntax highlighting, error reporting, code completion, and all of Typst LSP's other features. 
    This extension just adds some small additional features that I missed when using Typst LSP.

## Release Notes

### 0.0.4

- Added out-dent/de-dent with `enter` when cursor is at start of an empty list item.
- Added skip to next line with `ctrl/cmd + enter` when in a list context.
- Added insert a page break with `ctrl/cmd + enter` when not in a list context.


For previous versions, see the [CHANGELOG on GitHub](https://github.com/CFiggers/typst-companion/blob/main/CHANGELOG.md).

## Prior Art

The core logic of this extension is adapted, with attribution and gratitude, from [Markdown All-in-One](https://github.com/yzhang-gh/vscode-markdown/), under the following license:

MIT License, Copyright (c) 2017 张宇