# Dunder methods

https://dbader.org/blog/python-dunder-methods

Predefined methods, also called magic method. These let you mimic the behaviour of built-in methods.

     __init__

Init is a special method to construct onjects, basically our constructor.

     __str__, __repr__

from article:
>__repr__: The “official” string representation of an object. This is how you would make an object of the class. The goal of __repr__ is to be unambiguous.

>__str__: The “informal” or nicely printable string representation of an object. This is for the enduser.


### Iteration - see article for example.

     __len__, __getitem__, __reversed__


### Operator Overloading for Comparing Accounts

    __eq__, __lt__

Check what is available to you using the dir()

Use a decorator the decorator @total_ordering in order to access all of your dunder methods and avoid implementing them all.

### Operator Overloading for Merging Accounts:

    __add__


reverese add method 

    __radd__


### Callable Python objs:

    __call__

making an object callable like a normal function.

From article:
>"...the downside of having a __call__ method on your objects is that it can be hard to see what the purpose of calling the object is. Most of the time it’s therefore better to add an explicit method to the class. In this case it probably would’ve been more transparent to have a separate Account.print_statement() method."

### Context manager support, with statement

    __enter__, __exit__


Context Manager Definition, From the article:

> "A context manager is a simple “protocol” (or interface) that your object needs to follow so it can be used with the with statement. Basically all you need to do is add __enter__ and __exit__ methods to an object if you want it to function as a context manager."

# Statistic in Python

https://www.dataquest.io/blog/basic-statistics-in-python-probability/

Probabilty - "What are the chances of this particular event occurring?"

Sample space - the set of all possibilities that can potentially happen.

Normal distribution, bell shaped, from article:

> "In probability, the normal distribution is a particular distribution of the probability across all of the events. The x-axis takes on the values of events we want to know the probability of. The y-axis is the probability associated with each event, from 0 to 1."

Central Limit Theorem - from article
> "If we make many estimates, the Central Limit Theorem dictates that the distribution of these estimates will look like a normal distribution." 

Three SIgma Rule - from article:
> "The Three Sigma rule, also known as the empirical rule or 68-95-99.7 rule, is an expression of how many of our observations fall within a certain distance of the mean."

Z-score - from article:

>"The Z-score is a simple calculation that answers the question, “Given a data point, how many standard deviations is it away from the mean?”."

Finds the cumulative probability of our normal distribution. 

[code401 Reading Notes](../401Python/code401Table.md)