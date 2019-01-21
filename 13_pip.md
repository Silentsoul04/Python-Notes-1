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

   ![1547703257091](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547703257091.png)

10. Now if they require to install those packages using pip, then **pip install -r <file name that contains list of packages to be installed**.

    ![1547703370986](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547703370986.png)

    Then you can type pip list to check whether the packages are installed.

11. To update all of the packages, follow below picture

    ![1547703658478](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547703658478.png)

