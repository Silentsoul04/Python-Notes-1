# 2 Strings (Content by Preetha)

- Textual data- Strings
- Enclosed in single or double quotes
- len() returns the length of the string
- To access a range of characters
> name_of_string[starting_index:end_index]
> when the index positions are left emppty then it is taken as the very beginning and end.

- Functions on string
> upper()
> lower()
> count(substring)
> find(substring)
> replace(prev_substring, new_substring)

- Formatted strings
> message = '{}, {}'.fromat(message1,message2)

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

