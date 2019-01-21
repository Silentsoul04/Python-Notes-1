Generators are used for better performance as it boosts. No memory is wasted. It is same before and after.



>>> def square(alist):
			 num=[]
			 for n in alist:
				 num.append(n*n)
			 return num


>>> blist=[1,2,3,4,5]

>>> my=square(blist)

>>> print(my)

[1, 4, 9, 16, 25]
>>> 

>>> def square(alist):
			 num=[]
			 for n in alist:
				 yield(n*n)


>>> blist=[1,2,3,4,5]

>>> my=square(blist)

>>> print(my)

<generator object square at 0x0333DD70>
>>> next(my)

1
>>> next(my)

4
>>> my=(n*n for n in nums)

Traceback (most recent call last):
  File "<pyshell#52>", line 1, in <module>
    my=(n*n for n in nums)
NameError: name 'nums' is not defined

>>> my=(n*n for n in blist)   #one way of declaring the generator
>>> def people(num):
			 result=[]
			 for i in range(num):
				 people={'id':i,
			 'name':random.choice(names),'major':random.choice(majors)}
				 result.append(people)
			 return result


>>> def people_generator(num):
			 for i in range(num):
				 people={'id':i,
			 'name':random.choice(names),'major':random.choice(majors)}
			yield people