**datetime :**

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