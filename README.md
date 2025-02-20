Python Dev (Template)
=============================

## Description

A framework for starting a dockerized python development project with testing, jupyter and a flask API

## Working with the repo

Here's how to get set up to run the notebooks and/or code samples:

### Development machine prerequisites

The following minimum configuration should exist for development:

  * pyenv
     * pyenv install 3.13
  * poetry
  * bash

With optional:

  * docker

By convention, a data directory can be leveraged for development that is mounted as a shared volumne in Docker as /data. This has the default of $HOME/data, but can be overridden with the DATADIR environment variable.


### Development quickstart guide

* In a terminal, clone the repo and cd into the project directory.

#### Setup using docker (recommended)
```
% bin/dockerdev.sh
# poetry shell
```  

#### Setup without docker
```
% bin/start_dev.sh
% poetry shell
```  

#### Python interpreter:
```
# python
```

#### Jupyter notebook:
```
# bin/start_notebook.sh
```
* copy/paste url into browser

#### Testing & Lint:
```
# bin/run_tests.sh
# bin/run_lint.sh
```
