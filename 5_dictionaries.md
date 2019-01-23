# Dictionaries(preetha)

- Syntax: 
>`dict_name={'key':value,....}`

- To print:	
> `print(dict_name['key'])`
> `print(dict_name.get(key))`
> `print(dict_name.get(key,'message'))`

- To edit:		
>`dict_name.update({key:value})`

- To delete:	
> `del.dict_name[key]`
> `dict_name.pop(key)

- no.of keys:	
> `print(len(dict_name))`

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
