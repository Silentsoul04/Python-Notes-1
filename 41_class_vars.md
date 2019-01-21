1. Instance variables are unique for each instance and class variables are same for all instances.

   code:-

   ![ 1547985903084](https://github.com/adityakuppa26/Python-Notes/tree/lalith_notes/images/1547985903084.png) 

   ![1547985941788](https://github.com/adityakuppa26/Python-Notes/tree/lalith_notes/images/1547985941788.png) 

   we can also use self.raise_amount instead of Employee.raise_amount. Here raise_amount is class variable. 

2. When we access an attribute from an instance then it first checks with its variables. If it doesn't find then it checks with the class variables.

   1. 

      eg:-![1547986142545](https://github.com/adityakuppa26/Python-Notes/tree/lalith_notes/images/1547986142545.png) 

3. If we want to find the namespace of an instance, we use emp1.(two underscores)dict(two underscores) as shown below

   ![1547986374047](https://github.com/adityakuppa26/Python-Notes/tree/lalith_notes/images/1547986374047.png) 

   ![1547986397215](https://github.com/adityakuppa26/Python-Notes/tree/lalith_notes/images/1547986397215.png) 

   Employee.dict has raise_amount while emp.dict doesn't have that.

4. ![1547986469225](https://github.com/adityakuppa26/Python-Notes/tree/lalith_notes/images/1547986469225.png) 

   ![1547986486533](https://github.com/adityakuppa26/Python-Notes/tree/lalith_notes/images/1547986486533.png) 

   see the difference in above pictures.

5. finding no of employees:-

   ![1547986598294](https://github.com/adityakuppa26/Python-Notes/tree/lalith_notes/images/1547986598294.png) 

   ![1547986642239](https://github.com/adityakuppa26/Python-Notes/tree/lalith_notes/images/1547986642239.png) 

   Employee.no_of_emp should be used instead of instance.no_of_emp as it is counting the number of employees. Hence it is a class variable and needs to be Employee.no_of_emp

   
