How to set up a virtual environment and requirements for a python project

#####

1. Set up the virtual environment (this is used to install requiements on the environment without installing on the entire machine)

- run: pip -m venv .venv (the name is usually .venv, but whateer is used needs to be configured to the right path in vscode env settings)
- To activate, navigate to /.venv/bin and run: source activate
- To deactivate, run: deactivate
- To select the venv as the current python interpreter, press COMMAND+SHIFT+P, search for Python:Select Interpreter and choose venv

#####

2. Set up the requirements

- create a new file called <requirements.txt> in the same directory as the .py files

- To freeze the current requirements and display them in requirements.txt file, run: pip freeze > requirements.txt
- To install all the listed modules in the environment, run: pip install -r requirements.txt

- To uninstall a package, use the same command but with the uninstall keyword instead.
- To upgrade an existing module, use the same command but with the upgrade keyword.

- To output a list of outdated packages, run: pip list --outdated
- To update all packages, run: pip install -U -r requirements.txt

#####

3. Run the Flask App

! If flask could not be resolved, press COMMAND+SHIFT+P, search for Python:Select Interpreter and choose venv

- In a terminal, run: python3 app.py (or name of main python file)
- Press CTRL+C to quit
