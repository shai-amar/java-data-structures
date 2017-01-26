# java-data-structures
This repository implement various data structures, algorithms and search techniques for general use

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

## Key-Value store
Key-Value store structure represented in java by a **Hash Table** or a **Map**. 
Key-Value store structure is combined from a key that is ealvulated by a hash function and a value.

### Hash function
A Hush function is a function that generates a key that is allowing the retrivel of the data in a constant time.

### Hash function collision
Hash function generate a key with it you can store\retrive a value. 

There are times which different values produce the same key, meaning, with the same key you can retrieve multiple values.
There are several ways dealing with a key that already contains a value:
- Retrive it and replace it with the new value. For example: Java **HashTable** implements this startegy.
- Each key contains a bucket instead of a value that can contains multiple value. For example: Java **HashMap** implements bucket strategy and uses **LinkedList** as the bucket.  

![](/images/dictionaries/hashingConcept.png?raw=true)


### Hash table / Hash Map
**Definition:** A hash table (hash map) is a data structure used to implement an associative array, a structure that can map keys to values. A hash table uses a hash function to compute an index into an array of buckets or slots, from which the desired value can be found.
Hash Table and Hash Map are the almost the same but there are some differences:

####Null keys and null values
Hashmap allows one null key and any number of null values, while Hashtable do not allow null keys and null values in the HashTable object.

####Iterating the values
Hashmap object values are iterated by using iterator .HashTable is the only class other than vector which uses enumerator to iterate the values of HashTable object.

####Synchronization and thread safe
This is the most important difference between two . HashMap is non synchronized and not thread safe.On the other hand, HashTable is thread safe and synchronized.

![](/images/dictionaries/hashTable.png?raw=true)

Key-Value store structure is one of the most important data structures exist. Here is a brief comparison of various Key-Value store java implementations:

![](/images/dictionaries/javaStructureComparison.png?raw=true)

### Hashing
Hashing is the process of indexing and retrieving element (data) in a datastructure to provide faster way of finding the element using the hash key.

## Trees

**Definition:** A Tree is a data structure compiled from a **Root node** that is functioning a the father and the **Edges** that are functioning as its sons.
In the following examples we will see what are the components of a tree data structure and what they do.

####Root
The first node of a tree data structure is called the Root node - the father of all the other nodes. There is only one Root node in every tree data structure.

![](/images/trees/TreeRoot.png?raw=true)

####Edge

![](/images/trees/TreeEdge.png?raw=true)


####Parent

![](/images/trees/TreeParent.png?raw=true)

####Child

![](/images/trees/TreeChild.png?raw=true)

####Siblings

![](/images/trees/TreeSiblings.png?raw=true)

####Leaf

![](/images/trees/TreeLeaf.png?raw=true)

####Internal nodes

![](/images/trees/TreeInternal.png?raw=true)

####Degrees

![](/images/trees/TreeDegree.png?raw=true)

####Level

![](/images/trees/TreeLevels.png?raw=true)

####Height

![](/images/trees/TreeHeight.png?raw=true)

####Depth

![](/images/trees/TreeHeight.png?raw=true)

####Path

![](/images/trees/TreePath.png?raw=true)

####Sub tree

![](/images/trees/Subtree.png?raw=true)


### Binary tree
A binary tree is made of nodes, where each node contains a **left** pointer, a **right** pointer, and a data element.

The **root** pointer points to the topmost node in the tree. 

The left and right pointers recursively point to smaller **subtrees** on either side. A null pointer represents a binary tree with no elements - the empty tree.

The formal recursive definition is: a **binary tree** is either empty (represented by a null pointer), or is made of a single node, where the left and right pointers (recursive definition ahead) each point to a **binary tree**.

![](/images/trees/binaryTree.png?raw=true)


### AVL tree
### Balanced tree
### Suffix Tree
### Red Black tree
### Splay tree

## Sorting
### Heapsort
### Mergesort
### Quicksort
### Distribution sort
### Insertion sort
### Selection sort
### Radix sort


## Searching
### Linear search
### Binary search
### 

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
