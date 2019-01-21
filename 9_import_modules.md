**Importing Modules :**

* Syntax :

```pytho3
import module_name 
```

* The module is first looked for in the current directory, followed by other standard library directories.
* To look at the directories which are searched :

```python3
import sys

print(sys.path)
```

* In case, the module needed isn't in the working directory, but in some other directory on the system, the path to that module must be added to the sys.path.
* It can be added either by appending to sys.path list manually, otherwise, for windows, an environment variable with name PYTHONPATH can be set up.