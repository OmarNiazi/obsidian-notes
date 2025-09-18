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
template<typename T>
class CircularList{
	Node* head;
public:
	CircularList(): head(nullptr) {}
};
```
### Add at Head
```cpp
void add_at_head(const T& value){
	Node* temp = value;
	if(!head){
		head = temp;
	}
	else{
		
	}
}
```