1. Inheritance allows us to inherit attributes and methods from a parent class. This is useful because we can create sub classes and get all the functionality of parent class, then we can overwrite or add completely new functionality without affecting parent class in any way.

2. code:-

   ![1547994091655](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547994091655.png) 

   o/p:-

   ![1547994114213](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547994114213.png) 

   method resolution order:-First checks in the specified class that is instantiated. If it doesn't find then it goes to parent class. This chain is called method resolution order.

3. help function helps in visualizing method resolution order as shown below:-

   ![1547994338979](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547994338979.png) 

   o/p:-

   ![1547994353832](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547994353832.png) 

4.  ![1547994469061](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547994469061.png) 

   ![1547994532305](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547994532305.png) 

   ![1547994547146](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547994547146.png) 

   see the difference between above two pictures.

5. super().init allows employee class to handle first last and pay arguments. super() is used to refer to parent class.

   Instead of super, we can directly use parent class as shown below

   ![1547994786528](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547994786528.png) 

   For single inheritance, super() is better and for multiple inheritance usage of parent class is better

   entire example of developer class is:-

   ![1547994889255](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547994889255.png) 

6. Manager subclass:-

   ![1547995023537](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547995023537.png) 

   for initialization use lists or dictionaries only as in the above case(self.employees=[])

   execution code and o/p:-

   ![1547995182055](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547995182055.png) 

7. isinstance()-tells us if an object is an instance of a class

   ![1547995313693](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547995313693.png)

   ![1547995300702](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547995300702.png)

   ![1547995262099](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547995262099.png) 

8. issubclass()-tells us whether it is a subclass or not.

   ![1547995443615](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547995443615.png) 

   **Real world example:-** Exception module of python whisky library

   ![1547995490470](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547995490470.png) 

   ![1547995503771](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547995503771.png) 

   