# ECMAscript-overview documentation
A complete documentaion on the ECMAscript life cycle. 

###### ECMAscript is the standard followed by javascript.
Javacript language which was initially known as mocha ,later renamed to livescript was introduced by netscape, a company which had a major market share in browser business.
It was developed by Brenden Eich. Later a new competitor entered into the market with a much similar language called JScript, which followed their own standard and hence developers had to build a website in either ways to get it supported in both browsers.

Later netscape approached a ECMA (European Computer Manufacturers Association) for maintaining a standard on the web browser scripting language.  That gave birth to ECMAscript
From then, the current termed javascript is actually known as ECMAscript.
 
Version | Second Header
------------ | -------------
ECMAscript 1 | June 1991
ECMAscript 2 | June 1998
ECMAscript 3 | December 1999
ECMAscript 4 | Abandoned ( Never Released )
ECMAscript 5 | December 2009
ECMAscript 5.1 | June 20011
ECMAscript 6 | June 2015
ECMAscript 7 | June 2016
ECMAscript 8 | June 2017

# ECMAscript 1 

## Comments : There  are two types of comments : Single-line or Multi-line

### Single-line : 

  Single line comments start with //. Any text between // and the end of the line will be ignored by ECMAscript (will not be executed).
  ```
  // This is a comment . This line will not be executed.
  var a = 10;
  a = a + 10;
  ```
### Multi-line : 

Multi-line comments start with /* and end with */.Any text between /* and */ will be ignored by ECMAscript.
```
/*
This line including the next three lines
are not executed
Third line.
Fourth line
*/
document.getElementById("myH").innerHTML = "My First Page";
document.getElementById("myP").innerHTML = "My first paragraph.";
```

## Variables : Are used to store data values.
```
var x = 3;
var y = 2;
var z = x + y;
```
x stores the value 3
y stores the value 2
z stores the value 5

All variables must be identified with unique names.
The equal sign (=) is an "assignment" operator, not an "equal to" operator.

## Block : Defines scope
```
var h = 9;
{
  var a = 10;
}
```

## Empty statement: Defined using ;
```
var a;
```
# Operators : 
### Assignment Operator : The assignment operator (=) assigns a value to a variable.
`var x = 10;` 
### Addition Operator : The addition operator (+) adds numbers.
``` var x = 5;
var y = 2;
var z = x + y;
```
### Subtraction Operator : The subtraction operator (-) subtracts numbers.
``` var x = 5;
var y = 2;
var z = x - y;
```
### Multiplication Operator : The multiplication operator (*) multiplies numbers. 

``` 
var x = 5;
var y = 2;
var z = x * y;
``` 
### Division Operator : The division operator (/) divides numbers.

``` 
var x = 5;
var y = 2;
var z = x / y;
``` 
### Modulus Operator : The modulus operator (%) divides and returns reminder.

``` 
var x = 5;
var y = 2;
var z = x % y;
``` 
### Increment Operator : The increment operator (++) increments value of variable by 1;
```
var x = 10;
x++;
```
### Decrement Operator : The decrement operator (--) decrements value of variable by 1;

```
var x = 10;
x--;
```
### Addition Assignment Operator : The addition assignment operator (+=) adds a value to a variable.
```
var x = 10;
x += 5;
```
## ECMAscript Comparison Operators 

### ==	equal to : Used for comparison of expression
` a == b`
` 5 == 6`

### !=	not equal : Used to check for unequality
` a != b`
` 5 != 6`


### >	greater than : Compares if one expression in left is greater than the one in right hand side.
` a > b`
` 5 > 6`

### <	less than : Compares if one expression in left is lesser than the one in right hand side.
` a < b`
` 5 < 6`

### >=	greater than or equal to : Compares if one expression in left is greater than or equal to the one in right hand side.
` a >= b`
` 5 >= 6`
### <=	less than or equal to : Compares if one expression in left is lesser than or equal to the one in right hand side.
` a <= b`
` 5 <= 6`
### ?	ternary operator : Checks if a condition matches and returns different value for result of condition.
` a == b ? true: false`
` 5 > 6 ? 6 : 5`
## Logical operators 
### &&	logical and : Does a logical AND operation
`if (a == b && b ==c) {} `
### ||	logical or : Does a logical OR operation
`if (a == b || b ==c) {} `
### !	logical not  : Does a logical NOT operation
`if (!a == b) {} `




