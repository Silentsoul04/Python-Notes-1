1. **Naive datetimes:-** naive dates and times don't have enough info to determine things like timezone or daylight savings times but are easier to work with if you don't need that level of detail.

   **Aware datetimes:-** If you need that level of detail to avoid confusion then you need aware datetimes and they have enough info to determine things like timezones or daylight savings times.

2. **Creating date:-**

   ![1547907646763](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547907646763.png) 

   Don't give leading zeroes in passing arguments as shown in below picture as it gives an error

   ![1547907695661](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547907695661.png)

   Second method:- for getting current day 

   ![1547963097559](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547963097559.png)

   ![1547963179456](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547963179456.png)

   ![1547963212491](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547963212491.png)

   for weekday()-Monday is 0 and sunday is 6

   for isoweekday()-Monday is 1 and sunday is 7

3. **Time deltas:-** difference between two dates or times and are useful when we want to do operations on our dates or times

   eg:- ![1547963475853](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547963475853.png)

   ![1547963567822](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547963567822.png)

   ![1547963735576](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547963735576.png)           

   ![1547963772868](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547963772868.png)

   ![1547963813965](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547963813965.png)

4. **datetime.time:-** datetime.time(hours, minutes,seconds , microseconds)

   It doesnt deal with days months and years.

   ![1547963968657](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547963968657.png)

   to print out only hour, we can use t.hour in print()

5. **datetime.datetime:-** it gives us access to days to microseconds.

   ![1547964216364](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547964216364.png)

   we can have access to only date by using dt.date() in print() and dt.time() for only time.

   ![1547964303832](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547964303832.png) 

   ![1547964315539](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547964315539.png)

6. ![1547964388098](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547964388098.png)

   .today() returns current local date time with a timezone of none

   .now() gives us a option to pass in a timezone so if you leave the timezone empty, then these are similar.

   .utcnow() gives us the current UTC time but the TZ info is stiil set to none(it gives GMT )

7. pytz is a third party package which brings timezone database and it can be installed using pip. It is recommended to use with UTC

   ![1547965386553](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547965386553.png)

8. ![1547965457187](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547965457187.png) 

   ![1547965490220](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547965490220.png) 

   

9. To convert naive date time to timezone aware:-

   ![1547965686351](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547965686351.png) 

10. **Ways to display datetimes**:-

    - displaying in ISO format:-

      ![1547965780718](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547965780718.png)

    - ![1547965840011](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547965840011.png) 

      formats (eg:- %B) are presnt in documentation.

    - conversion of string into datetime:-

      ![1547965960291](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547965960291.png) 

      There is a package called **arrow** which makes it easier way to work with dates times.

