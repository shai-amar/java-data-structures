# java-data-structures
This repository implement various data structures and algorithms for general use

## Linked list
### Singly linked list
**Definition:** A graph G = (V,E) is singly-linked list if every element contains some data and a link to the next element, which allows to keep the structure. 

![](/images/lists/singlyLinkedList.gif?raw=true)


### Circular linked list
**Definition:** A graph G = (V,E) is a circular linked list if it is a sequence of elements in which every element has link to its next element in the sequence and the last element has a link to the first element in the sequence.

![](/images/lists/circular-linked-list.jpg?raw=true)

### Doubly linked list
**Definition:** A graph G = (V,E) is doubly-linked list if it is a singly-linked list and in addition every node in it also contains a link to the previous node. 

![](/images/lists/doublyLinkedList.gif?raw=true)

## Stacks and Queues
### Stack
**Definition:** Stack is an ordered list of similar data type. Stack is a **LIFO** structure. (Last in First out). **push()** function is used to insert new elements into the Stack and **pop()** is used to delete an element from the stack. Both insertion and deletion are allowed at only one end of Stack called **Top**.

![](/images/stacks/stack-data-structure.png?raw=true)

### Regular queue
**Definition:** Queue is also an abstract data type or a linear data structure, in which the first element is inserted from one end called REAR(also called tail), and the deletion of exisiting element takes place from the other end called as FRONT(also called head). This makes queue as FIFO data structure, which means that element inserted first will also be removed first.

The process to add an element into queue is called **Enqueue** and the process of removal of an element from queue is called **Dequeue**.

![](/images/queues/regular-queue.png?raw=true)

### Priority queue
**Definition:** Priority queue is an abstract data type which is like a regular queue or stack data structure, but where additionally each element has a __priority__ associated with it. In a priority queue, an element with high priority is served before an element with low priority. If two elements have the same priority, they are served according to their order in the queue.

![](/images/queues/priority-queue.gif?raw=true)

## Key value store
Key value store structure represented in java by a **Hash Table** or a **Map**. In different languages they are called in a different names. Objective-C equivalent is the **Dictionary**.

### Hash table / Hash Map
**Definition:** A hash table (hash map) is a data structure used to implement an associative array, a structure that can map keys to values. A hash table uses a hash function to compute an index into an array of buckets or slots, from which the desired value can be found.
Hash Table and Hash Map are the almost the same but there are some differences:

**Null keys** and **null values**
Hashmap allows one null key and any number of null values, while Hashtable do not allow null keys and null values in the HashTable object.

**Iterating the values**
Hashmap object values are iterated by using iterator .HashTable is the only class other than vector which uses enumerator to iterate the values of HashTable object.

**Synchronization** and **thread safe**
This is the most important difference between two . HashMap is non synchronized and not thread safe.On the other hand, HashTable is thread safe and synchronized.

![](/images/dictionaries/hashTable.png?raw=true)

### Map

## Trees
### Binary search tree
### Balanced search tree
### Suffix Tree

## Sorting and searching
### Heapsort
### Mergesort
### Quicksort
### Distribution sort
### Binary search

## Graph traversal
### Directed Graph
**Definition:** A graph G = (V,E) is directed if edge (x,y) ∈ E does NOT impliy that (y,x) is also in E

![](/images/graphs/directed_graph2.png?raw=true)

### Undirected graph
**Definition:** A graph G = (V,E) is undirected if edge (x,y) ∈ E implies that (y,x) is also in E

![](/images/graphs/undirected_graph.png?raw=true)

### Weighted graph
**Definition:** A graph G = (V,E) is weighted if it have a weight, or number, associated with each edge E. Some algorithms require all weights to be nonnegative, integral, positive, etc. Also known as edge-weighted graph.

![](/images/graphs/weighted_graph.gif?raw=true)

### Unweighted graph
**Definition:** A graph G = (V,E) is unweighted if it do not have a weight, or number, associated with each edge E.

![](/images/graphs/unweighted_graph.gif?raw=true)

### Simple graph
**Definition:** A simple graph G = (V,E), also called a strict graph is an unweighted, undirected graph G containing no graph loops or multiple edges. A simple graph may be either connected or disconnected.


### Non simple graph
### Sparse graph
### Dense graph
### Cyclic graph
### Acyclic graph
### Embedded graph
### Topological graph
### Implicit graph
### Explicit graph
### Labeled graph
### Unlabled graph
