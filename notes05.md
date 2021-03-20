## Review

### HTML Anatomy

In HTML there are 6 different headings

HTML is composed of what are called _elements_ and html element is composed ove an opening tag,
the content of the element, and the closing tag

```
<p>Hello World</p>

```

In this example here, the <p> is the opening tag, the "Hello World" text is the **content** and the
</p> is the closing tag. All closing tags look similar to their opening tag, but with a / present.

A tag and the content between it is called an HTML element.

<body> tag is a key tag only content inside the opening and closing body tags
can be displayed to the screen.

Any typ eof tag can go inside the body tags

HTML is organized as a collectino of family tree relationships

```html
<body>
   <p>Lorem Ipsum, this paragraph is a child</p>
</body>
```

As seen in the html code here, the paragraph element is **nested** inside of the body element.
When this happens it is considered the **child** of that element.  So here the <body> element is
seen as a parent to the <p> element. Also the main element is at the same level as the first <p> element
and these elements are called, you'd guess it, siblings.

```html
 <body> <!--This is an ancestor of the second <p> tag -->
    <p>This is a child of body</p>
    <main>
       <p>This is a child of main and a descendant of <body> </p>
    </main>
  </body>
```



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

### Different types of selectors
* Univresal selector *{}
* Type Selector h1,h2,h2 {}
* Class Selector .note {}
* ID Selector #intro{}
* Child Selector li>a {} matches all elements that are children of another
* Descendant Selector p a {} matches an element that is a descendant of another specified element. This targets any <a> elements that sit inside <p> elements
*  Adjacent and general sibling selectors which we won't cover they are barely used

### Color
* Within color there's different ways to specify color
* colors in rgb are specified from 0 to 255
* HexCodes are the hex vode values of rgb, shown in hexadecimal
```
 background-color: rgb(102,205,170)
 backround-color: #66cdaa
 backround-color: MediumAquaMarine
 background-color: rgba(0,0,0,0.5);
 
 ```
 
 Low contrast, high contrast and medium contrast
 low contrast is hard to see, high contrast can be strainig on the eyes with tones of text, medium contrast is good for tons of text
 
 Opacity, how opaque something is, the more opaque the less solid and more see through the item
 
 Theres HSL (Hue, Saturation and Lightness) the amount of white or balck in a color *luminosity*
 [brightness only adds black, lightness offers both white and black]
 
 #### HSL an HSLA
 hue is a value fom 0 - 360 with a again being the alpha, how transparent
