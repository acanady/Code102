## Lecture

Todays lecture covers more javascript and the ins and outs of functions, expressions, opreators, and refactoring code

### Scripts are instructions that we give a computer

Computers solve problems **programmatically** they follow a series of instructinos, on after the other.
The type of instructions they need are often different to the type of instructions you might give to another human.

When determining out script we first need to think about what is is we watn to accomplish and how our website will flow, here's an example of a flowchat

* When button gets clicked
* Get the name entered in the form
* If the name is


Here's an interesting exercise that I do with my highschool students, sadly we can't do it in person but it still has the same effect
Say we had a bag of marbles of unknown size, and a large gorup of people of unknown size, too many for you to count. This is a special bag, anhyone can put put their hand in and remove a marble. However, once you remove a marble, That specific person cannot take another marble out (So you couldn't just count all the marbles). Think of an **algorithm** to determine which is larger, the number of people in the crowd, or the number of marbles in the bag.

* When we refactor our code we change the source code without changing the behaviour. We do this in an effort to keep our code solid and easy to maintain

> Any fool can write code that a computer can undrstand. Good programmers write code that humans can understand -Martin Fowler

### Expressions and operators
An expression is any valid set of literals, variables, operators and expressions that evaluate to a single value. This may be a number, a string, or a logical value.
There are two main types, one that assigns a value simply, and one that uses to or more values to return a single value
 ```
 x = 7
 ```
 This is an example of an expression that declares and assigns the value 7 to the variable x
 
 ```
 x + 7
 //Arithmetic operators are (+,-,/,*,++,--, %)
 ```
This is an arithmetic expression that evaluates to 7, it does not perform an assignment. The operators used in such expressions are reffered to as **operators**
An arithemtic expression follows general orders or operation PEDMAS

A conditional expression is one that can have one of two values based on a condition. The syntax is as such

```
(condition) true: val1 | false : val2
```
In javascript if statements (Which include elsif and else) are examples of conditional statements

```
x = 5
if(x == 5){
 console.log('hello world');
}
```

The conditional expression here checks for equivalence on whether or not x equals 5 the double equals is a **comparison operator**

```
!=
>, <
>=, <=
==, ===
```

There are other logical operators such as **Or**, **Not**, **And** they take boolean valeues (True or False) as operands

For string values you can **concatenate** strings and variables to form new strings

```
x = 10
phrase = 'x is equal to ' + x;
console.log(phrase);
```
### What are functions
Functions let you group statements together to perform a specific task
If different parts of a script perform the same task, you can reuse the function (rather than repeating the same set of statements)

Here's a basic function

```
var msg = 'Signup to recieve 10% off your next purchase!'
function updateMessage(){
   var elem = document.getElementById('message');
   elem.textContent = msg;
}
```

### Declaring a function

TO create a function you give it a name and write the statements needed to achieve its task inside the curly braces

```
function sayHello(){
   document.write('Hello');
}
```
Functions store the code needed to perform a specific task and the script can ask the function to perform that task whenever it's needed.

To call a function you use the funciton name followed by a parantheses.

```
sayHello();
//Here we are invoking or calling this function
//A function can be called as many times as you want
```

### Functions that need information
Some functions will require information to work, these values go inside the parentheses.
The items that appear inside the parenthese are known as **paramaters** of the function 
Inside the function they act like variable names

```
function multiply(width, height){
   return width * height;
}
```

### Calling Functions that need information

When calling a function that has parameters you need to provide those values when calling the function.
We call the values these values **arguments** You can use either literal values or variables

```
var mult = multiply(3,5);
var a = 5;
var b = 6
var mult = multily(a,b);
```
### The return keyword
You'll see that I'm returning a value here, all functions can return values. They don't have to, but many do
The value that is returned can be stored in a variable for use later.
