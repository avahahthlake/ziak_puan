# 🫥 Introduction to data structures 🫥

What are data structures ? Well, data structures are ways of arranging data so
that we can access them efficiently. By *access*, we talk about insertion,
deletion, traversing, etc. There are different kinds of data structures btw...

## 🤭 Primitive data structures 🤭

Primitive data structures are the basic building blocks available within a
programming language. They may store single, simple values. Examples are integers (int) floating point numbers (floats) characters (chars) and booleans.

## 🤨 Non primitive data structures 😮

Non primitive data structures (*aka* user-defined data structures) are more
complex and are derived from the primitive data types. They are used to store
collection of values, often linking them together in specific arrangements.
Examples are arrays, linked list, stacks, queues, trees, graphs, etc...

* so their main difference is complexity

## 🏛️ Storage Classes 🏛

In programming, storage classes determine...

* A variable's scope (visibility)
* Lifetime (how long it exists)
* Memory Location
* Default initial value

## 🔠 C storage classes 🔤

* auto (automatic) -> This is the default class for local variables.
  They exists on the stack only within the block they are declared. With a
  garbage default value.
* register -> This suggests storing the variable in a CPU register for speed.
* static -> Retains value across function calls. They have local or file
  scope.
* extern -> This declares a global variable defined elsewhere. They have
  global scope.

## 🥶 Bit fields 🥶

Bit field is a feature in programming languages like C and C++ that allows
us to specify how many bit does each attribute in our structure or class
should occupy. This is all for memory efficiency.
``` c
// example usage of bit fields
struct StatusFlags {
    unsigned int error : 1;    // 1 bit for error status
    unsigned int ready : 1;    // 1 bit for ready status
    unsigned int mode : 2;     // 2 bits for mode selection (e.g., 0-3)
    unsigned int : 0;          // Special: Force alignment to the next underlying data type boundary
    unsigned int version : 4;  // 4 bits for version number
};
```

## Difference between structs and unions in C 🥰

| structs | unions |
| -------------- | --------------- |
| memory occupied is sum of all members' size, each member gets its own space | memory occupied is size of the largest member, all members share the same starting address |
| It holds multiple, distinct pieces of data together | It stores one of several related data types |
| All members are accessible at any time | Only one member can be accessed at a time |

```c
// struct example
struct Person {
    char name[50];
    int age;
    float salary;
};
```

```c
// union example
union Data {
    int i;
    float f;
    char str[20];
};
```


## 🫠 Array of structures 🫠

An array of structure is a data structure where each element of array is an
instance of a defined structure...🤩 It is used to *group data*, manage multiple records
efficiently, common examples include a list of employees, a collection of books, etc...

```c
// array of structures example
#include <stdio.h>
// Define a structure for a student
struct Student {
    char name[50];
    int roll_number;
    float marks;
};
// Function to input student details
void inputStudent(struct Student *s, int index) {
    printf("Enter details for student %d:\n", index + 1);
    printf("Name: ");
    scanf("%49s", s->name);  // safer
    printf("Roll Number: ");
    scanf("%d", &s->roll_number);
    printf("Marks: ");
    scanf("%f", &s->marks);
    printf("\n");
}
// Function to display student details
void displayStudent(struct Student s, int index) {
    printf("Student %d Details:\n", index + 1);
    printf("Name: %s\n", s.name);
    printf("Roll Number: %d\n", s.roll_number);
    printf("Marks: %.2f\n\n", s.marks);
}
int main() {
    const int SIZE = 3;
    struct Student students[SIZE];
    // Input data for all students
    for (int i = 0; i < SIZE; i++) {
        inputStudent(&students[i], i);
    }
    // Display all students' data
    for (int i = 0; i < SIZE; i++) {
        displayStudent(students[i], i);
    }
    return 0;
}
```

## Array within structure ☺

This means member(s) of the structure is(are) array(s).
```c
#include <stdio.h>
// Define a structure named Student
struct Student {
    int roll_number;
    char grade;
    int marks[5]; // Array to store marks in 5 subjects
};
int main() {
    // Declare a variable of type struct Student
    struct Student s1;
    // Assign values to the structure members
    s1.roll_number = 101;
    s1.grade = 'A';
    s1.marks[0] = 85;
    s1.marks[1] = 90;
    s1.marks[2] = 78;
    s1.marks[3] = 92;
    s1.marks[4] = 88;
    // Access and print the structure members
    printf("Student Roll Number: %d\n", s1.roll_number);
    printf("Student Grade: %c\n", s1.grade);
    printf("Marks in subjects: ");
    for (int i = 0; i < 5; i++) {
        printf("%d ", s1.marks[i]);
    }
    printf("\n");
    return 0;
}
```

