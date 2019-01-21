JavaScript object notation

JSON files are kind of dictionaries.
Load a json string into python object:

data=json.loads(string)

for person in data['people']:
print(person)

Dump a python object to json string:

new_string= json.dumps(data, indent=2)





import json

with open() as f:
 data=json.load(f)

for state in data['states']:
print(state)

with open('new_json.json','w') as f:
json.dump(data,f,indent=2)



**import json**
**from urllib.request import urlopen**

**with urlopen("url") as response:**
**source= response.read()**
**data=json.loads(source)**

**print(json.dumps(data,indent=2))**

