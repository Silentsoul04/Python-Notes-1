**Numeric Data :**

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