## 🙈 Structure within structure 🧑‍🏫

Structure within structure is a way of doing things in c/c++ where a member of a
structure is also a structure. This allows logical grouping of complex but related
data.

```c
// example
struct Date {
    int dd;
    int mm;
    int yyyy;
};
struct Employee {
    int id;
    char name[20];
    struct Date doj; // Nested structure variable
};
```

## 🤳 Self-referential structure 🤳

A Self-referential structure is a type of structure that has a member which is a pointer
to another instance of the same structure type. A good example and use of this kind of
structure is how nodes are modeled for linked lists, trees, etc...
```c
// example of self-referential structure
struct Node {
  int data;
  struct Node* left;
  struct Node* right;
};
```

## 😔 Pointers and Arrays 🫠

* A pointer is a special type of variable that stores the address of another variable.
* An array is a linear collection of similar type of data.
* When we define an array, the array name is actually the base address that behaves
  like a pointer to the address of the first element of the array.

## 🫠 Array of pointers 👈🏻

An array of pointers is a data structure where each element of the array is a pointer.
Advantages are -> flexible memory management.
```c
//syntax
int var1 = 10, var2 = 20, var3 = 30;
int *ptr_array[] = {&var1, &var2, &var3}; // Initializes with addresses of var1, var2, var3
```

## 😔 Pointers to function

Pointers to functions are basically pointer-variables that hold the starting memory
address of a function's machine code. Usually, they are used for dynamic function calls,
callbacks (passing function to to other functions) 
```c
#include <stdio.h>
// A function to add two numbers
int add(int a, int b) {
    return a + b;
}
// A function to subtract two numbers
int subtract(int a, int b) {
    return a - b;
}
int main() {
    // Declare a function pointer that points to a function taking two ints and returning an int
    int (*operation)(int, int); 
    // Assign the 'add' function to the pointer
    operation = add; 
    printf("Addition: %d\n", operation(10, 5)); // Output: Addition: 15
    // Assign the 'subtract' function to the pointer
    operation = subtract; 
    printf("Subtraction: %d\n", operation(10, 5)); // Output: Subtraction: 5
    return 0;
}
```

## 🤷 Different ways of dynamic memory allocation 🤷🏻‍♂

What is dynamic memory allocation ? Basically it is allocation of memory on the fly.
Which means allocating memory during program execution(runtime) from the heap, rather
than at compile time.

#### malloc()

malloc() allocates **a block of memory** of a specified size in bytes. It returns a
void pointer at the beginning of the allocated block. *The allocated memory is
uninitialized and may contain garbage values*
```c
    int *ptr = (int *)malloc(5 * sizeof(int)); // Allocates space for 5 integers
    if (ptr == NULL) {
        // Handle allocation failure
    }
```

#### calloc()

calloc() allocates memory for an array of n elements, each of a specified size, and
Initializes all bytes to 0. It returns void pointer to the allocated memory. If
allocation fails, it return NULL.
```c
    int *arr = (int *)calloc(10, sizeof(int)); // Allocates space for 10 integers, all initialized to 0
    if (arr == NULL) {
        // Handle allocation failure
    }
```

#### realloc()

realloc() changes the size of a previouly allocated memory block.
```c
    int *ptr = (int *)malloc(5 * sizeof(int));
    // ... use ptr ...
    ptr = (int *)realloc(ptr, 10 * sizeof(int)); // Resize to hold 10 integers
    if (ptr == NULL) {
        // Handle reallocation failure
    }
```

#### free()

So the free() deallocates previouly allocated dynamic memory, returning it to the heap
for reuse.
```c
    free(ptr); // Deallocate the memory pointed to by ptr
    ptr = NULL; // Good practice to set the pointer to NULL after freeing
```

### Why dynamic memory allocation is better 👌

Dynamic memory allocation is better than static memory allocation because it allows for
flexibility. Like handling data input of different sizes. Dynamic memory allocation
allows flexibility of the code.
