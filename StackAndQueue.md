<h1>Stack Data Structure</h1>

<h2>What is Stack?</h2>
<p>
Stack is a linear data structure that follows a particular order in which the operations are performed. The order may be LIFO(Last In First Out) or FILO(First In Last Out).
  LIFO implies that the element that is inserted last, comes out first and FILO implies that the element that is inserted first, comes out last.
<h3>
  Some key points related to stack
</h3>

  - It is called as stack because it behaves like a real-world stack, piles of books, etc.
  
- A Stack is an abstract data type with a pre-defined capacity, which means that it can store the elements of a limited size.
- It is a data structure that follows some order to insert and delete the elements, and that order can be LIFO or FILO.

  <h3>
    Standard Stack Operations </h3>
    
1. push(): When we insert an element in a stack then the operation is known as a push. If the stack is full then the overflow condition occurs.
2. pop(): When we delete an element from the stack, the operation is known as a pop. If the stack is empty means that no element exists in the stack, this state is known as an underflow state.
3. isEmpty(): It determines whether the stack is empty or not.
4. isFull(): It determines whether the stack is full or not.'
5. peek(): It returns the element at the given position.
6. count(): It returns the total number of elements available in a stack.
7. change(): It changes the element at the given position.
8. display(): It prints all the elements available in the stack.

</p>

<hr>
<h2>What is Queue</h2>
<p>
Queue, like Stack, is also an abstract data structure. The thing that makes queue different from stack is that a queue is open at both its ends. Hence, it follows FIFO (First-In-First-Out) structure, i.e.
  the data item inserted first will also be accessed first. The data is inserted into the queue through one end and deleted from it using the other end.

  <h3> Basic Operations</h3>
  
Queue operations also include initialization of a queue, usage and permanently deleting the data from the memory.

The most fundamental operations in the queue ADT include: enqueue(), dequeue(), peek(), isFull(), isEmpty(). These are all built-in operations to carry out data manipulation and to check the status of the queue.

Queue uses two pointers − front and rear. The front pointer accesses the data from the front end (helping in enqueueing) while the rear pointer accesses data from the rear end (helping in dequeuing).

Insertion operation: enqueue()
The enqueue() is a data manipulation operation that is used to insert elements into the stack. The following algorithm describes the enqueue() operation in a simpler way.
  Algorithm
  
  ```
1 − START
2 – Check if the queue is full.
3 − If the queue is full, produce overflow error and exit.
4 − If the queue is not full, increment rear pointer to point the next empty space.
5 − Add data element to the queue location, where the rear is pointing.
6 − return success.
7 – END
```
  <h3>Applications of Queue</h3>
Due to the fact that queue performs actions on first in first out basis which is quite fair for the ordering of actions. There are various applications of queues discussed as below.

- Queues are widely used as waiting lists for a single shared resource like printer, disk, CPU.
- Queues are used in asynchronous transfer of data (where data is not being transferred at the same rate between two processes) for eg. pipes, file IO, sockets.
- Queues are used as buffers in most of the applications like MP3 media player, CD player, etc.
- Queue are used to maintain the play list in media players in order to add and remove the songs from the play-list.
- Queues are used in operating systems for handling interrupts.
</p>

<hr>

<h2>Difference between Stack and Queue Data Structures</h2>

| Stack                                                   | Queue                                                    |
|---------------------------------------------------------|----------------------------------------------------------|
| It follows the LIFO (Last In First Out) order to store the elements, which means the element that is inserted last will come out first. | It follows the FIFO (First In First Out) order to store the elements, which means the element that is inserted first will come out first. |
| It has only one end, known as the top, at which both insertion and deletion take place. | It has two ends, known as the rear and front, which are used for insertion and deletion. The rear end is used to insert the elements, whereas the front end is used to delete the elements from the queue. |
| The insertion operation is known as push and the deletion operation is known as pop. | The insertion operation is known as enqueue and the deletion operation is known as dequeue. |
| The condition for checking whether the stack is empty is top == -1 as -1 refers to no element in the stack. | The condition for checking whether the queue is empty is front == -1 |
| The condition for checking if the stack is full is top == max-1 as max refers to the maximum number of elements that can be in the stack. | The condition for checking if the queue is full is rear == max-1 as max refers to the maximum number of elements that can be in the queue. |
| There are no other variants or types of the stack. | There are three types of queues known as circular, double-ended, and priority. |
| It has a simple implementation compared to queues as no two pointers are involved. | It has a complex implementation compared to stacks as two pointers front and rear are involved. |
| It is used to solve recursion-based problems. | It is used to solve sequential processing-based problems. |
| A real-life example of a stack can be the Undo/Redo operation in Word or Excel. | A real-life example of a queue can be an operating system process scheduling queues. |
