**OS module is imported to navigate file system,get file info, move files or change environment variables etc. **

1. import os

   print(dir(os))

   o/p:-shows all of attributes and methods that we have access to within this module

   ![1547795006464](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547795006464.png) 

2. for current directory:-

   print(os.getcwd())

3. for changing directory:-

   os.chdir('<path>')

   ![1547795154664](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547795154664.png)

4. for listing files and folders in directory:-

   print(os.listdir())

5. creating folder on desktop:-

   - os.mkdir('<folder name>')

     or

   - os.mkdirs('<folder name>')

     mkdirs helps us to create intermediate levels of directory but we can't do that with mkdir

     ![1547795389631](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547795389631.png)

     

6. removing/deleting folders:-

   os.rmdir('<folder name>')

   os.rmdirs('<folder name>')

   ![1547795695454](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547795695454.png)

7. renaming:-

   os.rename('<original file','final file')

8. to know info about file use os.stat('filename') and print it.

9. print(os.stat('filename').st_size) for size of file.

10. st_mtime is modification time. But as it is not understood we can use datetime to print the time and other timestamps.

    ![1547809163914](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547809163914.png)

11. os.walk() is a generator that yields a couple of three values as its walking the directory service and is used to obtain list of all files and directories in the path. 

    ![1547809513275](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547809513275.png) 

    <!--refer video for more clarification if needed-->

12. os.environ for getting environment variables

    ![1547809645043](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547809645043.png) 

    

13. os.path is used for finding path and also to combine home directory with the filename as shown below.

    ![1547809811831](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547809811831.png) 

    

14. os.path.basename('path') gives the basename of the path as shown below

    ![1547809952750](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547809952750.png)

    to get dir name, use:- os.path.dirname()

    ![1547810036131](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547810036131.png)

    to get both use split which prints dirname first and base name second

    ![1547810054071](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547810054071.png)

15. os.path.exists() to check if a path exists

    ![1547810096128](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547810096128.png)

16. to know if something is a file or not, use isdir and isfile as shown in below pictures

    ![1547810173980](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547810173980.png) 

    ![1547810187675](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547810187675.png) 

    

17. os.path.splitext() it splits root of the path and extension

    ![1547810244378](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547810244378.png)

18. If you want to see everything that is available within the OS path module then use print(dir(os.path))

     ![1547810338622](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547810338622.png)