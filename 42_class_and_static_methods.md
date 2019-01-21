Class Variables:



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
```
print(Employee.number_of_employees)
e1=Employee("Praveen","Raja",26000)
print(Employee.number_of_employees)

e1.amount_raise=2.04
print(Employee.amount_raise)

print(e1.amount_raise)
print(e1.salary)
e1.raise_amount()
print(e1.salary)


print(e1.__dict__)



Output:
0
1
1.04
2.04
26000
53040
{'fname': 'Praveen', 'lname': 'Raja', 'salary': 53040, 'amount_raise': 2.04}