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
