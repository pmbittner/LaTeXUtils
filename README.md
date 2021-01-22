# LaTeXUtils
Recurring commands and patterns I use across all my LaTeX documents.

Feel free to take what you need!

## Usage
Include individual files as you need (e.g., with `\input` or `\include`).
Including the main file [`LaTeXUtils.tex`](LaTeXUtils.tex) will include all utilities in [core](core):
```tex
\input{LaTeXUtils/LaTeXUtils.tex}
```

If the you checked out this repository not next to your document but somewhere else, tell the LaTeXUtils where it lives:
```tex
\newcommand{\latexutilsdir}{relative/path/from/this/file/to/LaTeXUtils}
\input{\latexutilsdir/LaTeXUtils.tex}
```
