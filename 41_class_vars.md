# Class Variables

```
class Employee:
	no_of_employees = 0
	raise_amount=1.04
	
	def __init__(self,first,last):
		self.first = first
		self.last = last
		self.email = first + '.' + last + 'oracle.com'
		self.pay = pay
		Employee.no_of_employees +=1
	
	def fullname(self):
		return '{} {}'.format(self.first,self.last)
		
```

- Here the 'raise amount' is a class variable.
- It can be accessed directly through the class or through individual instances.
- Variables like no_of_employees should be accessed through the class.
