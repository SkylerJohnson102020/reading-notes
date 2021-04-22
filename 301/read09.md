# Concepts of Functional Programming with JS

- Functional Programming - a style of building app structure that focuses more on the mathematical functions and less on changing state and mutable items.

- Pure functions - zero side effects and must return the same result as the given args.No external object given to the function. We want to set args. directly, not use global scoped variables.
         
        - Random number generators make a function impure
        - If we have a function that has a += 1 counter within, this is impure since it's result is changing. Set the function to always return a value + one and set a counter outside of the function will make it pure as the pure function will always return value + 1.
        - Pure functions are isolated, stable, sonsistent, etc.

- Benefits - Easier to test. Easy to memorize your functions.

- Review - Immutable means that something cannot be changed. The work around is to create a new object.

- Recursion - divide and conquer. Separating your problem into smaller pieces. Let your function work in the same way always, form the variables to fit the mold of the function. Keeping your variable unchanged.

- Referential tranperency - if the functions always returns the same result for the same given input. Easy to memorize your functions.

        pure function + immutable (variable, object, data) = referential transperency

- Functions as first class entities - treated as a value, used for data.

        - function is referred to from the constants and vars.
        - pass as param to other funcs.
        - returns as result from outside funcs.

- Higher-order functions - takes one to multiple funcs. as args or the result is the return of a function. filter, map, and reduce.

- filter() - expects a true or false value to see if whether or not the element is included in the result. 

        - imperative - creates a new empty array.
        - declaritive - less breakable and fewer moving parts.
        - (GREAT EXAMPLES IN DOCS.)


- map() - applies a function to it's elements, returns a new set of values that are returned. (SEE EXAMPLES)

- reduce() - take in data, return it consolidated or combining it.

https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2aa#id_token=eyJhbGciOiJSUzI1NiIsImtpZCI6ImRlOTU1NmFkNDY4MDMxMmMxMTdhZmFlZjI5MjBmNWY5OWE0Yzc5ZmQiLCJ0eXAiOiJKV1QifQ.eyJpc3MiOiJodHRwczovL2FjY291bnRzLmdvb2dsZS5jb20iLCJuYmYiOjE2MTkxMDA0NDYsImF1ZCI6IjIxNjI5NjAzNTgzNC1rMWs2cWUwNjBzMnRwMmEyamFtNGxqZGNtczAwc3R0Zy5hcHBzLmdvb2dsZXVzZXJjb250ZW50LmNvbSIsInN1YiI6IjExMjMwNTE1MDA3NTA4MDQ2MTE2MSIsImVtYWlsIjoiYmFzc2V1cGhAZ21haWwuY29tIiwiZW1haWxfdmVyaWZpZWQiOnRydWUsImF6cCI6IjIxNjI5NjAzNTgzNC1rMWs2cWUwNjBzMnRwMmEyamFtNGxqZGNtczAwc3R0Zy5hcHBzLmdvb2dsZXVzZXJjb250ZW50LmNvbSIsIm5hbWUiOiJTa3lsZXIgSm9obnNvbiIsInBpY3R1cmUiOiJodHRwczovL2xoMy5nb29nbGV1c2VyY29udGVudC5jb20vYS0vQU9oMTRHaHVWWkVjNW9VY3ZkSXFiZVpYRUNfMHBQMkRWUHdWb0ZOc1gzQTVfZz1zOTYtYyIsImdpdmVuX25hbWUiOiJTa3lsZXIiLCJmYW1pbHlfbmFtZSI6IkpvaG5zb24iLCJpYXQiOjE2MTkxMDA3NDYsImV4cCI6MTYxOTEwNDM0NiwianRpIjoiNWY0ZTczOTVkYzVkYjQyNzQxZjZmZjM0MGNiNjFhYjQ3MWQ2YzhiYiJ9.dkzIxXX0Nli6erJDDiH465QUh21MwT6MmA1GhQn8pXyysdSbJhGi0rm-UK-i-YZLpjK48tbdjEDkQf0ewE0Mjkcm93mbEn3griQudKuAE7wZxNHVfZhXVoByMIQBpaSDO9BWT3tMoc1YtMaBQbeGX_7lNRH0somM6LM8T3TXPVcfBfoeu9rKLkSh5siyEKrXlSJuWvxtKftcH98cnzmS0TGu3V1TiGtXk6PsaTvCWT1ZhhUBVi33kq7ETJXN2VsgDDABY2BpWb-jBxi2ipFMtTVDflTF8V9Z6RxW83uwYE9wW-fPOBrxrarIfgpXg7TJenecAHRgO8xMk01e4naiAw


# Fun with Refactoring 

https://dev.to/healeycodes/refactoring-javascript-for-performance-and-readability-with-examples-1hec

- Reactoring your code so it appears and works more solidly is huge, but you can also do too much refactoring to the point where it hinders the functionality of your script.

- hash function - this function maps and sets under the hood.

[code301 Reading Notes](/301/code301Table.md)