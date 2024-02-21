# Array Based Min Heap

This repository contains an implementation of a Array Based Min Heap, a complete binary tree where each node has a value less than or equal to its children's values.

## Overview

- `MinHeap` Class: Represents the Min Heap data structure.
  - Attributes:
    - `harr`: Pointer to an array of elements in the heap.
    - `capacity`: Maximum possible size of the heap.
    - `heap_size`: Current number of elements in the heap.
  - Methods:
    - `parent()`, `left()`, `right()`: Calculate parent, left child, and right child indices.
    - `getMin()`: Get the minimum element in the heap.
    - `insertKey()`: Insert a new key into the heap.
    - `decreaseKey()`: Decrease the value of a key and maintain the heap property.
    - `deleteKey()`: Delete a key from the heap.
    - `linearSearch()`: Search for a value in the heap using linear search.
    - `extractMin()`: Remove and return the minimum element from the heap.
    - `MinHeapify()`: Heapify a subtree rooted at a given index.
    - `printArray()`: Print the elements of the heap array.
    - `height()`: Calculate the height of the heap tree.

## Usage

1. Create an instance of the `MinHeap` class with the desired capacity.
2. Use the provided methods to perform operations like insertion, deletion, searching, etc.

```cpp
#include <iostream>
#include <cmath>
#include <climits>
#include <cstdlib> // For system("cls")
using namespace std;

// MinHeap class and main function definitions...

int main() {
    // Input size of Min Heap
    int s;
    cout << "Enter Size of Min Heap" << endl;
    cin >> s;
    MinHeap obj(s);
    cout << "Min Heap Created" << endl;

    // Menu-driven operations
    int option, val;
    do {
        cout << "What operation do you want to perform? " <<
            " Select Option number. Enter 0 to exit." << endl;
        cout << "1. Insert Key/Node" << endl;
        cout << "2. Search Key/Node" << endl;
        cout << "3. Delete Key/Node" << endl;
        cout << "4. Get Min" << endl;
        cout << "5. Extract Min" << endl;
        cout << "6. Height of Heap" << endl;
        cout << "7. Print/Traversal Heap values" << endl;
        cout << "8. Clear Screen" << endl;
        cout << "0. Exit Program" << endl;

        cin >> option;

        switch (option) {
            // Select option from Menu
        }

    } while (option != 0);

    return 0;
}
