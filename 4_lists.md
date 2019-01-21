*Lists and tuples help us to work with sequential data and sets are unordered collection of values with **NO** duplicates.*

**LISTS:-**

1. creation:-

    courses=['History','Math','Physics',CompSci]

   print(courses)

   it prints ['History','Math','Physics',CompSci]

2. Length:-

   print(len(courses))

   it returns 4

3. print(courses[0]) returns History

4. negative index start from the last of list

   i.e., print(courses[-1]) prints CompSci

   *Negative indexes are useful in printing final element in list*

5. You get an index error if u try to access an index that doesn't exist 

   eg:-print(courses[4]) returns index out of range

6. **Slicing:-**print(courses[0:2]) prints ['History','Math']

7. **Adding:-** 

   - using append:-

     courses.append('Art') adds art into courses

   - using insert:-

     courses.insert(0,'Art')

     it returns ['Art','History','Math','Physics',CompSci']

   - using extend:-

     courses=['History','Math','Physics',CompSci]

     courses_2=['Art','Education']

     courses.insert(0,courses_2) and printing it gives [['Art','Education'],History','Math','Physics',CompSci']

     so we use extend method i.e.,

     courses.extend(courses_2) and print them. U will get ['History','Math','Physics',CompSci','Art','Education']

8. **Remove:-**

   courses.remove('Math')

   or

   courses.pop()-pops last element from list 

   eg:-compsci in this example of history math physics and compsci

   we can also print the popped element by assigning it to some variable 

   eg: popped=courses.pop()

   print(popped) and it returns CompSci

9. **Reverse:-**

   courses.reverse() and print courses

10. **Sort:-**

    courses.sort() and it will print in alphabetic order starting from CompSci and in ascending order for numbers

    For descending, use courses.sort(reverse=True)

    If we want sorted list without altering the original list, use 

    sorted_courses=sorted(courses)

    print(sorted_courses) prints sorted version 

    print(courses) will print courses as it is starting from history.

11. **min,max,sum:-**

    nums=[1,2,3,4,5]

    print(min(nums)) returns 1

12. **Finding index:-**

    print(courses.index('CompSci')) returns 3

    and if the value is not present then it returns **ValueError**

13. **in function:-**

    - It is used to find whether a value is present in list or not and it returns boolean values

      eg:-courses=['History','Math','Physics',CompSci']

      print('Art' in courses) returns false

    - It can also be used in loops

      eg:- for item in courses:

      ​		print(courses)

      output:-

      History

      Math

      Physics

      CompSci

14. **Enumerate function:-**

    To access the index and the value

    ![1547632971624](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547632971624.png)

    ![1547633015666](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547633015666.png)

15. **List into String and vice-versa**:-

    *list into string:-*

    ![1547634081668](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547634081668.png)

    

    *string into list:-*

    by splitting the string that we created using **split()** function

    for eg:-![1547634187132](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547634187132.png)

    

    **TUPLES:-**

*Tuples are immutable(can't be modified ) and lists are mutable.*

eg:- ![1547634447180](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547634447180.png)

![1547634500030](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547634500030.png)

- we can't remove or append in tuples as they are immutable and they even have less methods compared to lists.

  **SETS:-**

  - output changes everytime we run the set. 

  - it also removes duplicates

    eg:- ![1547634739455](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547634739455.png)

  - **Membership test:-** used to test whether a value is part of a set. Sets do this a lot more efficiently than lists and tuples. 

    eg:- ![1547634864710](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547634864710.png)

  - They also determine what values they either share or don't share with other sets. 

    - **Intersection:-**

      eg:- ![1547635176896](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547635176896.png)

    - **Difference:-**

      eg:- ![1547635216138](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547635216138.png)

    - **Union:-**

      eg:- ![1547635252940](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547635252940.png)

      ​           

      ​      

**CREATING EMPTY LISTS, TUPLES AND SETS:-**

![1547635334670](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547635334670.png)