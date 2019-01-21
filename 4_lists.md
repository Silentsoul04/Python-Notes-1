**Lists**

* Ordered sequence of elements.
* Mutable
* Homogenous or Heterogenous
* Empty List declaration :

```python3
empty_list = []		# or
empty_list = list()
```

* Declaration 

```python3
> courses = ['math','physics','chemistry','biology']

> print(courses)		# ['math','physics','chemistry','biology']

> print(courses[1])		# physics; indexing a list's elements

> print(len(courses))		# 4; length of a list
```

* Adding elements into a list ;

```python3
courses = ['math','physics','chemistry','biology']

# append(element) : adds element at the end

courses.append('arts')
print(courses)			# ['math','physics','chemistry','biology','arts']

# insert(position,element): add element at the desired postion

courses.insert(0,'english')
print(courses)	# ['english','math','physics','chemistry','biology','arts']

# extend(list_name) : adds elements of one list to another

courses_extra=['sports','compsci']
courses.extend(courses_extra)
print(courses)
#['english','math','physics','chemistry','biology','arts','sports','compsci']
```

* Removing elements from a list :

```python3
courses=['math','physics','chemistry','biology']

# remove(element_name) : removes the desired element

courses.remove('math')
print(courses)			# ['physics','chemistry','biology']

# pop() : removes the last element and returns it

popped = courses.pop()
print(popped)				# biology
print(courses)				# ['physics','chemistry']
```

* Misc Operations on lists :

```python3
nums=[1,3,2,5,4]

# reverse() : reverses the list order

nums.reverse()
print(nums)			# [4,5,2,3,1]

# sort() : sorts the list in ascending order  (Timsort)

nums.sort()
print(nums)			# [1,2,3,4,5]

nums.sort(reverse=True)		# descending order
print(nums)			# [5,4,3,2,1]

# sorted(list_name) : returns a sorted copy, doesn't alter the original list

nums=[1,3,2,5,4]
sorted_nums=sorted(nums)
print(sorted_nums)			# [1,2,3,4,5]
print(nums)					# [1,3,2,5,4]

# min(list_name) : returns minimum element of the list

print(min(nums))		# 1

# max(list_name) : returns maximum element of the list

print(max(nums))		# 5

# sum(list_name) : returns sum of all the list elements

print(sum(nums))		# 15

# list_name.index('element_value') : returns index of an element

print(nums.index(5))		# 3

# join() and split()

courses=['math','physics','chemistry','biology']
course_str= ', '.join(courses)
print(course_str)		# math, physics, chemistry, biology

courses_new=course_str.split(', ')
print(courses_new)		# ['math', 'physics', 'chemistry', 'biology']
```



**Tuples :**

* Ordered, Immutable (cannot add, remove, modify), Homo and Hetero
* Empty Tuple declaration :

```python3
empty_tuple=()			# or
empty_tuple =tuple()	
```

* Declaration :

```python3
courses=('math','physics','chemistry','biology')

print(courses)		#('math', 'physics', 'chemistry', 'biology')
print(courses[0])	# math

courses[0]='arts'		# error : immutable
```

**Sets :**

* Unordered, No duplicates, Set objects are mutable, homo or hetero
* Empty set declaration :

```python3
empty_set=set()		# {} isn't right, it's a dictionary
```

* Membership check :

```python3
courses={'math','physics','chemistry'}

print('math' in courses)		# True
```

* Set operations :

```python3
courses={'math','physics','chemistry'}
arts={'math','design','history'}

> print(courses.intersection(arts))	  # {'math'}

> print(courses.union(arts))	# {'chemistry', 'design', 'history', 'math', 								 # 'physics'}

> print(courses.difference(arts))		# {'chemistry', 'physics'}
```




