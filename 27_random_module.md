# Random module

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


```