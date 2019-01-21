Data and functions together bind known as class. 



class Employee():

```python
#Below thing is like a constructor and methods automatically takes in the self argument 
def __init__(self,f,l,p):
    self.fname=f
    self.lname=l
    self.salary=p
def fullname(self):
    return '{} {}'.format(self.fname,self.lname)
```

e1=Employee("Praveen","Raja",26000)

print(e1.salary)
print(e1.fullname())
print(Employee.fullname(e1))


Output:
26000
Praveen Raja
Praveen Raja