## Bitwise Operators 
Operator |	Description |	Example |	Same as | Result	| Decimal
------------ | ------------- | ------------ | -------------|------------ | -------------
& |	AND |	5 & 1 |	0101 & 0001 |	0001	| 1
&#124;	| OR	| 5 &#124; 1 |	0101 &#124; 0001 |	0101	| 5
~	| NOT |	~ 5 |	 ~0101 |	1010	| 10
^	| XOR |	5 ^ 1 |	0101 ^ 0001 |	0100 | 4
<< |	Zero fill left shift |	5 << 1  |	0101 << 1 |	1010 | 10
*>>* |	Signed right shift |	5 >> 1 |	0101 >> 1 |	0010	| 2
*>>>* |	Zero fill right shift | 5 >>> 1 |	0101 >>> 1 |	0010	|  2


## Data Types
#### Undefined
#### null
#### Boolean
#### String
#### Number

## Functions : 

A ECMAscript function is a block of code designed to perform a particular task.
A ECMAscript function is executed when "something" invokes it (calls it).
You can reuse code: Define the code once, and use it many times.
You can use the same code many times with different arguments, to produce different results.


Syntax : ``` function name(parameter1, parameter2, parameter3) {
    code to be executed
} ```

Example : ``` var x = myFunction(4, 3);    // Function is called, return value will end up in x

function myFunction(a, b) {
    return a * b;            // Function returns the product of a and b
}```

## Objects : 


An object is a member of the type Object. It is an unordered collection of properties which contain primitive
values, objects, or functions. A function stored in the property of an object is called a method.
ECMAScript does not contain proper classes such as those in C++, Smalltalk, or Java, but rather, supports
constructors which create objects by executing code that allocates storage for the objects and initializes all or
part of them by assigning initial values to their properties. 

Example : 
``` var x = new String();        // Declares x as a String object
var y = new Number();        // Declares y as a Number object
var z = new Boolean();       // Declares z as a Boolean object
```
```
var person = {
    firstName:"John",
    lastName:"Doe",
    age:50,
    getAge: function() { return this.age; }
};
```


## Function Scope
#### There are two types of scope: Local scope & Global scope


ECMAscript has function scope: Each function creates a new scope.
Scope determines the accessibility (visibility) of these variables.
Variables defined inside a function are not accessible (visible) from outside the function.

### Local ECMAscript Variables
Variables declared within a ECMAscript function, become LOCAL to the function.
Local variables have local scope: They can only be accessed within the function.
Since local variables are only recognized inside their functions, variables with the same name can be used in different functions.
Local variables are created when a function starts, and deleted when the function is completed.

```
// code here can not use carName

function myFunction() {
    var carName = "Volvo";

    // code here can use carName
}
```

### Global ECMAscript Variables
A variable declared outside a function, becomes GLOBAL.
A global variable has global scope: All scripts and functions on a web page can access it. 
```
var carName = " Volvo";

// code here can use carName

function myFunction() {

    // code here can use carName 

}
```

## Events
### HTML events are "things" that happen to HTML elements.
When ECMAscript is used in HTML pages, ECMAscript can "react" on these events.
An HTML event can be something the browser does, or something a user does.
Here are some examples of HTML events:
An HTML web page has finished loading
An HTML input field was changed
An HTML button was clicked
Often, when events happen, you may want to do something.
ECMAscript lets you execute code when events are detected.

## ECMAscript Strings
### String value
A string value is a member of the type String and is the set of all finite ordered sequences of zero or more Unicode characters.
###  String type
The type String is the set of all finite ordered sequences of zero or more Unicode characters
`var x = "John Doe";`
### String object
A string object is a member of the type Object and is an instance of the String object which is a constructor. That
is, a string object is created by using the String constructor in a new expression, supplying a string as an
argument. The resulting object has an implicit (unnamed) property which is the string. A string object can be
coerced to a string value. A string object can be used anywhere a string value is expected.
``` var x = "John";
var y = new String("John");
```
### String Methods and Properties
Primitive values, like "John Doe", cannot have properties or methods (because they are not objects).
But with ECMAscript, methods and properties are also available to primitive values, because ECMAscript treats primitive values as objects when executing methods and properties.

#### String Length
The length property returns the length of a string
``` var txt = "ABCDEFGHIJKLMNOPQRSTUVWXYZ";
var sln = txt.length; 
``` 
#### String indexOf()
The indexOf() method returns the index of (the position of) the first occurrence of a specified text in a string. 
```
var str = "Please locate where 'locate' occurs!";
var pos = str.indexOf("locate");
```

