# Property Decorators

```
class Emp:
	def __init__(self,fname,lname,email):
		self.first = first
		self.last = last
		self.email = first+'.' + last+ '@oracle.com'
		
	def fullname(self):
		return first + last
```

- When there is a change in the name of a person then the email has to be updated. Hence for this,
```
@property
def email(self):
	return '{}.{}@oracle.com'.format(self.first,self.last)
```

​    	
