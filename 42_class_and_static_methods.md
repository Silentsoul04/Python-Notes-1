
# Class methods and static methods(preetha)

## Regular method

- Takes the instance as the first arguement.
- Usually, it is "self".
- Alters the members belonging to the instance of the class.

## Class methods

- Takes the class as the first arguement.
- Usually it is "cls"
- It is written using "classmethod" decorator.
- Class methods can be used as alternative constructors.

## Static methods

- They pass neither instance nor the class.
- They are logically connected to the class.
- It is created using the decorator "staticmethod".

**Class and static methods :**(aditya)

* Class methods : Class methods know about their class. They can’t access specific instance data, but they can call other static methods. Class methods don’t need **self** as an argument, but they do need a parameter called **cls**.  They can also access and modify the class variables.
* Static method : Static methods are methods that are related to a class in some way, but don’t need to access any class-specific data. You don’t have to use **self**, and you don’t even need to instantiate an instance, you can simply call your method. Static methods are great for utility functions, which perform a task in isolation. They don’t need to (and cannot) access class data. They should be completely self-contained, and only work with data passed in as arguments. 

```python3
  @staticmethod
    def some_other_function():
    print('Hello!')
 
 @classmethod
  def example_function(cls):
    """ This method is a class method! """
    print('I\'m a class method!')
    cls.some_other_function()
```
(lalith)
1. Regular methods in a class take the instance as the first argument.

2. Class method:- can access or modify state of class. It is done by using @class method and by sending class as first argument to regular methods.

   ![1547992190011](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547992190011.png) 

   cls is used by convention and we can't use class word for that.

   eg:-![1547992291241](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547992291241.png) 

   or

   ![1547992396867](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547992396867.png) 

   we can also use class methods as alternative constructors. It means we can use these methods in order to provide multiple ways of creating objects as shown below:-

   below picture is without usage of alternative constructors.

   ![1547992667019](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547992667019.png) 

   below picture is with use of alternative constructors 

   ![1547992983878](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547992983878.png)  

   We use class methods if we don't want other people to have to parse these strings everytime they want to create a new employee. So we use alternative constructors for them to pass in the string and we can create the employee for them.

   - Real world examples:-

     ![1547993075141](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547993075141.png) 

3. Static methods:- They don't have any class or instance as arguments passed into them. They are just like normal functions that have some logical connection with the class. They can't access or modify the state of the class.

   If you don't access instance or class anywhere within the function, then that method is a static method.

   ![1547993798728](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547993798728.png) 

   0=monday..... 6=sunday.

