# 19CSE201 - Advanced Programming 
![](https://img.shields.io/badge/Batch-23CYS-lightgreen) ![](https://img.shields.io/badge/UG-blue) ![](https://img.shields.io/badge/Subject-AP-blue)
<br/>

## Standard Template Library (STL)
![](https://img.shields.io/badge/Date-26_September-blue)

### Set
- Part of Associative Container.
- Stores unique elements in a sorted order, meaning there are no duplicate values.
- Uses a binary search tree (typically a Red-Black tree) internally, providing logarithmic time complexity for insertion, deletion, and searching operations.
- All elements in a set are stored only once, and their order is automatically maintained.
- Set stores ```key```.

##### Example 
```
#include <iostream>
#include <set>

int main() {
    std::set<int> mySet = {24, 5, 10, 2};

    // Insert element
    mySet.insert(18);
    mySet.insert(44);
    mySet.insert(24); //Duplicate Element
    
    //Erase element
    mySet.erase(5);

    // Iterate over the set
    for (const int &elem : mySet)
        std::cout << elem << " "; // Output: 2 3 4 5 6 8
        
    auto it = mySet.find(44);

    // Check if the element is found
    if (it != mySet.end()) {
        std::cout << "\nElement 44 found in the set.\n";
    } else {
        std::cout << "\nElement 44 not found in the set.\n";
    }

    return 0;
}
```

### Map
- Part of Associative Container.
- Uses a binary search tree (usually a Red-Black tree), providing logarithmic time for insertion, deletion, and access.
- Stores ```key-value``` pairs where each key is unique. Like set, it also stores elements in sorted order based on the key.

##### Example
```
#include <iostream>
#include <map>

int main() {
    std::map<int, std::string> myMap = {{1, "Adarsh R K"}, {2, "Adithya N S"}, {3, "Agilprasanna P"}};

    // Insert a key-value pair
    myMap[4] = "Aishwarya S";
    myMap[33] = "Krishnamoorthi P L";
    myMap[42] = "N Meera";

    // Iterate over the map
    for (const auto &pair : myMap)
        std::cout << pair.first << ": " << pair.second << "\n";
    // Output:
    // 1: One
    // 2: Two
    // 3: Three
    // 4: Four
    
      // Use find() to search for the key
    auto it = myMap.find(66);

    // Check if the key is found
    if (it != myMap.end()) {
        std::cout << "Key 66 found with value: " << it->second << "\n";
    } else {
        std::cout << "Key 66 not found in the map.\n";
    }

    return 0;
}
```

### Multiset

### Multimap
