# Inheritance(preetha)

- A class in python can inherit attributes and methods from another class called superclass.

```
class Employee:

	raise_amount=1.04
	
	def __init__(self,first,last):
		self.first = first
		self.last = last
		self.email = first + '.' + last + 'oracle.com'
		self.pay = pay
		
	def fullname(self):
		return '{} {}'.format(self.first,self.last)

class Developer(Employee): 			
	def __init__(self,first,last,prog_lang):
		super().__init__(first,last)
		self.prog_lang='java'
```

- Here, Developer is a subclass that inherits from the superclass Employee.
- The init in Developer directly calls the init in the superclass.
- For any member of a subclass, first the subclass is searched and if not found, then superclass is searched.
- The superclass is enclosed in () after the subclass name.

**Inheritance :**(aditya)

```python3
class Employee:
	raise_amount=1.04
	def __init__(self,fname,lname):
		# code
	def fullname(self):
		# code

class Developer(Employee): 			# inheritance
	def __init__(self,fname,lname,lang):
		super().__init__(fname,lname)			# calls superclass constructor
		self.lang='java'
```

* Developer class inherits all the attributes and methods of the Employee class.

* If the sub and the superclass both have thne same named attributes or methods, the subclass is first looked for to find them and later the superclass.
(lalith)
1. Inheritance allows us to inherit attributes and methods from a parent class. This is useful because we can create sub classes and get all the functionality of parent class, then we can overwrite or add completely new functionality without affecting parent class in any way.

2. code:-

   ![1547994091655](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547994091655.png) 

   o/p:-

   ![1547994114213](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547994114213.png) 

   method resolution order:-First checks in the specified class that is instantiated. If it doesn't find then it goes to parent class. This chain is called method resolution order.

3. help function helps in visualizing method resolution order as shown below:-

   ![1547994338979](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547994338979.png) 

   o/p:-

   ![1547994353832](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547994353832.png) 

4.  ![1547994469061](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547994469061.png) 

   ![1547994532305](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547994532305.png) 

   ![1547994547146](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547994547146.png) 

   see the difference between above two pictures.

5. super().init allows employee class to handle first last and pay arguments. super() is used to refer to parent class.

   Instead of super, we can directly use parent class as shown below

   ![1547994786528](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547994786528.png) 

   For single inheritance, super() is better and for multiple inheritance usage of parent class is better

   entire example of developer class is:-

   ![1547994889255](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547994889255.png) 

6. Manager subclass:-

   ![1547995023537](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547995023537.png) 

   for initialization use lists or dictionaries only as in the above case(self.employees=[])

   execution code and o/p:-

   ![1547995182055](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547995182055.png) 

7. isinstance()-tells us if an object is an instance of a class

   ![1547995313693](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547995313693.png)

   ![1547995300702](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547995300702.png)

   ![1547995262099](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547995262099.png) 

8. issubclass()-tells us whether it is a subclass or not.

   ![1547995443615](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547995443615.png) 

   **Real world example:-** Exception module of python whisky library

   ![1547995490470](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547995490470.png) 

   ![1547995503771](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547995503771.png) 

   

(prvnrj)

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

<<<<<<< HEAD

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
