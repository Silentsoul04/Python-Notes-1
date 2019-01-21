Regular method automatically takes the argument self.
class method takes the arguments instance of the class(automatically).
static method takes no arguments



class Employee():
    number_of_employees=0
    amount_raise=1.04
    #Below thing is like a constructor and self is the most important argument 
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
```


​        
#print(Employee.number_of_employees)
e1=Employee("Praveen","Raja",26000)
#print(Employee.number_of_employees)

Employee.finalraise(2.03)
#e1.finalraise(2.03) or
print(Employee.amount_raise)

print(e1.amount_raise)
#print(e1.salary)
#e1.raise_amount()
#print(e1.salary)


#print(e1.__dict__)

Output:

2.03
2.03




class Employee():
    number_of_employees=0
    amount_raise=1.04
    #Below thing is like a constructor and self is the most important argument 
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

#print(Employee.number_of_employees)
e1=Employee("Praveen","Raja",26000)
#print(Employee.number_of_employees)

Employee.finalraise(2.03)
#e1.finalraise(2.03) or
#print(Employee.amount_raise)

#print(e1.amount_raise)
#print(e1.salary)
#e1.raise_amount()
#print(e1.salary)
#print(e1.__dict__)

emp_string="Nikki-Varma-72000"
e2=Employee.convert(emp_string)

import datetime

day=datetime.date(2019,1,18)
print(Employee.is_day(day))
