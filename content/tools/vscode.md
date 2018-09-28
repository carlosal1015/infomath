+++
title = "Visual Studio Code"
date = 2018-09-05T17:45:05+02:00
draft = false

# Tags and categories
# For example, use `tags = []` for no tags, or the form `tags = ["A Tag", "Another Tag"]` for one or more tags.
tags = ["text editor", "desktop app"]

OS = ["apple", "windows", "linux"]

# Project summary to display on homepage.
summary = "Open-source hackable text editor, easy to use"

# Logo (or image preview) to be displayed on homepage.
logo = "tools/vscode.png"

# Optional external URL for project (replaces project detail page).
official_website = "https://code.visualstudio.com/"

selected=true

# Does the project detail page use math formatting?
math = false

# Does the project detail page use source code highlighting?
highlight = true


# Featured image
# Place your image in the `static/img/` folder and reference its filename below, e.g. `image = "example.jpg"`.
[header]
image = ""
caption = ""
+++


## Read the Documentation


[The Documentation](https://code.visualstudio.com/Docs) is exhaustive and detailed: **read the doc!** This is even more true before installing a (random) package: the functionnality you are looking for is probably in the core of vscode! At least, read the [Basic Editing](https://code.visualstudio.com/docs/editor/codebasics). For every languages or functionnality ([intellisense](https://code.visualstudio.com/docs/editor/intellisense), [debugging](https://code.visualstudio.com/docs/editor/debugging),...), the documentation also provides a list of **useful and recommended associated packages**. 


## Useful shortcuts

The full list can be accessed by doing : `ctrl` + `k` then `ctrl` + `r`. It might differs from the OS you are using :

- `ctrl` + `p` : command prompt to select file (add a `>` to use extension)
- `ctrl` + `shift` + `p` : command prompt (for extension)
- `ctrl` + `x`: cut entire line (if nothing selected)
- `ctrl` + `c`: copy entire line (if nothing selected)
- `ctrl` + `k` then `ctrl` + `c` : comment line
- `ctrl` + `k` then `ctrl` + `u` : uncomment line
- `alt` + `click` : insert new cursor
- `shift` + `alt` + `↑/↓` : insert cursor above/below
- `ctrl` + `f` : format line or multi-lines (= auto indent)

## Packages: everything you need!

We recommend the user to install only packages that have **many users** and to give priority to **recommended** packages. Here is a list of some packages that we tested (and approved!). Obviously keep the number of packages as small as possible: if you don't do C/C++, do not install the C/C++ package.

### Improved Graphical User Interface (GUI)

- [Project Manager](https://marketplace.visualstudio.com/items?itemName=alefragnani.project-manager)
- [vscode-icons](https://marketplace.visualstudio.com/items?itemName=robertohuertasm.vscode-icons)
- [Settings Sync](https://marketplace.visualstudio.com/items?itemName=Shan.code-settings-sync) : save your settings on your github account
- [Todo+](https://marketplace.visualstudio.com/items?itemName=fabiospampinato.vscode-todo-plus) : manage a TODO list
- [TODO Highlight](https://marketplace.visualstudio.com/items?itemName=wayou.vscode-todo-highlight) : highlight `TODO` and `FIXME` in a source code


### Languages

- [LaTeX Workshop](https://marketplace.visualstudio.com/items?itemName=James-Yu.latex-workshop)
- [Python](https://marketplace.visualstudio.com/items?itemName=ms-python.python)
- [C/C++](https://marketplace.visualstudio.com/items?itemName=ms-vscode.cpptools)
- [Markdown](https://code.visualstudio.com/Docs/languages/markdown) : [Markdown Lint](https://marketplace.visualstudio.com/items?itemName=DavidAnson.vscode-markdownlint), [Markdown Preview Github Styling](https://marketplace.visualstudio.com/items?itemName=bierner.markdown-preview-github-styles), [Markdown+Math](https://marketplace.visualstudio.com/items?itemName=goessner.mdmath)


