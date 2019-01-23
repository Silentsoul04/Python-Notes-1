


# Import Modules and Standard Libraries (preetha)

- from sys.path
```
import module_name
```

- from elsewhere
``` 
sys.path.append('location')
```

- Renaming
 ```
 import module_name as alias
 ```

- importing function from a module
```
from module_name import func_name
```

- importing variable from a module
``` 
from module_name import func_name, var_name
```

## Examples
- math
> math.radians(val)
> math.sin(val)

- datetime
> datetime.date.today()

- calender
> calender.isleap(2020)

- OS
> os.getcwd() 

**Importing Modules :**  (aditya)

* Syntax :

```pytho3
import module_name 
```

* The module is first looked for in the current directory, followed by other standard library directories.
* To look at the directories which are searched :

```python3
import sys

print(sys.path)
```

* In case, the module needed isn't in the working directory, but in some other directory on the system, the path to that module must be added to the sys.path.
* It can be added either by appending to sys.path list manually, otherwise, for windows, an environment variable with name PYTHONPATH can be set up.
(lalith)
**Importing modules:-**

- the module that is to be imported and the program to which the module is to be imported should be in the same directory.

- ley my_module be the module to be imported and its code is 

  ![1547654265059](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547654265059.png)

  and the program code is 

  ![1547654313357](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547654313357.png)

- we can also import in another way as follows:-

  ![1547654384200](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547654384200.png)

  to have access to test variable:-

  ![1547654449498](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547654449498.png)

  ![1547654499386](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547654499386.png)

-  To import everything, use **from my_module import ***

- When we say import, it checks some multiple locations and the locations that it checks is within a list called sys.path

  ![1547654788170](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547654788170.png)

  /Users/coreyschafer/Demos/Python-Imports is the **current directory** that we are working on and is the first directory that is added.

  second directory that is added is the **python path environment variable**

  and then it adds **standard library directories** and finally it adds **site package directory for third party packages**. 

- If the module to be imported is not in the current directory then we can perform two things to get it imported.

  1. this method is not feasible as for a large program you need to append different locations, so we go for second method. 

     First method is shown below <!--module to be imported is on desktop-->

     ![1547655977776](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547655977776.png)

  2. This is a feasible method and it uses python path environment variables

     start->control panel->advanced system settings->environment variables->new->give variable name  <!--variable name should be PYTHONPATH as we are converting shell variable into environment variable(sys.path are initialized with PYTHONPATH plus installation dependent default. This adds the path of the folder to the sys.path for current directory--> and variable value <!--here variable value is the location of the module in desktop-->

     then open cmd and type import <module name> and it works. If you wanna check then type sys.path to check whether it is added or not.<!--see video 9 for more clarification-->

  **Importing from standard variables**

  1. example library **random** is given below:-

     output is randomly printed everytime we execute it.

     ![1547661237176](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547661237176.png)

  2. Another example is **math** library:-

     ![1547661402307](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547661402307.png)

     ![1547661436549](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547661436549.png)

  3. **datetime and calendar** library:-

     ![1547663428174](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547663428174.png)

  4. **OS library module:-**

     ![1547663529796](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547663529796.png)

     - we can get the location of a module just by printing out its thunder(**means two underscores**) file attribute.

       ![1547663714021](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547663714021.png)

     -  another example is **antigravity module**

       its code is:-

       ![1547663875224](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547663875224.png)

     - execute import antigravity in program and u can find output in **browser** as :-

       ![1547663952561](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547663952561.png)
(prvnrj)
Enumerate function:

>>> list1=["b","p","r"]
>>> 
>>> for i in enumerate(list1):
	print(i)

	
(0, 'b')
(1, 'p')
(2, 'r')
>>> for i,value in enumerate(list1):
	print(i,value)

	
0 b
1 p
2 r
>>> for i,value in enumerate(list1,100):
	print(i,value)

	
100 b
101 p
102 r


file_name.py

import file_name

variable=file_name.function_name()
variable=file_name.variable_name()

import file_name as fn

variable=fn.function_name()
variable=fn.variable_name()

from file_name import function_name,variable_name

variable=function_name()
variable=variable_name()

import random,math,datetime

random.choice()

if the files are in another directories then we are supposed to add the paths using sys.path.append()

instead we Can change the environment variable!! computer->system->advanced system settings->environment variable-> Give PYTHONPATH, And the path of the folder that resides.
