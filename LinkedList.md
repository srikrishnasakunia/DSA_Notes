# Linked List

Linked List is a linear data structure, in which elements are not stored at a contiguous location, rather they are linked using pointers. Linked List forms a series of connected nodes, where each node stores the data and the address of the next node.

Node Structure: A node in a linked list typically consists of two components:
Data: It holds the actual value or data associated with the node.
Next Pointer: It stores the memory address (reference) of the next node in the sequence.
Head and Tail: The linked list is accessed through the head node, which points to the first node in the list. The last node in the list points to NULL or nullptr, indicating the end of the list. This node is known as the tail node.

Some Advantages -> 

1. Dynamic Data structure: The size of memory can be allocated or de-allocated at run time based on the operation insertion or deletion.
2. Ease of Insertion/Deletion: The insertion and deletion of elements are simpler than arrays since no elements need to be shifted after insertion and deletion, Just the address needed to be updated.
3. Efficient Memory Utilization: As we know Linked List is a dynamic data structure the size increases or decreases as per the requirement so this avoids the wastage of memory. 
4. Implementation: Various advanced data structures can be implemented using a linked list like a stack, queue, graph, hash maps, etc.

### Types of Linked List

1. Singly Linked List -> Contains two buckets in a single node. One bucket holds the actual data and another one holds the address of the next node.
   Since only next address is known, travesal happens in one single direction.
2. Doubly Linked List -> Contains three buckets in a single node. One bucket holds the actual data, and remaining two hold the address of the previous and the next node. Since both previous and next addresses are known, travesal happens in both direction.
3. Circular Linked List -> Can be implemented with both Singly and doubly Linked list, but here the end node will actually point to the head node instead of being null.

## Implementating a Linked List.

Linked List aren't predefined data type like array or string. Rather we have to define it on our own. For that we make our own class/ data class and write it structure. 

```
static class Node {
    int data;
    Node next;

    Node( int d) {
    data = d;
    next = null;
    }
 }
```
