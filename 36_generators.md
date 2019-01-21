# Generator - How to use them and benefits

- Generators are simple way of creating iterators.
- Overheads that occur in creating iterators are handled by generators in python.

## Creating a generator
- It can be done by defining a normal function with a yield statement instead of a return statement.
- A return statement terminates a function but yield function saves all the states and later continues from there.
- After the yield is executed the function is paused and the control is transferred to the caller.
- Local variables are remembered between calls.
- When the function terminated 'StopIteration' is raised.