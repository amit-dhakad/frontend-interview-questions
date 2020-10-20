# Frontend Interview Questions

Interview Questions for frontend developer


### Table of Contents

|     | Framework               | 
| --- | --------------------    |
|     | [Angular](#angular)     |
|     | [React](#react)         |
|     | [JavaScript](#javascript)             |
|     | [HTML](#html)                    |
|     | [CSS](#css)                     |






### Angular
| No. | Questions |
| --- | --------- |
|   | **Angular** |
|1  | [What is Angular](#what-is-angular) |
|2  | 

### React
| No. | Questions |
| --- | --------- |
|   | **React** |
|1  | [What is React?](#what-is-react) |
|2  | 

### JavaScript
| No. | Questions |
| --- | --------- |
|   | **JavaScript** |
|1  | [Which javascript design patterns have u worked on?](#which-javascript-design-patterns-have-u-worked-on) (Publicis sapient) |
|2  | [What is closure in javascript ](#What-is-closure-in-javascript) (Publicis sapient)|
|3  | [Change the context of this keyword in javascript.](#change-the-context-of-this-keyword-in-javascript) (Publicis sapient)|
|4  | [What is this keyword?](#what-is-this-keyword) (Publicis sapient)|


### HTML
| No. | Questions |
| --- | --------- |
|   | **HTML** |
|1  | [What do u understand by semantic element or semantic tags?](#what-do-you-understand-by-semantic-element-or-semantic-tags) (Publicis sapient) |
|2  | [What are web workers?](#what-are-web-workers) (Publicis sapient) | 
|3  | [What are data attributes in html?](#what-are-data-attributes-in-html)(Publicis sapient)|


### CSS
| No. | Questions |
| --- | --------- |
|   | **CSS** |
|1  | [ What do you understand by pseudo element in CSS? ](#what-do-you-understand-by-pseudo-element-in-css) (Publicis sapient) |
|2  | [ What is Specificity in css.](#what-is-specificity-in-css) (Publicis sapient) |
|3  | Which css library have u worked on? (Publicis sapient) |



## Angular

1. ### What is Angular?

## React

1. ### What is React?

    React is an **open-source frontend JavaScript library** which is used for building user interfaces especially for single page applications. It is used for handling view layer for web and mobile apps. React was created by [Jordan Walke](https://github.com/jordwalke), a software engineer working for Facebook. React was first deployed on Facebook's News Feed in 2011 and on Instagram in 2012.


   **[⬆ Back to Top](#react)**
   
   
   
 ## JavaScript
 1. ### Which javascript design patterns have u worked on.
    # read digitalocean blog :
      https://www.digitalocean.com/community/tutorial_series/javascript-design-patterns
 
 **[⬆ Back to Top](#javascript)**
 
 
 
 2. ### What is closure in javascript
 
 A closure is the combination of a function bundled together (enclosed) with references to its surrounding state (the lexical environment). In other words, a closure gives you access to an outer function’s scope from an inner function. In JavaScript, closures are created every time a function is created, at function creation time.
 
 ```javascript
      function init() {
  var name = 'Mozilla'; // name is a local variable created by init
  function displayName() { // displayName() is the inner function, a closure
    alert(name); // use variable declared in the parent function
  }
  displayName();
}
init();
```
init() creates a local variable called name and a function called displayName(). The displayName() function is an inner function that is defined inside init() and is available only within the body of the init() function. Note that the displayName() function has no local variables of its own. However, since inner functions have access to the variables of outer functions, displayName() can access the variable name declared in the parent function, init().
 
 **[⬆ Back to Top](#javascript)**
 
 
 3. ### Change the context of this keyword in javascript.
 
 ## No, it's not possible.

## You can call a method with a specified value for this (using method.apply()/method.call()) but you cannot re-assign the keyword, this (You can't change what this refers to from inside the function.).

## The file is ECMA-262.pdf and on page 39, section 10.1.7. This

There is a this value associated with every active execution context. The this value depends on the caller and the type of code being executed and is determined when control enters the execution context. The this value associated with an execution context is immutable.
 
 ## Setting the this keyword in javascript.
Javascript has 3 built in methods for setting the this keyword conveniently. They are all located on the Function.prototype object so every function can use them (since every function inherits from this prototype via prototypal inheritance). These functions are the following:

## Function.prototype.call(): 
This function takes the object which you want to use as this as a first argument. Then the remainder of the arguments are the respective arguments of the function which is called.
## Function.prototype.apply(): 
This function takes the object which you want to use as this as a first argument. Then the second argument is an array which contains the values of the arguments of the function which is called (first element of array is first argument of the function, second argument of the array is second argument of function etc.).

## Function.prototype.bind(): 
This function returns a new function which has a different value of this. It takes the object which you want to set as the this value as a first argument and then returns a new function object.

 
  **[⬆ Back to Top](#javascript)**
  
  
4. ### What is this keyword? 

What is this?
The JavaScript this keyword refers to the object it belongs to.

It has different values depending on where it is used:

In a method, this refers to the owner object.
Alone, this refers to the global object.
In a function, this refers to the global object.
In a function, in strict mode, this is undefined.
In an event, this refers to the element that received the event.
Methods like call(), and apply() can refer this to any object.
  
 **[⬆ Back to Top](#javascript)**
 
 ## HTML
 
 1. ### What do you understand by semantic element or semantic tags?

A semantic element clearly describes its meaning to both the browser and the developer.
Semantic elements = elements with a meaning.
Examples of non-semantic elements: <div> and <span> - Tells nothing about its content.
Examples of semantic elements: <form>, <table>, and <article> - Clearly defines its content.
    
    
   **[⬆ Back to Top](#html)**
    
    
  

2. ### What are web workers.
   
   A web worker is a JavaScript running in the background, without affecting the performance of the page.

What is a Web Worker?
When executing scripts in an HTML page, the page becomes unresponsive until the script is finished.

A web worker is a JavaScript that runs in the background, independently of other scripts, without affecting the performance of the page. You can continue to do whatever you want: clicking, selecting things, etc., while the web worker runs in the background.
   
   **[⬆ Back to Top](#html)**  
   
   
 3. ### What are data attributes in html?
 
   The data-* attribute is used to store custom data private to the page or application.

The data-* attribute gives us the ability to embed custom data attributes on all HTML elements.

The stored (custom) data can then be used in the page's JavaScript to create a more engaging user experience (without any Ajax calls or server-side database queries).

The data-* attribute consist of two parts:

The attribute name should not contain any uppercase letters, and must be at least one character long after the prefix "data-"
The attribute value can be any string
## Note: Custom attributes prefixed with "data-" will be completely ignored by the user agent.
   
   **[⬆ Back to Top](#html)**  
   
   
 
 ## CSS
 
 1. ### What do you understand by pseudo element in CSS?
 
      A CSS pseudo-element is a keyword added to a selector that lets you style a specific part of the selected element(s). For example, ::first-line can be used to change the font of the first line of a paragraph.
      
      ## Syntax
      ```css
      selector::pseudo-element {
        property: value;
       }
      ```
      
      ```css
      /* The first line of every <p> element. */
        p::first-line {
        color: blue;
       text-transform: uppercase;
      }
      ```
      
      
      
      ## Index of standard pseudo-elements
       
      |             |           |          |           | 
      | ----------  | --------- | -------- | ----------| 
      | ::after (:after) | ::backdrop | ::before (:before) | ::marker)|
      | ::cue  | ::cue-region | ::first-letter (:first-letter) | ::first-line (:first-line) |
      | ::grammar-error | ::marker | ::part() | ::placeholder |
       | ::selection | :: slotted() | ::spelling-err | 
 

     **[⬆ Back to Top](#css)**



  2. ### What is Specificity in css? 
  
  
  If there are two or more conflicting CSS rules that point to the same element, the browser follows some rules to determine which one is most specific and therefore wins out.

Think of specificity as a score/rank that determines which style declarations are ultimately applied to an element.

The universal selector (*) has low specificity, while ID selectors are highly specific! 

# Note: Specificity is a common reason why your CSS-rules don't apply to some elements, although you think they should.

## Specificity Hierarchy

Every selector has its place in the specificity hierarchy. There are four categories which define the specificity level of a selector:

Inline styles - An inline style is attached directly to the element to be styled. 
Example: 
  ```html  <h1 style="color: #ffffff;"> ```
IDs - An ID is a unique identifier for the page elements, such as #navbar.
Classes, attributes and pseudo-classes - This category includes .classes, [attributes] and pseudo-classes such as :hover, :focus etc.
Elements and pseudo-elements - This category includes element names and pseudo-elements, such as h1, div, :before and :after.

**[⬆ Back to Top](#css)**




