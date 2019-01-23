

# Comprehensions(preetha)

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



**Comprehension :**(aditya)

* List comprehension : easier way to write a list.

```python3
nums =[1,2,3,4,5,6,7,8,9]

# i want 'n' for each 'n' in nums if 'n' is even.

traditional way :
________________

my_list=[]

for n in nums:
	if n%2==0:
		my_list.append(n)
		
comprehension :
______________

my_list=[n for n in nums if n%2==0]
```

* Dictionary comprehension:

```python3
names=['bruce','clark','peter']
heros=['batman','superman','spiderman']

# i want a dict{'name':'hero'} for each name in zip(names,heros)

traditional way :
________________
my_dict={}

for name,hero in zip(names,heros):
	my_dict[name]=hero

comprehension :
______________
my_dict={name:hero for name,hero in zip(names,heros)}

```
(lalith)
**List Comprehension:-** is a easier and more readable way to create a list.

eg:- 1. comment section of for loop also prints the same output. [n for n in nums] is the **comprehension**.

![1547714995008](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547714995008.png)

2. ​        ![1547715126765](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547715126765.png)

3. **map** runs everything in the list through a certain function and lambda is an anonymous function. 

   ![1547715360887](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547715360887.png)

   map are tough to read and write. Hence **comprehensions are better**.

4. ![1547715618585](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547715618585.png)

5. same by using filter is 

   ![1547715685366](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547715685366.png)

6. ![1547739620781](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547739620781.png)

   o/p:- ![1547739653643](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547739653643.png) 

   **Comprehending Dictionaries:-**

   eg :- 

   1. zip function:-![1547739848324](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547739848324.png)

      o/p:-![1547739877844](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547739877844.png)

   2. ![1547739985505](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547739985505.png)

      with comprehension:-

      ![1547740070670](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547740070670.png) 

   3. If we don't want peter then 

      ![1547740129580](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547740129580.png) 

      **Comprehending sets:-**

      1. ![1547740217564](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547740217564.png) 

         o/p:- ![1547740238762](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547740238762.png) 

         with comprehension:-

         ![1547740319968](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547740319968.png) 

         prints same output.

         

         **Comprehending GENERATOR EXPRESSIONS:-**

         - similar to list comprehension.

         - ![1547740548618](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547740548618.png) 

           output also includes 1 and 4

         - with comprehension also prints the same output and the code is given below:-

           ![1547740612608](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547740612608.png)

(prvnrj)
Comprehensions:

list=[i for i in numbers if i%2==0]
list1=[i*i for i in numbers]

>>> a1=map(lambda n: n*n,a)

>>> a1

<map object at 0x03AB8830>
>>> print(a1)

<map object at 0x03AB8830>
>>> a
[9, 8, 5, 4, 5, 5, 9, 8, 3, 5, 5]

>>> a1=list(map(lambda n: n*n,a))

>>> a1

[81, 64, 25, 16, 25, 25, 81, 64, 9, 25, 25]

>>> a1=list(map(lambda n: n%2==0,a))

>>> a1

[False, True, False, True, False, False, False, True, False, False, False]

>>> a1=list(filter(lambda n: n%2==0,a))

>>> a1

[8, 4, 8]

>>> a=[(letter,num) for letter in 'abcd' for num in [1,2,3,4]]

>>> a

[('a', 1), ('a', 2), ('a', 3), ('a', 4), ('b', 1), ('b', 2), ('b', 3), ('b', 4), ('c', 1), ('c', 2), ('c', 3), ('c', 4), ('d', 1), ('d', 2), ('d', 3), ('d', 4)]

>>> a=[1,2,3,4]

>>> b=['b','praveen','raja','praveen raja b']

>>> zip(a,b)

<zip object at 0x00DF0080>

>>> list(zip(a,b))

[(1, 'b'), (2, 'praveen'), (3, 'raja'), (4, 'praveen raja b')]

>>> b=['b','praveen','raja','praveen raja b','bpr']

>>> zip(a,b)

<zip object at 0x00DF00D0>

>>> list(zip(a,b))

[(1, 'b'), (2, 'praveen'), (3, 'raja'), (4, 'praveen raja b')]

>>> a=[1,2,3,4,5]

>>> b=['b','praveen','raja','praveen raja b']

>>> list(zip(a,b))

[(1, 'b'), (2, 'praveen'), (3, 'raja'), (4, 'praveen raja b')]

>>> my={}

>>> for key,value in zip(a,b):
	    my[key]=value


>>> my

{1: 'b', 2: 'praveen', 3: 'raja', 4: 'praveen raja b'}

>>> my={key:value for key,value in zip(a,b) if key!=3}

>>> my

{1: 'b', 2: 'praveen', 4: 'praveen raja b'}
>>> num=[1,1,2,4,4,6,4,5,3,7]

>>> my={n for n in num}

>>> my

{1, 2, 3, 4, 5, 6, 7}
>>> #generator funciton

>>> def gen(list):
	    for i in list:
		    yield i*i


>>> my_gen_list=gen(my)

>>> my_gen_list

<generator object gen at 0x03ACECF0>

>>> list(my_gen_list)

[1, 8, 27, 64, 125, 216, 343]

