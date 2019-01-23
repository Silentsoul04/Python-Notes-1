
# 2 Strings (Content by Preetha)



- F strings
> message= f'{var1},{var2}'


**Strings** (Content by Aditya)

* series ( or an array ) of characters.

```python3
# declaration

> message='Hello World'    # single line strings

> message='Bobby's World'  	# error1
  message= "Bobby's World" 	# solution1

> message=""" hello
  world """                    # multiline string

> length=len(message)  		# length of string

> first_character= message[0]			# indexing string characters
```

* Methods :

```python3
msg="Hello"

> print(msg.lower())		# hello

> print(msg.upper())		# HELLO

> print(msg.count('l'))		# 3, counts the no. of occurrences of the substr
  print(msg.count('Hell'))	# 1

> print(msg.find('ello'))	# 1, gives start index of substr else -1
  print(msg.find('hello'))	# -1
  
> new_msg=msg.replace('e','a')
  print(new_msg)				# Hallo
  print(msg)					# Hello
```

* Concatenation :

```python3
greetings="Hello"
name="World"

> msg=greetings+' '+name
  print(msg)				# Hello World
"""
Useful for shorter strings, gets cluttered and messy for longer concats
"""

> msg='{},{}. Welcome!'.format(greetings,name)
  print(msg)			# Hello,World. Welcome!
"""
Easier and more readable during longer concats.
{} is used as a placeholder.
"""

> msg=f'{greetings},{name}. Welcome!'
  print(msg)			# Hello,World. Welcome!
"""
These are called f-strings.
Applicable only for python versions starting from 3.6
"""
```

(lalith)
**working with variables:-**

1. use descriptive variables.

   example:-

![1547615240373](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547615240373.png)

​	or my_message.

2. we can use double quotes if we need single quotes in the string to be printed and vice-versa

   example:-message="hello bobby's world"

   or we can use backslash as well

   example:-![1547615562252](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547615562252.png)

3. for using multiple lines,  add three quotes to the beginning and ending

   example:-![1547615749998](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547615749998.png)

4. for finding length of a string, use **len** function.

![1547615912398](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547615912398.png)

5. print(message[10]) then it prints **d** in hello world example 

6. **slicing:-**

   message[0:5] prints hello <!--it doesnt include 5th index character-->

   message[6:] prints world

7. Method is a function that belongs to a particular object

8. **functions on strings:-**

   - message.lower()-prints the message in lower case

   - message.upper()-prints the message in upper case

   - message.count()-count certain no. of characters

     eg:-count('l') in hello world gives 3 as output

   - message.find('world') gives 6 as output. if we some other string other than present string then it returns -1 eg:- find('universe') it returns -1 as we have only hello world.

   - message=message.replace('world','universe') to replace a word. it prints hello <!--assigning is necessary-->

   - **concatenation:-**

   1. message=greeting+name returns hellomichael where greeting='hello' and name='michael'. 

   2. message=greeting + ', ' + name + '. Welcome!' It prints hello, michael. Welcome!

   3. **string formatting:-** 

      we can also use place orders i.e., {}

      example:- message='{}, {}. Welcome!'.format(greeting,name)

   - **f strings:-**

     used to simplify string formatting.

     eg:-message=f'{greeting}, {name}. Welcome!'

     it prints same as above

     **advantage:-**we can directly use string functions inside brackets.

     eg:-{name.upper()} in above example.

     

     **dir variable**:-

     

![1547617987403](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547617987403.png)

- print(help(str))-to get information regarding string class. Help function is used only for classes. we can also use print(help(str.lower)) to get information regarding lower function.

(prvnrj)

>>> m1='Hi Prvn\'s frnd'
>>> print(m1)
Hi Prvn's frnd

Backslash character is used as escape character for '.
Double quotes can also be used.
For multiline strings triple quotes are used.

Methods and functions are basically the same thing.
Method is a function type specific to the object.

varaible_name.lower()-lowers the character.
variable_name.upper()
variable_name.count()-counts the string
variable_name.find()-returns the index
variable_name.replace(word_to_replace,word_to_be_replaced)- returns the replaced string but will never change the original string

'+' is used as concatenation operator

>>> greeting="hello"
>>> name="Praveen"
>>> greeting+name
'helloPraveen'

NOTE: It doesn't add any space.

>>> '{}. {}'.format(greeting,name)
'hello. Praveen'
>>> f'{greeting}. {name}'
'hello. Praveen'

