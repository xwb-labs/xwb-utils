XWB Utilities
=============================

## Description

General data structures, algorithms, and utilities for DS, AI, ML, and NLP.


## General project information

The purpose of this project is:

  * To support delivering a robust DS/AI/ML/NLP utilities library package.
  * To facilitate interactive development, demonstration, visualization, and testing of the library components via jupter notebooks and/or scripts.


## License

XWB Utilities (xwb-utils) are released under the terms of the MIT License. You may find the content of the license [here](http://opensource.org/licenses/MIT), or inside the LICENSE file.

## Packaged utilities

  * xwb_utils.Tree -- A simple generic tree data structure

## Development

### Development machine prerequisites

The following minimum configuration should exist for development:

  * miniconda
  * poetry
  * tox

With optional:

  * docker
  * bash

By convention, a data directory can be leveraged for development that is mounted as a shared volumne in Docker as /data. This has the default of $HOME/data, but can be overridden with the DATADIR environment variable.


### Development quickstart guide

  * In a terminal, clone the repo and cd into the project directory.

#### Using virtual environments

  * Development:
    * Manual: source ".project_vars", poetry install, poetry shell
    * Automated: execute "bin/start_dev.sh"  (requires "/bin/bash" on your machine)

  * Notebook:
    * execute "bin/start_notebook.sh"
      * copy/paste url into browser

#### Using docker

  * Development:
    * execute "tox -e dev"

  * Notebook:
    * execute "tox -e nb"
      * copy/paste url into browser
