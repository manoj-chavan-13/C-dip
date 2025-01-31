**Operators in C**

Operators in C are symbols that perform operations on variables and values. They are categorized into different types based on their functionality.

### **1. Arithmetic Operators**
Arithmetic operators are used to perform mathematical calculations.

| Operator | Description | Example |
|----------|-------------|---------|
| `+` | Addition | `a + b` |
| `-` | Subtraction | `a - b` |
| `*` | Multiplication | `a * b` |
| `/` | Division | `a / b` |
| `%` | Modulus (remainder) | `a % b` |

**Example:**
```c
#include <stdio.h>
int main() {
    int a = 10, b = 3;
    printf("Addition: %d\n", a + b);
    printf("Subtraction: %d\n", a - b);
    printf("Multiplication: %d\n", a * b);
    printf("Division: %d\n", a / b);
    printf("Modulus: %d\n", a % b);
    return 0;
}
```

### **2. Relational (Comparison) Operators**
These operators compare values and return a boolean result (true or false).

| Operator | Description | Example |
|----------|-------------|---------|
| `==` | Equal to | `a == b` |
| `!=` | Not equal to | `a != b` |
| `>` | Greater than | `a > b` |
| `<` | Less than | `a < b` |
| `>=` | Greater than or equal to | `a >= b` |
| `<=` | Less than or equal to | `a <= b` |

**Example:**
```c
if (a > b) {
    printf("a is greater than b");
}
```

### **3. Logical Operators**
Logical operators are used to perform logical operations (AND, OR, NOT).

| Operator | Description | Example |
|----------|-------------|---------|
| `&&` | Logical AND | `(a > 5 && b < 10)` |
| `||` | Logical OR | `(a > 5 || b < 10)` |
| `!` | Logical NOT | `!(a == b)` |

**Example:**
```c
if (a > 5 && b < 10) {
    printf("Both conditions are true");
}
```

### **4. Bitwise Operators**
Bitwise operators perform operations at the bit level.

| Operator | Description | Example |
|----------|-------------|---------|
| `&` | Bitwise AND | `a & b` |
| `|` | Bitwise OR | `a | b` |
| `^` | Bitwise XOR | `a ^ b` |
| `~` | Bitwise Complement | `~a` |
| `<<` | Left shift | `a << 2` |
| `>>` | Right shift | `a >> 2` |

**Example:**
```c
int result = a & b; // Performs bitwise AND
```

### **5. Assignment Operators**
Assignment operators assign values to variables.

| Operator | Description | Example |
|----------|-------------|---------|
| `=` | Assign | `a = 5` |
| `+=` | Add and assign | `a += 5` (same as `a = a + 5`) |
| `-=` | Subtract and assign | `a -= 5` |
| `*=` | Multiply and assign | `a *= 5` |
| `/=` | Divide and assign | `a /= 5` |
| `%=` | Modulus and assign | `a %= 5` |

### **6. Increment and Decrement Operators**
These operators increase or decrease a variable's value by 1.

| Operator | Description | Example |
|----------|-------------|---------|
| `++` | Increment | `a++` (post-increment), `++a` (pre-increment) |
| `--` | Decrement | `a--` (post-decrement), `--a` (pre-decrement) |

**Example:**
```c
int a = 5;
printf("Post-increment: %d\n", a++); // Prints 5, then increments
printf("Pre-increment: %d\n", ++a); // Increments first, then prints
```

### **7. Conditional (Ternary) Operator**
A compact way to write simple `if-else` conditions.

| Operator | Description | Example |
|----------|-------------|---------|
| `?:` | Ternary Operator | `result = (a > b) ? a : b;` |

**Example:**
```c
int max = (a > b) ? a : b; // Assigns the larger value to max
```

### **8. Special Operators**
- **Sizeof Operator (`sizeof`)**: Returns the size of a variable or data type.
  ```c
  int size = sizeof(int); // Returns 4 (on most systems)
  ```
- **Comma Operator (`,`)**: Used to separate multiple expressions.
  ```c
  int a = (1, 2, 3); // a is assigned 3
  ```
- **Pointer Operators (`&` and `*`)**:
  ```c
  int *ptr = &a; // Stores address of a in ptr
  ```

