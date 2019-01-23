
# Conditionals(preetha)

**Conditionals :** (aditya)

* <b>if</b> statement :

```python3
if condition :
	body
```

* <b> if else </b> statement :

```python3
if condition :
	body1
else:
	body2
```

* <b> if elif else </b> statement :

```python3
if condition_1 :
	body1
elif condition2 :
	body2
else :
	body3
```

* False values : False, None, Zero of any numeric type, empty sequence, empty dictionary.
(lalith)
**CONDITIONAL OPERATIONS:-**

1. - if True:

   print('condition was true')

   o/p:- condition was true

   - if False:

   print('condition was false')

   o/p:-

2. **Python doesn't have a switch case **because if and elif are plenty clean enough to do this.

   ![1547638100719](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547638100719.png)

   **BOOLEAN OPERATIONS:-**

   - AND

   - OR

   - NOT

     eg:- ![1547638327266](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547638327266.png)

    ![1547638361619](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547638361619.png)

1. a=[1,2,3]

   b=[1,2,3]

   print(a==b)

   o/p:- true

2. a=[1,2,3]

   b=[1,2,3]

   print(a is b)

   o/p:- false as they are **two different objects in memory** and we can print out the locations using built in ID function as shown below. 

   ![1547638587222](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547638587222.png)

   *If we assign b=a instead of assigning a value to b, then their id's are same and it returns true.*

   **WHAT PYTHON EVALUATES TO TRUE OR FALSE:-**

The things in comment section in below picture all evaluate to false in python and everything else will be evaluated to true by default.

![1547638867947](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547638867947.png)


(prvnrj)

=======
`Python` evaluates true or false using if, else and elif statements.
if condition:
   ...
elif condition:
   ...
else:
   ...
>>>>>>> origin/prvnrj_notes

Comparision operators

==
!=
>
<
>=
<=

and
not 
or
is

The operators "==" are different from "is".

code and output:

>>> a=[1,2,3]
>>> c=[1,2,3]
>>> print(a==c)
True
>>> print(a is c)
False

Because "is" operator compares the memory id of a and c.

>>> print(id(a))
63816248
>>> print(id(c))
59433448
>>> b=c
>>> print(id(b),id(c),b==c)
59433448 59433448 True

False values:
The kind of sequences which leads to the false values are as follows

False, None, zero, [],(),{},''

>>> string=''
>>> if string:
   print("It's there")
else:
   print("Nothing is present :/")

   
Nothing is present :/
