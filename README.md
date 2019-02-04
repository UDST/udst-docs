[![Docs Status](https://readthedocs.org/projects/udst-docs/badge/?version=latest)](https://udst-docs.readthedocs.io)

# udst-docs

This repo generates the landing page for UDST documentation, hosted at https://docs.udst.org and https://udst-docs.readthedocs.io.

### How it works

ReadTheDocs.org builds and hosts the Sphinx page defined in `docs/source/index.rst`. Builds are triggered when the master branch of this Github repo changes.

### Updating the landing page

The page is built using the Sphinx documentation generator. Here's a [good tutorial](https://pythonhosted.org/an_example_pypi_project/sphinx.html). Edit `index.rst` and `conf.py` to change what appears on the page.

### Previewing changes locally

Install `sphinx` and `sphinx_rtd_theme`.

From the `docs` directory, run `sphinx-build -b html source build` to build the documentation. HTML files will show up in `docs/build/`.

The build files won't be committed to the repo; ReadTheDocs will create a separate copy when the master branch is updated.

### Hosting and troubleshooting

Hosting settings are at https://readthedocs.org/projects/udst-docs/. If you don't have access, create a ReadTheDocs account and ask one of the existing maintainers to add you.

The DNS settings for the docs.udst.org subdomain contain a CNAME record redirecting traffic to readthedocs.io. ReadTheDocs handles the SSL certificate for https. 

Other UDST projects whose documentation uses this domain (e.g. [ChoiceModels](https://docs.udst.org/projects/choicemodels/en/latest)) have to be marked in ReadTheDocs as "subprojects" of the landing page.
