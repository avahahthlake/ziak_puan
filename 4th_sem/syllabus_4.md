# Syllabus of CSE UVCE 4th sem (literally)

## Design and Analysis of Algorithms (DAA)

### 🦣1️⃣

The Notion of Algorithm, Fundamentals of algorithmic Problem Solving. The Analysis of
Framework. Asymptotic Notations and Standard Efficiency Classes. Mathematical analysis of
Non-Recursive Algorithms. Mathematical Analysis of recursive algorithms. An Example: The
Fibonacci Numbers. Empirical Analysis of Algorithms. Algorithm Visualization.

### 🦣2️⃣

Brute-Force: Selection Sort and Bubble Sort. Sequential Search and Brute-Force String
Matching. Closest-Pair and Convex-Hull Problems by Brute Force. Exhaustive Search. Depth
First Search (DFS), Breadth First Search (BFS), Applications of DFS and BFS, Decrease and
conquer: Insertion Sort, Topological Sort, Generating Permutations, Binary search,
Computing Median and the Selection problem.

### 🦣3️⃣

Divide-and-Conquer: Mergesort, Quicksort, Binary Tree Traversals and Related Properties.
Multiplication of Large Integers and Strassen's Matrix Multiplication. Transform and
Conquer: Presorting and its Applications, Balanced Search Trees, Heaps and Heap sort.
Horner’s rule and Binary exponentiation, Space & Time Tradeoff: Horspool string matching
algorithm, B trees.

### 🦣4️⃣

Dynamic Programming: Basic examples, The Knapsack Problem and Memory Functions
Binomial Coefficients, Optimal Binary Search Trees, Warshall's and Floyd's Algorithms,
Greedy Approach: Prim's Algorithm. Kruskal's Algorithm. Dijkstra's Algorithm. Huffman
Trees.

### 🦣5️⃣

Backtracking: n-Queens Problem, Subset-Sum Problem, Branch-and-Bound: Travelling
Salesman problem, Knapsack Problem, Approximation Algorithms for NP hard problems,
Limitations of Algorithm Power: Decision Trees, P, NP, and NP-Complete Problems.

## Microprocessor and Microcontroller (MnM)

### 🦎1️⃣

The x86 microprocessor: Brief history
of the x86 family, Inside the 8088/86, Introduction to assembly programming, Introduction to
Program Segments, The Stack, Flag register, x86 Addressing Modes. Assembly language
programming: Directives & a Sample Program, Assemble, Link & Run a program, More Sample
programs, Control Transfer Instructions, Data Types and Data Definition, Full Segment
Definition, Flowcharts and Pseudo code.

### 🦎2️⃣

x86: Instructions sets description,
Arithmetic and logic instructions and programs: Unsigned Addition and Subtraction, Unsigned
Multiplication and Division, Logic Instructions, BCD and ASCII conversion, Rotate Instructions.
INT 21H and INT 10H Programming2️: BIOS INT 10H Programming, DOS Interrupt 21H.
8088/86 Interrupts, x86 PC and Interrupt Assignment.

### 🦎3️⃣

8255 Pin descriptions,
Architecture, Control register, Mode 0, Mode 1 and Mode 2 Operations, Interfacing of DAC and
ADC to 8086 in Mode 0 only. 8255 I/O programming: I/O addresses MAP of x86 PC’s,
programming and interfacing the 8255. 8253 – Programmable timer, pin functions, architecture,
Mode 0, 1, 2, 3, 4, and 5 operations, Programs for monostable and astable operations.

### 🦎4️⃣

Microprocessors versus
Microcontrollers, ARM Embedded Systems: The RISC design philosophy, The ARM Design
Philosophy, Embedded System Hardware, Embedded System Software, ARM Processor
Fundamentals: Registers, Current Program Status Register, Pipeline, Exceptions, Interrupts, and
the Vector Table, Core Extensions.

### 🦎5️⃣

