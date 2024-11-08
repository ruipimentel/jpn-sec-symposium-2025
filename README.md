# How to compile

Last time I tried, Overleaf couldn't be used because the compiler options (pdfLaTeX, LaTeX, XeLaTeX, LuaLaTeX) didn't include the necessary one (pLaTeX/pLaTeX2e).

The easiest way to compile is installing the following tools, then following the recommended compilation procedure.

## Necessary tools

* [TeX Live](https://www.tug.org/texlive/quickinstall.html)

## Recommended tools
* [Visual Studio Code](https://code.visualstudio.com/download)
* [LaTeX-Workshop](https://github.com/James-Yu/LaTeX-Workshop/wiki/Install) extension for VS Code

## Basic compilation procedure (recommended)

After installing the tools above, simply open the TEX file in VS Code (file has to be open for extension tab to appear), then use the LaTeX Workshop tab to execute the recipe (provided in the `settings.json` file).

## Basic compilation procedure (manual)

```
platex symposium.tex
bibtex symposium.aux
platex symposium.tex
platex symposium.tex
dvipdfmx symposium.dvi
```
