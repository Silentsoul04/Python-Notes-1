import os
from datetime import datetime
#os.chdir(''-changes the directory address)
print(os.getcwd())
print(dir(os))

print(os.listdir())

os.mkdir('folder name')- makes a directory only one
os.makedirs('folder name 2\sub folder')- makes many folders

os.rmdir()- removes the single directory (recommended)
os.removedirs('')-removes more than one folder (dangerous)

os.rename('filename to be renamed','renamed file')

os.stat('filename.filetype').st_size
time_stamp=os.stat('filename.filetype').st_mtime

print(datetime.fromtimestamp(mod_time))

from dirpath, dirname, filenames in os.walk(os.getcwd()):
    print() #prints all kind of directories and folders present in the folder. Gives a tree structure of the files in it.

file_path = os.path.join(os.environ.get('HOME'),'test.txt')

os.path.basename('')
os.path.dirname('')
os.path.split('')- #it splits the basename and dirname
os.path.exists()-checks the path returns boolean values
os.path.isdir()
os.path.splitext()-splits the extension
dir(os.path)