Property Decorators: Getters, setters and Deleters:



class Employee():
    #Below thing is like a constructor and self is the default argument 
    def __init__(self,f,l,p):
        self.fname=f
        self.lname=l
        self.salary=p
        

```python
@property
def email(self):
    return '{}.{}@oracle.com'.format(self.fname,self.lname)

@property
def fullname(self):
    return '{} {}'.format(self.fname,self.lname)

@fullname.setter
def fullname(self,name):
    first,last=name.split(" ")
    self.fname=first
    self.lname=last

@fullname.deleter
def fullname(self):
    print("Deleting the name!")
    self.fname=None
    self.lname=None
```

emp=Employee('Praveen','Raja',26000)

emp.fname="Prvn"

emp.fullname="Mahesh Babu"

print(emp.fname) #It will change 
print(emp.email)  #It will not change
print(emp.fullname)

del emp.fullname


Output:

Mahesh
Mahesh.Babu@oracle.com
Mahesh Babu
Deleting the name!