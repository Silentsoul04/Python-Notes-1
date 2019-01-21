**Variable scope:-**determines where our variables can be accessed from within the program

**LEGB:-**local enclosing global built-in

local:-variables defined within a function

enclosing:- is enclosing our variables in local scope of enclosing functions

global:- variables which are defined at top or declared explicitly by global keyword

built-in:-names that are pre assigned in python

**Python checks in legb order for checking scope , hence the name LEGB**

1. eg 1:- local and global

   ![1547712562423](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547712562423.png)

   eg 2:-

   ![1547712694155](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547712694155.png)

   if global x is not there in function then it would have printed local x followed by global x.

   eg 3:- ![1547712806207](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547712806207.png)

   eg 4:- ![1547712913781](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547712913781.png)

   z is local variable which is passed as an argument to the function.

2. builtin:-

   **dir ** in picture below gives a list of attributes of a given object.

   eg:- ![1547713130145](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547713130145.png)

   ![1547713192491](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547713192491.png)   

   see the captions also in picture below

   ![1547713312420](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547713312420.png)

3. Enclosing:-

   It is useful for nested functions.

   eg 1:-![1547713425614](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547713425614.png)

   eg 2:- ![1547713475983](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547713475983.png)

   eg 3:- **non local statement** is used in nested functions which act as global in normal functions i.e., it helps to access variables in outer loop as shown below

   ![1547713638656](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547713638656.png)           

   **adv:-**nonlocal statements are used in decorators and closure

   4. 

   ![1547713817771](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547713817771.png)

4. ![1547713777526](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547713777526.png)

   

   