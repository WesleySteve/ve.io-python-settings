# Python Settings

## Project objective
- Deliver a base skeleton configured to work with the Python language
  using the poetry package manager

## Necesary package
- Poetry

# WHere to find the tool
- https://python-poetry.org/

## Clone project
- $ git clone https://github.com/WesleySteve/ve.io-python-settings.git name-project
- $ git remote remove origin

## Step by step during project configuration
- 1. remove diretory .git
  - $ rm -rf .git
- 2. check poetry virtualenv
  - $ poetry config --list
- 3. configure poetry to use local virtualenv
  - $ poetry config virtualenvs.in-project true
- 4. check the configuration made
  - $ poetry config --list
- 5. modify file pyproject.toml
  - $ property packages = [{include = "python_settings"}] for name_package
- 6. start a local git repository
  - $ git init
- 7. enable poetry virtualenv
  - $ poetry shell
  - $ poetry install
- 8. install the pre-commit tool
  - $ pre-commit install
- 9. modify the name of package diretory
  - $ mv ve.io-python-Settings name-project
  - $ mv python_settings name_package
- 10. run initial tests
  -  $ task test
- 11. check the example documentation
  - $ task docs
- 12. perform the initial commit
  - $ git add .
  - $ git commit -m "Starting project"
