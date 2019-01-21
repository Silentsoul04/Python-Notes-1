# Inheritance

- A class in python can inherit attributes and methods from another class called superclass.

```
class Employee:

	raise_amount=1.04
	
	def __init__(self,first,last):
		self.first = first
		self.last = last
		self.email = first + '.' + last + 'oracle.com'
		self.pay = pay
		
	def fullname(self):
		return '{} {}'.format(self.first,self.last)

class Developer(Employee): 			
	def __init__(self,first,last,prog_lang):
		super().__init__(first,last)
		self.prog_lang='java'
```

- Here, Developer is a subclass that inherits from the superclass Employee.
- The init in Developer directly calls the init in the superclass.
- For any member of a subclass, first the subclass is searched and if not found, then superclass is searched.
- The superclass is enclosed in () after the subclass name.