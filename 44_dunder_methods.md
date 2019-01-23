
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
(lalith)
1. ![1547995818130](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547995818130.png) 

   Depending on what objects you are working with, the addition actually has different behaviour. 

2. Special methods helps to print out something a little bit more user-friendly. By using special methods we will be able to change some of the bulit-in behaviour and operations and these are surrounded by double underscores.

3. Dunder init means init surrounded by double underscores and it is called implicitly when an instance is created. Init is the first common **special method** that people use when working with classes.

4. Other two special methods are dunder repr and dunder str. These two allow us to **change how our objects are printed and displayed.**

   repr is meant to be an unambiguous representation of the object and should be used for debugging and logging etc. It is really meant to be seen by other developers.

   str is meant to be more of a readable representation of an object and is meant to be used as a display to the end-user. 

   If we have repr and don't have str then on calling str, we will use repr as a fallback.

   without repr and str:-

   ![1547996374129](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547996374129.png) 

   with repr:-

   ![1547996394361](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547996394361.png) 

   **When we create these methods try to display something that you can copy and paste back in the python code that would recreate that same object.**

   with str:- ![1547996537693](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547996537693.png) 

   with repr and str:-

   ![1547996578474](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547996578474.png) 

   or 

   ![1547996607939](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547996607939.png)

5. special methods for arithmetic:-

   ![1547996829757](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547996829757.png) 

   print(1+2) uses special method called dunder add. 

6. adding two employee salaries:-

   ![1547996901943](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547996901943.png) 

7. Other special methods are present in documentation.

   ![1547996960120](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547996960120.png) 

   eg:-

   ![1547997002444](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547997002444.png) 

8. dunder len method for employee:-

   ![1547997046376](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547997046376.png)

   https://docs.python.org/3/reference/datamodel.html#special-method-names 

9. Real world example:-

   **return NotImplemented** is used when you don't want to throw an error because the other object might know how to handle that operation. If other object doesn't know how to handle it, then it throws an error. 

   time:-

   ![1547997322615](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547997322615.png)

   date:- 

   ![1547997408114](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547997408114.png)  

   ![1547997357010](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547997357010.png) 

   
>
