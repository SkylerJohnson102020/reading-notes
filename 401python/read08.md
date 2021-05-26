# List Comprehensions

https://www.pythonforbeginners.com/basics/list-comprehensions-in-python

- A clean way to create lists. From article:

> "It consists of brackets containing an expression followed by a for clause, then
zero or more for or if clauses. The expressions can be anything, meaning you can
put in all kinds of objects in lists.

From article:

        new_list = []
        for i in old_list:
            if filter(i):
                new_list.append(expressions(i))

This code example from the article:

        for item in list:
            if conditional:
                expression

Is the same as this one from the article:

        new_list = [expression(i) for i in old_list if filter(i)]

The use of the square brackets serves as a reminder that hte data structure is a list.
 
From article:
> new_list
> The new list (result).

> expression(i)
> Expression is based on the variable used for each element in the old list.

> for i in old_list
> The word for followed by the variable name to use, followed by the word in the
old list.

> if filter(i)
> Apply a filter with an If-statement.


Great example below from the article, this:

        squares = []

        for x in range(10):
            squares.append(x**2)
        
        print squares
        [0, 1, 4, 9, 16, 25, 36, 49, 64, 81]

is the same as this:

        squares = [x**2 for x in range(10)]

        print squares
        [0, 1, 4, 9, 16, 25, 36, 49, 64, 81]

[code401 Reading Notes](../401Python/code401Table.md)