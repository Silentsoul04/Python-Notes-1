Context managers are used for efficiently managing resources..
We can create our own context managers..

example:

with open('filename.txt') as f:
f.write("This is the new writing")

Context managers can be defined as class and function..
It is used for connecting and disconnecting the databases..


class open_the_file():
    def __init__(self, filename, mode):
        self.filename=filename
        self.mode=mode


    def __enter__(self):
        self.file=open(self.filename,self.mode)
        return self.file

    def __exit__(self):
        self.file.close()

with open('Example.txt','w') as f:
    f.write('This is sample')

print(f.closed)


Output:
True

Before use of Context Managers:

import os

cwd=os.getcwd()
os.chdir('sample')
print(0s.listdir())
os.chdir(cwd)

After the use of Context Managers:

import os
from contextlib import contextmanager


@contextmanager
def change_dir(destination):
try:
	cwd=os.getcwd()
	os.chdir(destination)
	yield
finally:
	os.chdir(cwd)

with change_dir('Sampl-one'):
print(os.listdir())














