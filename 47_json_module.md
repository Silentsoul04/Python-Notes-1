**json module :**

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