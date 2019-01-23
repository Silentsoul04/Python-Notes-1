<
# Lists, Tuples, Sets(preetha)

## List
- Mutable
### Functions
- insert(position, "")
- append("")
- extend(var2)
- sort()
- > sort(reverse=True)
- enumerate()
- join()
- split()

## Tuple
- Immutable
- Lesser methods
- Used to only loop through and access

## Sets
- No particular order
- No duplicates

### Functions
- intersection()
- union()
- difference()

**Lists**(aditya)

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




(lalith)
*Lists and tuples help us to work with sequential data and sets are unordered collection of values with **NO** duplicates.*

**LISTS:-**

1. creation:-

    courses=['History','Math','Physics',CompSci]

   print(courses)

   it prints ['History','Math','Physics',CompSci]

2. Length:-

   print(len(courses))

   it returns 4

3. print(courses[0]) returns History

4. negative index start from the last of list

   i.e., print(courses[-1]) prints CompSci

   *Negative indexes are useful in printing final element in list*

5. You get an index error if u try to access an index that doesn't exist 

   eg:-print(courses[4]) returns index out of range

6. **Slicing:-**print(courses[0:2]) prints ['History','Math']

7. **Adding:-** 

   - using append:-

     courses.append('Art') adds art into courses

   - using insert:-

     courses.insert(0,'Art')

     it returns ['Art','History','Math','Physics',CompSci']

   - using extend:-

     courses=['History','Math','Physics',CompSci]

     courses_2=['Art','Education']

     courses.insert(0,courses_2) and printing it gives [['Art','Education'],History','Math','Physics',CompSci']

     so we use extend method i.e.,

     courses.extend(courses_2) and print them. U will get ['History','Math','Physics',CompSci','Art','Education']

8. **Remove:-**

   courses.remove('Math')

   or

   courses.pop()-pops last element from list 

   eg:-compsci in this example of history math physics and compsci

   we can also print the popped element by assigning it to some variable 

   eg: popped=courses.pop()

   print(popped) and it returns CompSci

9. **Reverse:-**

   courses.reverse() and print courses

10. **Sort:-**

    courses.sort() and it will print in alphabetic order starting from CompSci and in ascending order for numbers

    For descending, use courses.sort(reverse=True)

    If we want sorted list without altering the original list, use 

    sorted_courses=sorted(courses)

    print(sorted_courses) prints sorted version 

    print(courses) will print courses as it is starting from history.

11. **min,max,sum:-**

    nums=[1,2,3,4,5]

    print(min(nums)) returns 1

12. **Finding index:-**

    print(courses.index('CompSci')) returns 3

    and if the value is not present then it returns **ValueError**

13. **in function:-**

    - It is used to find whether a value is present in list or not and it returns boolean values

      eg:-courses=['History','Math','Physics',CompSci']

      print('Art' in courses) returns false

    - It can also be used in loops

      eg:- for item in courses:

      ​		print(courses)

      output:-

      History

      Math

      Physics

      CompSci

14. **Enumerate function:-**

    To access the index and the value

    ![1547632971624](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547632971624.png)

    ![1547633015666](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547633015666.png)

15. **List into String and vice-versa**:-

    *list into string:-*

    ![1547634081668](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547634081668.png)

    

    *string into list:-*

    by splitting the string that we created using **split()** function

    for eg:-![1547634187132](Chttps://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547634187132.png)

    

    **TUPLES:-**

*Tuples are immutable(can't be modified ) and lists are mutable.*

eg:- ![1547634447180](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547634447180.png)

![1547634500030](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547634500030.png)

- we can't remove or append in tuples as they are immutable and they even have less methods compared to lists.

  **SETS:-**

  - output changes everytime we run the set. 

  - it also removes duplicates

    eg:- ![1547634739455](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547634739455.png)

  - **Membership test:-** used to test whether a value is part of a set. Sets do this a lot more efficiently than lists and tuples. 

    eg:- ![1547634864710](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547634864710.png)

  - They also determine what values they either share or don't share with other sets. 

    - **Intersection:-**

      eg:- ![1547635176896](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547635176896.png)

    - **Difference:-**

      eg:- ![1547635216138](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547635216138.png)

    - **Union:-**

      eg:- ![1547635252940](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547635252940.png)

      ​           

      ​      

**CREATING EMPTY LISTS, TUPLES AND SETS:-**

![1547635334670](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547635334670.png)

