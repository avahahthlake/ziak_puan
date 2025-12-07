# 🖇️ Linked list 🖇️
A linked list is a type of data structure that uses nodes.
In a simple linked list, a node consist of *data* and *a pointer to the next node*

![linked-list](assets/linked-list.png)

### 📝 Representation of linked list in memory...🪦

![linked-memory](assets/linked-mem.png)

# 🖇Linked list definition using node 🖇
```c
struct Node {
  int data;
  struct Node* next;
};
```

# 🍉 Operations on linked list 🍉

## Traversals
Here is the algorithm to traverse a simple linked list

```algorithm
1. Create a temporary node(temp) and assign the head node's address.

2. Print the data which is present in the temp node.

3. After printing the data, move the temp pointer to the next node.

4. Do the above process until we reach the end.

```
## Insertions
#### at beginning
```algorithm
1. Declare a head pointer and make it as NULL.

2. Create a new node with the given data.

3. Make the new node point to the head node.

4. Finally, make the new node as the head node.

```
#### at the end
```algorithm
1. Declare head pointer and make it NULL.

2. Create a new node with the given data. And make the new node->next as NULL.
    (Because the new node is going to be the last node.)

3. If the head node is NULL (Empty Linked List),
         make the new node as the head.

4. If the head node is not null, (Linked list already has some elements),
         find the last node.
         make the last node->next as the new node.
```

## Deletion
```c
1. If the head node has the given key,

     make the head node points to the second node and free its memory.

2. Otherwise,

     From the current node, check whether the next node has the given key

     if yes, make the current->next = current->next->next and free the memory.

     else, update the current node to the next and do the above process (from step 2) till the last node.

```

