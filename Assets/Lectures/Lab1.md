# 19CSE201 - Advanced Programming 
![](https://img.shields.io/badge/Batch-23CYS-lightgreen) ![](https://img.shields.io/badge/UG-blue) ![](https://img.shields.io/badge/Subject-AP-blue)
![](https://img.shields.io/badge/-HPOJ-brown) <br/>
![](https://img.shields.io/badge/Lecture-2-orange) ![](https://img.shields.io/badge/Practical-3-orange) ![](https://img.shields.io/badge/Credits-3-orange)
## LAB1: Class, Object and Constructor

### Objective: Create a class Book with multiple constructors and functions, including private, and public member functions.

#### Instructions:

##### Class Definition:

Define a class ```Book``` with the following private data members:
- title (string)
- author (string)
- price (double)
- isbn (string)

##### Constructors:

- Implement a parameterized constructor that initializes all data members with the given values.

##### Member Functions:

- Implement a private member function ```validateISBN()``` that checks if the isbn is in the correct format (e.g., "XXX-XXXXXXXXXX" where X is a digit) and returns a boolean.
- Implement a public member function ```displayInfo()``` that prints the book's title, author, price, and ISBN.


##### Main Function:

In the ```main()``` function, create two Book objects:
- One using the parameterized constructor with valid values.
- One using the parameterized constructor with an invalid ISBN (to test ```validateISBN()```).
- Call the ```displayInfo()``` function for each object to display the book details.

