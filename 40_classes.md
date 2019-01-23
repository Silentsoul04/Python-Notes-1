
# Classes and Instances (preetha)

## Class and Instance
- Logical grouping of data and functions in a way that is easy to reuse and easy to build upon.
```
class Employee:
	pass
	
emp1 = Employee()
emp2 = Employee()
```

## Instance Variables
- These are variables that have unique values for each instance.

**Classes and Instances :**(aditya)

```python3
class Employee:
	def __init__(self,first,last):		# constructor
		self.first=first
		self.last=last
	def fullname(self):			# method
		return '{} {}'.format(self.first,self.last)

emp1=Employee('john','doe')		# instance
```
(lalith)
classes:- They allow us to logically group our data and functions in a way that's easy to reuse and also easy to build upon if needed.

method:- function that is associated with a class

class is basically a blueprint for creating instances and each unique employee that we create using our employee class in below example are the instance of that class.

Instances have different memory allocated for them.

eg:- self.first=first is similar to manually assigning like emp_1.first='name'. We can change as self.fname instead of self.first also.

![1547985394588](https://github.com/adityakuppa26/Python-Notes/tree/lalith_notes/images/1547985394588.png) 

![1547985457788](https://github.com/adityakuppa26/Python-Notes/tree/lalith_notes/images/1547985457788.png) 

![1547985520091](https://github.com/adityakuppa26/Python-Notes/tree/lalith_notes/images/1547985520091.png) 

calling methods using class name:-

![1547985629809](https://github.com/adityakuppa26/Python-Notes/tree/lalith_notes/images/1547985629809.png) 

(prvnrj)
Data and functions together bind known as class. 



class Employee():

```python
#Below thing is like a constructor and methods automatically takes in the self argument 
def __init__(self,f,l,p):
    self.fname=f
    self.lname=l
    self.salary=p
def fullname(self):
    return '{} {}'.format(self.fname,self.lname)
```

e1=Employee("Praveen","Raja",26000)

print(e1.salary)
print(e1.fullname())
print(Employee.fullname(e1))


Output:
26000
Praveen Raja
Praveen Raja

