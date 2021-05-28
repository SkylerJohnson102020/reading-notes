# Stack and Queues

https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-10/resources/stacks_and_queues.html


From article:

> "A stack is a data structure that consists of Nodes. Each Node references the next Node in the stack, but does not reference its previous."
> 1. Push - Nodes or items that are put into the stack are pushed
> 2. Pop - Nodes or items that are removed from the stack are popped. When you attempt to pop an empty stack an > exception will be raised.
> 3. Top - This is the top of the stack.
> 4. Peek - When you peek you will view the value of the top Node in the stack. When you attempt to peek an empty stack an exception will be raised.
> 5. IsEmpty - returns true when stack is empty otherwise returns false.

First in, Last out........

Last in, First out......

> "Pushing a Node onto a stack will always be an O(1) operation. When adding a Node, you push it into the stack by assigning it as the new top, with its next property equal to the original top."

>" Popping a Node off a stack is the action of removing a Node from the top. When conducting a pop, the top Node will be re-assigned to the Node that lives below and the top Node is returned to the user."

> "When conducting a peek, you will only be inspecting the top Node of the stack. 
Typically, you would check isEmpty before conducting a peek. This will ensure that an exception is not raised. Alternately, you can wrap the call in a try/catch block."


## What is a Queue
 From the article:

> Common terminology for a queue is
> 1. Enqueue - Nodes or items that are added to the queue.
> 2. Dequeue - Nodes or items that are removed from 
> 3. the queue. If called when the queue is empty an exception will be raised.
> 4. Front - This is the front/first Node of the queue.
> 5. Rear - This is the rear/last Node of the queue.
> 6. Peek - When you peek you will view the value of the front Node in the queue. If called when the queue is empty an exception will be raised.
> 7. IsEmpty - returns true when queue is empty otherwise returns false.



[code401 Reading Notes](../401Python/code401Table.md)