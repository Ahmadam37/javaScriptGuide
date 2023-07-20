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


 /* Also, I have read the book of Jon Duckett for JavaScript and I will write the summary of it in this repo. */





 ## Basic JAVASCRIPT INSTRUCTIONS

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
* Also, we have a multiline cooments and we do it to take out some of the code out, why we doing that, to test somthing in the code or debuging another lines of code but we dont want to remove it.

* Multi-line comment are often used for descriptions of how the script works, or to prevent a secrtion of the script from running when testing it.

```javascript
//MULTI-LINE COMMENT
/*
<div class="lango">
        <h1 id="helo">We will use Javascript</h1>
        <p>This is the test</p>
      </div>
*/
```



### What is a varibale? 

A script will have temporarily store the bit of information it needs to do its job. It can store this data in variables.

When you write a javascript, you have to tell the intepreter evrey indiviual step that you want it to perform. This sometimes involves more detail than you might expect.


Think about calculating the area of wall, in math the area of a rectangle is obtained by multiplying tow numbers:

* width * hight = area

You mghit be able to calculate this, but if you write a script you have to give computer very detailed instruction.

1. Remember the value for width.
2. Remember the value for hight.
3. multiply witdh by hight to get the area.
4. Return the result to the user.



### HOW TO DECLARE THEM.

```javascript
var quantity;
```

**var** is a keyword.
**quantity** is a varibale name.

**var** is an example of what programmers call a keyword.
The javascript intepreter knows that this keyword is used to create a varible. In order to use the varible, you must give a name.(This is sometimes called an identifier.) In this case, the varible is called **quantity**.


### HOW ASSIGN TO VARIBLE A VALUE.

```javascript
var quantity = 3;
```

You can now use the varible by its name. Here we set a value for the varible called **quantity**.
Where possible, a varible's name should describe the kind of data the varible holds.


### Data Types:

* NUMERIC DATA TYPE ==> The numeric data type handel numbers. ==> 0.75
* STRING DATA type ==> The string data type consists of letters and other characters. ==> 'Hi, Ahmad'
* BOOLEAN DATA TYPE ==> Boolean data types can have one of two values: true or false.

```javascript
 var price = 100; //This is a Numeric data type
      var myName = "Ahmad"; //This is a String data type
      var checkValue = true; //This is a boolean data type

//This is to check data type of each varible.
      console.log(typeof price);
      console.log(typeof myName);
      console.log(typeof checkValue);
```
Numbers are not only used for things like calculators; they are also used for tasks such as determining the size of the screen, moving the postion of an element on a page, or setting the amount of time an element should take to fade in.



### RULES FOR NAMING VARIABLES:

1. The name must begin with a letter, dollar sign ($), or an underscore(_). it must not start with a number
2. The name can contain letters, numbers, dollar sign ($), or an underscore (_). Note that you must not use dash(-) or a period (.) in a varible name.
3. You cannot use **keywords** or **reserved** words. Keywords are special word that tell the intepreter to do somthing. Reserved words are onse that may be used in a _future_ version of JavaScript.
4. All varibles are case sensitive, so score and Score would be diffrente variable names.
5. Use a name that describes the kind of Information that the variable stores.
6. If your varibale name is made up of more than one word, use a capital letter for the first word. 


### ARRAYS

An array is a special type of varible. It doesn't just store one value; it stores a list of values.

You should consider using an array whenever you are working with a **list** or set of values that are **related** to each other.

Arrays are especially helpful when you do not need to specify how many values it will hold.


### CREATING AN ARRAY:

You create an array and give it a name just like you would any other varible (using the var keyword followed by the name of the array).

```javascript
var colors;
colors = ['white', 'black', 'red'];

var el = document.getElementById('colors');
el.textContent = colors[0];
```

This technique called as an **array literal**.

```javascript
var colors;
colors = new Array('white',
 'black',
 'red')

var el = document.getElementById('colors');
el.textContent = colors[0];
```
This technique called as an **array constructor**.

**NOTE**: The array literal is preferred over the array constructor when you creating arrays.


