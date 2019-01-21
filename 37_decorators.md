1. First class functions:- allow us to treat functions like any other object.

   eg:- we can pass functions as an arguments to other functions, return functions, assign functions to variables etc. 

   Closures:- allow us to take advantage of first-class functions and return an inner function that remembers and has access to variables local to the scope in which they were created.

   eg:-here message variable is free variable.![1547980913051](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547980913051.png) 

   ![1547980931986](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547980931986.png) 

   here it prints message variable several times, that is called as closure. It remembers message variable even after the outer function is finished executing.

   ![1547981168797](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547981168797.png) 

   

2. **Decorators:-** it is a function that takes functions as arguments, perform some **functionality** and returns a function.

   ![1547981412382](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547981412382.png) 

   or

   ![1547981571530](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547981571530.png) 

3. ![1547981800834](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547981800834.png) 

   when passing two functions to single decorator function, use positional and keyword arguments as shown above.

4. **classes as decorators:-**

   ![1547981921202](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547981921202.png) 

5. **Practical examples of decorators:-**

   One of the common use cases for decorators in python is logging. It maintains info regarding how many times a function is called and what are the arguments passed into that function. 

   code:-

   ![1547982530448](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547982530448.png) 

   ![1547982566257](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547982566257.png) 

   once it is executed a log file is created and it has 

   ![1547982388871](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547982388871.png) 

   

6. **Timing how long the function should run** is another use of decorator.

   eg:- 

   ![1547982597068](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547982597068.png) 

   ![1547982629013](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547982629013.png) 

7. another example:-using decorators for single function

   ![1547982716661](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547982716661.png) 

   if the order is switched then it will run as we need it.

   ![1547982757966](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547982757966.png) 

   hence it didn't print the info in log file but created a wrapper file and the info is present in that file but not in log file as in above case before switching decorators.

   ![1547982854474](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547982854474.png) 

8. watch video from 24 to 30 for another example.

