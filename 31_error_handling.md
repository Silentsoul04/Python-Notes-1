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
