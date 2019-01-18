**random module :**

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