# 19CSE201 - Advanced Programming 
![](https://img.shields.io/badge/Batch-23CYS-lightgreen) ![](https://img.shields.io/badge/UG-blue) ![](https://img.shields.io/badge/Subject-AP-blue)
<br/>
![](https://img.shields.io/badge/Lecture-2-orange) ![](https://img.shields.io/badge/Practical-3-orange) ![](https://img.shields.io/badge/Credits-3-orange)

## LAB3: Operator Overloading
![](https://img.shields.io/badge/Date-05_August-blue)

### Objective
Create a C++ program to implement operator overloading for * which multiples two matrices based on the below code template.

```
#include <iostream>
using namespace std;

class Matrix 
{
    private:
        int rows;
        int columns;
        int **data;
        
    public:
    Matrix(int r, int c) {

            }
        }
    }
    
    void setvalue(int r, int c, int value) {
        data[r][c]=value;
    }
    
    Matrix operator*(Matrix const& other) {
        
    }
};

int main()
{  
    Matrix m1(3,2);
    Matrix m2(2,3);
    
    m1.setvalue(0,0,X);
    ...
    ...
    ...
    
    m2.setvalue(0,0,X);
    ...
    ...
    ...
    
    Matrix m3  = m1*m2;
    m3.print();
    return 0;
}
```

### Submission
[Click Here](https://aumscb.amrita.edu/portal/directtool/2d33fe56-9f97-4a02-9d40-6b40bf3abe85/) to Submit.

### new and delete operator 
#### new 
The _new_ operator is used to dynamically allocate memory from the heap (also called the free store). Unlike static or automatic memory allocation (such as with fixed-size arrays or stack-allocated variables), dynamic allocation enables the program to allocate memory as needed during execution.

###### Syntax 
```
dataType* pointerVariable = new dataType;
```

##### Example 
**Array Allocation:** The new[] operator can be used to allocate memory for an array when the size is determined at runtime.
```
int* arr = new int[10];  // Allocates memory for an array of 10 integers
```

#### delete
The _delete_ operator is used to deallocate memory that was previously allocated by the new operator. This is important because C++ does not have automatic garbage collection like some other languages (Java), so dynamically allocated memory must be manually freed when it is no longer needed.

###### Syntax
```
delete pointerVariable;
```

##### Example 
**Array Deallocation:** When using new[], the delete[] operator must be used to free the allocated array memory.
```
delete[] arr;  // Deallocates memory for the array of 10 integers
```

- **Memory Leaks:** If delete is not called after new, memory leaks occur, where the memory remains allocated but is no longer in use, wasting resources.

- **Dangling Pointers**: After calling delete, the pointer still points to the deallocated memory. Accessing this memory can lead to undefined behavior. To avoid this, set the pointer to nullptr after deletion:
```
delete ptr;
ptr = nullptr;  // Safe practice
```
