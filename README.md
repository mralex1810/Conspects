# Conspects && useful resources
ITMO CT M3138 useful resources including:

- _**Conspects**_
- Related books
- Links to recorded lections at youtube
- HomeTasks

## Supported subjects

- [Algorithms and data structures](Analgorithms)
- [Mathematical analysis](MathAnal)
- [Discrete Mathematics](DICKreteMath)
- [Computer architecture](CUMputerAAAAAAAAH)
- [Linear algebra](LinAnalgebra)

## Brief technical description 

There are two major conspect formats:
- LaTeX
- Markdown

both of them are compiled to pdf.

Latex is — through XeLaTeX compiler (its killer features were modern font support (vs. pdfLaTeX) and relatively fast compilation compared to LuaLaTeX).
And .md files are compiled to pdf by [pandoc](https://pandoc.org/).

But, unfortunately, these tools require: too much command line arguments and escaping characters, clearing temp files, providing temp files and many other additional procedures.
[latexmk](https://mg.readthedocs.io/latexmk.html) partially solves the issues, but still leaves much to be desired.

To automate those actions there are some scripts written within the framework of this repo.
Moreover, the scripts are also capable of detecting you changes (using Git API), 
committing them with proper commit messages and splitting the changes between commits wisely.


## Building && contributing instruction

- Insure you have a working latex distribution. The mainstream options are: tex-live for Linux && MacOS and MikTex for Windows.
  Note that MikTex automatically installs all required packages at compilation while tex-live requiers them to be pre-downloaded by `tlmgr` (tex-live manager) utility.
  If you experience problems with `tlmgr`'s work, visit this page: 
- Install font pack from directory `Fonts/Kurale`
- Install latexmk (via package manager on Linux or from binaries. In the second case — don't forget to install perl before…)
- Install an IDE for efficient work with latex (I've recently switched to Visual Studio Code from Texify Idea. It's a bit less clever but offers some tasty features…)