### VALUES IN ARRAY:
* Numbering item in an array:
  **Each item in an array is automatically given a number called index**
  ```javascript
  var color;
  //Index:    0       1       2     
  color = ['white', 'red', 'green']
  ```

  * Accesing item in an array;
**To retrive the second item on the list the array name is specified along with the index number in square brackets**
 ```javascript
var color;
color = ['white', 'red', 'green']
var item = color[2]
console.log(item)
//The output should be red
```
* Number of item in an array.
  **Each array has a property called 'Length', which holds the number of items in the array**
```javascript
var color;
color = ['white', 'red', 'green'];
var TheArrayLength = color.length;
console.log(TheArrayLength);
//The output should be ==> 3
```

* How to Changing Values in an array.
  **To access a value from an array, after the array name you specify the index number for that value inside square brackets.**
  ```javascript
  var color;
  color = ['white', 'red', 'green'];
  color[2] = 'black';

  console.log(color[2]);

  //The output should be ==> 'black'
  ```



### EXPRESSIONS
**An Expression evaluate into (result in) a single value. Broadly speaking there are two types of expression.**

1. Expression that just assign a value to a varible.
   * In order for a varible to be useful, it needs to be given a value. As you seen, this is done using the assignment operator (the equal sign).
   ```javascript
   var color = 'black';
   ```
   *Note***The value color is now black**


2. Epressions that use two or more values to return a single value.
   * You can perform operations on any number of individual values (see next page) to determine a single value.
     ```javascript
     var area = 3 * 2;
     ```
     *Note***The value of area is now**

## JavaScript Math Object
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

**Math.trunc()**

4. Math.trunc() static method returns the integer part of a number by removing any fractional digits.

```javascript
 const truncNumber = Math.trunc(4.16);
      console.log(
        "The Math.trunc() static method returns the integer part of a number by removing any fractional digits = " +
          truncNumber
      );
```

* The output:
  > 4

**Math.min()**

5. Math.min() the method return the minimum value in the array.

 ```javascript
 const arrayOne = [10, 9, 8, 0];
      const minNumber = Math.min(...arrayOne);
      console.log(
        "The Math.min() returns the smallest number in the array = " + minNumber
      );

```


* The output:
  > 0


**Math.max()**

6. Math.max() is a method to return the largest number in the array.

 ```javascript
 const arrayOne = [10, 9, 8, 0];
      const minNumber = Math.max(...arrayOne);
      console.log(
        "The Math.min() returns the largest number in the array = " + minNumber
      );

```

* The output:
  > 10


**Math.abs()**

7. Math.abs() static method returns the absolute value of a number.

```javascript
const absNumber = Math.abs(-8);
console.log(absNumber);
```

* The output:
  > 8


**Math.sgin()**

8. The Math.sign() static method is a useful tool for determining the sign of a number. If you need to know whether a number is positive, negative, or zero.

```javascript
const signNumber = -10;
const theSign = Math.sign(signNumber);
console.log(theSign);
```
* The output:
  > 10

**Math.pow()**

9. The Math.pow() method is a versatile tool that can be used to calculate a wide range of powers. If you need to calculate the power of a number.

The syntax for the Math.pow() method is as follows:

```javascript
Math.pow(base, exponent)
```

```javascript
      const base = 2;
      const exponent = 3;
      const powerNumber = Math.pow(base, exponent);
      console.log(powerNumber);
```
* The output:
  > 8



## Converting values in Javascript.

In this section we will learn how to convert the values from number to string and from string to number.

**parseFloat()**

1. parseFloat() is a method to convert an integer to a string.


```javascript
const floatToInteger = "12";
const floatNumber = parseFloat(floatToInteger);
console.log(floatNumber + 10);
```

* The output:
 > 22

* we can see here a method is useful for parsing strings that contain numbers. If you need to parse a string into a number, the parseFloat() method is a valuable resource.

Here are some additional benefits of using the parseFloat() method:

* It is a concise and easy-to-use method.
* It is a reliable method that will correctly parse most strings that contain numbers.
* It is a versatile method that can be used to parse a wide variety of strings.
