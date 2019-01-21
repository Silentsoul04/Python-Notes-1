**LEGB variable scopes :**

* Whenever a variable is used,  its existence is checked in the following order : L(local), E(enclosing), G(global), B(built-in).
* The enclosing variables can be accessed for a nested function using the nonlocal keyword as follows:

![nonlocal](images/nonlocal.PNG) 



**Note :** For slicing, the positive and the negative indices can be mixed up and used together.