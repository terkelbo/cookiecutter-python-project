# Standard Python Project Setup

This is a cookicutter template for a standard Python project setup which sets up a empty project the way I like to work on Python projects. The project uses `poetry` for dependency management, `tox`/`pytest` for testing, `pre-commit` for linting and formatting and `black` for formatting. It also uses mypy for static type checking and isort for import sorting.

Further it includes a VS Code settings file which is helpful when working on this type of project in VS Code.

To set up a new project run the following command:

1. `cookiecutter git@github.com:terkelbo/cookiecutter-python-project.git` (if using ssh) 
2. `cookiecutter https://github.com/terkelbo/cookiecutter-python-project.git` (if using https)

After running the command you will be prompted to enter the following values:

- `project_name`: The name of the project
- `name`: Your name
- `email`: Your email address
- `project_short_description`: A short description of the project
- `project_directory_name`: The name of the directory in which the project will be created (default value is a formatted version of `project_name`)
- `project_slug`: The slug of the project (default value is a formatted version of `project_name`)
- `python_version`: The python version to use for the project


Thereafter you can run `git init` in the project directory to initialise a git repository for the project. You can then run `make dev-setup` to set up the development environment for the project. This will install all the dependencies and set up the pre-commit hooks.
