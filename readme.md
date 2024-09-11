#include<iostream>
using namespace std;

#### Print Text

```cpp
int main(){
     cout << "Hello World";
    return 0;
 }
```

#### New Line

```cpp
int main(){
    cout << "Hello  \n";
    cout << " World" << "\n";
    cout << "Bangladesh" << endl;
    cout << "Bangladesh ";
    return 0;
}
```

##### Creates a horizontal tab -> \t

##### Inserts a backslash character (\) -> \\

##### Inserts a double quote character -> \"

#### Variables

- int - stores integers (whole numbers), without decimals, such as 123 or -123
- double - stores floating point numbers, with decimals, such as 19.99 or -19.99
- char - stores single characters, such as 'a' or 'B'. Char values are surrounded by single quotes
- string - stores text, such as "Hello World". String values are surrounded by double quotes
- bool - stores values with two states: true or false

##### int

```cpp
int main() {
    int myNum;
    myNum = 15;
    cout << myNum;
}
```

```cpp
int myNum = 5;               // Integer (whole number without decimals)
double myFloatNum = 5.99;    // Floating point number (with decimals)
char myLetter = 'D';         // Character
string myText = "Hello";     // String (text)
bool myBoolean = true;       // Boolean (true or false)
```

#### The general rules for naming variables are:

- Names can contain letters, digits and underscores
- Names must begin with a letter or an underscore (\_)
- Names are case-sensitive (myVar and myvar are different variables)
- Names cannot contain whitespaces or special characters like !, #, %, etc.
- Reserved words (like C++ keywords, such as int) cannot be used as names

##### When you do not want others (or yourself) to change existing variable values, use the const keyword

```cpp
int main() {
   const int myNum = 10;
    cout << myNum;
}
```

#### User Input

```cpp
int main() {
  int x;
  cout << "Type a number: ";      // Type a number and press enter
  cin >> x;                       // Get user input from the keyboard
  cout << "Your number is: " << x;
  return 0;
}
```

#### sum

```cpp
int main() {
    int x,y,z;
    cout << "Enter Your Number First Number";
    cin>> x;
    cout << "Enter Your Number Secend Number";
    cin>> y;

    z = x + y;
    cout << "Your Result is " << z;
}
```

##### Boolean

```cpp
int main() {
  bool isCodingFun = true;
  cout << isCodingFun << "\n";
  bool isFishTasty = false;
  cout << isFishTasty;
}
```

#### Characters

```cpp
int main () {
  char a = 65;
  cout << " Number" << a <<endl;
  cout << " Number" << (int)a ;
}
//Output : Number A
//Output : Number 65
```

#### String

```cpp
int main(){
    string greeting = " Hello Bangladesh";
    cout << greeting;
}
```

## C++ divides the operators into the following groups:

- Arithmetic operators
- Assignment operators
- Comparison operators
- Logical operators
- Bitwise operators

# Arithmetic Operators

In programming, arithmetic operators are used to perform basic mathematical operations. Below is a table listing the common arithmetic operators and their functions.

| Operator | Description         | Example        | Result                               |
| -------- | ------------------- | -------------- | ------------------------------------ |
| `+`      | Addition            | `a + b`        | Adds `a` and `b`                     |
| `-`      | Subtraction         | `a - b`        | Subtracts `b` from `a`               |
| `*`      | Multiplication      | `a * b`        | Multiplies `a` by `b`                |
| `/`      | Division            | `a / b`        | Divides `a` by `b` (quotient)        |
| `%`      | Modulus (Remainder) | `a % b`        | Remainder when `a` is divided by `b` |
| `++`     | Increment           | `++a` or `a++` | Increases the value of `a` by 1      |
| `--`     | Decrement           | `--a` or `a--` | Decreases the value of `a` by 1      |

### Examples

1. **Addition**:

   ```cpp
   int a = 5, b = 3;
   cout << a + b;  // Output: 8
   ```

2. **Subtraction**:

   ```cpp
   int a = 5, b = 3;
   cout << a - b;  // Output: 2
   ```

3. **Multiplication**:

   ```cpp
   int a = 5, b = 3;
   cout << a * b;  // Output: 15
   ```

4. **Division**:

   ```cpp
   int a = 6, b = 3;
   cout << a / b;  // Output: 2
   ```

5. **Modulus**:

   ```cpp
   int a = 5, b = 3;
   cout << a % b;  // Output: 2
   ```

6. **Increment**:

   ```cpp
   int a = 5;
   a++;
   cout << a;  // Output: 6
   ```

7. **Decrement**:
   ```cpp
   int a = 5;
   a--;
   cout << a;  // Output: 4
   ```

# Assignment Operators

Assignment operators are used to assign values to variables. Below is a table of common assignment operators and their functionality.

