
# Property Decorators(preetha)

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
**Property Decorators (getters, setters, deleters) :**(aditya)

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
(lalith)
1. **Property Decorator:-** This allows us to give our class attributes getter, setter and deleter functionality like may have seen in some other languages.

2. eg:-

   ![1548001286718](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1548001286718.png) 

   when we first name as shown below:-

   ![1548001302532](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1548001302532.png)

    Now if you want to change mail as well, then in python we use property decorators which are similar to that of getters and setters in java.

3. Property decorator allows us to define a method that we can access it like an attribute

   eg:-**Getter:-**

   ![1548002012569](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1548002012569.png) 

4. **Setter:-**

   ![1548002254408](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1548002254408.png) 

5. **Deleter:-**

   ![1548002403680](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1548002403680.png)

