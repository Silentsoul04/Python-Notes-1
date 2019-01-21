EASIER TO ASK FORGIVENESS THAN PERMISSION:

We donot care about the type of the object, whatever we asked to do now.. it has to do. (Pythonic).

The main advantage of it is we can access the object only once rather than using multiple times. First we access it, if it works then it displays otherwise it displays the error.


#Accessing files:

import os

my_file="C:/Users/bpraja/Desktop/git.txt"

'''
if os.access(my_file,os.R_OK):
    with open(my_file) as f:
        print(f.read())
else:
    print("File cannot be accessed")
'''

'''
#The pythonic way
try:
    f=open(my_file)

except IOError as e:
    print(e)
else:
    print(f.read())
'''    

#These are the most pythonic way of approach..

Details={'name':'Praveen','age':21,'job':'employee'}
a=[1,2,3,4]

try:
    print(f"I'm {Details['name']}, age is {Details['age']}, {Details['job']}")
except KeyError as e:
    print(e)
Output:

try :
    print(a[5])
except IndexError as e:
    print(e)

Output:
Index out of range

