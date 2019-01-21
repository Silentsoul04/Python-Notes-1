CSV-Comma separated files

They allow us to put into a plain text file some data and use some type of delimiter usually a comma to separate the different fields.

Comma is  a delimiter(which separate data), delimiter can slo be a tab space etc.

1. Reading CSV file:-

   reader method is using something called dialect that has some preset parameters for what it expects the format of our CSV file to be. So by default its expecting values to be separated by a comma and few other things.

   ![1547968844390](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547968844390.png)

   ![1547968901928](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547968901928.png) 

   ![1547968927947](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547968927947.png)

2. **Writing to a CSV file:-**

   we are using dash(-) as a delimiter

   ![1547969114264](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547969114264.png) 

   o/p:- created a new_names.csv file and its content is 

   ![1547969160392](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547969160392.png) 

   if we use delimiter='\t' then the content is

   ![1547969252257](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547969252257.png) 

   

3. If we forget to mention the delimiter then output is 

   ![1547969335483](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547969335483.png) 

   because it was expecting commas.

   Therefore if we mention delimiter, the output is

   ![1547969381972](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547969381972.png) 

4. **Dictionary Reader:-**

   ![1547969449155](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547969449155.png) 

   ![1547969504950](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547969504950.png)

5. **Dictionary Writer:-**

   code:-

   ![1547969580527](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547969580527.png) 

   o/p:-

   ![1547969608132](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547969608132.png) 

   - eg:- 

     code:-![1547969654139](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547969654139.png) 

     o/p:-

     ![1547969669673](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1547969669673.png) 

     **Dictionary Reader and Writer are more obvious ways than just reader and writer**