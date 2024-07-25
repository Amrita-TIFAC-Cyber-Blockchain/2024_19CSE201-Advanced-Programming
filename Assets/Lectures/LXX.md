# 20CYS402 - Distributed Systems and Cloud Computing
![](https://img.shields.io/badge/Batch-21CYS-lightgreen) ![](https://img.shields.io/badge/UG-blue) ![](https://img.shields.io/badge/Subject-DSCC-blue) <br/>
![](https://img.shields.io/badge/Lecture-2-orange) ![](https://img.shields.io/badge/Practical-3-orange) ![](https://img.shields.io/badge/Credits-3-orange)

## Introduction to Class and Object

Class defines a new datatype by encapsulating data (variables) and functions that operate on the data, making the code modular, reusable, and easier to maintain. 
In other words, a Class is a blueprint for creating (real-world) objects. 

```
class <<ClassName>> {
<<access-specifier>>:
    // Public members can be accessed from outside the class
    <<data-type>> attribute1; 
	...
	...
	...
	<<data-type>> attributen; 

    // Member function declaration
    void method() {
        // Function body
    }
};

```

```
#include <iostream>
using namespace std;

class Student {
public:
	int rollnumber;
    string name;
    
    void display() {
		cout << "Roll Number: " << rollnumber << endl;
        cout << "Name: " << name << endl;
    }
};
```