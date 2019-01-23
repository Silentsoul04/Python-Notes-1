
# 3 Integers and floats(preetha)
## Comparison
- Equal ==
- Not equal !=
- greater than >
- less than <
- Greater than or equal to >=
- Less than or equal to <=

**Numeric Data :**(aditya)

* Checking the data type of a variable:

```python3
var=5
print(type(var))		# <class,'int'>
```

* Arithmetic Operations :

```python3
op1=3
op2=4

> print(op1+op2)		# 7, addition

> print(op1-op2)		# -1, subtraction

> print(op1*op2)		# 12, multiplication

> print(op1/op2)		# 1.5 (for >= py v3.0), 1 (py v2.0), division

> print(op1//op2)		# 1, floor division

> print(op1**op2)		# 81, power

> print(op1%op2)		# 4, modulo

>print(abs(-4))			# 4, absolute value

> print(round(3.74,1))		# 3.70, round upto first decimal
```

* Compound Operators :  +=, -=, *=, /=  etc.
* Comparison Operators :  == (comparison), != (not equals), >= (ge), <= (le), > (greater than), < (less than) ; returns boolean values.
* Logical Operators : and, or, not, is.
* Note : The == operator compares the values in the objects whereas the 'is' keyword compares the id's of the objects.

**Common Typecastings :**

* String to Integer :

```python3
n1='100'
n2='200'

print(n1+n2)		# 100200

n1=int(n1)
n2=int(n2)
print(n1+n2)		# 300

# Note : int() is used to convert any data type to int 
```

* Integer to String :

```python3
n1=20

n1_string = str(n1)
```

* Character to ASCII equivalent :

```python3
var='A'

> print(ord(var))		# 65
```

* ASCII to Character equivalent :

```
var = 65

> print(chr(var))		# A
```

(lalith)
1. **type:-**

   print(type(num))

   returns <class 'int'>

   and for num=3.4 it returns float.

2. **basic operations:-**

![1547619317832](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547619317832.png)

​	for normal division it gives 1.5 as answer.

3. **power function:-**

   print(3**2) returns 9

4. Order of operations does work with python

   eg:-print(3*(2+1)) returns 9

5. **Incrementing:-**

   num=1

   num+=10

   print(num)

   it returns 11

6. print(abs(-10)) returns 10

7. print(round(3.75)) returns 4

   print(round(3.75,1)) returns 3.8

8. **Comparisions:-**

   They return boolean values

   ![1547629469786](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547629469786.png)

9. num_1='100'

   num_2='200'

   print(num_1 +num_2) returns 100200

10. So we use **casting**

    num_1='100'

    num_2='200'

    num_1=int(num_1)

    num_2=int(num_2)

    print(num_1 +num_2) returns 300

(prvnrj)
Integers and Floats
>>>>>>> origin/prvnrj_notes

>>> 3+2
5
>>> -1%2
1
>>> 2**-1
0.5
>>> 4//5
0
>>> 4/5
0.8
>>>round(23.55)
24

casting- converts the one data type to another datatype.

