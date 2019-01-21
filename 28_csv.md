**csv module :**

```python3
# reading a csv 

import csv

with open('names.csv','r') as csv_file:
	csv_reader=csv.reader(csv_file,delimiter=',')			# returns an object
	
for line in csv_reader:
	print(line)								# returns each line of the csv file as list
	
"""
writing into a csv
"""
	with open('new_names.csv','w') as new_file:
		csv_writer=csv.writer(new_file,delimiter='\t')
	
	for line in csv_reader:
		csv_writer.writerow(line)
```