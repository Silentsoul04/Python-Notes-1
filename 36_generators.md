
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

