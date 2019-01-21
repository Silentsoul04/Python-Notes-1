**Classes and Instances :**

```python3
class Employee:
	def __init__(self,first,last):		# constructor
		self.first=first
		self.last=last
	def fullname(self):			# method
		return '{} {}'.format(self.first,self.last)

emp1=Employee('john','doe')		# instance
```