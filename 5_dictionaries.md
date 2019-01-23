
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
