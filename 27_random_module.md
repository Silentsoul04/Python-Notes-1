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
(lalith)
**Shouldn't be used for security or cryptography and security module should be used for that**

1. random() function gives [0,1)

   ![1547967038816](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547967038816.png)

2. ![1547967056813](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547967056813.png)

3. ![1547967086564](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547967086564.png)

4. ![1547967132663](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547967132663.png)

   ![1547967193746](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547967193746.png)

   ![1547967260745](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547967260745.png)

   weights[18,18,2] gives 18 out of 38 chance for red , same for black and 2 for green 

5. randomly shuffling:-

   ![1547967348567](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547967348567.png)

   ![1547967377214](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547967377214.png)

   we use sample method to grab unique cards from our sequence rather than choice method which selects one card multiple times.

   ![1547967485910](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547967485910.png)

6. **overall example:-**

   generating 100 fake names, numbers etc.

   code:-

   ![1547967664301](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547967664301.png) 

   ![1547967678443](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547967678443.png) 

   o/p:-

   ![1547967700891](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547967700891.png)

(prvnrj)

import random

random.choices(, weights=[18,18,2],k=10)
random.randint()
random.random()
random.sample()- gives only unique values
