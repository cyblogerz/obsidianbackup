
Date: 2024-10-14     Time: 01:06

> [!NOTE]
> Taking notes is  a time consuming process but it will help in making the idea stick . - worth it 
> 
> 

Status: #baby

Tags : [[Data Structures]]

# Tree Datastructure

- Heirarchial data structure . It is used to organize and store data in the computer to be used more effectively.
- It consists of a **central node , structural node, sub-nodes ,** connected with edges.
- The tree data structure has leaves, roots and branches. 

### What is a tree data structure  ?

- Top most node of a tree - the **ROOT** , nodes below it are the child nodes. Each node can have - multiple children.its a recursive structure - each children have their own children .
-  It is a collection of nodes that are connected by edges and has a hierarchical relationship between the nodes.

##### The data in a tree are not stored in a sequential manner (not stored linearly), They are stored in multiple levels - heirarchical (non linear).  

## Terminologies in a tree.
- ***Parent node*** : Predecessor of a certain node is called the parent of that node .  
- ***Child node*** : the node which is the immediate successor of a certain node .
-  ***Root node*** : the top most node of a tree is called the root node. everything originates from this one.A non - empty tree - has only one root node .. and exactly one path from the root to all other nodes.
- ***Leaf Node or External Node***: The nodes which dont have any child .  
- ***Ancestor of a node***: Any predecessor nodes on the path of the root to that node are called Ancestors of that node.  
- ***Descendant:*** A node x is a descendant of another node y if and only if y is an ancestor of x.
- ***Sibling:*** Children of the same parent node are called siblings. ****{D,E}**** are called siblings.
- ***Level of a node:*** The count of edges on the path from the root node to that node. The root node has level **0**.
- ***Internal node:*** A node with at least one child is called Internal Node.
- ***Neighbour of a Node:*** Parent or child nodes of that node are called neighbors of that node.
- ***Subtree***: Any node of the tree along with its descendant.

## Representation
```python
class Node:
    def __init__(self, data):
        self.data = data
        self.children = []
```

## Where are trees used ?

- **Trees are used in flutter** - there are fundamentally three trees in flutter - the widget tree, element tree and the Render tree. [[Trees in flutter]]

-   Trees are used to store heirarchial structure like the **file system** in the computer.
![[Pasted image 20241014025748.png]]

- **Data compression**: Huffman coding is a popular technique for data compression that utilizes a binary tree. the leaves represents the characters and the frequency of occurence.
- **Compiler Design** : In compiler design - syntax tree used to denote the structure of a program.
- **Database Indexing** : B-Trees and other tree structures used for efficiently search and retrieve data.
- 



- Trees(like [[Binary Search Tree]]) provide moderate access / search (quicker than [[Linked List]]  and slower than [[Arrays]]) 
- Moderate insertion/ deletion (quicker than arrays and slower than unordered linked list)


# References
Similar notes and source ideas
[Geeks for geeks tree article](https://www.geeksforgeeks.org/introduction-to-tree-data-structure/)
