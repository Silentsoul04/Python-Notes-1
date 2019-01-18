**Class Variables :**

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