











**Pip Basics :**

* PIP is a package manager for Python packages, or modules if you like.

```pyth
pip help : lists all the commands that can be used with pip

pip install package_name : installs a package

pip uninstall package_name : uninstalls a package

pip list : lists all the installed packages

pip list -o : lists all the outdated packages

Note :

> To send a list of packages to someone, either list the packages, copy them and send them to the user, or use the freeze command as follows:

pip freeze > requirements.txt : places all the packages with their version numbers into the requirements file.

cat requirements.txt : used to view the req. file

> The receiver would install all the received list of packages using :

pip install -r requirements.txt : installs all the packages in the req. file

```
