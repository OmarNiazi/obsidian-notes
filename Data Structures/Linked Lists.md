Linked List is one of the fundamental data structures. The key difference between a list and an array is that an array stores data in continuous memory locations whereas a Linked list stores data in random memory location where each node has a pointer towards the next node in the sequence. Hence we can conclude that a list is fundamentally a collection of Nodes. A node is a structure or an object that consists of the data to be stored and 1 or more pointers depending on the type of linked list.

```mermaid
graph LR
    %% Node 1
    subgraph node1 [" "]
        data1[Data: 10]
        next1[Next]
    end
    
    %% Node 2
    subgraph node2 [" "]
        data2[Data: 20]
        next2[Next]
    end
    
    %% Node 3
    subgraph node3 [" "]
        data3[Data: 30]
        next3[Next]
    end
    
    %% Node 4
    subgraph node4 [" "]
        data4[Data: 40]
        next4[Next]
    end
    
    %% NULL terminator
    null[NULL]
    
    %% Connections from next pointer to next node
    next1 --> node2
    next2 --> node3
    next3 --> node4
    next4 --> null
    
    %% Head pointer
    head[Head] --> node1
    
    %% Styling
    classDef nodeStyle fill:#e1f5fe,stroke:#01579b,stroke-width:2px
    classDef dataStyle fill:#fff3e0,stroke:#e65100,stroke-width:1px
    classDef nextStyle fill:#f3e5f5,stroke:#4a148c,stroke-width:1px
    classDef headStyle fill:#c8e6c9,stroke:#1b5e20,stroke-width:2px
    classDef nullStyle fill:#ffebee,stroke:#c62828,stroke-width:2px
    
    class node1,node2,node3,node4 nodeStyle
    class data1,data2,data3,data4 dataStyle
    class next1,next2,next3,next4 nextStyle
    class head headStyle
    class null nullStyle
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

