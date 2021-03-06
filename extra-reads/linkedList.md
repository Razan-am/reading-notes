## Linked Lists

### ***What is a Linked List***
- A Linked List is a sequence of Nodes that are connected/linked 
         to each other
- A common analogy for Linked Lists is a train. The engine is the head and each car is a node. The train cars are linked together, but can be reordered by changing how the cars are linked.

### ***`Big O`*** Notation is a way of evaluating the performance of an algorithm.

![bigO](../imag/bigO.PNG)


- An `O(1)` function takes constant time, which is to say that it doesn’t matter how many elements we have, or how huge our input is: it’ll always take the same amount of time and memory to run our algorithm. 
- An `O(n)` function is linear, which means that as our input grows `from ten numbers, to ten thousand, to ten million`, the space and time that we need to run that algorithm grows linearly.

### ***Start with the simplest place we can insert an element into a linked list:***
1. First, we find the head node of the linked list.
2. Next, we’ll make our new node, and set its pointer to the 
     current first node of the list.
3. Lastly, we rearrange our head node’s pointer to point at our new node.

### ***What is linked list :***

 1. Linear data structures

![linked1](../imag/linked1.PNG)

2. Memory management
![linked2](../imag/linked2.PNG)

3. Parts of a linked list
![linked3](../imag/linked3.PNG)

4. Lists for all shapes and sizes
![linked4](../imag/linked4.PNG)

- Inserting elements at the beginning and end of a linked list

![end=biging](../imag/end-biginig.PNG)

###  ***What Problem(s) Do Linked Lists Solve?***
   - `Arrays` in JavaScript are implemented as objects and thus less efficient than arrays in other languages. Unless you need random access to elements, a `linked list` may be more efficient than a one-dimensional array.

### ***What Problem(s) Do Linked Lists Create?***
  - Linked Lists use more memory than arrays due to their pointers.
  - Linked Lists must be traversed sequentially.
