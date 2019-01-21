**Error handling :**

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