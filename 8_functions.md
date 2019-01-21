1. Functions are designed to perform a specific task , they help us to **reuse the code** and they are created by using def keyword which stands for definition. 

   **Pass keyword** is used to not to throw any errors for leaving it blank and we would like to fill the space at a later point in time

   eg:- ![1547640419342](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547640419342.png)

   ![1547640502517](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547640502517.png)

2. **Keeping your code dry:-**Don't repeat yourself.

3. If you call function which is returning something but we didn't assign the function call, then it prints nothing

   eg:-![1547641059483](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547641059483.png)

   else:-

   ![1547641083744](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547641083744.png)

   We can also perform string operations on above print function as shown print(hello_func().upper()) . It returns the string in upper case.

   **Passing Arguments:-**

   1. ![1547649270199](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547649270199.png)

2. *Default Arguments:-*

   ![1547649520434](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547649520434.png)

   

   ![1547649603666](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547649603666.png)

3. *Positional or keyword arguments:-*

   **Positional arguments have to come before keyword arguments**

   ![1547649809271](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547649809271.png)

   *args is positional arguments and **kwargs is keyword arguments. we use * as we don't know the number of arguments and names need not be args and kwargs. But as it is a convention we use these names. 

   - we use * and ** in below picture while calling to unpack the positional and keyword values

     ![1547650073209](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547650073209.png)

   **Example:-**

   - **docstrings** help document what a function or a class is supposed to do. for example """return true for leap years........""" in below picture.

     ![1547650527616](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547650527616.png) 
