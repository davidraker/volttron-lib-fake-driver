# volttron-lib-fake-driver

![Passing?](https://github.com/VOLTTRON/volttron-lib-fake-driver/actions/workflows/run-tests.yml/badge.svg)
[![pypi version](https://img.shields.io/pypi/v/volttron-lib-fake-driver.svg)](https://pypi.org/project/volttron-lib-fake-driver/)

This project contains Drivers supported and maintained by the Volttron team.

# Prerequisites

* Python 3.8

## Python

<details>
<summary>To install Python 3.8, we recommend using <a href="https://github.com/pyenv/pyenv"><code>pyenv</code></a>.</summary>

```bash
# install pyenv
git clone https://github.com/pyenv/pyenv ~/.pyenv

# setup pyenv (you should also put these three lines in .bashrc or similar)
export PATH="${HOME}/.pyenv/bin:${PATH}"
export PYENV_ROOT="${HOME}/.pyenv"
eval "$(pyenv init -)"

# install Python 3.8
pyenv install 3.8.10

# make it available globally
pyenv global system 3.8.10
```
</details>

# Installation

Create and activate a virtual environment.

```shell
python -m venv env
source env/bin/activate
```

Install volttron and start the platform.

```shell
pip install volttron

# Start platform with output going to volttron.log
volttron -vv -l volttron.log &
```

Install the library. You have two options. You can install this library using the version on PyPi:

```shell
pip install volttron-lib-fake-driver
```

Or you can install the local version of this library from this repo:

```shell
pip install -e .
```

# Development

Please see the following for contributing guidelines [contributing](https://github.com/eclipse-volttron/volttron-core/blob/develop/CONTRIBUTING.md).

Please see the following helpful guide about [developing modular VOLTTRON agents](https://github.com/eclipse-volttron/volttron-core/blob/develop/DEVELOPING_ON_MODULAR.md)

# Documentation

To build the docs, navigate to the 'docs' directory and build the documentation:

```shell
cd docs
make html
```

After the documentation is built, view the documentation in html form in your browser.
The html files will be located in `~<path to project directory>/docs/build/html`.

ℹ️ **PROTIP: To open the landing page of your documentation directly from the command line, run the following command:**

```shell
open <path to project directory>/docs/build/html/index.html
```

This will open the documentation landing page in your default browsert (e.g. Chrome, Firefox).

# Disclaimer Notice

This material was prepared as an account of work sponsored by an agency of the
United States Government.  Neither the United States Government nor the United
States Department of Energy, nor Battelle, nor any of their employees, nor any
jurisdiction or organization that has cooperated in the development of these
materials, makes any warranty, express or implied, or assumes any legal
liability or responsibility for the accuracy, completeness, or usefulness or any
information, apparatus, product, software, or process disclosed, or represents
that its use would not infringe privately owned rights.

Reference herein to any specific commercial product, process, or service by
trade name, trademark, manufacturer, or otherwise does not necessarily
constitute or imply its endorsement, recommendation, or favoring by the United
States Government or any agency thereof, or Battelle Memorial Institute. The
views and opinions of authors expressed herein do not necessarily state or
reflect those of the United States Government or any agency thereof.
