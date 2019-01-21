**working with variables:-**

1. use descriptive variables.

   example:-

![1547615240373](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547615240373.png)

​	or my_message.

2. we can use double quotes if we need single quotes in the string to be printed and vice-versa

   example:-message="hello bobby's world"

   or we can use backslash as well

   example:-![1547615562252](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547615562252.png)

3. for using multiple lines,  add three quotes to the beginning and ending

   example:-![1547615749998](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547615749998.png)

4. for finding length of a string, use **len** function.

![1547615912398](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547615912398.png)

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

     

![1547617987403](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547617987403.png)

- print(help(str))-to get information regarding string class. Help function is used only for classes. we can also use print(help(str.lower)) to get information regarding lower function.
