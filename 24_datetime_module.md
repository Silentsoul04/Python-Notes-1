
# 24 Datetime Module(preetha)

- To print a particular date:
> ```
> d = datetime.date(2019, 7, 24)
> print(d)
> ```
> Output:
> 2019-07-24

- Today's date:
> ```
> tday = datetime.date.today()
> print(tday)
> ```
> Output: 
> 2019-01-16

- Weekday
> Monday 0 and Sunday 6

- Isoweekday
> Monday 1 and Sunday 7

- Time delta
> ```
> tdelta = datetime.timedelta(days=7)
> tday = datetime.date.today()
> print(tday - tdelta)
> ```
> The output will be 2019-01-23
> ```
> tdelta = bday - tday
> ```
> This output would be the number of days between the two dates.

- Date time
>```
> dt = datetime.datetime(2019,1,16,30,45,100000)
> print(dt)
> ```
> Output: 2019 - 01-16

**datetime :**(aditya)

```python3
import datetime

dat=datetime.date(2018,2,14)  # format is yyyy-m-d
print(dat)						# 2018-02-14

tday=datetime.date.today()
print(tday)						# 2019-01-14
print(tday.year)			# 2019

tdelta = datetime.timedelta(days=7)
print(tday+tdelta)		# 2019-01-21

# date2 = date1 +/- tdelta
# tdelta = date1 +/- date2

dt=datetime.datetime(2019,1,14,20,32,45,1000)		#yyyy-m-d-hh-mm-ss-ms

Note : all the methods that can be used with date and time can be used with datetime as well.
```
