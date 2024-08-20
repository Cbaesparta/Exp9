# Exp9
## What are Pointers in C++?
In C++, a pointer is a type of variable that stores the memory address of another variable. Unlike regular variables that directly store data (like integers or characters), pointers store the location in memory where the actual data is kept. They enable indirect access to values, which can be beneficial in various scenarios, such as dynamic memory management and passing data efficiently in functions.

## Key Concepts of Pointers:
Memory Address: Each variable in memory has a unique location or address, where its data is stored.
Pointer Variable: A pointer holds this memory address, allowing you to refer to the variable indirectly.
Dereferencing: This is the process of accessing or modifying the data stored at the memory address that the pointer holds.
## Syntax of Pointers:
### Declaring a Pointer:

When declaring a pointer, you define the type of data the pointer will point to, followed by an asterisk (*), and then the name of the pointer.

int* ptr;  

### Assigning an Address to a Pointer:

To make a pointer point to a variable, you assign it the address of the variable using the address-of operator (&).

int num = 10;
int* ptr = &num;

### Dereferencing a Pointer:

Dereferencing a pointer means accessing the value stored at the memory address that the pointer is pointing to. This is done using the asterisk (*) before the pointer name.

int value = *ptr;
## code:
```
//name: Sai Sankar Jena
//prn: 23070123112
#include <iostream>
using namespace std;

int main() {
    int num1 = 4, num2 = 5;
    int *ptr1 = &num1; 
    int *ptr2 = &num2; 

    cout << "Original values: " << endl;
    cout << "num1 = " << *ptr1 << ", num2 = " << *ptr2 << endl;

    *ptr1 = (*ptr1) * (*ptr2); 
    cout << "After multiplication, new value of num1 = " << *ptr1 << endl;

    return 0;
}
```
## output:
```
Original values: 
num1 = 4, num2 = 5
After multiplication, new value of num1 = 20
```
## Key Syntax Elements:
1) int* ptr: Declares a pointer ptr that is capable of holding the address of an integer variable.
2) ptr = &num: Assigns the address of the variable num to the pointer ptr.
3) *ptr: Dereferences the pointer, which means it retrieves the value from the memory location stored in ptr.
 
