[![Docs Status](https://readthedocs.org/projects/udst-docs/badge/?version=latest)](https://udst-docs.readthedocs.io)

# udst-docs

This repo generates the ReadTheDocs landing page for UDST documentation.

### How it works

ReadTheDocs.org automatically builds the page defined in `docs/source/index.rst` and hosts it at https://udst-docs.readthedocs.io (soon http://docs.udst.org). Builds are triggered each time the master branch changes.

### Updating the page

Documentation is built using Sphinx. Here's a [good tutorial](https://pythonhosted.org/an_example_pypi_project/sphinx.html). Edit `index.rst` and `conf.py` to change what appears on the page.

### Previewing changes locally

Install `sphinx` and `sphinx_rtd_theme`.

From the `docs` directory, run `sphinx-build -b html source build` to build the documentation. HTML files will show up in `docs/build/`.

The build files won't be committed to the repo; ReadTheDocs will create a separate copy when the master branch is updated.

### Hosting and troubleshooting

Hosting settings are at https://readthedocs.org/projects/udst-docs/. If you don't have access, create a ReadTheDocs account and ask one of the existing maintainers to add you.

Other UDST projects whose documentation shares the same domain are marked in ReadTheDocs as "subprojects" of this one.

