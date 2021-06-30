## Linked Lists

Linked lists are a type of data structure.  They are most similar to arrays in that they represent a chunk, or list, or data.  But, there are some marked differences.


### LINKED LIST V. ARRAY
- Structure: linked lists are constructed out of nodes. These nodes contain data and reference to the next node (if it exists).  This "reference to next" is the glue that holds linked lists together. It is an object, inside of an object, inside of the object etc. 
- Memory: an array requires reference to it's data to be sequential and in order.  A linked list, however, does not require the reference to it's data to be stored in memory that is next to each other.  This makes linked lists more efficient than arrays in certain cases.
- Traversing: You can use multiple types of loops with arrays, but with linked lists you can really only use a while loop.
    - in order to traverse a linked list, always start at the head.
    - if the head's .next is null, then you have nothing to traverse. But, if the head's .next has a value, then you have traversable nodes.
    - in order to traverse (using a while loop), you need to set your head to current and then before the while loop restarts, you need to update your current variable to current.next --> this pops you into the next node.
    - you can replace your head node, insert within the linked list or insert at the end of the linked list, you just need to be careful in managing where you .next is pointed.  And, if you are inserting making sure that previous node's next now points to new inserted node.
    - you always need to start at the head. 
    
### Linear data structures
If we really want to understand the basics of linked lists, it’s important that we talk about what type of data structure they are.
One characteristic of linked lists is that they are linear data structures, which means that there is a sequence and an order to how they are constructed and traversed. We can think of a linear data structure like a game of hopscotch: in order to get to the end of the list, we have to go through all of the items in the list in order, or sequentially. Linear structures, however, are the opposite of non-linear structures. In non-linear data structures, items don’t have to be arranged in order, which means that we could traverse the data structure non-sequentially.

### Memory management
The biggest differentiator between arrays and linked lists is the way that they use memory in our machines. Those of us who work with dynamically typed languages like Ruby, JavaScript, or Python don’t have to think about how much memory an array uses when we write our code on a day to day basis because there are several layers of abstraction that end up with us not having to worry about memory allocation at all.

### what even is Big O?
Most of us have probably heard the term “Big O Notation”, even if we had no idea what it meant the first time that we heard someone use it. My personal experience with it has always been in the context of designing algorithms (or being asked to evaluate the efficiency of an algorithm). But Big O is really all over and omnipresent within computer science.

