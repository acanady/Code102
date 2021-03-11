## Review

### Expressions and operators
An expression is any valid set of literals, variables, operators and expressions that evaluate to a single value. This may be a number, a string, or a logical value.
There are two main types, one that assigns a value simply, and one that uses to or more values to return a single value
```
x = 7
```
This is an example of an expression that declares and assigns the value 7 to the variable x
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

### What are functions
Functions let you group statements together to perform a specific task
If different parts of a script perform the same task, you can reuse the function (rather than repeating the same set of statements)

Here's a basic function showing function calls

```
//This functions takes in a value a and b and returns a/b
function divide(a,b){
   if(b != 0){
      return a/b;
   }
   else{
      return undefined;
   }
}
```

## Loops