Introduction to the ARM Instruction Set: Data Processing
Instructions, Branch Instructions, Software Interrupt Instructions, Program Status Register
Instructions, Coprocessor Instructions, Loading Constants, Simple programming exercises.

## Operating Systems (OS)

### 🐁1️⃣

System structures: What operating systems do; Computer System organization;
Computer System architecture; Operating System structure; Operating System operations;
Process management; Memory management; Storage management; Protection and Security;
Distributed system; Special-purpose systems; Computing environments. Operating System
Services; User - Operating System interface; System calls; Types of system calls; System
programs; Virtual machines; Operating System generation; System boot. Process
Management Process concept; Process scheduling; Operations on processes; Inter process
communication

### 🐁2️⃣

Multi-Threaded Programming: Overview; Multithreading models; Thread Libraries;
Threading issues. Process Scheduling: Basic concepts; Scheduling Criteria; Scheduling
Algorithms; Multiple-processor scheduling; Thread scheduling. Process Synchronization:
Synchronization: The critical section problem; Peterson’s solution; Synchronization
hardware; Semaphores; Classical problems of synchronization; Monitors.

### 🐁3️⃣

Deadlocks: Deadlocks; System model; Deadlock characterization; Methods for handling
deadlocks; Deadlock prevention; Deadlock avoidance; Deadlock detection and recovery from
deadlock. Memory Management: Memory management strategies: Background; Swapping;
Contiguous memory allocation; Paging; Structure of page table; Segmentation

### 🐁4️⃣

Virtual Memory Management: Background; Demand paging; Copy-on-write; Page replacement; Allocation of frames; Thrashing. File System, Implementation of File System:
File system: File concept; Access methods; Directory structure; File system mounting; File
sharing; Protection: Implementing File system: File system structure; File system
implementation; Directory implementation; Allocation methods; Free space management.

### 🐁5️⃣

Secondary Storage Structures, Protection: Mass storage structures; Disk structure;
Disk attachment; Disk scheduling; Disk management; Swap space management. Protection:
Goals of protection, Principles of protection, Domain of protection, Access matrix,
Implementation of access matrix, Access control, Revocation of access rights, Capability-
Based systems. Case Study: The Linux Operating System: Linux history; Design principles;
Kernel modules; Process management; Scheduling; Memory Manage ment; File systems,
Input and output; Inter-process communication
Note: The concepts in all 5 units to be supported by Example Programs.

## Design and Analysis of Algorithms Laboratory (DAA-Lab)

1. Sort a given set of elements using Merge sort and determine the time required to sort the
elements. Repeat the experiment for different values of n, the number of elements in the
list to be sorted and plot graph of the time taken versus number of elements. The elements
can be read from file or generated using random number generator.
2. Sort a given set of elements using Quick sort and determine the Worst case and Average
case time required to sort the elements. Repeat the experiment for different values of n, the
number of elements in the list to be sorted and plot graph of the time taken versus number
of elements. The elements can be read from file or generated using random number
generator.
3. Perform insert and delete operations in Binary Search Tree.
4. Print all the nodes reachable from a given starting node in a digraph using BFS method.
5.
    a. Obtain the Topological ordering of vertices in a given digraph.
    b. Compute the transitive closure of a given directed graph using Warshall’s algorithm.
6. Sort a given set of elements using the Heap sort method and determine the time required to
sort the elements. Repeat the experiment for different values of n, the number of elements in
the list to be sorted and plot a graph of the time taken versus number of elements.
7. Search for a pattern string in a given text using Horspool String Matching algorithm.
8. Implement 0/1 Knapsack problem using dynamic programming.
9. Find Minimum Cost Spanning Tree of a given undirected graph using Prim’s algorithm.
10. Find Minimum Cost Spanning Tree of a given undirected graph using Kruskal's
algorithm.
11. From a given vertex in a weighted connected graph, find shortest paths to other vertices
using
Dijkstra's algorithm.
12. Solve Travelling Sales Person problem using dynamic programming approach.
13. Implement N Queen's problem using Back Tracking.
14. Find a subset of a given set S = {Sl, S2,.....,Sn} of n positive integers whose SUM is
equal
to a given positive integer d.

