Special (Magic/Dunder) Methods:

__init__() is a Dunder method
__repr__()
__str__()

print(1+2) gives 3 where + is an Dunder method __add__ already built.



class Employee():

```python
raise_amount=1.05
#Below thing is like a constructor and self is the most important argument 
def __init__(self,f,l,p):
    self.fname=f
    self.lname=l
    self.salary=p
    self.email=f+"."+l+"@oracle.com"
```


​        
```python
def fullname(self):
    return '{} {}'.format(self.fname,self.lname)
```


```python
def finalpay(self):
    self.salary=int(self.salary * self.raise_amount)

def __repr__(self): #It is for developers
    return "Employee('{}','{}',{})".format(self.fname,self.lname,self.salary)

def __str__(self): #The customer can see this output
    return "{} - {}".format(self.fullname(),self.email)

def __add__(self,other):
    return self.salary + other.salary

def __len__(self):
    return len(self.fullname())
```

e1=Employee('Mahesh','Babu',260000)
e2=Employee('Praveen','Raja',25000)

print('tester'.__len__())
print(e1 + e2)
print(len(e1))
print(repr(e1)) #same as e1.repr()
print(str(e1)) #same as e1.str()


Output:

6
285000
11
Employee('Mahesh','Babu',260000)
Mahesh Babu - Mahesh.Babu@oracle.com