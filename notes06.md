## Lecture
You saw in the readig how html, css, and javascript fit together

HTML, CSS, and Javaascript are what we  use to form modern webspites
HTML is the content layer, CSS is the presentation layer, and Javascrtip is the behaviour layer


Html is for structure of a webpage
- This is where the content of the page lives
- What is the website content? What does that mean?

Css is the presentation layer of the webpage
- The Css enchances the HTML page with rules that state how the HTML content is presented backgrounds, borders, box dimensions, colors, fonts, etc.

Javascript is the behaviour layer of the webpage
- This changes how the page behaves, adding interactivity. We will aim to keep as much of our javascript as possible in seprate files

We will try to keep as much CSS, HTML, and Javascript in their respective files. It's not strictly necessary
for it to work, however it helps with organization and is standard in the industry

### Progressive Enhancement
The three layers form the basis of a popular approach to building webpages called progressive enhancement.
You start with HTML only, not all browsers support the latest CSS so your webpage should still work
even if CSS is disabled
Same with javascript, its added last and enhances the usability of the page, but some browsers have javascript
disabled, so the webpage should still work, even if javascript is turned off, it just might lose some
functionality.

### Javascript in HTML

* Link to a javascript file from an html page
```
<script src = "js/add-content.js"></script>
```
* This tells the browser to go ahead and load the script file, just like the src attribute on an <img> tag
* Sometimes you'll see javascript in the HTML between opening <script> and closing </script> tags

```
<!Doctype html>
<html>
   <head>
      <title>My Web Page</title>
      <link rel="stylesheet" href="css/style.css"/>
    </head>
   <body>
      <h1>Food Blog</h1>
      <script>document.write('<h3>Welcome</h3>');</script>
      <p>Thanks for coming to my website,are you a foodie><em>901-846-2547</em></p>
    </body>
</html>
```

### Statement

* A script is a series of instructions that a computer can follow one-by-one. Each individual instruction or step is known as a **statement**. Statements should end with a semicolon.
* The curly braces indicate the start and end of a **code block**
* Javascript is case sensetive, so **hourNow** is different from say **HOURNOW**, in variable names we don't put spaces

```
var today = new Date();
var hourNow = today.getHours();
var greeting;

if (hourNow > 18 ){
   greeting = 'Good Evening';
} else if (hourNow > 12){
  greeting = 'Good afternoon';
}else if (hourNow > 0){
   greeting = 'Good morning';
} else {
   greeting = 'Welcome';
}
document.write(greeting);
```


### Comments

* A comment is good to put in your code and it explains what your code does
* A **multi-line** comment as the name says, stretches over multiple lines
* A **single-line** comment, as the name says, stretches over a single line //


```
/* This script displays a greeting to the user based upon the current time.
It is an example from JavaScript & jQuery book */

var today = new Date();
var hourNow = today.getHours();
var greeting;

if (hourNow > 18 ){
   greeting = 'Good Evening';
} else if (hourNow > 12){
  greeting = 'Good afternoon';
}else if (hourNow > 0){
   greeting = 'Good morning';
} else {
   greeting = 'Welcome';
}
document.write(greeting);
```

### Objects and Methods
The **document** object represents the entire webpage. All web browsers implement this object
The **document** object has sever methods and properties, they are known as **members** of that object.
You can access the members of an object by using a dot between the object name and the name of the member you want to access

```
document.write('Good afternoon!');
```
The **write()** method of the **document** allows new content to be writen into the page
whever the **\<script>** element sits.

Sometimes methods need information to work properly. This data is given inside of the parentheses.
Each piece of informaiton is called a **paramater** of the method. In this case the **write()** method
needs to know what it is you want to write into the page.

#### Your javascript code will run whever the \<script> element is on the page

### What is a variable?
When writing JavaScript you tell the interpreter each individual stp you want it to perform
```
var width = 0;
var height = 3;
var area = width * height;
console.log(area);
```

This script here does a few things
1. Remember the value for width
2. Remember the value for height
3. Multiply width times height and store it in the area variable
4. Return the value to the user

The data stored in a variable can change (or vary) each time a script runs

