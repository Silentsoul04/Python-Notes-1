
# Efficiently Managing Resources(preetha)

- 2 ways to open a file: with and without using a context manager.
- Context managers allow us to specify what exactly we want to set up and tear down when working with file objects.
- It handles the tear down the necessary resources.
- To open it using context manager use "with".
- No need to close the file after working with it.

## Using a class
``` 
class Open_file():
	def __init__(self, filename, mode):
		self.filename=filename
		self.mode=mode
		
	def __enter__(self):
		self.file=open(self.filename.self.mode)
		return self.file
		
	def __exit__(self,exc_type,exc_val,traceback):
		self.file.close()
		
with Open_file('sample.txt','w') as f:
	write('Testing')

```

## Using a function

- context manager has to be imported from contextlib
```
from contextlib import contextmanager

@contextmanager
def open_file(file,mode):
	f=open(file,mode)
	yield f
	f.close()

with Open_file('sample.txt','w') as f:
	write('The whole message.')
```

## Without a context manager
``` 
import os
from contextlib import contextmanager

cwd = os.getcwd()
os.chdir('Sample-Dir-One')
print(os.listdir())
os.chdir(cwd)


cwd = os.getcwd()
os.chdir('Sample-Dir-Two')
print(os.listdir())
os.chdir(cwd)
```
## creating a context manager
```
@contextmanager
def change_dir(destination):
	try:
		cwd = os.getcwd()
		os.chdir(destination)
		yield
	finally:
		os.chdir(cwd)
```
**Context Manager :**(aditya)

* for the efficient management of resources.
* say for a file, even if we dont explicitly close it, it handles the operation.
* context manager with a class :

![context_manager_class](images/context_manager_1.PNG)

* context manager with function :

![context_manager_function](images/context_manager_2.PNG) 
(lalith)
1. **Context managers:-** allow us to properly manage resources so that we can specify exactly what we want to set up and tear down when working with certain objects. 

   eg:- in files, with is a context manager.

   ![1548011486290](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1548011486290.png) 

   it automatically closes the file.

2. we can write our own context managers  by using a class or by using functions with decorators.

   creating using class:-eg is files

   enter and exit are the setup and teardown of our context managers.

   ![1548011833885](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1548011833885.png) 

   and sample.txt is created and has Testing written in it.

   creating using function:-

   we need to import contextmanager from contextlib.

   ![1548012112387](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1548012112387.png) 

   or

   ![1548012151209](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1548012151209.png) 

3. Practical example:- for this example, we need to import os and contextmanager

   without context managers:-

   ![1548012244652](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1548012244652.png) 

   with context managers:-

   ![1548012402123](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1548012402123.png) 

   **Context managers can be used for opening and closing database connections, acquiring and releasing locks etc.**

