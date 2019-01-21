**Importing modules:-**

- the module that is to be imported and the program to which the module is to be imported should be in the same directory.

- ley my_module be the module to be imported and its code is 

  ![1547654265059](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547654265059.png)

  and the program code is 

  ![1547654313357](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547654313357.png)

- we can also import in another way as follows:-

  ![1547654384200](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547654384200.png)

  to have access to test variable:-

  ![1547654449498](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547654449498.png)

  ![1547654499386](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547654499386.png)

-  To import everything, use **from my_module import ***

- When we say import, it checks some multiple locations and the locations that it checks is within a list called sys.path

  ![1547654788170](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547654788170.png)

  /Users/coreyschafer/Demos/Python-Imports is the **current directory** that we are working on and is the first directory that is added.

  second directory that is added is the **python path environment variable**

  and then it adds **standard library directories** and finally it adds **site package directory for third party packages**. 

- If the module to be imported is not in the current directory then we can perform two things to get it imported.

  1. this method is not feasible as for a large program you need to append different locations, so we go for second method. 

     First method is shown below <!--module to be imported is on desktop-->

     ![1547655977776](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547655977776.png)

  2. This is a feasible method and it uses python path environment variables

     start->control panel->advanced system settings->environment variables->new->give variable name  <!--variable name should be PYTHONPATH as we are converting shell variable into environment variable(sys.path are initialized with PYTHONPATH plus installation dependent default. This adds the path of the folder to the sys.path for current directory--> and variable value <!--here variable value is the location of the module in desktop-->

     then open cmd and type import <module name> and it works. If you wanna check then type sys.path to check whether it is added or not.<!--see video 9 for more clarification-->

  **Importing from standard variables**

  1. example library **random** is given below:-

     output is randomly printed everytime we execute it.

     ![1547661237176](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547661237176.png)

  2. Another example is **math** library:-

     ![1547661402307](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547661402307.png)

     ![1547661436549](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547661436549.png)

  3. **datetime and calendar** library:-

     ![1547663428174](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547663428174.png)

  4. **OS library module:-**

     ![1547663529796](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547663529796.png)

     - we can get the location of a module just by printing out its thunder(**means two underscores**) file attribute.

       ![1547663714021](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547663714021.png)

     -  another example is **antigravity module**

       its code is:-

       ![1547663875224](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547663875224.png)

     - execute import antigravity in program and u can find output in **browser** as :-

       ![1547663952561](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547663952561.png)