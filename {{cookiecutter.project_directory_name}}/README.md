# {{cookiecutter.project_name}}

{{cookiecutter.project_short_description}}

# Development

The project uses python {{cookiecutter.python_version}} and can be setup using the following command:

`make dev-setup`

The project is optimised for working on VS code and a settings file is included in the git repo. The project uses `black` for formatting, `pylint` for linting and `isort` for import sorting. The project also uses `pytest` for testing. The project uses `pre-commit` to run the formatting and linting checks before every commit. The project uses `poetry` for dependency management.

The project uses tox for testing. You can run the tests by running the command `tox` in the root of the project.
