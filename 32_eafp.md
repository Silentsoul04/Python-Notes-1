
# Duck typing and EAFP (preetha)

## Duck Typing

- If an object walks like a duck and quacks like a duck then it is considered as a duck.
- Instead of checking if an item is a duck it is sufficient if it behaves like a duck even if it is not exactly a duck.

## Look before you leap

- Checking for the condition for an exception before executing the statement.
- The statement does not get executed if the condition fails.
- example:
```
if 'name' n person and 'age' in person and 'job' in person:
	print("I am {name}, {age} years old and my job is {job}.".format(**person))
else:
	print('missing some keys')
```

## Easier to ask for forgiveness than permission

- First trying to execute the statemnt, if it fails then executing the exception part.
- example:
```
try:
	print("I am {name}, {age} years old and my job is {job}.".format(**person))
except KeyError as e:
	print('missing {} key'.format(e))

**EAFP(easier to ask forgiveness than permission) :** (aditya)

* try to access something or write a code, if it doesn't work then just handle it.

![eafp](images/eafp.PNG)  

* advantages : more readable, lesser code as a result of lesser checks.

**F-strings :**

```python3
vals=[26,3,23]
print(f"my fav numbers are {vals[0]} and {vals[1]}")

pi=3.1456783422
print(f"pi value rounded is {pi:.4f}")

```