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
