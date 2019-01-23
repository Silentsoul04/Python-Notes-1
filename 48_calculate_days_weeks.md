# Calculating number of days, weeks, or months to reach specific goals(preetha)

## Example 1:  A code to pay off a particular amount of balance with a set interest rate

```
import datetime
import calender

balance = 5000
interest_rate = 13 * 0.01
monthly payment = 500

today = datetime.date.today()
days_in_current_month = calender.monthrange(today.year , today.month)[1]
days_until_end_of_month = days_in_current_month - today.day

start_date = today + datetime.timedelta(days=day_till_end_motnh + 1)
end_date = start_date

while balance > 0:
	interest_charge = (interest_rate / 12)*balance
	balance += interest_charge
	balance -= monthly_payment
	
	balance = round(balance,2)
	if balance < 0:
		balance = 0
	
	print(end_date, balance)
	
	days_in_current_month = calender.monthrange(today.year , end_date.month)[1]

	end_sate = end_date + end.timedelta(days=days_in_current_month)
	
```

## Example 2: To reach a target weight
```
import datetime
current weight = 220
goal_weight = 180
avg_lbs_week = 1.5

start_date = datetime.date.today()
end_date = start_date

while current_weight > goal_weight:
	end_date+=datetime.timedelta(days=7)
	current_weight -=avg_lbs_week

print(f'Reaced goal in {(end_date-start_date).days //7 }weeks')
```
**Calculating no. of days, weeks and months :**(aditya)

* import datetime, calendar
* calendar.monthrange(year,month) : returns a list of the starting day of the month and the no. of days in the month.
* Expected date to reach the subscriber goal:

![no_of_days](images/no_of_days.PNG)  
