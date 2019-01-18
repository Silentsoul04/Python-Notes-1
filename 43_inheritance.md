**Inheritance :**

```python3
class Employee:
	raise_amount=1.04
	def __init__(self,fname,lname):
		# code
	def fullname(self):
		# code

class Developer(Employee): 			# inheritance
	def __init__(self,fname,lname,lang):
		super().__init__(fname,lname)			# calls superclass constructor
		self.lang='java'
```

* Developer class inherits all the attributes and methods of the Employee class.

* If the sub and the superclass both have thne same named attributes or methods, the subclass is first looked for to find them and later the superclass.