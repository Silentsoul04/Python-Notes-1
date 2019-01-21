# String Formatting

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