#### String lastIndexOf()
The lastIndexOf() method returns the index of the last occurrence of a specified text in a string.
``` 
var str = "Please locate where 'locate' occurs!";
var pos = str.lastIndexOf("locate");
```

Both the indexOf(), and the lastIndexOf() methods return -1 if the text is not found.

#### String valueOf()
Returns this string value.

#### String charAt() 
The charAt() method returns the character at a specified index (position) in a string.

``` 
var str = "HELLO WORLD";
str.charAt(0);            // returns H
```

#### String charCodeAt()
The charCodeAt() method returns the unicode of the character at a specified index in a string.

```
var str = "HELLO WORLD";

str.charCodeAt(0);         // returns 72
```

#### String slice()
slice() extracts a part of a string and returns the extracted part in a new string.

The method takes 2 parameters: the starting index (position), and the ending index (position).

``` 
var str = "Apple, Banana, Kiwi";
var res = str.slice(7, 13);
```
If a parameter is negative, the position is counted from the end of the string.

#### String substring()
substring() is similar to slice().
The difference is that substring() cannot accept negative indexes.
Can be with one parameter or two .
```
var str = "Apple, Banana, Kiwi";
var res = str.substring(7);
var res2 = str.substring(7, 13); 
```
First parameter states the starting point and second one states th end point.

#### Converting to Upper and Lower Case
A string is converted to upper case with toUpperCase().
```
var text1 = "Hello World!";       // String
var text2 = text1.toUpperCase();  // text2 is text1 converted to upper
```
A string is converted to lower case with toLowerCase().
```
var text1 = "Hello World!";       // String
var text2 = text1.toLowerCase();  // text2 is text1 converted to lower
```

### ECMAscript Number
####  Number value
A number value a member of the type Number and is a direct representation of a number.
#### Number type
The type Number is a set of values representing numbers. In ECMAScript the set of values represent the doubleprecision
64-bit format IEEE 754 value along with a special “Not-a-Number” (NaN) value, positive infinity, and
negative infinity.

#### Number object
A number object is a member of the type Object and is an instance of the Number object which is a constructor.
That is, a number object is created by using the Number constructor in a new expression, supplying a number as
an argument. The resulting object has an implicit (unnamed) property which is the number. A number object can
be coerced to a number value. A number object can be used anywhere a number value is expected. Note that a
number object can have shared properties by adding them to the Number prototype.

```
var x = 123;
var y = new Number(123);

// typeof x returns number
// typeof y returns object
```

ECMAscript has only one type of number. Numbers can be written with or without decimals.
```
var x = 3.14;    // A number with decimals
var y = 3;       // A number without decimals
Try it yourself »
```

```
var x = 100;         // x is a number

var y = "100";       // y is a string
```
#### NaN - Not a Number
NaN is a ECMAscript reserved word indicating that a number is not a legal number.

Trying to do arithmetic with a non-numeric string will result in NaN (Not a Number).

``` 
var x = 100 / "Apple";  // x will be NaN (Not a Number)
```
However, if the string contains a numeric value , the result will be a number.
```
var x = 100 / "10";     // x will be 10
```

#### You can use the global ECMAscript function isNaN() to find out if a value is a number.
```
var x = 100 / "Apple";
isNaN(x);               // returns true because x is Not a Number
```
#### Infinity
Infinity is the value ECMAscript will return if you calculate a number outside the largest possible number.
The primitive value Infinity represents the positive infinite number value.
```
var myNumber = 2;
while (myNumber != Infinity) {          // Execute until Infinity
    myNumber = myNumber * myNumber;
}
```
#### Hexadecimal
ECMAscript interprets numeric constants as hexadecimal if they are preceded by 0x.

#### Objects cannot be compared.
```
var x = new Number(500);             
var y = new Number(500);

// (x == y) is false because objects cannot be compared
```

#### Number toString()
toString() returns a number as a string.

```
var x = 123;
x.toString();            // returns 123 from variable x
(123).toString();        // returns 123 from literal 123
(100 + 23).toString();   // returns 123 from expression 100 + 23
```
By default, ECMAscript displays numbers as base 10 decimals.

But you can use the toString() method to output numbers as base 16 (hex), base 8 (octal), or base 2 (binary).

