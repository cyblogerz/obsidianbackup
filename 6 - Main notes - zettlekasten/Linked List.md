Date: 2024-10-15     Time: 19:40

> [!NOTE]
> Taking notes is  a time consuming process but it will help in making the idea stick . - worth it 
> 
> 

Status: #baby

Tags : [[Data Structures]] 

# Linked List

- it is a fundamental data structure 
- linear data structure consists of nodes 
- Efficient insertion and deletion compared to arrays
- It can be used to implement stacks, queues and deque,


# What is linked list?

- linear data strucuture that consists of series of nodes connected by pointers (c/c++) or references as in python/ java

 -  Node structure - (data and a pointer to the next )
 - Nodes are not stored contiguosly in memory . so it allows efficient insertion / deletion.
 - Linked list has sequential access to the elements whereas in arrays it is random and the memory in linked list is allocated to individual elements.

### Applications of linked list within computer science
- Dynamic memory allocation
- implementation of stacks and queues
- Maintaining a directory of names
- Performing arithematic operations
-  Manipulation of polynomials

### Applications of linked list in real world 

- ***Image viewer***    :   Previous and next images are linked  and they can be accessed by the next and previous buttons .
- ***GPS navigation system***:  Linked lists can be used to store and manage a list of locations and routes, allowing users to easily navigate to their desired destination.

```
Why linked list is used in GPS navigation system ?

- They can grow and shrink in size . In a GPS system, the list of locations (waypoints) can change as users add, remove, or reorder destinations along the route.
- In a linked list inserting or deleting locations is efficient, especially when they happen in the middle of the route
```


- In linked list every element are spread out in the [[memory]]  space.
- in array it is the opposite - it is contagious.
- linked list have a head and a tail.
- 

### Big O - Linked list

adding element to end - O(1)
Removing from the end - 
the process includes traversing through the linked list to reach to the end . o(N), n is the no . of elements.

Adding at the head - O(1) - doesnt matter how any items are there in list.







# References
Similar notes and source ideas


