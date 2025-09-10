Linked List is one of the fundamental data structures. The key difference between a list and an array is that an array stores data in continuous memory locations whereas a Linked list stores data in random memory location where each node has a pointer towards the next node in the sequence. Hence we can conclude that a list is fundamentally a collection of Nodes. A node is a structure or an object that consists of the data to be stored and 1 or more pointers depending on the type of linked list.

```mermaid
graph LR
    A1[data: 1]:::data --> A2[next*]:::ptr
    B1[data: 2]:::data --> B2[next*]:::ptr
    C1[data: 3]:::data --> C2[next*]:::ptr
    D1[data: 4]:::data --> D2[NULL]:::ptr

    A2 --> B1
    B2 --> C1
    C2 --> D1

    classDef data fill:#a0d8ef,stroke:#333,stroke-width:1px;
    classDef ptr fill:#f9d776,stroke:#333,stroke-width:1px;
```

In case of a singly linked list:
```cpp
template <typename T>
struct Node {
	T* data;
	Node* next
	
	Node(T data = T()) : data(data), next(nullptr) {}
};
```
In case of a doubly linked list:
```cpp
template <typename T>
struct Node {
	T* data;
	Node* next
	Node* prev
	
	Node(T data = T()) : data(data), next(nullptr), prev(nullptr) {}
};
```

A singly linked list class is written as follows:
```cpp
template <typename T>
class LinkedList {
	Node<T>* head;
	
public:
	LinkedList() : head(new Node<T>()) {}
	LinkedList(T data) : head(new Node<T>(data)) {}
	
	// Insert, remove, print, search funcs
};
```

Some of the functions of a linked list are as follows:
- Constructors
- isEmpty()
- insert()
- remove()
- print()
- find()
And many more