```
var myNumber = 128;
myNumber.toString(16);  // returns 80
myNumber.toString(8);   // returns 200
myNumber.toString(2);   // returns 10000000
```
#### Number valueOf()
valueOf() returns a number as a number.
```
var x = 123;
x.valueOf();            // returns 123 from variable x
(123).valueOf();        // returns 123 from literal 123
(100 + 23).valueOf();   // returns 123 from expression 100 + 23
```

#### Number parseInt()
parseInt() parses a string and returns a whole number. Spaces are allowed. Only the first number is returned.
```
parseInt("10");         // returns 10
parseInt("10.33");      // returns 10
parseInt("10 20 30");   // returns 10
parseInt("10 years");   // returns 10
parseInt("years 10");   // returns NaN 
```

#### Number parseFloat()
parseFloat() parses a string and returns a number. Spaces are allowed. Only the first number is returned.
```
parseFloat("10");        // returns 10
parseFloat("10.33");     // returns 10.33
parseFloat("10 20 30");  // returns 10
parseFloat("10 years");  // returns 10
parseFloat("years 10");  // returns NaN
```

### Math Object
The ECMAscript Math object allows you to perform mathematical tasks on numbers.

```
Math.E        // returns Euler's number
Math.PI       // returns PI
Math.SQRT2    // returns the square root of 2
Math.SQRT1_2  // returns the square root of 1/2
Math.LN2      // returns the natural logarithm of 2
Math.LN10     // returns the natural logarithm of 10
Math.LOG2E    // returns base 2 logarithm of E
Math.LOG10E   // returns base 10 logarithm of E
```
#### Math Object Methods

Method | Description
------- | ----------
abs(x) |	Returns the absolute value of x
acos(x) |	Returns the arccosine of x, in radians
asin(x) |	Returns the arcsine of x, in radians
atan(x) |	Returns the arctangent of x as a numeric value between -PI/2 and PI/2 radians
atan2(y, x) |	Returns the arctangent of the quotient of its arguments
ceil(x) |	Returns the value of x rounded up to its nearest integer
cos(x) |	Returns the cosine of x (x is in radians)
exp(x) |	Returns the value of Ex
floor(x) |	Returns the value of x rounded down to its nearest integer
log(x) |	Returns the natural logarithm (base E) of x
max(x, y, z, ..., n) |	Returns the number with the highest value
min(x, y, z, ..., n) |	Returns the number with the lowest value
pow(x, y) |	Returns the value of x to the power of y
random() |	Returns a random number between 0 and 1
round(x) |	Returns the value of x rounded to its nearest integer
sin(x) |	Returns the sine of x (x is in radians)
sqrt(x) |	Returns the square root of x
tan(x) |	Returns the tangent of an angle


## ECMAscript Dates
The Date object lets you work with dates (years, months, days, hours, minutes, seconds, and milliseconds)
### ECMAscript Date Formats
A ECMAscript date can be written as a string:

Fri Feb 02 2018 05:05:05 GMT+0530 (IST)

or as a number:

1517528105860

Dates written as numbers, specifiy the number of milliseconds since January 1, 1970, 00:00:00.

The Date object lets us work with dates.

A date consists of a year, a month, a day, an hour, a minute, a second, and milliseconds.

Date objects are created with the new Date() constructor.

There are 4 ways of initiating a date.

```
new Date()
new Date(milliseconds)
new Date(dateString)
new Date(year, month, day, hours, minutes, seconds, milliseconds)
```

### Date Methods
#### toString() Method
Date is converted to a string, with the toString() method.
```
d = new Date();
d = d.toString();
```
#### valueOf() Method
Return time 

#### Other main Date methods
Method |	Description
-------  | -----------
getDate() |	Get the day as a number (1-31)
getDay() |	Get the weekday as a number (0-6)
getFullYear() |	Get the four digit year (yyyy)
getHours() |	Get the hour (0-23)
getMilliseconds() |	Get the milliseconds (0-999)
getMinutes() |	Get the minutes (0-59)
getMonth() |	Get the month (0-11)
getSeconds() |	Get the seconds (0-59)
getTime() |	Get the time (milliseconds since January 1, 1970)

#### UTC Date Methods
UTC date methods are used for working UTC dates (Universal Time Zone dates).

Method | Description
------- | --------
getUTCDate() |	Same as getDate(), but returns the UTC date
getUTCDay() |	Same as getDay(), but returns the UTC day
getUTCFullYear() |	Same as getFullYear(), but returns the UTC year
getUTCHours() |	Same as getHours(), but returns the UTC hour
getUTCMilliseconds() |	Same as getMilliseconds(), but returns the UTC milliseconds
getUTCMinutes() |	Same as getMinutes(), but returns the UTC minutes
getUTCMonth() |	Same as getMonth(), but returns the UTC month
getUTCSeconds() |	Same as getSeconds(), but returns the UTC seconds

