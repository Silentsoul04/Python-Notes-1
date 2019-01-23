
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
