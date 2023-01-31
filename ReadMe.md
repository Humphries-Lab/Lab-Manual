# Humphries' lab manual

Source behind the lab manual of the [Humphries lab][1],
which is hosted at:

**→ [humphries-lab.github.io/Lab-Manual][2]**

[1]: https://humphries-lab.org
[2]: https://humphries-lab.github.io/Lab-Manual


## Editing the manual

You can make edits to the lab manual straight from your browser:

1. Every page on the website contains an _edit this page_ icon (in the
   top-right-hand corner of the page, to the right of the main heading).
2. Clicking that icon opens the source of the page on GitHub.
   (This will be one of the markdown files in [`content/`](content))
3. Make your proposed edits, and click the green _Commit changes_ button.
4. This will open a _Pull Request_ (PR), for review by someone from the lab.
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

[Clone] this repository, and in its root directory, [run]:
```
pip install -r requirements.txt
```
and
```
mkdocs serve
```
This will build and serve a live-reloading version of the website at
http://127.0.0.1:8000 \
The server can be stopped with `Ctrl-C`.


[miniforge]: https://github.com/conda-forge/miniforge#download
[Clone]: https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository
[run]: https://www.twilio.com/docs/usage/tutorials/a-beginners-guide-to-the-command-line


## About

The lab manual was originally written in LaTeX by Mark Humphries, and
was converted to the current editable-website form by
[Tomas Fiers](https://tomasfiers.net).

The website is built using [MkDocs], which is a so called 'static-site
generator' (i.e. a markdown-to-html convertor), written in Python.\
It is styled with the [mkdocs-material] theme.

MkDocs and mkdocs-material are configured using the
[`mkdocs.yml`](mkdocs.yml) YAML file in the root directory. It defines
which pages are included (and in which order), what goes in the website
footer, which plugins are enabled, etc.

On every commit to the `main` branch on GitHub, the [GitHub Actions] 'workflow'
defined in [`.github/workflows/build.yml`][CI] starts, which runs
`mkdocs, and commits the resulting HTML, CSS, and Javascript files to
the [`gh-pages`] branch, which is what is visible on the website.

For more on how to customize the website (beyond just editing its
content) please see the documentation [of MkDocs][3] and 
[mkdocs-material][4].\
Those resources are also useful when you're wondering how to achieve
a particular effect with the particular markdown syntax used here.

[MkDocs]: https://www.mkdocs.org
[mkdocs-material]: https://squidfunk.github.io/mkdocs-material
[GitHub Action]: https://docs.github.com/en/actions
[CI]: github/workflows/build.yml
[`gh-pages`]: https://github.com/Humphries-Lab/Lab-Manual/tree/gh-pages
[3]: https://www.mkdocs.org/user-guide/
[4]: https://squidfunk.github.io/mkdocs-material/creating-your-site/#advanced-configuration
