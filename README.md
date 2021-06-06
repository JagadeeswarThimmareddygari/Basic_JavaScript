# Basic_JavaScript

### Table of Contents

- [Comment your javascript](#comment-your-javascript)
- [Declare JavaScript Variables](#declare-javascript-variables)
- [Storing values with the assignment operator](#storing-values-with-the-assignment-operator)
- [Assigning the value of one variable to another](#assigning-the-value-of-one-variable-to-another)
- [Initializing the variable with the assignment operator](#initializing-the-variable-with-the-assignment-operator)
- [Understanding uninitialized variables](#understanding-uninitialized-variables)





## Comment your javascript

```javascript
//This is an in-line comment
/* This is a 
multi-line comment*/
```
---

## Declare Javascript Variables

Javascript provides 8 different data types which are null,undefined,boolean,string,symbol,bigint,number,object.
Variables allow computers to store and manipulate data in a dynamic fashion. 
```javascript
// declare a variable by putting var keyword in front of it.
var ourName;
let userName;
const myNumber;
```
In JavaScript we end statements with semicolons. Variable names can be made up of numbers, letters, and $ or _, but may not contain spaces or start with a number.

---

## Storing values with the assignment operator

In JavaScript, you can store a value in a variable with the assignment operator (=)
```javascript
var myVar;
myVar=10;
```
 
## Assigning the value of one variable to another variable

```javascript
var myVar;
myVar=10;
var myNum;
myNum=myVar;
```
---
## Initializing the variable with the assignment operator

```javascript
var myVar=0;
```
---
## Understanding Uninitialized Variables

```javascript

When JavaScript variables are declared, they have an initial value of undefined. If you do a mathematical operation on an undefined variable your result will be NaN which means "Not a Number". If you concatenate a string with an undefined variable, you will get a literal string of undefined
```javascript
var a;
var b;
var c;

a=a+1;
b=b+5;
c=c+' String!';
```
---

## Understanding Case Sensitivity in Variables

In JavaScript all variables and function names are case sensitive. This means that capitalization matters.
MYVAR is not the same as MyVar nor myvar. It is possible to have multiple distinct variables with the same name but different casing. It is strongly recommended that for the sake of clarity, you do not use this language feature.

```javascript
// Variable declarations
var studlyCapVar;
var properCamelCase;
var titleCaseOver;

// Variable assignments
studlyCapVar = 10;
properCamelCase= "A String";
titleCaseOver = 9000;
```
--- 

## Add Two Numbers with JavaScript

```javascript
var myVar=5+10;
// myVar  now has the value 15
```
---

## Increment a number with javascript
```javascript
myVar=10;
myVar++

//myVar value is incremented by 1 and now has the value 11. It's equivalent of myVar = myVar+1;
```
---

## Decrement a number with javascript
```javascript
var myVar=10;
myVar--;
//myVar value is decremented by 1 and now has the value 9. It's equivalent of myVar=myVar-1;
```
---

## Create a decimal with JavaScript
```javascript
//We can store decimal numbers in variables too. Decimal numbers are sometimes referred to as floating point numbers or floats.
myDecimal=5.7
```
---
## Compound assignment with augmented audition
``` javascript
var myVar=1;
myVar+=5;
```
---
## Compound assignment with augmented substration
```javascript
var myVar=10;
myVar-=5;
//It's equivalent to myVar=myVar-5;
```
---

## Declare a string variable

```javascript
var myName="your name";
```
---
## Escaping Literal quotes in strings

```javascript
var sampleStr="Novin said, \"Jd is learning Javascript\".";
```
---
## Quoting strings with single quotes

```javascript
var myStr = "<a href='http://www.example.com' target='_blank'>Link</a>";
```
---
## Escape sequence in strings

|code   | output         |
|-------|----------------|
| \'    | single quote   |
| \"    | double quote   |
| \\    | blackslash     |
| \n    | newline        |
| \r    | carriage return|
| \t    | tab            |
| \b    | word boundary  |
| \f    | form feed      |
```javascript
var myStr='FirstLine\n\t\\SecondLine\nThirdLine'; // Change this line
/*myStr:
 FirstLine
    \SecondLine
 ThirdLine
 */
```
## Find the length of the string
You can find the length of a String value by writing .length after the string variable or string literal

```javascript
var x="jdreddy";
var y=x.length;
console.log(y) // the value of y will be 7.
```
---
## Use bracket notation to find the first character in the string
Bracket notation is a way to get a character at a specific index within a string.

```javascript
var firstName='novin';
var firstLetter=firstName[0];
console.log(firstLetter)
```
## Understanding string Immutability 
In JavaScript, String values are immutable, which means that they cannot be altered once created.
For example, the code:
```javascript
var myStr="Bob";
myStr[0]='J';
```
cannot change the value of myStr to Job, because the contents of myStr cannot be altered. Note that this does not mean that myStr cannot be changed, just that the individual characters of a string literal cannot be changed. The only way to change myStr would be to assign it with a new string, like this:
```javascript
var myStr='Bob';
myStr='Job';
```
---

## Use Bracket Notation to Find the Nth character in a String

You can also use bracket notation to get the character at other positions within a string.
Remember that computers start counting at 0, so the first character is actually the zeroth character.
Example:
```javascript
var firstName='ada';
var secondLetterOfFirstName=firstName[1];
```
---
## Use Bracket Notation to Find the Last character in a String

```javascript
var firstName='jdreddy';
var lastLetter=firstName[firstName.length-1];
```
---
## Store multiple values in one variable using javascript arrays
With JavaScript array variables, we can store several pieces of data in one place.
You start an array declaration with an opening square bracket, end it with a closing square bracket, and put a comma between each entry, like this:

```javascript
var sandwich=['peanut butter','jelly','breed']
```
---
## Nest one array within Anoher array
```javascript
var myVar=[['jd',19].['novin',23]];
//This is called multi-dimensional array
```
---

## Access Array with Indexes
```javascript
var myArray=[10,20,30];
var data=myArray[0]
```
---
## Modify Array with Indexes
```javascript
var myArray=[10,20,30]
myArray[0]=50;
```
## Access Multidimensional array with indexes

```javascript
var myArray = [[1,2,3], [4,5,6], [7,8,9], [[10,11,12], 13, 14]];
var myData = myArray[2][1];
```
## Manipulate Array with push
An easy way to append data to the end of an array is via the push() function.
.push() takes one or more parameters and "pushes" them onto the end of the array.
Example:
```javascript
var arr1 = [1,2,3];
arr1.push(4);

var arr2 = ["Stimpson", "J", "cat"];
arr2.push(["happy", "joy"]);
```
---
## Manipulate Array with pop()

Another way to change the data in an array is with the .pop() function.
.pop() is used to pop a value off of the end of an array. We can store this popped off value by assigning it to a variable. In other words, .pop() removes the last element from an array and returns that element.
Example:
```javascript
var threeArr = [1, 4, 6];
var oneDown = threeArr.pop();
console.log(oneDown);
console.log(threeArr);
```
---
## Manipulate Array with shift():

pop() always removes the last element of an array. What if you want to remove the first?
That's where .shift() comes in. It works just like .pop(), except it removes the first element instead of the last.

```javascript
var ourArray = ["Stimpson", "J", ["cat"]];
var removedFromOurArray = ourArray.shift();
```
---
## Manipulate Array with unshift():

Not only can you shift elements off of the beginning of an array, you can also unshift elements to the beginning of an array i.e. add elements in front of the array.
.unshift() works exactly like .push(), but instead of adding the element at the end of the array, unshift() adds the element at the beginning of the array.
Example:
```javascript
var ourArray = ["Stimpson", "J", "cat"];
ourArray.shift();
ourArray.unshift("Happy");
```
After the shift, ourArray would have the value ["J", "cat"]. After the unshift, ourArray would have the value ["Happy", "J", "cat"].

---
## Write Reusable JavaScript with the functions
In JavaScript, we can divide up our code into reusable parts called functions.
Example:
```javascript
function functionName() {
  console.log("Hello World");
}
functionName();
```
You can call or invoke this function by using its name followed by parentheses, like this: functionName(); Each time the function is called it will print out the message Hello World on the dev console. All of the code between the curly braces will be executed every time the function is called.
---
## Passing Values to Functions with Arguments

Parameters are variables that act as placeholders for the values that are to be input to a function when it is called. When a function is defined, it is typically defined along with one or more parameters. The actual values that are input (or "passed") into a function when it is called are known as arguments.
Example:
```javascript
function testFun(param1,param2){
  console.log(param1,param2);
}
testFun('jd','reddy');
```









