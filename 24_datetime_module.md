Python 3.7.2 (tags/v3.7.2:9a3ffc0492, Dec 23 2018, 22:20:52) [MSC v.1916 32 bit (Intel)] on win32
Type "help", "copyright", "credits" or "license()" for more information.

>>> import datetime
>>> 
>>> import datetime
>>> datetime.date.today()
>>> datetime.date(2019, 1, 16)
>>> print(datetime.date.today())
>>> 2019-01-16
>>> print(datetime.date.today().day())
>>> Traceback (most recent call last):
>>>   File "<pyshell#4>", line 1, in <module>
>>>     print(datetime.date.today().day())
>>> TypeError: 'int' object is not callable
>>> tdy=datetime.date.today()
>>> tdy.year
>>> 2019
>>> tdy.day
>>> 16
>>> tdy.weekday
>>> <built-in method weekday of datetime.date object at 0x03DDDFE0>
>>> tdy.weekday()
>>> 2
>>> delta=datetime.timedelta(days=6)
>>> tdy + delta
>>> datetime.date(2019, 1, 22)
>>> bday=datetime.date(2019,11,7)
>>> bday-tdy
>>> datetime.timedelta(days=295)
>>>
>>> t=datetime.time(11,28,23)
>>> t
>>> datetime.time(11, 28, 23)
>>> print(t)
>>> 11:28:23
>>> t.hour
>>> 11
>>> dt=datetime.datetime(2019,1,16,11,30,45,1432)
>>> datetime.timedelta(hours=12)
>>> datetime.timedelta(seconds=43200)
>>>
>>>
>>> datetime.datetime.today()
>>> datetime.datetime(2019, 1, 16, 23, 32, 9, 649011)
>>> datetime.datetime.now()
>>> datetime.datetime(2019, 1, 16, 23, 32, 19, 395208)
>>> datetime.datetime.utcnownow()
>>> Traceback (most recent call last):
>>>   File "<pyshell#25>", line 1, in <module>
>>>     datetime.datetime.utcnownow()
>>> AttributeError: type object 'datetime.datetime' has no attribute 'utcnownow'
>>> datetime.datetime.utcnow()
>>> datetime.datetime(2019, 1, 16, 18, 2, 32, 892460)
>>> import pytz
>>> Traceback (most recent call last):
>>>   File "<pyshell#27>", line 1, in <module>
>>>     import pytz
>>> ModuleNotFoundError: No module named 'pytz'
>>> pip install pytz
>>> SyntaxError: invalid syntax
>>> dt_utcnow.astimezone(pytz.timezone('India/Kolkata')
>>>  )
>>> Traceback (most recent call last):
>>>   File "<pyshell#30>", line 1, in <module>
>>>     dt_utcnow.astimezone(pytz.timezone('India/Kolkata')
>>> NameError: name 'dt_utcnow' is not defined
>>>