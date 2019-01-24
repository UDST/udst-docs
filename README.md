# udst-docs

This repo generates the ReadTheDocs landing page for UDST documentation.

### How it works

ReadTheDocs.org automatically builds the page defined in `docs/source/index.rst` and hosts it at udst-docs.readthedocs.io (soon docs.udst.org). Builds are triggered each time the master branch changes.

### Updating the documentation

Documentation is built using Sphinx. Here's a [good tutorial](https://pythonhosted.org/an_example_pypi_project/sphinx.html) about its markup syntax.

### Previewing changes locally

Install `sphinx` and `sphinx_rtd_theme`.

From the `docs` directory, run `sphinx-build -b html source build` to build the documentation. HTML files will show up in `docs/build/`.

These locally-generated files won't be committed to the repo; ReadTheDocs will build a separate copy when the master branch is updated.

### Hosting and troubleshooting

Hosting settings are at https://readthedocs.org/projects/udst-docs/. If you don't have access, create a ReadTheDocs account and ask one of the existing maintainers to add you.

Other UDST projects whose documentation shares the same domain are set up in ReadTheDocs as "subprojects" of this one.

