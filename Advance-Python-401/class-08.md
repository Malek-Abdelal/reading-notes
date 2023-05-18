# Class 08 Reading

## Stacks & Queues

**1. Stack:**

A stack is a linear data structure that follows the Last-In-First-Out (LIFO) principle. It means that the last element added to the stack is the first one to be removed. Think of it as a stack of plates where you can only remove the topmost plate or add a new plate on top.

**Key operations:**

- Push: Adds an element to the top of the stack.
- Pop: Removes the top element from the stack.
- Peek/Top: Returns the top element without removing it.
- IsEmpty: Checks if the stack is empty.

Common use cases for stacks include expression evaluation, undo/redo functionality, function call stack in programming languages, and backtracking algorithms.

**2. Queue:**

A queue is also a linear data structure, but it follows the First-In-First-Out (FIFO) principle. It means that the first element added to the queue is the first one to be removed. Think of it as a queue of people waiting in line where the person who arrives first gets served first.

**Key operations:**

- Enqueue: Adds an element to the end (rear) of the queue.
- Dequeue: Removes the element from the front of the queue.
- Front: Returns the element at the front without removing it.
- IsEmpty: Checks if the queue is empty.

Queues are commonly used in scenarios that involve scheduling, buffering, printing tasks, breadth-first search, and handling requests.

**3. Priority Queue:**
A priority queue is an abstract data type that represents a set of elements, each associated with a priority. The elements with higher priorities are dequeued before the ones with lower priorities. It's like a queue where elements have different priorities and are served based on their priority level.

**Key operations:**

- Insert: Adds an element to the priority queue with a specific priority.
- Delete: Removes the element with the highest priority.
- FindMin/FindMax: Retrieves the element with the highest or lowest priority without removing it.
- IsEmpty: Checks if the priority queue is empty.

Priority queues are used in various applications, such as task scheduling, event handling, graph algorithms like Dijkstra's algorithm, and Huffman coding.

**4. Circular Queue:**

A circular queue is an extension of the queue data structure, where the last element points back to the first element to create a circular structure. This allows efficient utilization of space in certain scenarios.

**Key operations:**

- Enqueue: Adds an element to the rear of the circular queue.
- Dequeue: Removes the element from the front of the circular queue.
- Front: Returns the element at the front without removing it.
- IsEmpty: Checks if the circular queue is empty.

- IsFull: Checks if the circular queue is full.

Circular queues are useful when there's a fixed buffer size, and elements need to be added and removed in a circular manner.