## Microprocessor and Microcontroller Laboratory

SOFTWARE PROGRAMS: PART A

1. Design and develop an assembly language program to search a key e lement “X” in a
list of ‘n’ 16-bit numbers. Adopt Binary search algorithm in your program for
searching.
2. Design and develop an assembly program to sort a given set of ‘n’ 16-bit numbers in
ascending order. Adopt Bubble Sort algorithm to sort given elements.
3. Develop an assembly language program to reverse a given string and verify whether it
is a palindrome or not. Display the appropriate message.
4. Develop an assembly language program to compute nCr using recursive procedure.
Assume that ‘n’ and ‘r’ are non-negative integers.
5. Design and develop an assembly language program to read the current time and Date
from the system and display it in the standard format on the screen.
6. To write and simulate ARM assembly language programs for data transfer, arithmetic
and logical operations (Demonstrate with the help of a suitable program).
7. To write and simulate C Programs for ARM microprocessor using KEIL
(Demonstrate with the help of a suitable program)

HARDWARE PROGRAMS: PART B

1. Design and develop an assembly program to demonstrate BCD Up-Down Counter
(00-99) on the Logic Controller Interface.
2. Design and develop an assembly program to read the status of two 8-bit inputs (X &
Y) from the Logic Controller Interface and display X*Y.
3. Design and develop an assembly program to display messages “FIRE” and “HELP”
alternately with flickering effects on a 7-segment display interface for a suitable
period of time. Ensure a flashing rate that makes it easy to read both the messages
(Examiner does not specify these delay values nor is it necessary for the student to
compute these values).
4. Design and develop an assembly program to drive a Stepper Motor interface and
rotate the motor in specified direction (clockwise or counter-clockwise) by N steps
(Direction and N are specified by the examiner). Introduce suitable delay between
successive steps. (Any arbitrary value for the delay may be assumed by the student).
5. Design and develop an assembly language program to generate the Sine Wave using
DAC interface (The output of the DAC is to be displayed on the CRO).
6. Design and develop an assembly language program to generate a Half Rectified Sine
waveform using the DAC interface. (The output of the DAC is to be displayed on the
CRO).
7. To interface LCD with ARM processor-- ARM7TDMI/LPC2148. Write and execute
programs in C language for displaying text messages and numbers on LCD
8. To interface Stepper motor with ARM processor-- ARM7TDMI/LPC2148. Write a
program to rotate stepper motor.

## UNIX System Programming Laboratory

IMPLEMENT THE FOLLOWING PROGRAMS USING C OR C++:

1. Check the following limits:
No. of clock ticks, Max. no. of child processes, Max. path length, Max. no. of characters
in a file name, Max. no. of open files/ process
2. a. Copy of a file using system calls.
b. Output the contents of its Environment list
3. a. Emulate the UNIX ln command
b. Create a child from parent process using fork() and counter counts till 5 in both
processes and displays.
4. Illustrate two processes communicating using shared memory.
5. Demonstrate producer and consumer problem using semaphores.
6. Demonstrate round robin scheduling algorithm and calculates average waiting time and
average turnaround time.
7. Implement priority-based scheduling algorithm and calculates average waiting time and average turnaround time.
1. Act as sender to send data in message queues and receiver that reads data from message
queue.
1. Where a parent writes a message to pipe and child reads message from pipe.
2.  Demonstrate setting up a simple web server and host website on your own Linux
computer.
1.  a. Create two threads using pthread, where both thread counts until 100 and joins later.
b. Create two threads using pthreads. Here, main thread creates 5 other threads for 5
times and each new thread print “Hello World” message with its thread number.
1.  Using Socket APIs establish communication between remote and local processes.

