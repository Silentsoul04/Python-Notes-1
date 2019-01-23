

# Sorting(preetha)

- A new sorted list
```
list2 = sorted(list1)
```

-  Sorting the list
```
list1.sort()
```

- Sorting the list in descending order 
```
list2 = sorted(list1,reverse=True)
```
```
list1.sort(reverse=True)
```

- Using a key 
```
sorted_list = sorted(list_1, key=abs)
```

**Sorting Lists, Tuples, Objects :**  (aditya)

* sort(), sorted().
* Sorting on a custom criteria :

```python3
l=[1,2,3,-6,-4,-5]

s_li=sorted(l)		# [-6,-5,-4,1,2,3]

s_li=sorted(l,key=abs)		#[1,2,3,-4,-5,-6] , key takes a function name
```

* Sorting Objects :

![sorting_objects](images/sorting.PNG)

(lalith)
**Sorting lists:-**

1. ![1547785181934](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547785181934.png)

   o/p:-![1547785198633](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547785198633.png) 

2. ![1547785238676](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547785238676.png)

3. ![1547785282026](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547785282026.png)

4. ![1547785329784](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547785329784.png)

   **Sorted method is better** than sort method as it gives us the **flexibility** because we can pass in any iterable as opposed to sort method which works specifically on lists.

   **Sorting tuples**  eg:- ![1547785898769](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547785898769.png) 

   so we need to use sorted as shown below

   ![1547785939920](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547785939920.png)

   **Sorting dictionaries:-**

   ![1547786044108](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547786044108.png) 

   this sorts only keys in ascending order.

   **Overall examples:-**

   

   ![1547786216127](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547786216127.png) 

   o/p:- ![1547786238233](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547786238233.png)

   **Sorting objects:-**

   1. ![1547787074081](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547787074081.png) 

      ![1547787108103](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547787108103.png)

      So we need to sort against an attribute in the object. Hence we use key.

   2. ![1547787157871](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547787157871.png) 

      this is based on name

      ![1547787178712](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547787178712.png) 

      this is based on age

      ![1547787253893](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547787253893.png) 

      this is based on salary.

   3. we can also sort them by using **lambda**

      ![1547787298134](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547787298134.png)

      

   4. we can also sort by using **attrgetter**

      ![1547787333737](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547787333737.png)

   

