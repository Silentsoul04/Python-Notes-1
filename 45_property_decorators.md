**Property Decorators (getters, setters, deleters) :**

```python3
class Emp:
	def __init__(self,fname,lname,email):
		self.fname=fname
		self.lname=lname
		self.email=fname+'.'+lname+'@company.com'
	def fullname(self):
    	return fname+lname

emp1=Emp('aditya','kuppa')

print(emp1.first,emp1.email,emp1.fullname())	#aditya aditya.kuppa... adityakuppa

"""
this shouldn't happen, since email isn't fetched every now and then it isn't updated to the new one, to resolve this we use getters.
"""
emp1.fname='adi'

print(emp1.first,emp1.email,emp1.fullname())	#adi aditya.kuppa.... adikuppa

"""
getter :
its a method, that can be used as a property

setter:
used to set attributes from the property methods

deleter:
deletes the property and updates the related attributes.

class Emp:
	def __init__(self,fname,lname,email):
		self.fname=fname
		self.lname=lname
		self.mail=fname+'.'+lname+'@company.com'
	@property												# getter				
	def email(self):
		return "{}.{}@company.com".format(self.fname,self.lname	)
	@property
	def fullname(self):
    	return fname+' '+lname
    @fullname.setter							# setter
    def fullname(self,name):							# same name as property method
    	first,last=name.split(' ')
    	self.fname=first
    	self.lname=last
    @fullname.deleter
    	def fullname(self):
    		print('deleted')
    		self.fname=None
    		self.lname=None
emp1.fname='adi'

print(emp1.first,emp1.email,emp1.fullname)  #adi adi.kuppa... adi kuppa

emp1.fullname='kuppa aditya'
print(emp1.first,emp1.email,emp1.fullname)	#kuppa kuppa.aditya... kuppa aditya

del emp1.fullname
"""
```