### Declaring a variable
Before you can use a variable, you need to announce that you want to use it, this is called
**declaring** the variable
 ```
 var quantity;
 ```
 
 var is an example of what you call a keywoard. The javascript interpreter
 knows that this keyword is used to create a variable. Then the variable n eeds a name.
 if a variable has more than one word it is sometimes written in **camelCase** or **snake_case**
 
 ### Assigning variable values
 
 ```
 quantity = 3;
 ```
 Once you have created a variable, you can assign a value to it.
 This  can also be done on the same line of code with one statement by writing
 
 ```
 var quantity = 3;
 ```
 
 The equals sign is an **assignment operator** it says that you are going to assign a value to the variable
 until the variable has a value assigned to it, the value is **undefined**
 
 Variables must start with either a letter, an underscore or a $. There are three main types 
 of variables, numbers, strings, and booleans.
 
 Numbers are self explanatory and we've seen those already. A **string** is any collection of characters or numbers surrounded by quotes. A **boolean** is a true or false value.
 
 ### String Concatenation
 You'll see a lot of this going forward so it's important to focus on it now. String concatenation
 is when you add two strings together. Here's an example
 
 ```
 console.log('Hello' + 'World');
 ```
 
 If I save this and refresh the webpage we'll see the text HelloWorld in the console, notice that
 there's no space, that's because inside the two strings, that is the text in between the quotes, there is no space. I can add one by adding a space somewhere inside the qutoes.
 
 Now this isn't all that useful with two literal string values, that is values that i just defined. But we can use this on variables and on numbers to create strings based off of other iput
 
 ```
 var age = 10;
 var name = "Charlie";
 var phrase = name + ' is ' + age + ' years old.';
 console.log(phrase);
 ```
 
 If we were to chanage the age and name variables the phrase would change to reflect that.
 
 ### Adding dynamic components
 Let's use some javascript to add some dynamic components to our webpage it may not be totally useful for a professional webpage but this exercise will help us understand how to get info from the user
 and what we can do with it.
 
 Let's use the prompt command to prompt the user for a number between 1 and 10.
 Then we'll display the number that they entered.
 
 ```
 var user_number = prompt('Enter a number between 1 and 10);
 console.log(user_number);
 ```
It may be more useful to display the users input on the website itself. We can do that using **document.write()**
document.write() allows you to write html code directly to the document from javascript! Since we're
writing html code it's good practice to use html tags as well, though it's not strictly necessary for
it to work.

```
var phrase = "The number entered was " + user_number;
document.write('<p>'+ phrase + '</p>')
```

Let's take in some user input and display a message to the user based on the input that they entered.
To accomplish this we're going to use an If Statement. Recall from the video that an if statement asks a yes or no question and goes down a particular branch dependent on the answer

the syntax for these if statemnents in javascritp is

```
if(condition) {
   //do something
}
```

what goes inside of the condition block is our question, also known as a  conditional statement.
A conditional statement is a statement that has two possible outcomes, true or false.

Let's prompt the user for their age and tell them that they're a child, a teenager, or an adult depending on what they enter. Our first conditional statement is

```
var age = prompt('Enter your age');
if (age > 19){
    alert('You are an adult');
}
```
Let's test this first condition. Great, we got the proper alert.
Next we'll add what's called an else if statement.

```
var age = prompt('Enter your age');
if (age > 19){
    alert('You are an adult');
}
else if (age > 12){
    alert('You are a teenager');
}
```

Great, now we can test this and yep we get the proper outcome in both cases. The way we read this
conditional statement is first we ask is the age greater than 19. If it is tell them they are an adult.
If the age isn't greater than 19 then let's ask a different question, is the age greater than 12. If it is then you are a teenager. The final condition we need to check for is if they are less than 12 in which case we want to tell them that they are a child. This can be accomplished with an else statement
```
var age = prompt('Enter your age');
if (age > 19){
    alert('You are an adult');
}
else if (age > 12){
    alert('You are a teenager');
}
else {
    alert('You are a kid');
}
```

The else keyword is the default action taken if both the if and the else if are false. So if we're not older than 19 and we're not older than 12 then we must be 12 or younger and so we tell them they are a kid.
