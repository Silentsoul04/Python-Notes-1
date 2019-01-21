import datetime
import calendar

balance=5000
interest_rate= 13*.01
monthly_payment=500

today=datetime.date.today()
days_in_current_month=calendar.monthrange(today.year, today.month)[1]
days_till_end_month=days_in_current_month-today.day


start_date = today + datetime.timedelta(days=days_till_end_month + 1)
print(start_date)
end_date = start_date


while balance>0:
    interest_charge = (interest_rate/12)*balance
    balance+=interest_charge
    balance-=monthly_payment

    balance=round(balance,2)

    if balance<0:
        balance=0 

    print(end_date, balance)

    dys_in_current_month = calendar.monthrange(end_date.year, end_date.month)[1]
    print(days_in_current_month,end_date.month)
    end_date = end_date + datetime.timedelta(days=days_in_current_month)


Output:
2019-02-01
2019-02-01 4554.17
28 2
2019-03-01 4103.51
31 3
2019-04-01 3647.96
30 4
2019-05-01 3187.48
31 5
2019-06-01 2722.01
30 6
2019-07-01 2251.5
31 7
2019-08-01 1775.89
31 8
2019-09-01 1295.13
30 9
2019-10-01 809.16
31 10
2019-11-01 317.93
30 11
2019-12-01 0
31 12



import datetime

actual_weight=54
target = 65
avg_wt_lbs=1

today=datetime.date.today()

end_date=today

while actual_weight < target:
    end_date+=datetime.timedelta(days=7)
    actual_weight+=avg_wt_lbs

print(end_date)

print(f'Completed in {(end_date-today).days} days')


Output:

2019-04-07
Completed in 77 days