| Operator | Description                                                         | Example  | Equivalent To | Result                                                          |
| -------- | ------------------------------------------------------------------- | -------- | ------------- | --------------------------------------------------------------- |
| `=`      | Assigns the right-hand value to the left-hand variable              | `a = b`  | N/A           | Assigns the value of `b` to `a`                                 |
| `+=`     | Adds the right-hand value to the left-hand variable                 | `a += b` | `a = a + b`   | Adds `b` to `a` and assigns the result to `a`                   |
| `-=`     | Subtracts the right-hand value from the left-hand variable          | `a -= b` | `a = a - b`   | Subtracts `b` from `a` and assigns the result to `a`            |
| `*=`     | Multiplies the left-hand variable by the right-hand value           | `a *= b` | `a = a * b`   | Multiplies `a` by `b` and assigns the result to `a`             |
| `/=`     | Divides the left-hand variable by the right-hand value              | `a /= b` | `a = a / b`   | Divides `a` by `b` and assigns the result to `a`                |
| `%=`     | Takes the modulus of the left-hand variable by the right-hand value | `a %= b` | `a = a % b`   | Computes the remainder of `a / b` and assigns the result to `a` |

### Examples

1. **Simple Assignment (`=`)**:

   ```cpp
   int a = 10;
   int b = 5;
   a = b;
   cout << a;  // Output: 5
   ```

2. **Add and Assign (`+=`)**:

   ```cpp
   int a = 10;
   int b = 5;
   a += b;
   cout << a;  // Output: 15
   ```

3. **Subtract and Assign (`-=`)**:

   ```cpp
   int a = 10;
   int b = 5;
   a -= b;
   cout << a;  // Output: 5
   ```

4. **Multiply and Assign (`*=`)**:

   ```cpp
   int a = 10;
   int b = 5;
   a *= b;
   cout << a;  // Output: 50
   ```

5. **Divide and Assign (`/=`)**:

   ```cpp
   int a = 10;
   int b = 5;
   a /= b;
   cout << a;  // Output: 2
   ```

6. **Modulus and Assign (`%=`)**:
   ```cpp
   int a = 10;
   int b = 3;
   a %= b;
   cout << a;  // Output: 1
   ```

# Comparison Operators

Comparison operators are used to compare two values. They return a boolean result (`true` or `false`) depending on whether the comparison is valid. Below is a table listing the common comparison operators and their functionality.

| Operator | Description              | Example  | Result                                                       |
| -------- | ------------------------ | -------- | ------------------------------------------------------------ |
| `==`     | Equal to                 | `a == b` | Returns `true` if `a` is equal to `b`, otherwise `false`     |
| `!=`     | Not equal to             | `a != b` | Returns `true` if `a` is not equal to `b`, otherwise `false` |
| `>`      | Greater than             | `a > b`  | Returns `true` if `a` is greater than `b`                    |
| `<`      | Less than                | `a < b`  | Returns `true` if `a` is less than `b`                       |
| `>=`     | Greater than or equal to | `a >= b` | Returns `true` if `a` is greater than or equal to `b`        |
| `<=`     | Less than or equal to    | `a <= b` | Returns `true` if `a` is less than or equal to `b`           |

### Examples

1. **Equal to (`==`)**:

   ```cpp
   int a = 10;
   int b = 5;
   cout << (a == b);  // Output: 0 (false)
   ```

2. **Not equal to (`!=`)**:

   ```cpp
   int a = 10;
   int b = 5;
   cout << (a != b);  // Output: 1 (true)
   ```

3. **Greater than (`>`)**:

   ```cpp
   int a = 10;
   int b = 5;
   cout << (a > b);  // Output: 1 (true)
   ```

4. **Less than (`<`)**:

   ```cpp
   int a = 10;
   int b = 5;
   cout << (a < b);  // Output: 0 (false)
   ```

5. **Greater than or equal to (`>=`)**:

   ```cpp
   int a = 5;
   int b = 5;
   cout << (a >= b);  // Output: 1 (true)
   ```

6. **Less than or equal to (`<=`)**:
   ```cpp
   int a = 5;
   int b = 5;
   cout << (a <= b);  // Output: 1 (true)
   ```

# Logical Operators

Logical operators are used to perform logical operations on expressions, typically involving boolean values. They return a boolean result (`true` or `false`) based on the logic applied. Below is a table listing common logical operators and their functions.

| Operator | Description            | Example  | Result                                                           |
| -------- | ---------------------- | -------- | ---------------------------------------------------------------- | --- | --- | --- | ---------------------------------------------------------------- |
| `&&`     | Logical AND            | `a && b` | Returns `true` if both `a` and `b` are `true`, otherwise `false` |
| `        |                        | `        | Logical OR                                                       | `a  |     | b`  | Returns `true` if either `a` or `b` is `true`, otherwise `false` |
| `!`      | Logical NOT (Negation) | `!a`     | Returns `true` if `a` is `false`, and `false` if `a` is `true`   |

