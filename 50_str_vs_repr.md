str vs repr

The goal of __repr__ is to be unambigous
The goal of __str__  is to be readable

import datetime
import pytz

a=datetime.datetime.utcnow().replace(tzinfo=pytz.UTC)

b=str(a)

str(a)
str(b)

repr(a)
repr(b)

Output:
2019-01-20 15:58:16.732776+00:00
2019-01-20 15:58:16.732776+00:00
datetime.datetime(2019, 1, 20, 15, 58, 16, 732776, tzinfo=<UTC>)
'2019-01-20 15:58:16.732776+00:00'


As repr gives the output which is helpful to the developers, it is developer friendly.