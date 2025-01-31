

# **Complete C Programming Course Guide**

## **Week 1: Problem Solving Using Computers**

### **1.1 Introduction**

- **Definition**: Problem-solving is the process of breaking down complex issues into smaller, manageable parts to find solutions.
- **Role of Computers**: Computers help automate solutions, perform calculations, and handle large datasets efficiently.
- **Steps in Problem Solving**:
  1. **Understanding the problem**
  2. **Designing an algorithm**
  3. **Implementing the solution**
  4. **Testing and debugging**

### **1.2 Computers and Computing**

- **Definition of Computing**: Computing involves processing data using computers to generate meaningful results.
- **Basic Components of a Computer**:
  - Input devices (Keyboard, Mouse)
  - Processing unit (CPU, Memory)
  - Output devices (Monitor, Printer)
- **Binary Representation**:
  - Computers understand only **0s and 1s** (Binary System).
  - Example: Decimal `10` → Binary `1010`.

### **1.3 Programming**

- **Definition**: Programming is writing instructions that a computer can execute.
- **Types of Programming Languages**:
  - Low-level (Assembly, Machine Code)
  - High-level (C, Python, Java)
- **Compilers and Interpreters**:
  - **Compiler**: Translates code all at once (C, C++)
  - **Interpreter**: Translates code line by line (Python, JavaScript)

---

## **Week 2: Internal Representation of Data**

### **2.1 Number Systems**

- **Decimal (Base 10)**: Digits from 0-9 (e.g., `25`)
- **Binary (Base 2)**: Digits 0,1 (e.g., `1101`)
- **Octal (Base 8)**: Digits 0-7 (e.g., `37`)
- **Hexadecimal (Base 16)**: Digits 0-9, A-F (e.g., `2F`)

### **2.2 Negative Number Representation**

- **Sign-Magnitude**: Most significant bit (MSB) represents sign.
- **Two's Complement** (Most widely used):
  - Example: `-5` in 8-bit → `11111011`

---

## **Week 3: Elements of C Program – Part 1**

### **3.1 Basic C Program Structure**

```c
#include <stdio.h>
int main() {
    printf("Hello, World!\n");
    return 0;
}
```

### **3.2 Compilation and Execution**

- **GCC Compiler** (Linux/Windows):

```sh
gcc program.c -o program
./program
```

### **3.3 Data Types & Variables**

- **Primitive Data Types**:
  - `int` (e.g., `int age = 20;`)
  - `float` (e.g., `float price = 19.99;`)
  - `char` (e.g., `char grade = 'A';`)

---

## **Week 4: Elements of C Program – Part 2**

### **4.1 Operators in C**

- **Arithmetic**: `+ - * / %`
- **Relational**: `== != > < >= <=`
- **Logical**: `&& || !`
- **Bitwise**: `& | ^ << >>`

---

## **Week 5: Conditional Statements**

```c
if (age >= 18) {
    printf("Adult");
} else {
    printf("Minor");
}
```

```c
switch(choice) {
    case 1: printf("One"); break;
    case 2: printf("Two"); break;
    default: printf("Invalid");
}
```

---

## **Week 6: Loops**

```c
for(int i = 0; i < 5; i++) {
    printf("%d ", i);
}
```

```c
int i = 0;
while(i < 5) {
    printf("%d ", i);
    i++;
}
```

```c
do {
    printf("Hello");
} while(0);
```

---

## **Week 7: Functions**

- **Function Definition**:

```c
void greet() {
    printf("Hello, World!");
}
int main() {
    greet();
    return 0;
}
```

- **Call by Value vs Call by Reference**

---

## **Week 8 & 9: Arrays**

- **1D Array**

```c
int arr[5] = {1, 2, 3, 4, 5};
```

- **2D Array**

```c
int matrix[2][2] = {{1,2}, {3,4}};
```

---

## **Week 10: Strings**

```c
char name[20];
scanf("%s", name);
printf("%s", name);
```

```c
strcat(str1, str2);
strlen(str1);
strcmp(str1, str2);
```

---

## **Week 11: Structures & Unions**

- **Structures**

```c
struct Student {
    char name[50];
    int age;
};
```

---

## **Week 12 & 13: Pointers**

```c
int a = 10;
int *ptr = &a;
printf("%d", *ptr);
```

---

## **Week 14: Dynamic Memory Management**

```c
int *ptr = (int*)malloc(5 * sizeof(int));
free(ptr);
```

---

## **Week 15: Linked Lists**

```c
struct Node {
    int data;
    struct Node* next;
};
```

---

## **Week 16: File I/O & Command Line Arguments**

- **Writing to a File**

```c
FILE *fptr;
fptr = fopen("file.txt", "w");
fprintf(fptr, "Hello File");
fclose(fptr);
```

- **Command Line Arguments**

```c
int main(int argc, char *argv[]) {
    printf("Argument: %s", argv[1]);
}
```

---



