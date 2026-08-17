<img src="docs/images/logo.svg" alt="drawing" width="250px"/>

[![Build and deploy docs](https://github.com/aeftimia/model-validation-toolkit/actions/workflows/docs.yml/badge.svg)](https://github.com/aeftimia/model-validation-toolkit/actions/workflows/docs.yml)[![PyPI version](https://img.shields.io/pypi/v/mvtk)](https://pypi.org/project/mvtk/)

# Model Validation Tookit

> This is [aeftimia](https://github.com/aeftimia)'s fork of FINRA's [Model Validation Toolkit](https://github.com/FINRAOS/model-validation-toolkit). Docs for this fork are published at <https://aeftimia.github.io/model-validation-toolkit/>.

## Installation

Run `pip install mvtk`.

**Windows users**: Until [Jaxlib is supported on windows
natively](https://github.com/google/jax/issues/438) you will need to either use
this library from a Linux subsystem or within a Docker container.
Alternatively, you can [build jaxlib from
source](https://jax.readthedocs.io/en/latest/developer.html#additional-notes-for-building-jaxlib-from-source-on-windows).

## Developers

Check out this repository and `cd` into the directory.

Run `pip install -e ".[doc]"`.

The `[doc]` is used to install dependencies for building documentation. You
will need [pandoc](https://pandoc.org/) installed.

# Submodules
You can import:

- `mvtk.credibility` for assessing credibility from sample size.
- `mvtk.interprenet` for building interpretable neural nets.
- `mvtk.thresholding` for adaptive thresholding.
- `mvtk.sobol` for Sobol sensitivity analysis
- `mvtk.supervisor` for divergence analysis
- `mvtk.metrics` for specialised metrics

# Documentation
You can run `make -C docs html` on a Mac or `make.bat -C docs html` on a PC to just rebuild the docs. In this case, point your browser to ```docs/_build/html/index.html``` to view the homepage. If your browser was already pointing to documentation that you changed, you can refresh the page to see the changes.
