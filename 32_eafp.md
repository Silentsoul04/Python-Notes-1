Pythonic means following conventions and coding styles of the python language in order to write clean and readable code.

Two aspects of being pythonic:-

1. Duck Typing
2. Easier to ask forgiveness than permission.



1. **Duck Typing:-** It is called duck typing because the object walks like a duck and quacks like a duck then its a duck. It means we simply don't care what type of object we're working with instead we only care if our object can do what we asked it to do.

   eg:-1. Not a ducktyping example

   ![1547974842084](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547974842084.png) 

   o/p:-

   ![1547974892019](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547974892019.png)

   2. Example for ducktyping:-

      ![1547974935234](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547974935234.png)

   so it is dangerous because we may pass just any object that will potentially throw an error . So we place some checks to make sure that those quack and fly method exist. So this is where EAFP concept come into place.

2. **EAFP:-**

   1. **Non-pythonic way:-** it is called as look before you leap.

      ![1547975272526](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547975272526.png) 

      

   2. pythonic way:- This is called EAFP

      ![1547975330188](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547975330188.png) 

      another example:-

      ![1547975476778](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547975476778.png)



3. Another example:- 

   1. Non-pythonic way:-

      ![1547975632311](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547975632311.png) 

      ![1547975688567](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547975688567.png)

   2. Pythonic way:-

      ![1547975766261](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547975766261.png) 

      ![1547975804598](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547975804598.png) 

4. Example with lists:-

   1. Non-pythonic way:-

      ![1547975906094](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547975906094.png)

   2. Pythonic way:-

      ![1547975949018](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547975949018.png)

**Adv of EAFP**:-1. It is faster in situations where you don;t have so many exceptions.

2. It is more readable.

3. It can also handle race condition

   eg:-

   ![1547976845299](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547976845299.png)
