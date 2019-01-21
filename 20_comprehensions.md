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

>>> 