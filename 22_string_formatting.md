**String Formatting :**

* format(), f-strings.

```python
greetings='Hello'
name='Aditya'
pi=3.1456783

print("{},{}".format(greetings,name))	# Hello,Aditya

print("{1},{0}".format(greetings,name))		# Aditya,Hello

print("{name},{greetings}".format(name=name,greetings=greetings))	#Aditya,Hello

print(f"{name},{greetings} !")	# Aditya,Hello

print(f"{pi:.4f}")	# 3.1456
```