#### Compare Dates
Dates can easily be compared.

The following example compares today's date with January 14, 2100: 
```
var today, someday, text;
today = new Date();
someday = new Date();
someday.setFullYear(2100, 0, 14);

if (someday > today) {
    text = "Today is before January 14, 2100.";
} else {
    text = "Today is after January 14, 2100.";
}
```

## ECMAscript Arrays
An array is a special variable, which can hold more than one value at a time.

If you have a list of items (a list of car names, for example), storing the cars in single variables could look like this:
```
var car1 = "Saab";
var car2 = "Volvo";
var car3 = "BMW";
```
The above would be like this ,when made to an array : 
` var cars = new Array("Saab", "Volvo", "BMW");`

Accessing the elements of array can be like this : 
` var name = cars[0]; `

To access full array : 
` var carList = cars; `

### Array Methods 
#### Converting Arrays to Strings
The ECMAscript method toString() converts an array to a string of (comma separated) array values.
```
var fruits = ["Banana", "Orange", "Apple", "Mango"];
var string = fruits.toString();
```

#### The join() method also joins all array elements into a string.

It behaves just like toString(), but in addition you can specify the separator:
```
var fruits = ["Banana", "Orange", "Apple", "Mango"];
var string = fruits.join(" * ");
```

#### Sorting an Array
The sort() method sorts an array alphabetically.
```
var fruits = ["Banana", "Orange", "Apple", "Mango"];
fruits.sort();            // Sorts the elements of fruits
```
#### Reversing an Array
The reverse() method reverses the elements in an array.
You can use it to sort an array in descending order.

``` var fruits = ["Banana", "Orange", "Apple", "Mango"];
fruits.sort();            // Sorts the elements of fruits 
fruits.reverse();         // Reverses the order of the elements
```

## Boolean Values
Very often, in programming, you will need a data type that can only have one of two values, like

YES / NO
ON / OFF
TRUE / FALSE
For this, ECMAscript has a Boolean data type. It can only take the values true or false.

### Boolean value
A boolean value is a member of the type Boolean and is one of either two unique values, true and false

### Boolean type
The type Boolean represents a logical entity and consists of exactly two unique values. One is called true and the
other is called false.

### Boolean object
A Boolean object is a member of the type Object and is an instance of the Boolean object which is a constructor.
That is, a boolean object is created by using the Boolean constructor in a new expression, supplying a boolean as
an argument. The resulting object has an implicit (unnamed) property which is the boolean. A boolean object can
be coerced to a boolean value. A boolean object can be used anywhere a boolean value is expected.

### The Boolean() Function
You can use the Boolean() function to find out if an expression (or a variable) is true.
` Boolean(10 > 9)        // returns true`

Everything With a "Value" is True.

```
100

3.14

-15

"Hello"

"false"

7 + 1 + 3.14
```

Everything Without a "Value" is False
```
var x = 0;
Boolean(x);       // returns false
```
```
var x = "";
Boolean(x);       // returns false
```
The Boolean value of NaN is false:

```
var x = 10 / "H";
Boolean(x);       // returns false
```

### Boolean Object 
` var y = new Boolean(false); `

```
var x = false;
var y = new Boolean(false);

// typeof x returns boolean
// typeof y returns object
```

```
var x = new Boolean(false);             
var y = new Boolean(false);

// (x == y) is false because objects cannot be compared
```

## Conditional Statements 
Very often when you write code, you want to perform different actions for different decisions.

You can use conditional statements in your code to do this.
In ECMAscript we have the following conditional statements:
Use if to specify a block of code to be executed, if a specified condition is true
Use else to specify a block of code to be executed, if the same condition is false.

### The If statement
Use the if statement to specify a block of JavaScript code to be executed if a condition is true.
Syntax : ```
if (condition) {
    block of code to be executed if the condition is true
}
```

Example : 
```
if (hour < 18) {
    greeting = "Good day";
}```

### The else Statement
Use the else statement to specify a block of code to be executed if the condition is false.

Syntax : 
```
if (condition) {
    block of code to be executed if the condition is true
} else { 
    block of code to be executed if the condition is false
}
```

## Iteration statements or Loops : Used for executing a block a number of times.


* While 
* For
* For...in

