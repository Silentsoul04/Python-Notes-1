# CSV Modules

- Simple files used to store tabular data
- Every line is a record

- To open and read
```
import csv
with open('names.csv','r' as csv file:
	csv_reader = csv.reader(csv_file)
	for line in csv_reader:
		print(line[1])
```
- Here, names is a csv file that has first name, email and last name separated by a comma. The above program will print the first index or in this case the first name of all the records.

- To write
```
import csv
with open('names.csv','r' as csv file:
	csv_reader = csv.reader(csv_file)
	
	with open('new_names.csv','w') as new_file:
		csv_writer = csv.writer(new_file, delimiter = '-')
		
		for line in csv_reader:
			csv_writer.writerow(line)
```
- Here a new file is created where the comma delimiter in the old file is replaced by a '-' in the new file.
- In case any of the data in any record contains the same delimiter then they are enclosed in quotes.