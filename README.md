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

## Initializing the variable with the assignment operator

```javascript
var myVar=0;
```

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
## Add Two Numbers with JavaScript

```javascript
var myVar=5+10;
// myVar  now has the value 15
```

## Increment a number with javascript
```javascript
myVar=10;
myVar++

//myVar value is incremented by 1 and now has the value 11. It's equivalent of myVar = myVar+1;
```




