
# Import Modules and Standard Libraries (preetha)

- from sys.path
```
import module_name
```

- from elsewhere
``` 
sys.path.append('location')
```

- Renaming
 ```
 import module_name as alias
 ```

- importing function from a module
```
from module_name import func_name
```

- importing variable from a module
``` 
from module_name import func_name, var_name
```

## Examples
- math
> math.radians(val)
> math.sin(val)

- datetime
> datetime.date.today()

- calender
> calender.isleap(2020)

- OS
> os.getcwd() 

**Importing Modules :**  (aditya)

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
