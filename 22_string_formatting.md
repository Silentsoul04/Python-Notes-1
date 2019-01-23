
# String Formatting(preetha)

## format()
```
sentence = 'My name is {} and I am {} years old.'.format(person['name'],person['age'])
```
``` 
sentence = 'My name is{0[name]} and I am {0[age]} years old'.format(person)
```
where person is a class.
```
sentence = 'The value is {:02}'.format(i)
```
> This prints the value of i using 2digits.
```
sentence = 'Pi is equal to {:.3f}'.format(pi)
```
> This statement prints the value of pi upto 3 decimal digits.
```
sentence = '1 Mb is  equal to {:,.2f} bytes'.format(1000**2)
```
> It prints: 1 Mb is equal to 1,000,000.00 bytes.

**String Formatting :**(aditya)

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

(lalith)
**Dictionaries:-**![1547788340851](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547788340851.png) 

![1547788357972](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547788357972.png) 

![1547788381679](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547788381679.png) 

![1547788434298](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547788434298.png)

![1547788495412](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547788495412.png) 

**Lists:-**

![1547788530727](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547788530727.png)

**Objects:-**

![1547789026792](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547789026792.png)

![1547792546727](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547792546727.png)
![1547792642566](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547792642566.png)

**Numbers:-**

![1547793479824](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547793479824.png)

**: indicates we are formatting something.**

![1547793464038](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547793464038.png)

![1547793506292](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547793506292.png)

**Decimal places:-**

![1547793569476](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547793569476.png)

![1547793614311](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547793614311.png)

![1547793658562](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547793658562.png)

**Dates:-**

![1547793724145](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547793724145.png) 

- check up the formatting options in documentation <!--https://docs.python.org/3/library/datetime.html#strftime-and-strptime-behaviour--> that are used in below picture

  ![1547793947944](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547793947944.png)           

  ![1547794046529](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547794046529.png)

(prvnrj)

Formatting

>>> d
{2: 'b', 1: 'a', 3: 'c'}
>>> '{0[1]},{0[2]}'.format(d)
'a,b'
P1=Person('John',21)
'{0.name} {0.age}'.format(P1)
'{name} {age}'.format(**P1)

for i in range(1,11):
	'{:02}'.format(i) #Prints the decimal values about two digits ex 01,02,03,04..etc

'{:.2f}'.format(pi)
>>>3.14

comma separator
'{:,}'.format(1000)

>>>1,000
>>>

>>> import datetime
>>> datetime.datetime(2019, 1, 16, 4, 53,54)
datetime.datetime(2019, 1, 16, 4, 53, 54)
\
>>> datetime.datetime(2019, 1, 16, 4, 53,54)
datetime.datetime(2019, 1, 16, 4, 53, 54)
>>> print(datetime.datetime(2019, 1, 16, 4, 53, 54))
2019-01-16 04:53:54
>>> my=datetime.datetime(2019, 1, 16, 4, 53,54)
			    

>>> '{:%B/%d,%Y}'.format(datetime.datetime(2019, 1, 16, 4, 53,54))
			    
'January/16,2019'
>>> '{0:%B}/{0:%d},{0:%Y}'.format(datetime.datetime(2019, 1, 16, 4, 53,54))
			    
'January/16,2019'
