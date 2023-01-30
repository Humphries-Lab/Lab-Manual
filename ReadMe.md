# Lab-Manual

Source behind the Lab Manual of the [Humphries Lab](https://humphries-lab.org),
which is hosted at:

→ https://Humphries-Lab.github.io/Lab-Manual

You can edit the source files on github* and the website will
automatically update after a short while.

\* {todo: explanation how: write access, PR or main}, 
<!-- If you are a member of the Humphries-Lab github organization, you can also directly 'commit to main'. -->

The following is not necessary to edit the website.\
But if you'd like, you can try out changes and build the website on your own computer too:


## Local live build

Make sure you have a recent-ish Python version installed and available on your PATH.\
<sub>If you haven't got Python, you can install it via e.g. `conda`, for which I recommend the [miniforge] distribution.</sub>

[miniforge]: https://github.com/conda-forge/miniforge#download

Clone this repository, and in the root directory run:
```
$ pip install -r requirements.txt 
$ mkdocs serve
```
This will build and serve a live-reloading version of the website at
`http://127.0.0.1:8000/`.\
The server can be stopped with `Ctrl-C`.


## About

The manual was originally written in LaTeX by Mark,
then converted to markdown using Pandoc,
and finally wrangled into this form by Tomas Fiers.

The website is built using [mkdocs], which is a so called 'static-site
generator' (i.e. a markdown-to-html convertor), written in Python.\
It is styled with the [mkdocs material theme].

[mkdocs]: https://www.mkdocs.org
[mkdocs material theme]: https://squidfunk.github.io/mkdocs-material
