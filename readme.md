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

### Notes

- **Division (`/`)** performs integer division when both operands are integers.
- **Modulus (`%`)** works only with integers and returns the remainder of the division.

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

### Notes

- Assignment operators are a shorthand way to modify variables and assign new values in a single step.
- The right-hand operand can be a variable, constant, or expression.

This table summarizes the assignment operators and their usage in common programming scenarios.
