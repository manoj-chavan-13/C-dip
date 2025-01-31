**Variables and Data Types in C**

### **1. Variables in C**

A variable in C is a named storage location that holds a value. It has a specific type that determines the size and layout of the memory, as well as the range of values that can be stored.

#### **1.1 Declaration of Variables**

In C, variables must be declared before use. The syntax for declaring a variable is:

```c
 data_type variable_name;
```

#### **1.2 Variable Initialization**

A variable can be assigned a value at the time of declaration:

```c
 int age = 25;
 float pi = 3.14;
 char grade = 'A';
```

#### **1.3 Rules for Naming Variables**

- Must start with a letter (A-Z or a-z) or underscore (\_).
- Can be followed by letters, digits (0-9), or underscores.
- Cannot be a C keyword.
- Case-sensitive (e.g., `age` and `Age` are different variables).

#### **1.4 Example of Variable Usage**

```c
#include <stdio.h>
int main() {
    int a = 10;
    float b = 5.5;
    char c = 'X';
    printf("Integer: %d\n", a);
    printf("Float: %f\n", b);
    printf("Character: %c\n", c);
    return 0;
}
```

### **2. Data Types in C**

C provides several fundamental data types for handling different kinds of data:

#### **2.1 Basic Data Types**

| Data Type | Size (bytes) | Range                           |
| --------- | ------------ | ------------------------------- |
| `int`     | 4            | -2,147,483,648 to 2,147,483,647 |
| `float`   | 4            | 1.2E-38 to 3.4E+38              |
| `double`  | 8            | 2.3E-308 to 1.7E+308            |
| `char`    | 1            | -128 to 127 or 0 to 255         |

#### **2.2 Derived Data Types**

- **Arrays**: Collection of elements of the same type.
- **Pointers**: Variables that store memory addresses.
- **Structures**: User-defined types that group related variables.
- **Unions**: Similar to structures but share memory space.

#### **2.3 Type Modifiers**

Type modifiers extend the functionality of standard data types.

| Modifier   | Description                                      |
| ---------- | ------------------------------------------------ |
| `short`    | Reduces storage size for `int`                   |
| `long`     | Increases storage size for `int` and `double`    |
| `signed`   | Allows storing both positive and negative values |
| `unsigned` | Stores only positive values                      |

#### **2.4 Example of Different Data Types**

```c
#include <stdio.h>
int main() {
    short s = 32767;
    long l = 2147483647;
    unsigned int ui = 4294967295;
    double d = 3.141592653589793;
    printf("Short: %d\n", s);
    printf("Long: %ld\n", l);
    printf("Unsigned Int: %u\n", ui);
    printf("Double: %lf\n", d);
    return 0;
}
```

#### **2.5 Type Conversion**

C allows implicit and explicit type conversions.

- **Implicit Conversion (Type Promotion)**: Automatic conversion of lower data type to a higher one.
  ```c
  int num = 5;
  float result = num / 2.0; // num is promoted to float
  ```
- **Explicit Conversion (Type Casting)**: Manually converting data types using type casting.
  ```c
  int x = 10, y = 3;
  float res = (float)x / y; // Explicitly converting x to float
  ```

### **Summary**

- Variables store data and must be declared before use.
- Data types define the kind of data a variable can hold.
- Type modifiers adjust the behavior of data types.
- Type conversion allows data types to be changed during operations.



