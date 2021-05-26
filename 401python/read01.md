# Pain and Suffering 

1. What’s your perspective? 

- I have developed over years of a brutal career with many sacrifices and the challenges that Code Fellows has presented, I just tell myself that being in a terrible and frustrating position is just par for the course. One of my music teachers told me something I carry with me to this day, "Embrace the suck."

2. Why are you doing this?

- My career pays very little and I had to piece together multiple positions that all paid in the four figures. I drove 25,000 - 30,000 miles a year for work and always scraped the bottom of the barrel every summer when musicians are out of work. Then, the 2020 pandemic shut down our extrememly fragile industry. My wife and I had a son and I decided that I couldn't take it anymore. I wanted to find something new where I could better myself, and my psyche, but also the lives of my family members. I couldn't just find anything, I needed to find something that enabled me to continue to problem solve, be challenged, and be creative. This is why I am here.

3. Do you want what comes at the end of this journey?

- I want it all, the pain, challenge, waiting, etc., I'll be ready. 

4. Are you doing this for you?

- I am doing this for me and especially my family.


# Big O Notation

https://rob-bell.net/2009/06/a-beginners-guide-to-big-o-notation

- Big O - worst-case scenario, always assumes the largest/longest performance outcome. Evaluating efficiency. How well does this perform? How much time and memory does it take?

- O(1) - algorithm which executes in the same time/space. **Constant** time - does not matter what the size of the file, it takes the same time.

- O(N) - grows **linear** and in proportion to the size of the input. N represents the number of nodes in list. Depends on the size of the file to determine performance.

- O(N**2) - performance is the square of the of the input data. Common with nested loops. Growth is exponential.

- O(2^N) - growth doubles with every new addition to the input. Growth is **exponential**. Rises very fast.

- Logarithms O(log N) - **Linear** growth. A good way to search sorted data. Basically starting in the middle and comparing, then eliminating the possibilities. It halves the data each time it works to eliminate one half each time and eventually will find the value. Great explanation in the article.

- Stacks - a data structure that is an array or list of function calls and their params. A stack of books, plates, papers, etc.

# Names and Values in Python

- Names refer to values. 

- Many names can refer to one value. 

- Names are reassigned independently from one another. 

- Mutable aliasing - Values exist until there are no references left. Assignment does not copy data, you create an additional name referring to the same list. Can have multiple names.

- Immutable data types - ints, floats, strings, tuples

- Rebinding - changes a value

- Mutating - changing a list. (append a value to the end.)


[code401 Reading Notes](../401Python/code401Table.md)