### Truth Table

Here is a truth table for the logical operators:

| Expression          | `a`   | `b`   | `a && b` | `a    |       | b`  | `!a` |
| ------------------- | ----- | ----- | -------- | ----- | ----- | --- | ---- |
| Both `true`         | true  | true  | true     | true  | false |
| `a` true, `b` false | true  | false | false    | true  | false |
| `a` false, `b` true | false | true  | false    | true  | true  |
| Both `false`        | false | false | false    | false | true  |

### Examples

1. **Logical AND (`&&`)**:

   ```cpp
   bool a = true;
   bool b = false;
   cout << (a && b);  // Output: 0 (false)
   ```

2. **Logical OR (`||`)**:

   ```cpp
   bool a = true;
   bool b = false;
   cout << (a || b);  // Output: 1 (true)
   ```

3. **Logical NOT (`!`)**:
   ```cpp
   bool a = true;
   cout << (!a);  // Output: 0 (false)
   ```

# Bitwise Operators

Bitwise operators are used to perform operations at the binary level on integer values. They manipulate bits directly and are primarily used in low-level programming. Below is a table of the most common bitwise operators and their functionality.

| Operator | Description                    | Example    | Result                                                                   |
| -------- | ------------------------------ | ---------- | ------------------------------------------------------------------------ | --- | ---------------------------------------------------------- |
| `&`      | Bitwise AND                    | `a & b`    | Performs a binary AND on `a` and `b` (1 if both bits are 1, otherwise 0) |
| `        | `                              | Bitwise OR | `a                                                                       | b`  | Performs a binary OR on `a` and `b` (1 if either bit is 1) |
| `^`      | Bitwise XOR (Exclusive OR)     | `a ^ b`    | Performs a binary XOR on `a` and `b` (1 if bits are different)           |
| `~`      | Bitwise NOT (One's Complement) | `~a`       | Inverts all the bits in `a` (1 becomes 0, 0 becomes 1)                   |
| `<<`     | Left shift                     | `a << b`   | Shifts the bits of `a` left by `b` positions (multiply by `2^b`)         |
| `>>`     | Right shift                    | `a >> b`   | Shifts the bits of `a` right by `b` positions (divide by `2^b`)          |

### Examples

1. **Bitwise AND (`&`)**:

   ```cpp
   int a = 5;  // Binary: 0101
   int b = 3;  // Binary: 0011
   cout << (a & b);  // Output: 1 (Binary: 0001)
   ```

2. **Bitwise OR (`|`)**:

   ```cpp
   int a = 5;  // Binary: 0101
   int b = 3;  // Binary: 0011
   cout << (a | b);  // Output: 7 (Binary: 0111)
   ```

3. **Bitwise XOR (`^`)**:

   ```cpp
   int a = 5;  // Binary: 0101
   int b = 3;  // Binary: 0011
   cout << (a ^ b);  // Output: 6 (Binary: 0110)
   ```

4. **Bitwise NOT (`~`)**:

   ```cpp
   int a = 5;  // Binary: 0101
   cout << (~a);  // Output: -6 (Binary: 1010 in 2's complement form)
   ```

5. **Left Shift (`<<`)**:

   ```cpp
   int a = 5;  // Binary: 0101
   cout << (a << 1);  // Output: 10 (Binary: 1010, which is 5 * 2^1)
   ```

6. **Right Shift (`>>`)**:
   ```cpp
   int a = 5;  // Binary: 0101
   cout << (a >> 1);  // Output: 2 (Binary: 0010, which is 5 / 2^1)
   ```

### Bitwise Truth Table (AND, OR, XOR)

| `a` | `b` | `a & b` | `a  | b`  | `a ^ b` |
| --- | --- | ------- | --- | --- | ------- |
| 0   | 0   | 0       | 0   | 0   |
| 0   | 1   | 0       | 1   | 1   |
| 1   | 0   | 0       | 1   | 1   |
| 1   | 1   | 1       | 1   | 0   |

### Notes

- **Bitwise AND (`&`)** sets a bit to `1` if both corresponding bits are `1`.
- **Bitwise OR (`|`)** sets a bit to `1` if at least one corresponding bit is `1`.
- **Bitwise XOR (`^`)** sets a bit to `1` if only one of the corresponding bits is `1`.
- **Bitwise NOT (`~`)** inverts all bits.
- **Left Shift (`<<`)** multiplies the number by powers of two.
- **Right Shift (`>>`)** divides the number by powers of two (with integer division).

This table explains the bitwise operators and provides examples to clarify how they work in practice.
