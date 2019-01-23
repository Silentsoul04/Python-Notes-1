
# 31 Exception Handling(preetha)


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

(lalith)
1. ![1547972964134](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547972964134.png)

2. ![1547973058717](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547973058717.png) 

3. ![1547973083307](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547973083307.png) 

4. ![1547973143027](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547973143027.png) 

   else is executed if exception is not raised as shown above

5. **Finally clause:-** executes no matter what happens

   eg:-

   ![1547973281001](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547973281001.png) 

   ![1547973303633](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547973303633.png) 

   6. We can raise exception manually using **raise**

      eg:-

      ![1547973355720](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547973355720.png)

(prvnrj)
 try:
    #open('file.txt')
    #var
    print("try")
except Exception:
    print("Bad variable")
except FileNotFoundError:
    print("File not found")
else:
    print("In else")
finally:
    print("Executes whatever condition maybe")


output:
try
In else
Executes whatever condition maybe


try:
    open('file.txt')
    #var
    print("try")
except FileNotFoundError:
    print("File not found")
except Exception:
    print("Bad variable")

else:
    print("In else")
finally:
    print("Executes whatever condition maybe")

Output:
File not found
Executes whatever condition maybe

try:
    open('file.txt')
    var=bad_var
    print("try")
except Exception as e:
    print("Bad variable")
    print(e)
except FileNotFoundError as e:
    print("File not found")
    print(e)


else:
    print("In else")
finally:
    print("Executes whatever condition maybe")

Output:

Bad variable
[Errno 2] No such file or directory: 'file.txt'
Executes whatever condition maybe


try:
    #open('file.txt')
    var=bad_var
    print("try")
except Exception as e:
    print("Bad variable")
    print(e)
except FileNotFoundError as e:
    print("File not found")
    print(e)


else:
    print("In else")
finally:
    print("Executes whatever condition maybe")

Output:
Bad variable
name 'bad_var' is not defined
Executes whatever condition maybe


try:
    #open('file.txt')
    var=bad_var
    print("try")
except FileNotFoundError as e:
    print("File not found")
    print(e)
except Exception as e:
    print("Bad variable")
    print(e)


else:
    print("In else")
finally:
    print("Executes whatever condition maybe")

Output:
Bad variable
name 'bad_var' is not defined
Executes whatever condition maybe


try:
    file=open('file.txt')
    if file.name=='file.txt':
        raise Exception #Manually we can raise error!!
        
```python
#var=bad_var
print("try")
```

except FileNotFoundError as e:
    print("File not found")
    print(e)
except Exception as e:
    print(e)


else:
    print("In else")
finally:
    print("Executes whatever condition maybe")

