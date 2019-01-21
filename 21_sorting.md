**Sorting Lists, Tuples, Objects :**

* sort(), sorted().
* Sorting on a custom criteria :

```python3
l=[1,2,3,-6,-4,-5]

s_li=sorted(l)		# [-6,-5,-4,1,2,3]

s_li=sorted(l,key=abs)		#[1,2,3,-4,-5,-6] , key takes a function name
```

* Sorting Objects :

![sorting_objects](images/sorting.PNG)