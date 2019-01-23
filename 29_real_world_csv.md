

# Parsing Names from a csv to html



- This program parses the contributors' names from csv file to html.
(lalith)
**csv module is better than using split method.**

- instead of using for loop, we can also use print(list(csv_data)) but it is not readable.

  <!--Check video for the example-->

(prvnrj)
import csv

name=[]
html_output=''

with open('file.csv','r') as open_file:
    csv_read=csv.reader(open_file)

```python
next(csv_read) #first line contains the headers
next(csv_read) #goes to the next line as it is a bad line

for line in csv_read:
    if line[0]=='No reward':
        break or continue
    name.append(f'{line[0] line[1]}')

html_output+=f'<p>There are {len(name)}</p>'
html_output+='\n<ul>'
for n in names:
    html_output+=f'\n\t<li>{name}</li>'
html_output+='\n</ul>'
print(html_output)

with open('file.csv','r') as open_file:
    csv_read=csv.DictReader(open_file)

```python
#next(csv_read) #first line contains the headers
next(csv_read) #goes to the next line as it is a bad line

for line in csv_read:
    if line['first name']=='No reward':
        break or continue
    name.append(f'{line["first name"] line["second name"]}')

html_output+=f'<p>There are {len(name)}</p>'
html_output+='\n<ul>'
for n in names:
    html_output+=f'\n\t<li>{name}</li>'
html_output+='\n</ul>'
print(html_output)
```

