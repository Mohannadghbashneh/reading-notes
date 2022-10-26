## Stack and Queue

## Reading:
### Stack
- A stack is a linear data structure that follows the principle of Last In First Out (LIFO). This means the last element inserted inside the stack is removed first.
#### Basic Operations of Stack
- Push: Add an element to the top of a stack
- Pop: Remove an element from the top of a stack
- IsEmpty: Check if the stack is empty
- IsFull: Check if the stack is full
- Peek: Get the value of the top element without removing it
![Stack](https://cdn.programiz.com/sites/tutorial2program/files/stack.png)

### Applications of Stack
- Stack is used for evaluating expression with operands and operations.
- Matching tags in HTML and XML
- Undo function in any text editor.
- Infix to Postfix conversion.
- Stacks are used for backtracking and parenthesis matching.
- Stacks are used for conversion of one arithmetic notation to another arithmetic notation.
- Stacks are useful for function calls, storing the activation records and deleting them after returning from the function. It is very useful in processing the function calls.
- Stacks help in reversing any set of data or strings.


### Queue
- A queue is a linear data structure that follows the principle of First In First Out (FIFO). This means the first element inserted inside the queue is removed first.

#### Basic Operations of Queue
- Enqueue: Add an element to the end of a queue
- Dequeue: Remove an element from the front of a queue
- IsEmpty: Check if the queue is empty
- IsFull: Check if the queue is full
- Peek: Get the value of the front element without removing it
![Queue](https://cdn.programiz.com/sites/tutorial2program/files/queue.png)


### FIFO & LILO and LIFO & FILO Principles:
- Queue: First In First Out (FIFO): The first object into a queue is the first object to leave the queue, used by a queue.
- Stack: Last In First Out (LIFO): The last object into a stack is the first object to leave the stack, used by a stack
##### OR
- Stack: First In Last Out (FILO): The first object or item in a stack is the last object or item to leave the stack.
- Queue: Last In Last Out (LILO): The last object or item in a queue is the last object or item to leave the queue.

#### Applications of Queue
- Queue is used when things don’t have to be processed immediately, but have to be processed in First InFirst Out order like Breadth First Search.
- Queue is also used when a resource is shared among multiple consumers. Examples include CPU scheduling, Disk Scheduling.
- When data is transferred asynchronously (data not necessarily received at same rate as sent) between two processes. Examples include IO Buffers, pipes, file IO, etc.