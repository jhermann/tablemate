# tablemate

Prettify your tabular data, either on the command line or in Python code.

 [![Travis CI](https://api.travis-ci.org/jhermann/tablemate.svg)](https://travis-ci.org/jhermann/tablemate)
 [![Coveralls](https://img.shields.io/coveralls/jhermann/tablemate.svg)](https://coveralls.io/r/jhermann/tablemate)
 [![GitHub Issues](https://img.shields.io/github/issues/jhermann/tablemate.svg)](https://github.com/jhermann/tablemate/issues)
 [![License](https://img.shields.io/pypi/l/tablemate.svg)](https://github.com/jhermann/tablemate/blob/master/LICENSE)
 [![Development Status](https://pypip.in/status/tablemate/badge.svg)](https://pypi.python.org/pypi/tablemate/)
 [![Latest Version](https://img.shields.io/pypi/v/tablemate.svg)](https://pypi.python.org/pypi/tablemate/)
 [![Download format](https://pypip.in/format/tablemate/badge.svg)](https://pypi.python.org/pypi/tablemate/)
 [![Downloads](https://img.shields.io/pypi/dw/tablemate.svg)](https://pypi.python.org/pypi/tablemate/)


## Overview

…


## Installation

*Tablemate* can be installed via ``pip install tablemate`` as usual,
see [releases](https://github.com/jhermann/tablemate/releases) for an overview of available versions.
To get a bleeding-edge version from source, use these commands:

```sh
repo="jhermann/tablemate"
pip install -r "https://raw.githubusercontent.com/$repo/master/requirements.txt"
pip install -UI -e "git+https://github.com/$repo.git#egg=${repo#*/}"
```

See [Contributing](#contributing) on how to create a full development environment.

To add bash completion, read the [Click docs](http://click.pocoo.org/4/bashcomplete/#activation) about it,
or just follow these instructions:

```sh
cmdname=tablemate
mkdir -p ~/.bash_completion.d
_$(tr a-z- A-Z_ <<<"$cmdname")_COMPLETE=source $cmdname >~/.bash_completion.d/$cmdname.sh
grep /.bash_completion.d/$cmdname.sh ~/.bash_completion >/dev/null \
    || echo >>~/.bash_completion ". ~/.bash_completion.d/$cmdname.sh"
. "/etc/bash_completion"
```


## Usage

…


## Contributing

To create a working directory for this project, call these commands:

```sh
git clone "https://github.com/jhermann/tablemate.git"
cd "tablemate"
. .env --yes --develop
invoke build --docs test check
```

See [CONTRIBUTING](https://github.com/jhermann/tablemate/blob/master/CONTRIBUTING.md) for more.


## References

**Tools**

* [Cookiecutter](http://cookiecutter.readthedocs.org/en/latest/)
* [PyInvoke](http://www.pyinvoke.org/)
* [pytest](http://pytest.org/latest/contents.html)
* [tox](https://tox.readthedocs.org/en/latest/)
* [Pylint](http://docs.pylint.org/)
* [twine](https://github.com/pypa/twine#twine)
* [bpython](http://docs.bpython-interpreter.org/)
* [yolk3k](https://github.com/myint/yolk#yolk)

**Packages**

* [Rituals](https://jhermann.github.io/rituals)
* [Click](http://click.pocoo.org/)


## Acknowledgements

…
