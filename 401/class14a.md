## Trees

### Terms

- Node - A Tree node is a component which may contain it’s own values, and references to other nodes

- Root - The root is the node at the beginning of the 

- K - A number that specifies the maximum number of children any node may have in a k-ary tree. In a binary tree, k = 2.

- Left - A reference to one child node, in a binary tree

- Right - A reference to the other child node, in a binary tree

- Edge - The edge in a tree is the link between a parent and child node

- Leaf - A leaf is a node that does not have any children

- Height - The height of a tree is the number of edges from the root to the furthest leaf

### Traversing trees is very important, especially when looking for a Node. There are two types of traversal

* Depth First
- With this type of traversal we go through the depth(height) first
There are multiple ways to carry out depth first traversal, and each method changes the order in which we search/print the root so it is important to consider this and what our ultimate goal is when choosing a method.

- Pre-order: root >> left >> right
- In-order: left >> root >> right
- Post-order: left >> right >> root

* Breadth First

### Pseudocode

ALGORITHM breadthFirst(root)

INPUT  <-- root node
OUTPUT <-- front node of queue to console

Queue breadth <-- new Queue()
breadth.enqueue(root)

while breadth.peek()

node front = breadth.dequeue()
OUTPUT <-- front.value

if front.left is not NULL
breadth.enqueue(front.left)

if front.right is not NULL
breadth.enqueue(front.right)

- Breadth first traversal iterates through the tree by going through each level of the tree node-by-node.

- The biggest difference between each of the traversals is when you are looking at the root node.
- repeat the dequeue + enqueue children process
- When we reach a node that doesn’t have any children, we just dequeue it without any further enqueue.




## The most common way to traverse through a tree is to use recursion

### Below is the concepts when creating each method

#### Pre-order

ALGORITHM preOrder(root)

OUTPUT <-- root.value

if root.left is not NULL
preOrder(root.left)

if root.right is not NULL
preOrder(root.right)

#### In-order

ALGORITHM inOrder(root)

INPUT <-- root node
OUTPUT <-- in-order output of tree node's values

if root.left is not NULL
inOrder(root.left)

OUTPUT <-- root.value

if root.right is not NULL
inOrder(root.right)

#### Post-order
ALGORITHM postOrder(root)

INPUT <-- root node
OUTPUT <-- post-order output of tree node's values

if root.left is not NULL
postOrder(root.left)

if root.right is not NULL
        postOrder(root.right)

OUTPUT <-- root.value

* We check if our root has a certain value and then we will move to the next node treat it as the current root and then continue this process.

 This is the heart of recursion: when we complete a function call, we pop it off the stack and are able to continue execution through the previous function call

