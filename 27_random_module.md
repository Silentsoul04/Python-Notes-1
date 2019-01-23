
# Random module(preetha)

- value = random.random() returns a radom value between 0 and 1

- For a floating point between a range,
> value = random.uniform(1,10)

- for random whole numbers
> val = random.randint(1,6)

- for a random value from a given set of values
> val = random.choice( list, weights,  number_of_times)

- to shuffle a set of values
> ```
> deck = list(range(1,53))
> radom.shuffle(deck)
> ```
```

- To pick from a set
> ```
> hand  random.sample(<list_name>, <no.of.cards>)
> ```



**random module :**(aditya)

```python3
import random

val=random.random() 		# random no. between 0 and 1
val=random.uniform(1,10)		# random no. in the specified range
val= random.randint(1,6)		# random no. from 1-6 inclusive of both

greetings=['hi','hello','hola','heylo','hey']
val=random.choice(greetings)		# randomly chooses an element from the list
results=random.choices(greetings,k=10)		# returns a list of 10 random values (might 											# repeat)

vals=list(range(1,20))
random.shuffle(vals)			# shuffles the vals list 
cand=random.sample(vals,k=5)		# returns a sample list of 5 random values(unique)

```