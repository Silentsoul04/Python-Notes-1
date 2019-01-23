# CSV Modules(preetha)

- Simple files used to store tabular data
- Every line is a record

- To open and read
```

		
		for line in csv_reader:
			csv_writer.writerow(line)
```
- Here a new file is created where the comma delimiter in the old file is replaced by a '-' in the new file.
- In case any of the data in any record contains the same delimiter then they are enclosed in quotes.

**csv module :**(aditya)

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
(lalith)
CSV-Comma separated files

They allow us to put into a plain text file some data and use some type of delimiter usually a comma to separate the different fields.

Comma is  a delimiter(which separate data), delimiter can slo be a tab space etc.

1. Reading CSV file:-

   reader method is using something called dialect that has some preset parameters for what it expects the format of our CSV file to be. So by default its expecting values to be separated by a comma and few other things.

   ![1547968844390](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547968844390.png)

   ![1547968901928](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547968901928.png) 

   ![1547968927947](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547968927947.png)

2. **Writing to a CSV file:-**

   we are using dash(-) as a delimiter

   ![1547969114264](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547969114264.png) 

   o/p:- created a new_names.csv file and its content is 

   ![1547969160392](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547969160392.png) 

   if we use delimiter='\t' then the content is

   ![1547969252257](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547969252257.png) 

   

3. If we forget to mention the delimiter then output is 

   ![1547969335483](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547969335483.png) 

   because it was expecting commas.

   Therefore if we mention delimiter, the output is

   ![1547969381972](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547969381972.png) 

4. **Dictionary Reader:-**

   ![1547969449155](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547969449155.png) 

   ![1547969504950](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547969504950.png)

5. **Dictionary Writer:-**

   code:-

   ![1547969580527](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547969580527.png) 

   o/p:-

   ![1547969608132](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547969608132.png) 

   - eg:- 

     code:-![1547969654139](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547969654139.png) 

     o/p:-

     ![1547969669673](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547969669673.png) 

     **Dictionary Reader and Writer are more obvious ways than just reader and writer**

(prvnrj)
```python
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
#next(csv_reader)
csv_writer.writeheader()-#writes the fields name..
for line in csv_reader:
	del line['email']
	csv_writer.writerow(line)
