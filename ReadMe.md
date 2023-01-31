# Humphries' lab manual

Source behind the lab manual of the [Humphries lab][1],
which is hosted at:

**→ [humphries-lab.github.io/Lab-Manual][2]**

[1]: https://humphries-lab.org
[2]: https://humphries-lab.github.io/Lab-Manual


## Editing the manual

You can make edits to the lab manual straight from your browser:

1. Every page on the website contains an _edit this page_ icon (in the
   top-right-hand corner of the page, right of the main heading).
2. Clicking that icon opens the source of the page on GitHub.
   (This will be one of the markdown files in [`content/`](content))
3. Make your proposed edits, and click the green _Commit changes_ button.
4. This will open a Pull Request, for review by someone from the lab.
    - If you are a member of the _Humphries-Lab_ GitHub Organization,
      you can also directly 'commit to `main`', which will update the
      website immediately, without review.

When the PR is reviewed and merged (or when the commit to `main` is
made), the website will automatically be rebuilt (by a GitHub/Microsoft
computer), and the website will be updated after a short while.

<br>

The following is not necessary to edit the website.\
But if you'd like, you can try out changes and build the website
locally, on your own computer:


## Local live build

Make sure you have a recent-ish Python version installed and available on your PATH.\
<sub>If you haven't got Python, you can install it via e.g. `conda`, for
which I recommend the [miniforge] distribution.</sub>

[miniforge]: https://github.com/conda-forge/miniforge#download

Clone this repository, and in the root directory run:
```
pip install -r requirements.txt
```
and
```
mkdocs serve
```
This will build and serve a live-reloading version of the website at
`http://127.0.0.1:8000`.\
The server can be stopped with `Ctrl-C`.


## About

The lab manual was originally written in LaTeX by Mark,
then converted to markdown using Pandoc,
and finally wrangled into this form by Tomas Fiers.

The website is built using [mkdocs], which is a so called 'static-site
generator' (i.e. a markdown-to-html convertor), written in Python.\
It is styled with the [mkdocs material theme].\
See the documentation of those two projects for further information
on customizing more than just the content of the website.

[mkdocs]: https://www.mkdocs.org
[mkdocs material theme]: https://squidfunk.github.io/mkdocs-material
