# Linked Lists

https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-05/resources/singly_linked_list.html

> "A Linked List is a sequence of Nodes that are connected/linked to each other. The most defining feature of a Linked List is that each Node references the next Node in the link."

Singly - reference to the next node, only moves in one direction, traverses forward.

Doubly - reference to the next and previous node, traverses froward and back.

Circular - doesn't end with a node with a none value, ends with a tail. The node after the tail is the beginning of the list.

Node - individual items/links contained in a linked list. Every node holds the data for each link.

Head - beginning of list.

Use a while loop to find the node. If the current node is null, you know you've reached the end of the list and did not find the value, so the loop breaks and returns false.

add() - addbefore and addafter are available.


## What’s a Linked List, Anyway? [Part 1]

https://medium.com/basecs/whats-a-linked-list-anyway-part-1-d8b7e6508b9d

A linked list is a linear data structure meaning that they are a sequence and have a specific order in their construction.

There are also, of course, non-linear data structures.

Memory is the big difference between these two types.

Great example from the article explaining storage:

> "When an array (**static data structure**) is created, it needs a certain amount of memory. If we had 7 letters that we needed to store in an array, we would need 7 bytes of memory to represent that array. But, we’d need all of that memory in one contiguous block. That is to say, our computer would need to locate 7 bytes of memory that was free, one byte next to the another, all together, in one place.
>**On the other hand**, when a linked list (**dynamic data structure**) is born, it doesn’t need 7 bytes of memory all in one place. One byte could live somewhere, while the next byte could be stored in another place in memory altogether! Linked lists don’t need to take up a single block of memory; instead, the memory that they use can be scattered throughout."

One node contains a value, or the data it holds, and a reference ("address") to the next node.(Singly)


## What’s a Linked List, Anyway? [Part 2]

https://medium.com/basecs/whats-a-linked-list-anyway-part-2-131d96f71996

BigO analyzes the performance of an algorithm.

BigO - how much time and how much memory something needs. How quickly will this runtime grow?

Change the size of a linked list - rearrange the pointers, references.



[code401 Reading Notes](/401Python/code401Table.md)