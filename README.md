# LaTeXUtils
Recurring commands and patterns I use across all my LaTeX documents.

Feel free to take what you need!
I welcome any issues or pull-requests.

## Usage
Include individual files as you need (e.g., with `\input`).
Including the main file [`LaTeXUtils.tex`](LaTeXUtils.tex) will include all utilities in [core](core) (except for [`lst.tex`](core/lst.tex) and [`tabular.tex`](core/tabular.tex)):
```tex
\input{LaTeXUtils/LaTeXUtils.tex}
```

If the you checked out this repository not next to your document but somewhere else, tell the LaTeXUtils where it lives:
```tex
\newcommand{\latexutilsdir}{relative/path/from/this/file/to/LaTeXUtils}
\input{\latexutilsdir/LaTeXUtils.tex}
```

Dependencies are documented at the top of each file.
For instance, [`abbreviations.tex`](abbreviations.tex) requires the package `xpunctuate`:
```tex
%\usepackage{xpunctuate}

\providecommand{\eg}[0]{e.g\xperiod}
\providecommand{\ie}[0]{i.e\xperiod}
...
```
