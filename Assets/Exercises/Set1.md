# 19CSE201 - Advanced Programming 
![](https://img.shields.io/badge/Batch-23CYS-lightgreen) ![](https://img.shields.io/badge/UG-blue) ![](https://img.shields.io/badge/Subject-AP-blue) <br/>
![](https://img.shields.io/badge/Lecture-2-orange) ![](https://img.shields.io/badge/Practical-3-orange) ![](https://img.shields.io/badge/Credits-3-orange)

## Function Overloading Exercises
![](https://img.shields.io/badge/Duration-08_Aug_to_15_Aug-blue)

### Question - 1 

**Objective:** 
Create a class ```Matrix``` that represents a 2D matrix. 
The class should support the following constructors:

- ```Default Constructor```: Initializes a 3x3 matrix with all elements set to zero.
- ```Parameterized Constructor```: Initializes a matrix of given rows and columns with all elements set to a given value.
- ```Constructor from 2D Array```: Initializes a matrix from a given 2D array.

**Instructions:** 
Write a Program to implement the class with Constructor and below member functions:
- ```print```: Print the matrix.

### Question - 2 

**Objective:** 
Create a class ```Vector``` that represents a 2D vector. Perform ```dotProduct```, ```crossProduct``` and ```magnitude``` operations over these vectors. Additionally overload these functions.

**Instructions:** 
Write a Program to implement the class with Constructor and overload the following functions:

- ```dotProduct```: to calculate the dot product of two vectors.
- ```crossProduct```: to calculate the cross product of two vectors.
- ```magnitude```: to calculate the magnitude of a vector.

**Template**
```
#include <iostream>
#include <cmath>

class Vector {
private:
    double x;
    double y;

public:
    Vector(double x = 0, double y = 0) : x(x), y(y) {}

    // Overload dotProduct for two vectors
    double dotProduct(const Vector& other) const {
       
    }

    // Overload crossProduct for two vectors
    double crossProduct(const Vector& other) const {
        
    }

    // Overload magnitude to calculate the magnitude of the vector
    double magnitude() const {
        
    }

    void print() const {
        std::cout << "(" << x << ", " << y << ")" << std::endl;
    }
};

int main() {
    Vector v1(3.0, 4.0);
    Vector v2(1.0, 2.0);

    double dot = v1.dotProduct(v2);
    std::cout << "Dot product of v1 and v2: " << dot << std::endl;

    double cross = v1.crossProduct(v2);
    std::cout << "Cross product of v1 and v2: " << cross << std::endl;

    double mag = v1.magnitude();
    std::cout << "Magnitude of v1: " << mag << std::endl;

    return 0;
}
```

### Question - 3

**Objective:** 
Create a class ```Polynomial``` that represents a polynomial. Perform various operations like ```add```, ```subtract``` and ```evaluate```. Additionally overload these functions.

**Instructions:** 
Write a Program to implement the class with Constructor and overload the following functions:
- ```add```: to add two polynomials.
- ```subtract```: to subtract one polynomial from another.
- ```evaluate```: to evaluate the polynomial for a given value of x.
