
# Use underlying operating System Functionality(preetha)

- OS modules are used to interact with the underlying Operating system.
- It is used to navigate the file system.
- Get file information.
- Look up and chane environment variables.

**OS Module :**(aditya)

* Used to  utilise the functionality of the underlying operatig system.
* import OS
(lalith)
**OS module is imported to navigate file system,get file info, move files or change environment variables etc. **

1. import os

   print(dir(os))

   o/p:-shows all of attributes and methods that we have access to within this module

   ![1547795006464](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547795006464.png) 

2. for current directory:-

   print(os.getcwd())

3. for changing directory:-

   os.chdir('<path>')

   ![1547795154664](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547795154664.png)

4. for listing files and folders in directory:-

   print(os.listdir())

5. creating folder on desktop:-

   - os.mkdir('<folder name>')

     or

   - os.mkdirs('<folder name>')

     mkdirs helps us to create intermediate levels of directory but we can't do that with mkdir

     ![1547795389631](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547795389631.png)

     

6. removing/deleting folders:-

   os.rmdir('<folder name>')

   os.rmdirs('<folder name>')

   ![1547795695454](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547795695454.png)

7. renaming:-

   os.rename('<original file','final file')

8. to know info about file use os.stat('filename') and print it.

9. print(os.stat('filename').st_size) for size of file.

10. st_mtime is modification time. But as it is not understood we can use datetime to print the time and other timestamps.

    ![1547809163914](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547809163914.png)

11. os.walk() is a generator that yields a couple of three values as its walking the directory service and is used to obtain list of all files and directories in the path. 

    ![1547809513275](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547809513275.png) 

    <!--refer video for more clarification if needed-->

12. os.environ for getting environment variables

    ![1547809645043](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547809645043.png) 

    

13. os.path is used for finding path and also to combine home directory with the filename as shown below.

    ![1547809811831](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547809811831.png) 

    

14. os.path.basename('path') gives the basename of the path as shown below

    ![1547809952750](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547809952750.png)

    to get dir name, use:- os.path.dirname()

    ![1547810036131](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547810036131.png)

    to get both use split which prints dirname first and base name second

    ![1547810054071](Chttps://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547810054071.png)

15. os.path.exists() to check if a path exists

    ![1547810096128](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547810096128.png)

16. to know if something is a file or not, use isdir and isfile as shown in below pictures

    ![1547810173980](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547810173980.png) 

    ![1547810187675](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547810187675.png) 

    

17. os.path.splitext() it splits root of the path and extension

    ![1547810244378](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547810244378.png)

18. If you want to see everything that is available within the OS path module then use print(dir(os.path))

     ![1547810338622](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547810338622.png)

(prvnrj)

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
