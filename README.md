# AETROS Python SDK / CLI

<p align="center">
<img src="https://avatars2.githubusercontent.com/u/17340113?v=3&s=200" />
</p>

[![Build Status](https://travis-ci.org/aetros/aetros-cli.svg?branch=master)](https://travis-ci.org/aetros/aetros-cli)
[![PyPI version](https://badge.fury.io/py/aetros.svg)](https://badge.fury.io/py/aetros)

This package is a python application you need to use when you want to train [simple models](http://aetros.com/docu/trainer/models/simple-model)
or if you want to integrate AETROS in your [python model](http://aetros.com/docu/trainer/models/custom-python) using the [AETROS Python SDK](http://aetros.com/docu/python-sdk/getting-started).

### Simple models

It basically retrieves all model information from AETROS, compiles and starts the training, attached with a special logger
callback that sends all information to AETROS Trainer so you can monitor the whole training.

It also contains dataset provider (`aetros.auto_dataset`, with downloader, generator, in-memory iterator and augmentor) for image datasets
which is used if you have a image dataset configured in AETROS Trainer.

### Python models

Please see our documentation [Python SDK: Getting started](http://aetros.com/docu/python-sdk/getting-started).

## Installation

```bash
$ sudo pip install aetros

# update
$ sudo pip install aetros --upgrade
```

### Requirement

For Simple models (where we generate the Keras code for you), you need to install Keras 1/2 and Python 2.7/3.

For Python models (where you integrate our Python SDK), you only need Python 2/3.


## Installation development version

If you want to install current master (which is recommended during the closed-beta) you need to execute:

```bash
$ git clone https://github.com/aetros/aetros-cli.git
$ cd aetros-cli
$ python setup.py install
$ aetros --help
```

You can alternatively to `git clone` download the zip at https://github.com/aetros/aetros-cli/archive/master.zip.
