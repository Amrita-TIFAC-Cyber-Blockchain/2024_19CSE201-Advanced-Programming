# 19CSE201 - Advanced Programming 
![](https://img.shields.io/badge/Batch-23CYS-lightgreen) ![](https://img.shields.io/badge/UG-blue) ![](https://img.shields.io/badge/Subject-AP-blue)
<br/>
![](https://img.shields.io/badge/Lecture-2-orange) ![](https://img.shields.io/badge/Practical-3-orange) ![](https://img.shields.io/badge/Credits-3-orange)

![](https://img.shields.io/badge/Date-05_August-blue)

## Introduction to Operator Overloading
Operator overloading is a compile-time polymorphism. Operator Overloading gives a special meaning to an existing operator without changing its original meaning.

In the below example, '+' operator is overloading to perform addition of two Complex Numbers (objects of Complex Class).

```
#include <iostream>
using namespace std;

// Class representing a complex number
class Complex {
private:
    int real, imag;  // Real and imaginary parts

public:
    // Constructor with initialization list
    Complex(int r, int i) : real(r), imag(i) {}

    // Default constructor
    Complex() : real(0), imag(0) {}

    // Operator overloading for addition of two Complex objects
    Complex operator+(Complex const& obj) const {
        return Complex(real + obj.real, imag + obj.imag);
    }
    
    // Function to print the complex number
    void print() const {
        cout << real << " + i" << imag << '\n';
    }
};

int main() {
    Complex c1(10, 5), c2(2, 4);
    Complex c3 = c1 + c2;
    c3.print();  // Output: 12 + i9
    return 0;
}
```

### Exercise
Please implement the operator overloading function for *.

#### Solution
```
 Complex operator*(Complex const &other){
        return Complex((real*other.real)-(img*other.img), (img*other.real)+(real*other.img));
    }
```

## Operators - Cannot be overloaded
- Conditional or Ternary Operator (?:) 
- Size of Operator (sizeof)
- Scope Resolution Operator (::)
- Class member selector Operator (.)
- Member pointer selector Operator (.*)
- Object type Operator (typeid)
