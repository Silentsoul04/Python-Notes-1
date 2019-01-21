# 24 Datetime Module

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
