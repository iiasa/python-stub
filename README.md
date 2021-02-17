# A template repo for IIASA Python projects

Copyright (c) 2021 IIASA

![License](https://img.shields.io/github/license/iiasa/python-stub)
[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)

## Overview

Template repository for creating python packages and Sphinx-based documentation pages in line with the IIASA design guidelines

## Configuration

To start a new Python package from this repo, 
click on the green **Use this template** button on top-right of this page.
Detailed instructions to create a new repository from a template can be found
[here](https://help.github.com/en/articles/creating-a-repository-from-a-template).

Then, make the following changes:

0. Change the text of the `LICENSE` file (optional).
0. Update the url in the license badge in this readme to point to the new repository.
0. Rename the folder `python_stub` to the intended package name.
0. Update the package name, author info and url in `setup.cfg`.
0. Update the package name, author info and copyright in `doc/source/conf.py`.
0. Delete the configuration section from this readme and update the title and overview section.

Make sure to commit all changes to your new repository - then program away!

## Recommendations

This package uses the [Black](https://black.readthedocs.io/) code style.
A GitHub Action workflow is configured to check that your commits conform to the style.

We recommend that you follow the [numpydoc](https://numpydoc.readthedocs.io) docstring formatting.

Looking for more ideas to include fancy modules in your package?  
Take a look at the [cookiecutter-hypermodern-python](https://github.com/cjolowicz/cookiecutter-hypermodern-python) repository!

## Installation

Install the package including the requirements for building the docs.

    pip install --editable .[doc]

## Building the docs

Navigate to the doc folder and run Sphinx.

    make --directory=doc html

The rendered html pages will be located in `doc/build/html/index.html`.
