# task3
#The ampersand



The & symbol is used as an operator in C++. It is used in 2 different places, one as a bitwise and operator and one as a pointer address of operator.

In Windows, it is used as a code to precede an underlined character. As a result, in some input dialogs, you have to enter a double ampersand (&&) to actually define a single ampersand.


##Bitwise AND
The ampersand (&) normally means "and" such as in the statement==> if (x >= 100 && x >= 199).

The bitwise AND operator (&) compares each bit of the first operand to that bit of the second operand. If both bits are 1, the bit is set to 1. Otherwise, the bit is set to 0. Both operands to the bitwise AND operator must be of integral types. 

##Address Of operator

C++ provides two-pointer operators, which are Address of Operator (&) and Indirection Operator (*).

A pointer is a variable that contains the address of another variable or you can say that a variable that contains the address of another variable is said to "point to" the other variable. A variable can be any data type including an object, structure or again pointer itself.

The address of Operator (&), and it is the complement of *. It is a unary operator that returns the address of the variable(r-value) specified by its operand.

##Declaration

It can declare a type to be a reference:
```
int x = 9;
int& y = x; //here the ampersand means that y is a reference to integer 
```

##Indication
It can be used to indicate that a function receives its parameters passed by reference:
```
int ind(int& x); //function takes an integer passed by reference 
int ind(const int& x); //function takes an integer passed by constant reference 
int ind(int&& x); //function takes an integer passed by rvalue/universal reference 
```

#The const

When modifying a data declaration, the const keyword specifies that the method(), variable, pointer variable, and with the object of a class is not modifiable.

In C++, you can use the const keyword instead of the #define preprocessor directive to define constant values. Values defined with const are subject to type checking, and can be used in place of constant expressions.

##Usage

1) we can specify the size of an array with a const variable as follows:
```
const int maxary = 255;
char store_char[maxary];  // allowed in C++; not allowed in C
```

2) The const keyword can also be used in pointer declarations:
```
int main() {
   char *test = 0 , *test1 ;
   char *const aptr = test;
   *aptr = 'a';   
   aptr = test1;  
}
```
##Const member functions

Declaring a member function with the const keyword specifies that the function is a "read-only" function that does not modify the object for which it is called. A constant member function cannot modify any non-static data members or call any member functions that aren't constant.To declare a constant member function, place the const keyword after the closing parenthesis of the argument list. The const keyword is required in both the declaration and the definition.
