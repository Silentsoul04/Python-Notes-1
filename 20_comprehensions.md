# Comprehensions

- concise way to create a list
```
list_name[expression]
```
## examples

- Constructing a list
> ```
> my_list = [n for n in list_1]
> my_list = [n*n for n in list_1 ]
> my_list = map(lambda n: n*n, list_1)
> my_list = [n in list_1 if n%2==0]
> ```
```

- Constructing a combination of two lists
> ```
> my_list = [(var_1,var_2) for var_1 in list_1 for var_2 in list_2]
> ```

- Constructing a dict
> ```
> my_dict = {var1:var2 for zip(list1,list2) if var1!=val }
```

- Constructing a set
> ```
> my_set = {n for n in list1}
> ```
```

- Constructing a Generator Expression
> ```
> my_gen= (n*n for n in list1)


```