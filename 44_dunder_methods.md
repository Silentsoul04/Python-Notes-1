1. ![1547995818130](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547995818130.png) 

   Depending on what objects you are working with, the addition actually has different behaviour. 

2. Special methods helps to print out something a little bit more user-friendly. By using special methods we will be able to change some of the bulit-in behaviour and operations and these are surrounded by double underscores.

3. Dunder init means init surrounded by double underscores and it is called implicitly when an instance is created. Init is the first common **special method** that people use when working with classes.

4. Other two special methods are dunder repr and dunder str. These two allow us to **change how our objects are printed and displayed.**

   repr is meant to be an unambiguous representation of the object and should be used for debugging and logging etc. It is really meant to be seen by other developers.

   str is meant to be more of a readable representation of an object and is meant to be used as a display to the end-user. 

   If we have repr and don't have str then on calling str, we will use repr as a fallback.

   without repr and str:-

   ![1547996374129](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547996374129.png) 

   with repr:-

   ![1547996394361](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547996394361.png) 

   **When we create these methods try to display something that you can copy and paste back in the python code that would recreate that same object.**

   with str:- ![1547996537693](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547996537693.png) 

   with repr and str:-

   ![1547996578474](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547996578474.png) 

   or 

   ![1547996607939](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547996607939.png)

5. special methods for arithmetic:-

   ![1547996829757](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547996829757.png) 

   print(1+2) uses special method called dunder add. 

6. adding two employee salaries:-

   ![1547996901943](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547996901943.png) 

7. Other special methods are present in documentation.

   ![1547996960120](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547996960120.png) 

   eg:-

   ![1547997002444](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547997002444.png) 

8. dunder len method for employee:-

   ![1547997046376](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547997046376.png)

   https://docs.python.org/3/reference/datamodel.html#special-method-names 

9. Real world example:-

   **return NotImplemented** is used when you don't want to throw an error because the other object might know how to handle that operation. If other object doesn't know how to handle it, then it throws an error. 

   time:-

   ![1547997322615](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547997322615.png)

   date:- 

   ![1547997408114](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547997408114.png)  

   ![1547997357010](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547997357010.png) 

   