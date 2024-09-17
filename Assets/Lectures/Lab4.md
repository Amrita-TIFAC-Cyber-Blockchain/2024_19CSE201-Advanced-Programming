# 19CSE201 - Advanced Programming 
![](https://img.shields.io/badge/Batch-23CYS-lightgreen) ![](https://img.shields.io/badge/UG-blue) ![](https://img.shields.io/badge/Subject-AP-blue)
<br/>

## Standard Template Library (STL)
![](https://img.shields.io/badge/Date-19_September-blue)

The Standard Template Library (STL) defines powerful, template-based, reusable components that implements common data structures and algorithms. 
STL extensively uses generic programming based on templates

### Components of STL
- Containers: data structures that store objects of any type
  - Sequence Containers: linear data structures (vector, deque and linked list)
  - Associative Containers: non-linear containers (set, multiset, map and multimap)
  - Container Adapters: constrained sequence containers (stack, queue and priority queue)
- Iterators: used to iterate/manipulate container elements
- Algorithms: searching, sorting and many others

#### Sequence Container
They support iterators. 

##### Vector

```
#include <iostream>
#include <vector>

using namespace std;

int main() {
    // Declaration of a vector of integers
    vector<int> myVector;

    // Add elements to the vector
    myVector.push_back(10);
    myVector.push_back(20);
    myVector.push_back(30);

    // Check if the vector is empty
    if (myVector.empty()) {
        cout << "Vector is empty.\n";
    } else {
        cout << "Vector is not empty.\n";
    }

    // Access elements using indexing
    cout << "First element: " << myVector[0] << "\n";

    // Access elements using iterators
    cout << "Elements of the vector: ";
    for (auto it = myVector.begin(); it != myVector.end(); ++it) {
        cout << *it << " ";
    }
    cout << "\n";

    // Size of the vector
    cout << "Size of the vector: " << myVector.size() << "\n";

    // Clear the vector
    myVector.clear();

    // Check if the vector is empty after clearing
    if (myVector.empty()) {
        cout << "Vector is empty after clearing.\n";
    } else {
        cout << "Vector is not empty after clearing.\n";
    }

    return 0;
}
```

#### Container Adapters
They are implemented using the sequence containers and these do not support iterators. 

##### Stack
Last-in-First-Out or First-in-Last-Out datastructure. 

```
#include <iostream>
#include <stack>

using namespace std;

int main() {
    // Declaration of a stack of integers
    stack<int> myStack;

    // Push elements onto the stack
    myStack.push(10);
    myStack.push(20);
    myStack.push(30);

    // Check if the stack is empty
    if (myStack.empty()) {
        cout << "Stack is empty.\n";
    } else {
        cout << "Stack is not empty.\n";
    }

    // Access the top element of the stack
    cout << "Top element: " << myStack.top() << "\n";

    // Pop the top element from the stack
    myStack.pop();

    // Size of the stack
    cout << "Size of the stack: " << myStack.size() << "\n";

    // Print elements of the stack
    cout << "Elements of the stack: ";
    while (!myStack.empty()) {
        cout << myStack.top() << " ";
        myStack.pop();
    }
    cout << "\n";

    return 0;
}
```

##### Queue
First-in-First-Out or Last-in-Last-Out datastructure. 

```
#include <iostream>
#include <queue>

using namespace std;

int main() {
    // Declaration of a queue of integers
    queue<int> myQueue;

    // Enqueue elements into the queue
    myQueue.push(10);
    myQueue.push(20);
    myQueue.push(30);

    // Check if the queue is empty
    if (myQueue.empty()) {
        cout << "Queue is empty.\n";
    } else {
        cout << "Queue is not empty.\n";
    }

    // Access the front element of the queue
    cout << "Front element: " << myQueue.front() << "\n";

    // Access the back element of the queue
    cout << "Back element: " << myQueue.back() << "\n";

    // Dequeue the front element from the queue
    myQueue.pop();

    // Size of the queue
    cout << "Size of the queue: " << myQueue.size() << "\n";

    // Print elements of the queue
    cout << "Elements of the queue: ";
    while (!myQueue.empty()) {
        cout << myQueue.front() << " ";
        myQueue.pop();
    }
    cout << "\n";

    return 0;
}
```





