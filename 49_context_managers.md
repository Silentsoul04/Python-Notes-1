1. **Context managers:-** allow us to properly manage resources so that we can specify exactly what we want to set up and tear down when working with certain objects. 

   eg:- in files, with is a context manager.

   ![1548011486290](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1548011486290.png) 

   it automatically closes the file.

2. we can write our own context managers  by using a class or by using functions with decorators.

   creating using class:-eg is files

   enter and exit are the setup and teardown of our context managers.

   ![1548011833885](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1548011833885.png) 

   and sample.txt is created and has Testing written in it.

   creating using function:-

   we need to import contextmanager from contextlib.

   ![1548012112387](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1548012112387.png) 

   or

   ![1548012151209](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1548012151209.png) 

3. Practical example:- for this example, we need to import os and contextmanager

   without context managers:-

   ![1548012244652](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1548012244652.png) 

   with context managers:-

   ![1548012402123](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1548012402123.png) 

   **Context managers can be used for opening and closing database connections, acquiring and releasing locks etc.**