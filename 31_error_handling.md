
# 31 Exception Handling(preetha)

```
try:
	f= open('file_name.txt')
except FileNotFoundError as e:
	print(e)
except Exception as e:
	print(e)
else:
	print(f.read())
	f.close()
finally:
	print("Executing finally")
```
- The more specific exceptions are written above the general ones.
- 'e' in the above code prints the actual error that occured
- If the there were no exceptions the the else part gets executed.
- Irrespective of the execution of the exception part, finally gets executed.

**Error handling :**(aditya)

```pyhton3
try :
	// code that might contain errors
	
except FileNotFoundError as fe:
	print(fe)					# when an error occurs in try, control comes here
	
except Exception:
	print('something wrong')

else:
	// code that runs if try doesn't throw an exception
	
finally:
	// code that runs irrespective of try throwing an error or not
```

