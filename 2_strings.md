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
