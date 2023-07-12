# javaScript Guide
This repository contains a guide to learning JavaScript. The guide covers the basics of JavaScript, including variables, functions, objects, arrays, and events. It also covers more advanced topics, such as closures, promises, and async/await.

The guide is written in Markdown and uses code blocks to demonstrate JavaScript syntax. It is also accompanied by a number of exercises that allow you to practice what you have learned.

The target audience for this guide is anyone who wants to learn JavaScript. Whether you are a beginner or an experienced developer, this guide will help you to understand the basics of JavaScript and to write JavaScript code.

Contents

* Introduction to JavaScript
* Variables
* Functions
* Objects
* Arrays
* Events
* Closures
* Promises
* Async/await
* Exercises
* Contributing

This repository is open to contributions. If you find any errors in the guide or if you have suggestions for improvement, please feel free to open an issue or submit a pull request.

License

This repository is licensed under the MIT License.

I hope this helps!


 /* Also I have read the book of JON DUCKETT for JavaScript and i will write the summry of it in this repo */





 # Basic JAVASCRIPT INSTRUCTIONS

 ### In this section you will learn read and write Javascript and you will learn how to give browser instruction you want it to follow.
 
**Statements**
    * Script is a serise of instructions that a computer can follow one-byone each indiviual instruction or step in kown as a statment.
(NOTE: Statment should end with semicolon.)

```javascript
var today = new Date();
var hourNow = today.getHours();
var greeting;

if(hourNow > 18){
greeting = 'Good evening'
} else if (hourNow > 12){
greeting = 'Good morning'
} else {
greeting = 'welcome'
}
document.write(greeting)
```

We will look at what the code on the above dose shorlty, but for the moment not that.

 * Each of the lines of code in the code are statment unless the line include "if", "else if","else" are not statment.
 * The code include "if", "else if","else" determines which code should run. 



### Now we will talk about COMMENTS

**Comments**
  1. You should write comment to explin what your code dose.
  1. They help your code easier to read and understand.
  1. This can help you and others who read your code.

  ```javascript
var today = new Date(); // Create a new data object.
var hourNow = today.getHours(); // Find the current hour.
var greeting;

// Display the approprate greeting on the current time.
if(hourNow > 18){
greeting = 'Good evening'
} else if (hourNow > 12){
greeting = 'Good morning'
} else {
greeting = 'welcome'
}
document.write(greeting)
```
















# JavaScript Math Object
### The JavaScript Math object is a built-in object that provides a number of methods and properties for performing mathematical tasks. 


**Math.ceil()**
1. Math.ceil() is a method to reound the number to the largest number.

  ```javascript
const ceilNumber = Math.ceil(10.1); // This is to Round the number to the lagrgest number
```

* The output is:

> 11


**Math.floor()**
2. Math.floor() is a method to round the number to the smallest number.

  ```javascript
const floorNumber = Math.floor(10.1); // This is to Round the number to the smallest number
```

* The output is:
  > 10


**Math.round**
3. Math.round() is a method to eound the number to the nearest integer.
 
 ```javascript
const roundNumber = Math.round(9.9); // This is to round the number to the nearest integer.
```

* The output is:
  > 10