### While  :  The while loop loops through a block of code as long as a specified condition is true.
```
while (condition) {
    code block to be executed
}
```
Example : 
```
var a = 10;
while (a > 0) {
a = a - 1;
}
```
### For : The for loop is often the tool you will use when you want to create a loop.
Syntax : 
```
for (statement 1; statement 2; statement 3) {
    code block to be executed
}
```
Example : 
```
for (i = 0; i < 5; i++) {
    text += "The number is " + i + "<br>";
}
```
### For..in : The for/in statement loops through the properties of an object
Syntax : 
```
for (index in object/array) { array[index] }
```
Example : ```
var a = [1,2,3];
for (var i in a) {
c = a[i];
}```


## Break and Continue statements 
The break statement "jumps out" of a loop.
The continue statement "jumps over" one iteration in the loop.

### The Break Statement 
You have already seen the break statement used in an earlier chapter of this tutorial. It was used to "jump out" of a switch() statement.

The break statement can also be used to jump out of a loop.  

The break statement breaks the loop and continues executing the code after the loop (if any):
```
for (i = 0; i < 10; i++) {
    if (i === 3) { break; }
    text += "The number is " + i + "<br>";
}
```

### The Continue Statement
The continue statement breaks one iteration (in the loop), if a specified condition occurs, and continues with the next iteration in the loop.

This example skips the value of 3:
```
for (i = 0; i < 10; i++) {
    if (i === 3) { continue; }
    text += "The number is " + i + "<br>";
}
```

### The WITH statement
` with ( Expression ) Statement`

The with statement adds a computed object to the front of the scope chain of the current execution context, then
executes a statement with this augmented scope chain, then restores the scope chain.

###  The RETURN statement
An ECMAScript program is considered syntactically incorrect and may not be executed at all if it contains a
return statement that is not within the Block of a FunctionDeclaration. It causes a function to cease execution
and return a value to the caller. If Expression is omitted, the return value is the undefined value. Otherwise, the
return value is the value of Expression.
```
If (a == 1) {
    return true;
} else {
    return;
}
```
## The constructor Property
The constructor property returns the constructor function for all JavaScript variables.
```
"John".constructor                // Returns function String()  {[native code]}
(3.14).constructor                // Returns function Number()  {[native code]}
false.constructor                 // Returns function Boolean() {[native code]}
[1,2,3,4].constructor             // Returns function Array()   {[native code]}
{name:'John',age:34}.constructor  // Returns function Object()  {[native code]}
new Date().constructor            // Returns function Date()    {[native code]}
function () {}.constructor        // Returns function Function(){[native code]}
Try it Yourself »
```

## JavaScript Bitwise Operators 

Operator | Name |	Description
------- | ------ | -----------
& |	AND |	Sets each bit to 1 if both bits are 1
| |	OR |	Sets each bit to 1 if one of two bits is 1
^ |	XOR |	Sets each bit to 1 if only one of two bits is 1
~ |	NOT |	Inverts all the bits
<< |	Zero fill left shift |	Shifts left by pushing zeros in from the right and let the leftmost bits fall off
*>>* |	Signed right shift |	Shifts right by pushing copies of the leftmost bit in from the left, and let the rightmost bits fall off
*>>>* |	Zero fill right shift |	Shifts right by pushing zeros in from the left, and let the rightmost bits fall off

## Future Reserved Words
The following words are used as keywords in proposed extensions and are therefore reserved to allow for the
possibility of future adoption of those extensions  : 

case,
debugger,
export,
super,
catch,
default, 
extends,
switch,
class,
do,
finally,
throw,
const,
enum,
import, 
try



# ECMAscript 2 
### The development of this Standard started in November 1996. The first edition of this ECMA Standard was adopted by the ECMA General Assembly of June 1997.
### That ECMA Standard was submitted to ISO/IEC JTC 1 for adoption under the fast-track procedure, and approved as international standard ISO/IEC 16262, in April 1998. The ECMA General Assembly of June 1998 has approved the second edition of ECMA-262 to keep it fully aligned with ISO/IEC 16262. Changes from the first edition are editorial in nature.

#### Future implementations : 
The work on standardization of the language was happening to support regular expressions, richer control statements and
better string handling, in addition to the core language standardized in the first two editions of the ECMA Standard.
These features and others, such as try/catch exception handling and better internationalization facilities, are were
documented in anticipation of the third edition of the standard about the end of 1999 which would contain the actual second version of the language.

