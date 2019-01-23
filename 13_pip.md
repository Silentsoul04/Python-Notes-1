# Package Management System   (preetha)

- pip help "command"
- pip search "package name"
- pip list 
- > lists all the packages
- pip list -o
- > to check if all packages are up to date
- pip install -U
- > to upgrade
- pip freeze > requirements.txt
- > to send all the packages details for installation

**Pip Basics :** (aditya)

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
(lalith)
1. First set environment variable for pip. It is in scripts of python 37-32. Add it to **Path** environment variable.<!--If it is already set then ignore this step-->

2. Then run **pip help** command in cmd which brings out all the commands and options that you can use.

3. **pip help install** command brings up the options for install.

4. Finding a package is performed by **pip search <package name> ** and then install

   eg:- ![1547702724121](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547702724121.png)

5. **pip list** gives us all the packages installed with their versions.

6. To uninstall a package **pip uninstall <package name>** and type yes.

7. **pip list -o** or **pip list --outdated** gives the latest version available for the packages installed.

8. **pip install -U <package name>** to update and we can update one package at a time.

9. If you want to provide somebody a list of packages that they need for their project by using **freeze** command, we can send them as shown below.

   ![1547703257091](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547703257091.png)

10. Now if they require to install those packages using pip, then **pip install -r <file name that contains list of packages to be installed**.

    ![1547703370986](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547703370986.png)

    Then you can type pip list to check whether the packages are installed.

11. To update all of the packages, follow below picture

    ![1547703658478](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547703658478.png)


(prvnrj)
pip commands

pip install numpy
pip list
pip search Pympler

cat req.txt
pip install -r req.txt
pip list --outdated

