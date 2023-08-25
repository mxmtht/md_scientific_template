# Writing a paper with Markdown

Some tips for compiling MarkDown documents to PDF with Latex citations.

## Prerequisites

Install pandoc:

```
brew install pandoc
sudo apt-get install pandoc
```

Install TeX Live:

```
brew install texlive
sudo apt-get install texlive
```

## Resources

* Resource for citation style files: https://github.com/citation-style-language
* Documentation for MarkDown and citations:
* * https://kieranhealy.org/blog/archives/2014/01/23/plain-text/
* * https://v4.chriskrycho.com/2015/academic-markdown-and-citations.html
* * https://pandoc.org/MANUAL.html#option--citeproc


## Render a file to pdf from this dir

```
pandoc in.md --citeproc  --bibliography bibliography.bib --csl=apa.csl --pdf-engine=xelatex  -o out.pdf
```
