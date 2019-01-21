# JSON

- Very common data format for storing information.
- Fetching data from nline API
- Used for coniguration of files and different kinds of data storage on local machine.
- Stands for Java Script Object Notation.

```
data = json.loads(people_string)
```

- Object to dict
- array to list
- string to str
- null to none
```
with open('states.json') as f:
	data = json.load(f)
	
for state n data['states']:
	print(state['name'])
```
