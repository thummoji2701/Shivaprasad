          DATASTRUCTURES
**1. Arrays:**

**Definition:** Arrays are sequential collections of elements of the same data type stored in contiguous memory locations.

**Types:**
- One-dimensional arrays
- Multi-dimensional arrays

**Operations:**
- Access: O(1)
- Insertion (at the end): O(1)
- Deletion (at the end): O(1)
- Search (unsorted): O(n)
- Search (sorted): O(log n)

**Example:** 
```c
// One-dimensional array
int numbers[] = {1, 2, 3, 4, 5};

// Two-dimensional array
int matrix[3][3] = {{1, 2, 3}, {4, 5, 6}, {7, 8, 9}};
```

**2. Linked Lists:**

**Definition:** Linked lists are linear data structures consisting of nodes where each node contains data and a pointer to the next node.

**Types:**
- Singly linked list
- Doubly linked list
- Circular linked list

**Operations:**
- Insertion (at the beginning): O(1)
- Insertion (at the end): O(n) if no tail pointer, O(1) if tail pointer exists
- Deletion (at the beginning): O(1)
- Deletion (at the end): O(n) if no tail pointer, O(1) if tail pointer exists
- Search: O(n)

**Example:** 
```c
struct Node {
    int data;
    struct Node* next;
};

// Singly linked list
struct Node* head = NULL;
head = (struct Node*)malloc(sizeof(struct Node));
head->data = 1;
head->next = NULL;
```

**3. Stacks:**

**Definition:** Stacks are linear data structures that follow the Last In, First Out (LIFO) principle.

**Types:**
- Array-based stack
- Linked list-based stack

**Operations:**
- Push: O(1)
- Pop: O(1)
- Peek: O(1)

**Example:** 
```c
// Array-based stack
#define MAX_SIZE 100
int stack[MAX_SIZE];
int top = -1;

// Linked list-based stack
struct StackNode {
    int data;
    struct StackNode* next;
};
```

**4. Queues:**

**Definition:** Queues are linear data structures that follow the First In, First Out (FIFO) principle.

**Types:**
- Array-based queue
- Linked list-based queue
- Circular queue

**Operations:**
- Enqueue: O(1)
- Dequeue: O(1)
- Peek: O(1)

**Example:** 
```c
// Array-based queue
#define MAX_SIZE 100
int queue[MAX_SIZE];
int front = -1, rear = -1;

// Linked list-based queue
struct QueueNode {
    int data;
    struct QueueNode* next;
};
struct QueueNode *front = NULL, *rear = NULL;
```

**5. Trees:**

**Definition:** Trees are hierarchical data structures consisting of nodes where each node has zero or more child nodes.

**Types:**
- Binary tree
- Binary search tree
- AVL tree
- B-tree

**Operations:**
- Insertion: O(log n) average, O(n) worst-case
- Deletion: O(log n) average, O(n) worst-case
- Search: O(log n) average, O(n) worst-case

**Example:** 
```c
struct TreeNode {
    int val;
    struct TreeNode* left;
    struct TreeNode* right;
};
```

**6. Graphs:**

**Definition:** Graphs are non-linear data structures consisting of vertices (nodes) connected by edges.

**Types:**
- Directed graph
- Undirected graph
- Weighted graph
- Directed Acyclic Graph (DAG)

**Operations:**
- Add vertex: O(1)
- Add edge: O(1)
- Remove vertex: O(V + E)
- Remove edge: O(E)

**Example:** 
```c
struct Graph {
    int V;
    struct ListNode** array;
};

struct ListNode {
    int dest;
    struct ListNode* next;
};
