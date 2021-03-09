## Lecture

### Thinking Inside the Box

CSS stands for Cascading Style Sheets
Let's start todays class by going through a quick review of others code, we'll be starting at
lesson 5, we're going to take a look at lab 4. Lab 4 tasked you with developig your first ever
website using nothing but HTML code. Now I want to review that.

* Show students how to deploy their site with Github Pages
* Take any questions from students

### CSS and it's Uses

Generally we want our CSS to exist in a file separate from the rest of our webpage, this file ends with
.css
It works by associate specific **rules** with HTML elements.
It contains two parts: a **selector** and a **decleration**

```
p { 
   font-family: Arial;
   }
```

* p is the selector, font-family is the decleartion
* A deceleration is made up of two parts, a propery, and a value.
* In the case above, the property is the font-family and the value is Arial, all declerations are ended with a colon as part of the CSS syntax

# Different types of selectors
* Univresal selector *{}
* Type Selector h1,h2,h2 {}
* Class Selector .note {}
* ID Selector #intro{}
* Child Selector li>a {} matches all elements that are children of another
* Descendant Selector p a {} matches an element that is a descendant of another specified element. This targets any <a> elements that sit inside <p> elements
*  Adjacent and general sibling selectors which we won't cover they are barely used
