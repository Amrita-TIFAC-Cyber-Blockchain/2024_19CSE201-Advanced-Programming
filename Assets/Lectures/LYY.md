# 20CYS402 - Distributed Systems and Cloud Computing
![](https://img.shields.io/badge/Batch-21CYS-lightgreen) ![](https://img.shields.io/badge/UG-blue) ![](https://img.shields.io/badge/Subject-DSCC-blue) <br/>
![](https://img.shields.io/badge/Lecture-2-orange) ![](https://img.shields.io/badge/Practical-3-orange) ![](https://img.shields.io/badge/Credits-3-orange)

## Introduction to Constructors

Constructors are special member functions that are automatically executed when an object is created. They are used to initialize the object's attributes. There are two main types of constructors: default constructors and parameterized constructors.

### Default Constructor 
A default constructor is that takes no arguments. If no constructors are defined in a class, C++ automatically provides a default constructor that does nothing.

```
class <<ClassName>> {
public:
    <<ClassName>>() {
        // Constructor body
    }
};
```

### Parameterized Constructors
A parameterized constructor is that takes arguments to initialize an object with specific values.

```
class <<ClassName>> {
public:
    <<ClassName>>(parameter_list) {
        // Constructor body
    }
};
```