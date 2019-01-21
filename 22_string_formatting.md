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