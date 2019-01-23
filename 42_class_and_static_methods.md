# Class methods and static methods(preetha)

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

(prvnrj)
Regular method automatically takes the argument self.
class method takes the arguments instance of the class(automatically).
static method takes no arguments




class Employee():
    number_of_employees=0
    amount_raise=1.04
    #Below thing is like a constructor and self is the most important argument 
    def __init__(self,f,l,p):
        self.fname=f
        self.lname=l
        self.salary=p

```python
    Employee.number_of_employees+=1
def fullname(self):
    return '{} {}'.format(self.fname,self.lname)
def raise_amount(self):
    self.salary=int(self.salary * self.amount_raise)

@classmethod
def finalraise(cls,amt):
    cls.amount_raise=amt
```


​        
#print(Employee.number_of_employees)
e1=Employee("Praveen","Raja",26000)
#print(Employee.number_of_employees)

Employee.finalraise(2.03)
#e1.finalraise(2.03) or
print(Employee.amount_raise)

print(e1.amount_raise)
#print(e1.salary)
#e1.raise_amount()
#print(e1.salary)


#print(e1.__dict__)

Output:

2.03
2.03




class Employee():
    number_of_employees=0
    amount_raise=1.04
    #Below thing is like a constructor and self is the most important argument 
    def __init__(self,f,l,p):
        self.fname=f
        self.lname=l
        self.salary=p

```python
    Employee.number_of_employees+=1
def fullname(self):
    return '{} {}'.format(self.fname,self.lname)
def raise_amount(self):
    self.salary=int(self.salary * self.amount_raise)

@classmethod
def finalraise(cls,amt):
    cls.amount_raise=amt

@classmethod
def convert(cls,string):
    f,l,p=string.split("-")
    return cls(f,l,p)

@staticmethod
def is_day(day):
    if day.weekday()==1 or day.weekday()==2:
        return False
    return True
```

#print(Employee.number_of_employees)
e1=Employee("Praveen","Raja",26000)
#print(Employee.number_of_employees)

Employee.finalraise(2.03)
#e1.finalraise(2.03) or
#print(Employee.amount_raise)

#print(e1.amount_raise)
#print(e1.salary)
#e1.raise_amount()
#print(e1.salary)
#print(e1.__dict__)

emp_string="Nikki-Varma-72000"
e2=Employee.convert(emp_string)

import datetime

day=datetime.date(2019,1,18)
print(Employee.is_day(day))
