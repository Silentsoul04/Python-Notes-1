1. JSON is a common data format for storing some information. JSON is used a lot when fetching data from online API's , also used for configuration files and different kinds of data can be saved on your local machine.

2. JSON stands for **Java Script Object Notation** because it was inspired by java script but it is now independent of an language.

3. Every language these days have libraries for parsing and generating JSON data.

4. eg:-python string that happens to be valid JSON

   ![1548002833495](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1548002833495.png) 

   It is a multi line string. 

5. Loading above thing into python object so that we can work with data more easily:-

   json.loads("string name") method is used.

   ![1548002970399](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1548002970399.png) 

   if we print(type(data)) it returns 

   <class 'dict'> as output.

6. conversion table used while loading json into an object:-

   ![1548003080547](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1548003080547.png) 

   ![1548003158474](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1548003158474.png) 

7. ![1548003196079](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1548003196079.png) 

   ![1548003224525](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1548003224525.png) 

8. Dumping python object into a JSON string:-

   json.dumps() method is used.

   ![1548003322746](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1548003322746.png) 

   here we are deleting phone and then performing dumping.

   If we want to make it readable we pass indent in arguments as shown below:-

   ![1548003405757](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1548003405757.png) 

   intended:-for each level it is intended 2 times

   ![1548003461106](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1548003461106.png) 

   ![1548003491903](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1548003491903.png) 

   ![1548003443367](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1548003443367.png) 

9. Soring keys when dumped into json:-

   ![1548003547364](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1548003547364.png) 

10. Loading json files into python objects:-

    json file is in the same directory where python script is present in this example.

    json.load() method is used to load json file into python object whereas json.loads() for json string.

    JSON file with states key and its a list of objects:-

    ![1548003889650](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1548003889650.png) 

    code and o/p:-

    ![1548003942720](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1548003942720.png) 

    eg:-![1548003975045](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1548003975045.png) 

11. Writing python objects into json files:-

    Removing one of the keys and writing into a new json file.

    json.dump() converts python object into json file and json.dumps() converts python object into json string.

    code:-

    ![1548004187653](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1548004187653.png) 

    then new_states file is created and its content is shown below:-

    ![1548004228680](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1548004228680.png) 

    we can use indent=2 as json.dump(data,f,indent=2) and run for more readability.

12. Real world example:-

    It is common for websites to return JSON from their APIs so that its easy to parse.

    example is yahoo finance API that converts US dollars into other currency.

    python file:-

    ![1548004602162](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1548004602162.png) response.read() just gets the response from the website.

    ![1548004656411](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1548004656411.png)

    finding out if the count is 188:-

    ![1548004757161](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1548004757161.png) 

    Looping through all the 188 resources:-

    ![1548004792010](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1548004792010.png) 

    Printing names and prices:-

    ![1548004866366](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1548004866366.png) 

    converting above names and prices into a dictionary:-

    ![1548004945729](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1548004945729.png) 

    50 US dollars will be 42.325 euros

    Converting 50 US dollars into indian rupees:-![1548005008070](C:\Users\lchitrag\AppData\Roaming\Typora\typora-user-images\1548005008070.png) 

    