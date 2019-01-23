# Special Methods(preetha)

- Dunder -Double underscores
- Dunder init methods are automatically called when we create an instance.
- 
## Dunder repr() 

- unambiguous representation of the object
- used for debugging and logging

## Dunder str()

- Readable representation
- Meant to be used as display to end user.

**Special/Dunder Methods :** (aditya)

* Used for special functionality for objects and for operator overloading.

```python3
class Employee:
	def __init__(self,fname,lname):
		# code
# print(Employee('aditya','kuppa'))		<__main__.Employee object at 0x003409B0>

	def __repr__(self):					# generally used for logging, debugging
		return "Employee('{}','{}')".format(self.fname,self.lname)
# print(Employee('aditya','kuppa'))		Employee('adi','kuppa')

	def __str__(self):					# used for being more readable for users
		return "{}".format(self.fname+self.lname)
# print(Employee('aditya','kuppa'))			adityakuppa

	def __len__(self):					# overloading len()
		return len(self.fname+self.lname)
# print(len(Employee('aditya','kuppa')))		11	
```
