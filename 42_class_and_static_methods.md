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
