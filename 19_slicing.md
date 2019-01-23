# Slicing lists and strings(preetha)

```python
a=[9,8,5,4,5,5,9,8,3,5,5]
```
list_name[start:end:step]
```
-  step and idices can be either positive or negative
-  When left blank they are by default the very beginning, end and 1 respectively

**Slicing :**(aditya)

```python3
msg="Hello"

> print(msg[0:2])      # He

> print(msg[:4])		# Hell

> print(msg[0:])		# Hello


courses = ['math','physics','chemistry','biology']

> print(courses[0:2])		# math physics

> print(courses[-1])		# biology; negative sign indicates indexing from 							 # backwards


```

(lalith)
**slicing lists:-**

![1547714445817](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547714445817.png)

![1547714467511](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547714467511.png)

![1547714496203](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547714496203.png)

entire list in reverse:-

![1547714537568](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547714537568.png)

**Slicing Strings:-**

![1547714591850](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547714591850.png)

![1547714676501](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547714676501.png)

(prvnrj)
index:
   0,1,2,3,4,5,6,7,8,9,10
   -11,-10,-9,-8,-7,-6,-5,-4,-3,-2,-1
a[start:end:increment]

>>> a=[9,8,5,4,5,5,9,8,3,5,5]

>>> a[-9:8]

[5, 4, 5, 5, 9, 8]

>>> a[-9:8:-1
      ]

[]
>>> a[-9:8:-1]

[]
>>> a[-9:-8:-1]

[]

>>> a[-9:-11:-1]

[5, 8]

>>> a[-9::-1]

[5, 8, 9]

>>> a[::-1]

[5, 5, 3, 8, 9, 5, 5, 4, 5, 8, 9]

>>> a[::
      ]

[9, 8, 5, 4, 5, 5, 9, 8, 3, 5, 5]

