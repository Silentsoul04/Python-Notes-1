# Parsing Names from a csv to html

```
import csv
html_output = ''
names = []
with open('patrons.csv','r') as data_file:
	csv_data = csv.reader(data_file)
	
	#To avoid headers and first line of bad data
	next(csv_data)
	next(csv_data)
	
	for line in csv_data:
		names.append(f"{line[0]} {line[1]}")
	
html_output += f'<p>There are currently {len(names)} public contributors. Thank you. <p>'

html_output += '\n<ul>'

for name in names:
	html_output += f'\n\t<li>{name}</li>'
	
html_output += '\n</ul>'

print(html_output)
```

- This program parses the contributors' names from csv file to html.