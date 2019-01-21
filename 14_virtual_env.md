**Virtual Environments :**

* Used to separate the packages, dependencies and the versions we would use for different projects.
* Suppose, there are different  projects using different versions of python, and updating the python globally would break down one of them, thus using virtual envs helps us maintain both versions.

```python3
virtualenv env_name : creates a virtualenv

source env_name/bin/activate : activates the virtual env

# Now we can install the packages required into this virtual env.

deactivate : deactivates the virtual env
```