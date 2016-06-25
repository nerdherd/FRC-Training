# Programming Basics
These lessons will cover the fundamental programming skills needed to write simple applications.
### Data Types
Before starting with any programming language, it is helpful to understand each data type. Below are all of the datatypes you will use when programming the robot.
- `boolean` (8 bit): Either true or false.
- `int`	    (32 bit): Signed integer. (Signed means that it can be negative or positive)
- `float`   (32 bit): Signed floating point number (decimal).
- `double`  (64 bit): Double precision floating point number. Used very frequently in FRC.
- `String`  (Variable): A collection of characters of variable size. "Hello World!", for instance.

### Variables
A variable in programming is just like a variable in math. It has a name, and can be set to all sorts of different values. Unlike math, however, variables in programming are not limited to just numbers. A variable can be any of the above data types. Below are some examples of defining variables.
```
boolean Helix = true;
String foo = "bar";
double pi = 3.14159265;
int integer = 1;
```  

### Functions
Functions in programming are just like functions in math! Consider the following:
```
f(x)=x+3
When x = 3, f(x) = 6
```
In this case, f(x) is the function and x is the parameter. We pass the parameter into the function, and it returns a value -- 6, in this case. We could rewrite that example in java like so:
```
int f(int x) {
  return x+3;
}
```
The `int` before `f(int x)` specifies that the function returns an integer. `int x` means that it will only take in integers as arguments. This function returns `x+3`. Functions in programming are not limited to numbers, either; consider the following:
```
String sayHello() {
  return "Hello!";
}
```
It is important to note that you use the keyword `void` for any function that does not return anything.
### If/Else Statements
A man comes home from work. His wife tells him, "Go to the store and buy a gallon of milk, and if they have eggs, buy a dozen". He comes home with 13 gallons of milk. "What happened?!" asked his wife. "They had eggs." This man was a programmer.
An if/else statement can be used to make decisions in your program. A situation like the one described above may be written like so:
```
void visitStore(boolean eggs) {
  //Buy 1 gallon of milk
  if (eggs) {
    //If there are eggs, buy 12 gallons of milk.
  } else {
    //If there are not eggs, go home.
  }
}
```
If/else statements are very simple in this way -- they follow the pattern of "If x, then y."
### Loops
There are two kinds of loops that you will frequently encounter, `for` and `while`.
```
for (int i = 0; i < 10; i++) {
  //Do something
}
```
The example above is a `for` loop. It is fairly intuitive; for some integer `i`, do something, then add 1 to `i`. Repeat this process until `i=10`.
```
boolean a = true;
while (a = true) {
  //Do something
}
```
The above example is a `while` loop. This code will run forever, until something causes `a` to be `false`. You should try to avoid `while` loops until you understand more about threading because they can cause this kind of infinite loop.
### Further Reading and References
* [Oracle Java Tutorial](https://docs.oracle.com/javase/tutorial/)
