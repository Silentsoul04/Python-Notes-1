# 31 Exception Handling

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