# ECMAscript 3 
### The third edition of the Standard and includes powerful regular expressions, better string handling, new control statements, try/catch exception handling, tighter definition of errors, formatting for numeric output and minor changes.

## Addition of Object Initializer.
In previous version of ECMAscript , to create a new object , we were to use following : 
` var a = new Object({'name' : 'john'}); `
But now, in this version of ECMAscript an object can  be initialized using ` {} `.
Example : ` var n = {'name' : 'john'};`

`var car = {type:"Fiat", model:"500", color:"white"};`
## Grouping operator : `()`
This is an operator used to group expressions ,so that it is more readable and also easily executable.
Example : 
```
var a = 1;
var b = 2;
var c = 3;
var d = a*(b + c); // This states that , (b+c) will be evaluated and then multiplied by variable a.

// without the grouping operator expression would have been : var d = a * b + c; and the it would have got evaluated in an order where a*b is evaluated first and then result is added to c.
```

This operator was also introduced in context to usage of `type of ` and `delete`

## Function Expression 
The function keyword can be used to define a function inside an expression.
```
var getRectArea = function(width, height) {
    return width * height;
}
```
## Introduced 'instanceof' Operator
This operator was introduced to check if an object created is an instance of contructor class.

```
 // defining constructors
function C() {}
function D() {}

var o = new C();

// true, because: Object.getPrototypeOf(o) === C.prototype
o instanceof C;

// false, because D.prototype is nowhere in o's prototype chain
o instanceof D;
```

## Introduced 'in' operator 
The in operator returns true if the specified property is in the specified object or its prototype chain.

```
var car = {make: 'Honda', model: 'Accord', year: 1998};

console.log('make' in car);
// expected output: true

delete car.make;
if ('make' in car === false) {
  car.make = 'Suzuki';
}

console.log(car.make);
// expected output: "Suzuki"

```

## The Strict Equals Operator ' === '
The Strict Equals operator returns true if the operands are strictly equal (see above) with no type conversion.
```
3 === 3   // true
3 === '3' // false
var object1 = {'key': 'value'}, object2 = {'key': 'value'};
object1 === object2 //false
```

## The Strict inequality Operator ' !== '
The strict inequality operator returns true if the operands are not equal and/or not of the same type.
```
3 !== '3' // true
3 !== 3 // false
4 !== 3   // true
```

## do..while() Iteration
The do...while statement creates a loop that executes a specified statement until the test condition evaluates to false. The condition is evaluated after executing the statement, resulting in the specified statement executing at least once.

```
var result = "";
var i = 0;

do {
  i = i + 1;
  result = result + i;
} while (i < 5);

console.log(result);
// expected result: "12345"
```

## Switch condition 
The switch statement evaluates an expression, matching the expression's value to a case clause, and executes statements associated with that case, as well as statements in cases that follow the matching case.

```
var expr = 'Papayas';
switch (expr) {
  case 'Oranges':
    console.log('Oranges are $0.59 a pound.');
    break;
  case 'Mangoes':
  case 'Papayas':
    console.log('Mangoes and papayas are $2.79 a pound.');
    // expected output: "Mangoes and papayas are $2.79 a pound."
    break;
  default:
    console.log('Sorry, we are out of ' + expr + '.');
}
```

## Labeled statements 
The labeled statement can be used with break or continue statements. It is prefixing a statement with an identifier which you can refer to.

```
var str = "";

loop1:
for (var i = 0; i < 5; i++) {
  if (i === 1) {
    continue loop1;
  }
  str = str + i;
}

console.log(str);
// expected output: "0234"

```

