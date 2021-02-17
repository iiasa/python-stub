# A template repo for IIASA Python projects

Copyright (c) 2021 IIASA

![GitHub](https://img.shields.io/github/license/iiasa/python-stub)

## Overview

Template repository for creating python packages and Sphinx-based documentation pages in line with the IIASA design guidelines

## Configuration

To start a new Python package from this repo, 
click on the green **Use this template** button on top-right of this page.
Detailed instructions to create a new repository from a template can be found
[here](https://help.github.com/en/articles/creating-a-repository-from-a-template).

Then, make the following changes:

0. Change the text of the `LICENSE` file and the badge in this readme (optional).
1. Rename the folder `python_stub` to the intended package name.
2. Update the package name, author info and url in `setup.cfg`.
3. Update the package name, author info and copyright in `doc/source/conf.py`.
4. Delete the configuration section from this readme and update the title and overview section.

Make sure to commit all changes to your new repository - then program away!

## Installation

Install the package including the requirements for building the docs.

    pip install -e .[doc]

## Building the docs

Navigate to the doc folder and run Sphinx.

    cd doc
    make html

The rendered html pages will be located in `doc/build/html/index.html`.
