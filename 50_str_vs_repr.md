
# str() and repr() (preetha)

## str()
- Returns a string containing a nicely printable representation of an object.
- It's goal is to print a string. if no values are passed then an empty string is printed.
- It does not always attempt to return a string that is acceptable to eval().
- The goal is to be readable.

## repr()
- Returns a string containing a printable representation of an object.
- It attempts to return a string same as eval() would.
- The goal is to be unambiguous.
- 

**__str__() vs __repr__() :** (aditya)

* goal of str() is to be readable.
* goal of repr() is to be unambiguous.

![str_vs_repr](images/str_vs_repr.PNG)
(lalith)
1. ![1548007076170](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1548007076170.png) 

2. ![1548007109611](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1548007109611.png) 

   ![1548007123952](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1548007123952.png) 

3. ![1548007196979](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1548007196979.png) 

   Unambiguous means it looks more like a python command if we copy and paste.

   ![1548007319923](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1548007319923.png) 

   the above picture is in command prompt.

4. ![1548007379251](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1548007379251.png) 

5. **repr is meant for developers and str is meant for end-users(user-friendly).**

