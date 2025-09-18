This is an extension of regular linked lists, with the only difference being that the last element points back to the head. This changes the structure of Node and the List class in a few ways.
### Node:

```cpp
// NODE 
template<typename T>
struct Node{
	T data;
	Node* next;
	Node(const T& value): data(value), next(*this) {}
};

```

### List
```cpp
twmp
```