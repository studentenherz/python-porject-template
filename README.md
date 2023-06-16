# Python Project

This template has configuration files to comply with coding style guidelines.

### Coding style guidelines

The configurations in [.editorconfig](./.editorconfig), [.flake8](./.flake8), and [pyproject.toml](./pyptoject.toml) are put in place in order to format and check compliance with [PEP 8](https://pep8.org) (with some exceptions).

[.pre-commit-config.yaml](./.pre-commit-config.yaml) defines a set of hooks to be executed right before each commit so that `black` and `flake8` are called on the changes made.

To set it up:

1. Create a virtual environment for the development.
2. Install the packages in [requirements.txt](requirements.txt):
   ```shell
   pip install -r requirements.txt
   ```
3. Install the hooks running:
   ```shell
   pre-commit install
   ```
4. Now on every `git commit` the `pre-commit` hook (inside `.git/hooks/`) will be run.
