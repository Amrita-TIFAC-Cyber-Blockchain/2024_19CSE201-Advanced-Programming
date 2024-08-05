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
