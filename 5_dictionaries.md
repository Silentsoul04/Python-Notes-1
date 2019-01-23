# Dictionaries(preetha)

- keys:		
> `print(dict_name.keys())`

- values:		
> `print(dict_name.values())`

- keys and values:	
> `print(dict_name.items())`

**Dictionary :**(aditya)

* Key-Value pairs
* Values can be any data types and keys are usually strings but can be any other mutable data types.
* Declaration :

```python3
student={'name':'Aditya','age':21,'courses':['math','physics']}

print(student) #{'name': 'Aditya', 'age': 21, 'courses': ['math', 'physics']}

> print(student['name'])	# Aditya
  print(student['gender'])	# Key error
  
> print(student.get('name'))	# Aditya
  print(student.get('gender'))	# None
  print(student.get('gender','not found'))	# not found
```

* Adding to a dictionary :

```python3
student={'name':'Aditya','age':21,'courses':['math','physics']}

> student['gender']='male'
  print(student)   #{'name': 'Aditya', 'age': 21, 'courses': ['math', 						   #'physics'], 'gender': 'male'}

Note : Updating the value of an existing key overwrites the existing value.
```

* Updating a dictionary :

```python3
student={'name':'Aditya','age':21,'courses':['math','physics']}

> Single values can be updated by overwriting the existing values.

> student.update({'name':'Adi','phone':'1234567'})	# updates multiple values
  print(student)
  """
  {'name': 'Adi', 'age': 21, 'courses': ['math', 'physics'], 'phone': '1234567'}
  """
```

* Deleting a key-value pair :

```python3
student={'name':'Aditya','age':21,'courses':['math','physics']}

age=student.pop('age')
print(student)  # {'name': 'Aditya', 'courses': ['math', 'physics']}
```

* Misc :

```python3
student={'name':'Aditya','age':21,'courses':['math','physics']}

> print(student.keys())	# prints all the keys
> print(student.values()) # prints all the values
> print(len(student))	# length of the dictionary
> print(student.items())	# list of key-value pairs

# Looping through a dictionary :

for key,value in student.items():
	print(key,value)
```
(lalith)
**DICTIONARIES:-**

1. **Creation:-**

   ![1547636004600](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547636004600.png)              

2. **Accessing:-**

   ![1547636050718](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547636050718.png)       

   *We get keyError if we try to access key which is not present*

   - **Get method:-** we can get none instead of error if we access key which is not present.

     eg:- 1.![1547636209725](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547636209725.png)

     2. we can assign the value to be printed if we don't find the key

        ![1547636326275](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547636326275.png)

     

3. **Adding:-**

   ![1547636422271](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547636422271.png)

4. **Updating:-**

   Using update method

   eg:- ![1547636517285](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547636517285.png)

5. **Deleting:-**

   - using del keyword

     eg:-![1547636662877](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547636662877.png)

   - using pop keyword

     eg:- ![1547636970504](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547636970504.png)

    

6. **Length:-**

   use print(len(student)) and it prints 3 bcoz we have 3 keys

7. **To find keys:-**

   print(student.keys()) it returns dict_keys(['name','age','courses'])

8. **To find values:-**

   print(student.values()) it returns

   dict_values(['John',25,['Math',CompSci']])

9. **To find both keys and values:-**

   print(student.items()) it returns

   dict_items([('name','John'),('age',25),('courses',['Math',CompSci'])])

10. **Looping:-**

    - for key in student:

      print(key)

      output:-name

      age

      courses

    - ![1547637423567](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547637423567.png)

    ​	
>
(prvnrj)
Instead of using indexing method to access the key-value pairs, it is better to use the get method to access the key-value. If incase key-value is not available, this get method function returns the None.

>>> d={1:'a',2:'b'}
>>> d.get(1)
'a'
>>> d.get(3)
>>> d[3]='c'
>>> d
{1: 'a', 2: 'b', 3: 'c'}
>>> d.update(1:'A',2:'B',3:'C')
SyntaxError: invalid syntax
>>> d.update(1='A',2='B',3='C')
SyntaxError: keyword can't be an expression
>>> d.update({1:'A',2:'B',3:'C'})
>>> d
{1: 'A', 2: 'B', 3: 'C'}
>>> d.get(4,"Not found")
'Not found'
>>> del d[2]
>>> d
{1: 'A', 3: 'C'}
>>> d.update({1:'A',2:'B',3:'C'})
>>> popped=d.pop()
Traceback (most recent call last):
  File "<pyshell#104>", line 1, in <module>
    popped=d.pop()
TypeError: pop expected at least 1 arguments, got 0
>>> popped=d.pop(2)
>>> d
{1: 'A', 3: 'C'}
>>> d.update({1:'A',2:'B',3:'C'})
>>> d.keys()
dict_keys([1, 3, 2])
>>> d.values()
dict_values(['A', 'C', 'B'])
>>> d.items()
dict_items([(1, 'A'), (3, 'C'), (2, 'B')])
>>> for key in d:
  print(key)

  
1
3
2
>>> for key,values in d.items():
  print(key,value)

  
Traceback (most recent call last):
  File "<pyshell#116>", line 2, in <module>
    print(key,value)
NameError: name 'value' is not defined
>>> for key,values in d.items():
  print(key,values)

  
1 A
3 C
2 B
>>> for key in d:
  print(d[key])

	
A
C
B
