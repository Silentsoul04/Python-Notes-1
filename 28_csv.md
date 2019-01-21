import csv

with open('file.csv','r') as csv_file:
	csv_reader = csv.reader(csv_file)
	with open('newfile.csv','w') as new_file:
		csv_writer=csv.writer(new_file,delimiter="-")
	#next(csv_reader)
	for line in csv_reader:
		csv_writer.writerow(line)

if needed delimiter can be "\t"
if delimiter is changed from comma to any other thing then it should be passed as delimiter argument.

csv.reader(new_file, delimiter="-")

csv.DictReader(new_file) - where keys are fields and values are field values

line['email']

import csv

with open('file.csv','r') as csv_file:
	csv_reader = csv.DictReader(csv_file)
	with open('newfile.csv','w') as new_file:
		fieldnames=['f_name','last_name','email'] #first row.
		csv_writer=csv.DictWriter(new_file,fieldnames=fieldnames,delimiter="-")
		
```python
#next(csv_reader)
csv_writer.writeheader()-#writes the fields name..
for line in csv_reader:
	del line['email']
	csv_writer.writerow(line)
```