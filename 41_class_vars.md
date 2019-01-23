# Class Variables(preetha)

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

**Class Variables :**(aditya)

* Same copy of variable for the entire class (i.e for all the instances of the class).

```python3
class Employee:
	raise_amount=1.04					# class variable
	def __init__(self,first,last):		# constructor
		self.first=first
		self.last=last
	def fullname(self):			# method
		return '{} {}'.format(self.first,self.last)
emp1=Employee('adi','kuppa')
emp2=Employee('john','doe')
print(emp1.raise_amount,emp2.raise_amount,Employee.raise_amount)	#1.04 1.04 1.04
```