## Web Design Laboratory

LAB PROGRAMS

1. Create a table to show your class time table.
2. Use tables to provide layout to your HTML page describing your college
infrastructure.
3. Use span and div tags to provide a layout to the above page instead of
a table layout.
4. Use frames such that page is divided into 3 frames 20% on left to show
contents of pages, 60% in center to show body of page, remaining on right
to show remarks.
5. Embed Audio and Video into your HTML web page.
6. Develop static pages (using only HTML) of an online book store, the pages
should resemble: <www.amazon.com>, the website should consist the
following pages, home page, registration and user login, user profile page,
books catalog, shopping cart, payment by credit card, order confirmation.
7. Write an HTML page that contains a selection box with a list of 5 countries,
when the user selects a country, its capital should be printed next to the list;
Add CSS to customize the properties of the font of the capital (color, bold
and font size).
8. Write a java script program to test the first character of a string is uppercase
or not. b. Write a pattern that matches e-mail addresses. c. Write a java
script function to print an integer with commas as thousands separators.
9. A simple calculator web application that takes two numbers and an operator
(+, ,/,*and %) from an HTML page and returns the result page with the
operation performed on the operands. b. Write PHP program how to send
mail using PHP.

## Mathematics

### ➕➖➗1

Sets in a complex plane - Functions of a complex variables. Limit, Continuity and
differentiability (definitions only). Analytic function - Riemann equations in Cartesian and polar forms. Harmonic functions, Constructions of analytic functions (Cartesian and polar
forms). Line integral - - function and for derivatives, Conformal transformations: and .
Bilinear transformations.

### ➕➖➗2

Power series, convergence, radius of convergence, Taylor's and Laurent's theorems
(Statements only) Singularities. Poles Calculation of residues. Residue theorem (without proof) problems. Evaluation of Contour integrals

### ➕➖➗3

Numerical solution of algebraic and transcendental equations-solution by Bisection, Ramanujan method, linear iteration and Newton-Raphson methods. Solution of linear
simultaneous equations: Gauss elimination method, Gauss Jordan method, Gauss Seidel
methods, LU decomposition method, methods of Crout, Doolittle and Cholesky.

### ➕➖➗4

Finite differences (Forward and backward differences), Interpolation, Newtons forward and backward interpolation formulae, Central difference formulae: stirlings and Bessels formula. Interpolation with unequal spaced points: Lagarange interpolation formula, and inverse interpolation formulae. Divided differences and their properties: Newtons general interpolation formula. Interpolation by iteration, Numerical differentiation using Newtons forward and
backward interpolation formulae, Numerical integration: Trapezoidal method, Simpson 1/3
rule Simpons3/8th rule.

### ➕➖➗5

Numerical solution of ordinary differential equations. Solutions by Taylor's series, Picard's method of successive approximation, modifiend Euler's method, Runge Kutta methods of second and fourth order, Predictor and corrector methods - Adams - Bashforth method, Adams-Moultons method.

## Constitution of India and Professional Ethics

### 😎1

Preamble to the Constitution of India. Fundamental rights under Part-III-details of Exercise of
rights, Limitations & Important case laws.

### 😎2

Relevance of Directive principles of State Policy under Part-IV, Fundamental Duties & their
significance.

### 😎3

Union Executive President, Prime Minister, Parliament & the Supreme Court of India.
State Executive Governors, Chief Minister, State Legislator and High Courts.

### 😎4

Constitutional Provisions for Scheduled Castes & Tribes, Women & Children & Backward
classes; Emergency Provisions; Electoral process; Amendment procedure; Latest Important
Constitutional amendments

### 😎5

Scope & aims of engineering ethics, Responsibility of Engineers; Impediments to
responsibility; Honesty, Integrity and reliability, risks, safety & liability in engineering.
