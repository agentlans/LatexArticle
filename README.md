# LatexArticle
Cookiecutter template for a Latex article with
- ams packages and shortcuts
- lmodern and microtype
- block comments
- biblatex

TeX files are compiled with pdflatex.

## Install and Use
Required:
- [cookiecutter](https://www.cookiecutter.io/) package
- the Latex packages and programs listed above

On the command line, run `cookiecutter gh:agentlans/LatexArticle`

Cookiecutter will ask you questions like these to customize your template.
```
full_name [Professor James Moriarty]: 
title [A Treatise on the Binomial Theorem]: 
project_slug [ATreatiseontheBinomialTheorem]: 
bibliography [y]: 
bib_file [example.bib]: 
hide_page_num [y]: 
date [Date]: 
```

Then enter the directory `ATreatiseontheBinomialTheorem`
(or your project's name). Either run:
- `make` to create the PDF file
- `make view` to create the PDF file and open a viewer
  - (requires Evince installed, which is part of GNOME desktop)

## Author and Licence

LatexArticle by Alan Tseng is licensed under the Creative Commons CC0 1.0 Universal License.
