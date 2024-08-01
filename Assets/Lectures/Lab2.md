# 19CSE201 - Advanced Programming 
![](https://img.shields.io/badge/Batch-23CYS-lightgreen) ![](https://img.shields.io/badge/UG-blue) ![](https://img.shields.io/badge/Subject-AP-blue)
![](https://img.shields.io/badge/-HPOJ-brown) <br/>
![](https://img.shields.io/badge/Lecture-2-orange) ![](https://img.shields.io/badge/Practical-3-orange) ![](https://img.shields.io/badge/Credits-3-orange)

## Classes & Objects, Constructors & Destructor, Function Overloading

### Problem Statement:
Create a C++ program to manage the details of books. The program should allow adding new books, displaying book details, and calculating the price of books with different discount rates.

### Requirements:
Define a class ```Book``` with the following private members:
- ```int bookID```
- ```string title```
- ```string author```
- ```float price```
  
Implement the following public member functions:
- Default constructor
- Parameterized constructor to initialize bookID, title, author, and price
- Destructor
- A function displayDetails to display the details of a book
- Function overloading for calculatePrice:
  - ```calculatePrice()```: Calculate and return the price without any discount.
  - ```calculatePrice(float discount)```: Calculate and return the price after applying a discount percentage.

#### Instructions:
- Create a ```Book``` class as described above.
- Implement the default constructor to initialize member variables with default values.
- Implement the parameterized constructor to initialize member variables with given values.
- Implement the destructor to display a message when a Book object is destroyed.
- Implement the displayDetails function to display book details.
- Implement the calculatePrice function with function overloading to handle no discount and discount scenarios.

In the main function, demonstrate the usage of all implemented features.
