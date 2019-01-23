
# Virtual environment (preetha)
=======
virtual environment is used to support the various versions of the frameworks we use. It separates the various dependencies.
>>>>>>> origin/prvnrj_notes


1. Install the Virtual environment
2. Activate
3. list the packages
4. Install the necessary packages using pip commands
5. Deactivate


- to delete
> rm -rf name_of_env/

**Virtual Environments :** (aditya)

* Used to separate the packages, dependencies and the versions we would use for different projects.
* Suppose, there are different  projects using different versions of python, and updating the python globally would break down one of them, thus using virtual envs helps us maintain both versions.

```python3
virtualenv env_name : creates a virtualenv

source env_name/bin/activate : activates the virtual env

# Now we can install the packages required into this virtual env.

deactivate : deactivates the virtual env
```

(lalith)
1. Virtual env is used to separate python environments for different projects i.e. to separate out the packages dependencies and versions that you are going to use from project to project.
2. **pip install virtualenv ** to install virtual env in computer <!--if installed then ignore-->

Once u complete installing then check the video.

(prvnrj)

C:\>pip install virtualenv
Collecting virtualenv
  Downloading https://files.pythonhosted.org/packages/6a/d1/e0d142ce7b8a5c76adbfad01d853bca84c7c0240e35577498e20bc2ade7d/virtualenv-16.2.0-py2.py3-none-any.whl (1.9MB)
    100% |████████████████████████████████| 1.9MB 535kB/s
Requirement already satisfied: setuptools>=18.0.0 in c:\users\bpraja\appdata\local\programs\python\python37-32\lib\site-packages (from virtualenv) (40.6.3)
Installing collected packages: virtualenv
Successfully installed virtualenv-16.2.0

C:\>mkdir virtual

C:\>cd virtual

C:\virtual>virtualenv project1
Using base prefix 'c:\\users\\bpraja\\appdata\\local\\programs\\python\\python37-32'
New python executable in C:\virtual\project1\Scripts\python.exe
Installing setuptools, pip, wheel...
done.

C:\virtual>source project1/bin/activate
'source' is not recognized as an internal or external command,
operable program or batch file.

C:\virtual>dir
 Volume in drive C is System
 Volume Serial Number is A0D4-8FC8

 Directory of C:\virtual

01/22/2019  01:12 AM    <DIR>          .
01/22/2019  01:12 AM    <DIR>          ..
01/22/2019  01:13 AM    <DIR>          project1
               0 File(s)              0 bytes
               3 Dir(s)  141,331,042,304 bytes free

C:\virtual>cd project1

C:\virtual\project1>dir
 Volume in drive C is System
 Volume Serial Number is A0D4-8FC8

 Directory of C:\virtual\project1

01/22/2019  01:13 AM    <DIR>          .
01/22/2019  01:13 AM    <DIR>          ..
01/10/2019  03:15 PM    <DIR>          Include
01/22/2019  01:13 AM    <DIR>          Lib
01/22/2019  01:13 AM    <DIR>          Scripts
01/22/2019  01:12 AM    <DIR>          tcl
               0 File(s)              0 bytes
               6 Dir(s)  141,330,845,696 bytes free

C:\virtual\project1>cd Scripts

C:\virtual\project1\Scripts>dir
 Volume in drive C is System
 Volume Serial Number is A0D4-8FC8

 Directory of C:\virtual\project1\Scripts

01/22/2019  01:13 AM    <DIR>          .
01/22/2019  01:13 AM    <DIR>          ..
01/22/2019  01:13 AM             2,190 activate
01/22/2019  01:13 AM               759 activate.bat
01/22/2019  01:13 AM             1,544 activate.ps1
01/22/2019  01:13 AM               999 activate.xsh
01/22/2019  01:13 AM             1,512 activate_this.py
01/22/2019  01:13 AM               512 deactivate.bat
01/22/2019  01:13 AM            93,049 easy_install-3.7.exe
01/22/2019  01:13 AM            93,049 easy_install.exe
01/22/2019  01:13 AM            93,031 pip.exe
01/22/2019  01:13 AM            93,031 pip3.7.exe
01/22/2019  01:13 AM            93,031 pip3.exe
01/22/2019  01:13 AM            97,296 python.exe
01/22/2019  01:13 AM            58,896 python3.dll
01/22/2019  01:13 AM         3,638,800 python37.dll
01/22/2019  01:13 AM            95,760 pythonw.exe
01/22/2019  01:13 AM            93,027 wheel.exe
              16 File(s)      4,456,486 bytes
               2 Dir(s)  141,330,825,216 bytes free

C:\virtual\project1\Scripts>activate

(project1) C:\virtual\project1\Scripts>cd ..

(project1) C:\virtual\project1>cd ..

(project1) C:\virtual>which python
'which' is not recognized as an internal or external command,
operable program or batch file.

(project1) C:\virtual>cd ..

(project1) C:\>which python
'which' is not recognized as an internal or external command,
operable program or batch file.

(project1) C:\>cd virtual

(project1) C:\virtual>cd project1

(project1) C:\virtual\project1>which python
'which' is not recognized as an internal or external command,
operable program or batch file.

(project1) C:\virtual\project1>pip list
Package    Version
---------- -------
pip        18.1
setuptools 40.6.3
wheel      0.32.3

(project1) C:\virtual\project1>pip install numpy
Collecting numpy
  Downloading https://files.pythonhosted.org/packages/94/b5/f4bdf7bce5f8b35a2a83a0b70c545ca061a50b54724b5287505064906b14/numpy-1.16.0-cp37-cp37m-win32.whl (10.0MB)
    100% |████████████████████████████████| 10.0MB 499kB/s
Installing collected packages: numpy
Successfully installed numpy-1.16.0

(project1) C:\virtual\project1>pip install pytz
Collecting pytz
  Downloading https://files.pythonhosted.org/packages/61/28/1d3920e4d1d50b19bc5d24398a7cd85cc7b9a75a490570d5a30c57622d34/pytz-2018.9-py2.py3-none-any.whl (510kB)
    100% |████████████████████████████████| 512kB 594kB/s
Installing collected packages: pytz
Successfully installed pytz-2018.9

(project1) C:\virtual\project1>pip install psutil
Collecting psutil
  Downloading https://files.pythonhosted.org/packages/21/1e/fe6731e5f03ddf2e57d5b307f25bba294262bc88e27a0fbefdb3515d1727/psutil-5.4.8-cp37-cp37m-win32.whl (222kB)
    100% |████████████████████████████████| 225kB 388kB/s
Installing collected packages: psutil
Successfully installed psutil-5.4.8

(project1) C:\virtual\project1>deactivate
C:\virtual\project1>

