**Comprehension :**

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