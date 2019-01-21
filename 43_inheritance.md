

class Employee():
    number_of_employees=0
    amount_raise=1.04
    #Below thing is like a constructor and self is the default argument 
    def __init__(self,f,l,p):
        self.fname=f
        self.lname=l
        self.salary=p

```python
    Employee.number_of_employees+=1
def fullname(self):
    return '{} {}'.format(self.fname,self.lname)
def raise_amount(self):
    self.salary=int(self.salary * self.amount_raise)

@classmethod
def finalraise(cls,amt):
    cls.amount_raise=amt

@classmethod
def convert(cls,string):
    f,l,p=string.split("-")
    return cls(f,l,p)

@staticmethod
def is_day(day):
    if day.weekday()==1 or day.weekday()==2:
        return False
    return True
```

class Developer(Employee):
    amount_raise=2.03

```python
def __init__(self,f,l,p,lang):
    super().__init__(f,l,p)
    self.lang=lang
```


​    
#print(Employee.number_of_employees)
d1=Developer("Praveen","Raja",26000,"Python")
#print(Employee.number_of_employees)
d2=Developer("Nikki","Varma",60000,"ROR")
print(d2.lname,d2.lang)

print(d2.salary)
d2.raise_amount()
print(d2.salary)

print(d1.salary)
d1.raise_amount()
print(d1.salary)

print(help(Developer))


Output:

Varma ROR
60000
121799
26000
52779





class Employee():
    number_of_employees=0
    amount_raise=1.04
    #Below thing is like a constructor and self is the default argument 
    def __init__(self,f,l,p):
        self.fname=f
        self.lname=l
        self.salary=p

```python
    Employee.number_of_employees+=1
def fullname(self):
    return '{} {}'.format(self.fname,self.lname)
def raise_amount(self):
    self.salary=int(self.salary * self.amount_raise)

@classmethod
def finalraise(cls,amt):
    cls.amount_raise=amt

@classmethod
def convert(cls,string):
    f,l,p=string.split("-")
    return cls(f,l,p)

@staticmethod
def is_day(day):
    if day.weekday()==1 or day.weekday()==2:
        return False
    return True
```

class Developer(Employee):
    amount_raise=2.03

```python
def __init__(self,f,l,p,lang):
    super().__init__(f,l,p)
    self.lang=lang
```

class Manager(Employee):
    def __init__(self,f,l,p,emp_list=None):
        super().__init__(f,l,p)
        if emp_list is None:
            self.emp_list=[]
        else:
            self.emp_list=emp_list

```python
def add_emp(self,emp):
    if emp not in self.emp_list:
        self.emp_list.append(emp)

def remove_emp(self,emp):
    if emp in self.emp_list:
        self.emp_list.remove(emp)

def print_emp(self):
    for emp in self.emp_list:
        print("-->",emp.fname)
```


​        




#print(Employee.number_of_employees)
d1=Developer("Praveen","Raja",26000,"Python")
#print(Employee.number_of_employees)
d2=Developer("Nikki","Varma",60000,"ROR")


mgr_1=Manager("Corey","Schafer",10000,[d1])

print(mgr_1.lname)
mgr_1.add_emp(d2)
print(mgr_1.print_emp())
mgr_1.remove_emp(d2)

print(issubclass(Manager,Employee))
print(isinstance(d1,Developer))

Output:

Schafer
--> Praveen
--> Nikki
None
>>> 
= RESTART: C:/Users/bpraja/AppData/Local/Programs/Python/Python37-32/dec.py =
Schafer
--> Praveen
--> Nikki
None
True
True