## Throw statements
The throw statement throws a user-defined exception. Execution of the current function will stop (the statements after throw won't be executed), and control will be passed to the first catch block in the call stack. If no catch block exists among caller functions, the program will terminate.

```
function getRectArea(width, height) {
  if (isNaN(width) || isNaN(height)) {
    throw "Parameter is not a number!";
  }
}

try {
  getRectArea(3, 'A');
}
catch(e) {
  console.log(e);
  // expected output: "Parameter is not a number!"
}
```
## Try statements
The try...catch statement marks a block of statements to try, and specifies a response, should an exception be thrown.

Syntax : 
```
try {
   try_statements
}
[catch (exception_var_1 if condition_1) { // non-standard
   catch_statements_1
}]
...
[catch (exception_var_2) {
   catch_statements_2
}]
[finally {
   finally_statements
}]
```

Example : 
``` 
try {
  eval('alert("Hello world)');
}
catch(error) {
  console.log(error);
  // expected output: SyntaxError: unterminated string literal
  // Note - error messages will vary depending on browser
}

```

## Function Objects 
A new concept was introduced by which function could be used to define an object, and hence in ECMAscript function were also considered as objects.
```
function Car(name ,type) {
    this.name = name;
    this.type = type;
}
var abc = new Car('abc','sedan');
var a =  abc instanceof Car; // true
var b =  typeof Car;  // Function
var c = Car instanceof Object; // true
```


## URI Handling Function Properties inntroduced
Uniform Resource Identifiers, or URIs, are strings that identify resources (e.g. web pages or files) and transport protocols by which to access them (e.g. HTTP or FTP) on the Internet. So to utilise this , following functions were introduced, which provided minimal support to URI in ECMAscript.

### encodeURI (uri)
The encodeURI function computes a new version of a URI in which each instance of certain
characters is replaced by one, two or three escape sequences representing the UTF-8 encoding of the
character.
This function encodes special characters, except: , / ? : @ & = + $ #.

```
var uri = "my test.asp?name=ståle&car=saab";
var res = encodeURI(uri); //  my%20test.asp?name=st%C3%A5le&car=saab
```
### encodeURIComponent (uriComponent)
The encodeURIComponent function computes a new version of a URI in which each instance of
certain characters is replaced by one, two or three escape sequences representing the UTF-8 encoding
of the character.
This function encodes special characters. In addition, it encodes the following characters: , / ? : @ & = + $ #

```
var uri = "https://example.com/my test.asp?name=ståle&car=saab";
var res = encodeURIComponent(uri);  
//  https%3A%2F%2Fexample.com%2Fmy%20test.asp%3Fname%3Dst%C3%A5le%26car%3Dsaab
```

### decodeURI (encodedURI) 
The decodeURI function computes a new version of a URI in which each escape sequence and UTF-
8 encoding of the sort that might be introduced by the encodeURI function is replaced with the character that it represents. Escape sequences that could not have been introduced by encodeURI are
not replaced.
The decodeURI() function is used to decode a URI.
```
var uri = "my test.asp?name=ståle&car=saab";
var enc = encodeURI(uri);
var dec = decodeURI(enc);
var res = enc + dec;
```
### decodeURIComponent (encodedURIComponent)
The decodeURIComponent function computes a new version of a URI in which each escape
sequence and UTF-8 encoding of the sort that might be introduced by the encodeURIComponent
function is replaced with the character that it represents.
This function replaces each escape sequence in the encoded URI component with the character that it represents.

```
function containsEncodedComponents(x) {
  // ie ?,=,&,/ etc
  return (decodeURI(x) !== decodeURIComponent(x));
}

console.log(containsEncodedComponents('%3Fx%3Dtest')); // ?x=test
// expected output: true

console.log(containsEncodedComponents('%D1%88%D0%B5%D0%BB%D0%BB%D1%8B')); // шеллы
// expected output: false

```

## Regular Expressions
Regular expressions are patterns used to match character combinations in strings. In ECMAscript, regular expressions are also objects.
These patterns are used with the exec method of RegExp and replace method of String.
A regular expression is a sequence of characters that forms a search pattern.

When you search for data in a text, you can use this search pattern to describe what you are searching for.
A regular expression can be a single character, or a more complicated pattern.
Regular expressions can be used to perform text search and text replace operations.
A regular expression can be created using the RegExp() with new operator by passing in the pattern.
Example : 
` var re = new RegExp('ab+c');`

### String replace function 
The replace() method returns a new string with some or all matches of a pattern replaced by a replacement. The pattern can be a string or a RegExp, and the replacement can be a string or a function to be called for each match.

```
var str = 'abcdefgh'; 
var txt = str.replace("abc","dce"); 
// str = dcedefgh
```
### Exec function of RegExp
The exec() method tests for a match in a string.
This method returns the matched text if it finds a match, otherwise it returns null.

```
var str = "The best things in life are free";
var patt = new RegExp("e");
var res = patt.exec(str);
```

## Error Object introduced 
 The Error constructor creates an error object. Instances of Error objects are thrown when runtime errors occur. The Error object can also be used as a base object for user-defined exceptions. See below for standard built-in error types.

 Syntax : `new Error([message[, fileName[, lineNumber]]]) `

 Example : 
 ```
 try {
  throw new Error('Whoops!');
} catch (e) {
  console.log(e.name + ': ' + e.message);
}
 ```

