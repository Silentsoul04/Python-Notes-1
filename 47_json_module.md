# JSON (preetha)

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

**json module :** (aditya)

```python3
import json

# suppose people_string contains a json string

data=json.loads(people_string)		# returns the string data into a dict
# work with the data
new_string=json.dumps(data)			# modified json string obtained from data
# use json.dumps(data,indent=2) for better readability
# states.json is a json file

with open('states.json') as f:
	data=json.load(f)
# work with the data and write it down into a new json file
with open('new_states.json') as f:
	json.dump(data,f)
```
