

# Generator - How to use them and benefits (preetha)

- Generators are simple way of creating iterators.
- Overheads that occur in creating iterators are handled by generators in python.

## Creating a generator
- It can be done by defining a normal function with a yield statement instead of a return statement.
- A return statement terminates a function but yield function saves all the states and later continues from there.
- After the yield is executed the function is paused and the control is transferred to the caller.
- Local variables are remembered between calls.
- When the function terminated 'StopIteration' is raised.

**Generators :**(aditya)

* Generators are a special class of functions that simplify the task of writing iterators.  Regular functions compute a value and return it, but generators return an iterator that returns a stream of values.

  You’re doubtless familiar with how regular function calls work in Python or C. When you call a function, it gets a private namespace where its local variables are created.  When the function reaches a `return` statement, the local variables are destroyed and the value is returned to the caller.  A later call to the same function creates a new private namespace and a fresh set of local variables. But, what if the local variables weren’t thrown away on exiting a function?  What if you could later resume the function where it left off?  This is what generators provide; they can be thought of as resumable functions.

  Here’s the simplest example of a generator function:

  ```
  def generate_ints(N):
      for i in range(N):
          yield i
  ```

  Generators are a lazy way to build iterables. They are useful when the fully realized list would not fit in memory, or when the cost to calculate each list element is high and you want to do it as late as possible. But they can only be iterated over once. 

(lalith)
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

   

   

