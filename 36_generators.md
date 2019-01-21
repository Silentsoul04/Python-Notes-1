1. Generators don't hold the entire result in memory. It yields one result at a time.

   Generator is a function that returns an object(iterator) which we can iterate over(one value at a time) bu using **yield**(i.e., yielding something).

   ![1547979049774](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547979049774.png) 

   what happens if we put extra next()? It gives StopIteration as an error.

2. Another way of above example:

   ![1547979170929](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547979170929.png) 

   

3. **ADV**:-more readable

4. Another way of above example using comprehension:-

   ![1547979264835](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547979264835.png) 

   

5. Creating generator object:-

   ![1547979328985](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547979328985.png) 

   

6. ![1547979371867](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547979371867.png) 

7. **Generator is better performer than list**

   eg:-

   common code:-

   ![1547979682028](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547979682028.png)  

   code and output for list:-

   ![1547979709438](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547979709438.png) 

   code and o/p for generator:-

    ![1547979751005](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547979751005.png) 

   converting generator into list:-

   ![1547979787750](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547979787750.png) 

   

   
