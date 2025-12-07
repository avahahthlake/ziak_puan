# 🍔 Stack 📚
A stack is an abstract data type that serves as a collection of elements
with two operations -> push and pop. A stack uses the Last In First Out (*LIFO*) policy.

![stacks](assets/stacks.png)

### Array implementation of stacks
```c
#define MAX 5
int stack[MAX];
int top = -1;
// push function
void push(int value) {
  if (top >= MAX-1) {
    printf("Stack overflowed. Cannot push %d\n", value);
    return;
  } else {
    ++top;
    stack[top] = value;
    printf("Pushed %d\n", value);
    return;
  }
}
// pop function
void pop() {
  if (top <= -1) {
    printf("Stack underflowed. No element to pop\n");
    return;
  } else {
    printf("Poped %d\n", stack[top]);
    top--;
    return;
  }
}
```

# Applications of stacks 🈸
### Polish Notation 💅 and reverse Polish Notation 💅🏿
***These eliminate parentheses and operator precedence issues***, thus making it
easier for machines to do computations.

This is how stacks help in evaluating Polish notation expressions...
1. Read left to right... Process the expression one token at a time.
2. Operand encountered... Push the number(operand) onto the stack
3. Operator encountered...
    * pop the top two operands from the stack (say op2 and op1)
    * perform the operation (op1 + op2)
    * push the result back onto the stack

Here is an example of postfix (reverse Polish Notation expression) evaluation.
Suppose we have the expression ... 3 4 + 2 *
```evaluation
push 3 (stack = [3])
push 4 (stack = [3, 4])
operator + : pop 4, pop 3, calculate 3+4=7, push 7 (stack = [7])
push 2 (stack = [7, 2])
operator * : pop 2, pop 7, calculate 7*2=14, push 14 (stack = [14])
then result is 14
```

### Infix to prefix and infix to postfix conversion 👶
*I need to deal with this later...* 💣

### How recursion uses the ***call-stack*** in a factorial()
Each time a function (say factorial(n)) is called, a **stack-frame**
containing its parameters, local variable and return address is pushed onto the stack.

For a recursive function like factorial() this repeats till the base case is hit.

  * recursive-calls...If n is greater than the base case factorial(n) calls factorial(n-1). This new call pushes another stack-frame onto the stack, effectively pausing the execution of the previous call. The process continues, with each recursive call adding a new frame until the base case is reached.
  * base case and unwinding... When base case is reached (say n = 0), the function returns a value, this return causes the topmost stack-frame to be popped off the stack.
  * returning values and calculation ...As each stack frame is popped, the execution of the calling function resumes from where it is left off. The return-value from the deeper call is then used in the calculation of the current call (e.g. n*factorial(n-1), ...)
  * this popping of stack-frame continues until the initial stack-frame is reached and finally...
  * the return value happens...

![stack-frame-factorial](assets/stack-frame-factorial.png)

### Fibonacci in C 😊
```c
#include <stdio.h>
int getFib(int n) {
    if (n <= 1) {
        return n;
    }
    return getFib(n - 1) + getFib(n - 2);
}
int main() {
    int n = 10; // Number of terms to print
    printf("Fibonacci Series: ");
    for (int i = 0; i < n; i++) {
        printf("%d, ", getFib(i));
    }
    printf("\n");
    return 0;
}
```

### Tower of Hanoi in C 🤗
```c
#include <stdio.h>
#include <stdlib.h>
void hanoi(int n, char fr, char tr, char ar) // fr = from rod, tr = to rod, ar = aux rod
{
  if (n == 1)
  {
    printf("\n Move disk 1 from rod %c to rod %c", fr, tr);
    return;
  }
  hanoi(n-1, fr, ar, tr);
  printf("\n Move disk %d from rod %c to rod %c", n, fr, tr);
  hanoi(n-1, ar, tr, fr);
}
int main(int argc, char* argv[])
{
  int n = atoi(argv[1]); // n implies the number of discs
  hanoi(n, 'A', 'C', 'B');
  printf("\n");
  return 0;
}
```
