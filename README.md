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

```
var fruits = ["Banana", "Orange", "Apple", "Mango"];
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
Use the if statement to specify a block of ECMAscript code to be executed if a condition is true.
Syntax : 
```
if (condition) {
    block of code to be executed if the condition is true
}
```

Example : 
```
if (hour < 18) {
    greeting = "Good day";
}
```


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
Example : 
```
var a = [1,2,3];
for (var i in a) {
c = a[i];
}
```


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
The constructor property returns the constructor function for all ECMAscript variables.
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

## ECMAscript Bitwise Operators 

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

# ECMAscript 4 
### This version of ECMAscript was abandoned , hence was never released.

# ECMAscript 5
#### In this version of ECMAscript few  new concepts were introduced in the prototypes of Objects and arrays as well as , many more.

## Strict Mode 
Strict mode is enabled using 'use strict' keyword in the beginning of program. 
It is not a statement, but a literal expression, ignored by earlier versions of ECMAscript.
The purpose of "use strict" is to indicate that the code should be executed in "strict mode".
With strict mode, you can not, for example, use undeclared variables.

### Invalid code in STRICT MODE 
```
"use strict";
x = 3.14;  // This will cause an error because x is not declared
```

```
"use strict";
myFunction();

function myFunction() {
    y = 3.14;   // This will also cause an error because y is not declared
}
```

```
x = 3.14;       // This will not cause an error. 
myFunction();

function myFunction() {
   "use strict";
    y = 3.14;   // This will cause an error
}
```

###### Strict mode makes it easier to write "secure" ECMAscript.
As an example, in normal ECMAscript, mistyping a variable name creates a new global variable. In strict mode, this will throw an error, making it impossible to accidentally create a global variable.
In strict mode, any assignment to a non-writable property, a getter-only property, a non-existing property, a non-existing variable, or a non-existing object, will throw an error.

```
"use strict";
x = {p1:10, p2:20};      // This will cause an error
```

Deleting a variable (or object) is not allowed.
```
"use strict";
var x = 3.14;
delete x; 
```

Deleting a function is not allowed
```
"use strict";
function x(p1, p2) {}; 
delete x;                // This will cause an error 
```
Duplicating a parameter name
```
"use strict";
function x(p1, p1) {};   // This will cause an error
```

Octal numeric iterals are not allowed
```
"use strict";
var x = 010;             // This will cause an error
```

Ocatal escape charecters are not allowed
```
"use strict";
var x = "\010"; 
```

Writing to a read-only property is not allowed.
```
"use strict";
var obj = {};
Object.defineProperty(obj, "x", {value:0, writable:false});

obj.x = 3.14;            // This will cause an error
```

Writing to a getter-only property is not allowed
```
"use strict";
var obj = {get x() {return 0} };

obj.x = 3.14;            // This will cause an error
```

Deleting an undeletable property is not allowed.
"use strict";
delete Object.prototype; // This will cause an error

The string "eval" cannot be used as a variable.
"use strict";
var eval = 3.14;         // This will cause an error

The string "arguments" cannot be used as a variable:
```
"use strict";
var arguments = 3.14;    // This will cause an error
```
with statement is not allowed.
```
"use strict";
with (Math){x = cos(2)}; // This will cause an error
```
For security reasons, eval() is not allowed to create variables in the scope from which it was called.
```
"use strict";
eval ("var x = 2");
alert (x);               // This will cause an error
```
Future reserved keywords are not allowed in strict mode. These are:

* implements
* interface
* let
* package
* private
* protected
* public
* static
* yield


## Accessor Functions
There are two types of .accessor functions: 
* getter
* setter

Accessor function are used to allow developer manage what should happen when a object property is accessed and when object property is set.

### Getter function 
lets consider an example object : 
```
var user =  {
    name : 'john',
    age : 56,
    get name2() {
        return this.name.toUpperCase();
    }
}
```
So here when we try to access property of user -> `user.name2` it returns the value as 'JOHN'
Hence the developer can decide what value must be returned when that particular property is accessed.
Same property can be set using Setter functions.

### Setter function
Lets consider the above example with a setter function.
```
var user = {
    name: 'john',
    age: 56,
    get: name2() {
        return this.name.toUpperCase();
    },
    set: name2(newName) {
        this.name = newName.toUpperCase();
    }
};
```
Here when we try to set the property of user -> `user.name2` it takes the value as parameter of set function and then executes the code inside it.

### Researved words can be used as property keys
The ECMAscript researved words can be used as property keys of object and also as nonqouted keys.

```
var a = {
    new: 'new property',
    age: 89
};
```

### Legal trailing comas.
The trailing commas are considered as legal, which means a comma used at te end of each property or value of an object or array with no values after it ,are considered legal.
Example : 
```
var obj = {
    a:1,
    b:2,
};
```

### Multiline string literals

A string can be written in multi-lines by using back-slash '/' at the end of each line.

var stn = 'first line /
    second line/
    third line';

### Object.create()
Object.create() function is used to create a object using a prototype object as first parameter and 
a properties object as second parameters.
Example : 
```
var userPrototype = {
    age: 0,
    fullname: function() {
        return this.firstname + ' ' + this.lastname;
    },
    getLastname: function() {
        return this.lastname;
    }
} 

var jone = Object.create(userPrototype, {height: {value:'183'}});
```
### Object.getPrototypeOf()
We can get the prototype of an object using Object.getPrototypeOf() function .
An object is to passed to this function and it returs that objects prototype.
Example : 
```
var userPrototype = {
    age: 0,
    fullname: function() {
        return this.firstname + ' ' + this.lastname;
    },
    getLastname: function() {
        return this.lastname;
    }
} 

var jone = Object.create(userPrototype, {firstname: {value:'jone'}, lastname: {value: 'mathews'}});

Object.getPrototypeOf(jone); // {age: 0, fullname: ƒ, getLastname: ƒ}

```
### Object.defineProperty()
The Object.defineProperty() method defines a new property directly on an object, or modifies an existing property on an object, and returns the object.
```
const object1 = {};

Object.defineProperty(object1, 'property1', {
  value: 42,
  writable: false
});

object1.property1 = 77;
// throws an error in strict mode

console.log(object1.property1);
// expected output: 42

```

### Object.defineProperties()
The Object.defineProperties() method defines new or modifies existing properties directly on an object, returning the object.
```
onst object1 = {};

Object.defineProperties(object1, {
  property1: {
    value: 42,
    writable: true
  },
  property2: {}
});

console.log(object1.property1);
// expected output: 42
```
### Object.getOwnPropertyDescriptor()
The Object.getOwnPropertyDescriptor() method returns a property descriptor for an own property (that is, one directly present on an object and not in the object's prototype chain) of a given object.

```
const object1 = {
  property1: 42
}

const descriptor1 = Object.getOwnPropertyDescriptor(object1, 'property1');

console.log(descriptor1.configurable);
// expected output: true

console.log(descriptor1.value);
// expected output: 42

```
### Object.keys()
The Object.keys() method returns an array of a given object's own enumerable properties, in the same order as that provided by a for...in loop (the difference being that a for-in loop enumerates properties in the prototype chain as well).
This basically return an array containing keys of the object but doesn't include the non-enumerable properties.
```
var arr = ['a', 'b', 'c'];
console.log(Object.keys(arr)); // console: ['0', '1', '2']

// array like object
var obj = { 0: 'a', 1: 'b', 2: 'c' };
console.log(Object.keys(obj)); // console: ['0', '1', '2']
```
### Object.getOwnPropertyNames()
Object.getOwnPropertyNames() does the same task as Object.keys() but it also returns the non-enumerable properties of an object.
```
const object1 = {
  a: 1,
  b: 2,
  c: 3
};

console.log(Object.getOwnPropertyNames(object1));
// expected output: Array ["a", "b", "c"]

```
### Object.preventExtensions()
The Object.preventExtensions() method prevents new properties from ever being added to an object (i.e. prevents future extensions to the object).
```
const object1 = {};

Object.preventExtensions(object1);

try {
  Object.defineProperty(object1, 'property1', {
    value: 42
  });
} catch (e) {
  console.log(e);
  // Expected output: TypeError: Cannot define property property1, object is not extensible
}
```
### Object.isExtensible()
The Object.isExtensible() method determines if an object is extensible (whether it can have new properties added to it).
```
const object1 = {};

console.log(Object.isExtensible(object1));
// expected output: true

Object.preventExtensions(object1);

console.log(Object.isExtensible(object1));
// expected output: false
```

### Object.seal()
The Object.seal() method seals an object, preventing new properties from being added to it and marking all existing properties as non-configurable. Values of present properties can still be changed as long as they are writable.
```
const object1 = {
  property1: 42
};

Object.seal(object1);
object1.property1 = 33;
console.log(object1.property1);
// expected output: 33

delete object1.property1; // cannot delete when sealed
console.log(object1.property1);
// expected output: 33
```
### Object.isSealed()
The Object.isSealed() method determines if an object is sealed.
```
const object1 = {
  property1: 42
};

console.log(Object.isSealed(object1));
// expected output: false

Object.seal(object1);

console.log(Object.isSealed(object1));
// expected output: true

```
### Object.freeze()
The Object.freeze() method freezes an object: that is, prevents new properties from being added to it; prevents existing properties from being removed; and prevents existing properties, or their enumerability, configurability, or writability, from being changed, it also prevents the prototype from being changed.  The method returns the object in a frozen state.
```
const object1 = {
  property1: 42
};

const object2 = Object.freeze(object1);

object2.property1 = 33;
// Throws an error in strict mode

console.log(object2.property1);
// expected output: 42
```
### Object.isFrozen()
The Object.isFrozen() determines if an object is frozen.
const object1 = {
  property1: 42
};

console.log(Object.isFrozen(object1));
// expected output: false

Object.freeze(object1);

console.log(Object.isFrozen(object1));
// expected output: true


### Function.bind()
The bind() method creates a new function that, when called, has its this keyword set to the provided value and also passes arguments if provided while the function is being called.

```
var model = {
    a:'name',
    getValue: function() {
        return this.a;
    },
    getArguments: function() {
        console.log(this.a);
        return arguments;
    }
}

var newFunc = model.getArguments;
newFunc(); //  undefined as it doesn't have any property 'a'.
var anotherFunc = newFunc.bind(model,12,3,4);
anotherFunc() // Same function returns arguments and also logs the value of propert 'a' in model. 
```


### Date.now() 
The number of milliseconds between midnight, January 1, 1970, and the current date and time.
```
var start = Date.now();  
var response = prompt("What is your name?", "");  
var end = Date.now();  
var elapsed = (end - start) / 1000;  
```

### Date.toISOString()
The toISOString() method returns a string in simplified extended ISO format (ISO 8601), which is always 24 or 27 characters long (YYYY-MM-DDTHH:mm:ss.sssZ or ±YYYYYY-MM-DDTHH:mm:ss.sssZ, respectively). The timezone is always zero UTC offset, as denoted by the suffix "Z".

```
var event = new Date('05 October 2011 14:48 UTC');
console.log(event.toString());
// expected output: Wed Oct 05 2011 16:48:00 GMT+0200 (CEST)
// (note: your timezone may vary)

console.log(event.toISOString());
// expected output: 2011-10-05T14:48:00.000Z
```
## JSON related functions
### JSON.parse() 
The JSON.parse() method parses a JSON string, constructing the ECMAscript value or object described by the string. An optional reviver function can be provided to perform a transformation on the resulting object before it is returned.
```
var json = '{"result":true, "count":42}';
obj = JSON.parse(json);

console.log(obj.count);
// expected output: 42

console.log(obj.result);
// expected output: true

```

```
JSON.parse('{"p": 5}', (key, value) =>
  typeof value === 'number'
    ? value * 2 // return value * 2 for numbers
    : value     // return everything else unchanged
);

// { p: 10 }
```

### JSON.stringify()
The JSON.stringify() method converts a ECMAscript value to a JSON string, optionally replacing values if a replacer function is specified, or optionally including only the specified properties if a replacer array is specified

```
console.log(JSON.stringify({ x: 5, y: 6 }));
// expected output: "{"x":5,"y":6}"

console.log(JSON.stringify([new Number(3), new String('false'), new Boolean(false)]));
// expected output: "[3,"false",false]"

console.log(JSON.stringify({ x: [10, undefined, function(){}, Symbol('')] }));
// expected output: "{"x":[10,null,null,null]}"

console.log(JSON.stringify(new Date(2006, 0, 2, 15, 4, 5)));
// expected output: ""2006-01-02T15:04:05.000Z""
```

## Array Functions

### Array.isArray()
The isArray() method determines whether an object is an array.
```
var a = [1,2,3];
console.log(Array.isArray(a)); // true
```

### Array.prototype.every()
The every() method tests whether all elements in the array pass the test implemented by the provided function.
```
var a = [10,20,30];
console.log(a.every(function(b) { return b > 10}));  // false
console.log(a.every(function(b) { return b > 9}));  // true
```

### Array.prototype.filter() 
The filter function iterates through each vlue in array and returns the ones which satifies the mentioned condition.
```
var arr = [1,2,3,40,35];
var newArray = arr.filter(function(val) {
    return val % 2 === 0; // condition :  values multiple of 2.
});

console.log(newArray); // [2,40] 
```

### Array.prototype.forEach()
The forEach() function iterates through array value .

Example : 
```
var arr = [1,2,3];
arr.forEach(function(val) { console.log(val);}); // 1,2,3
```

### Array.prototype.indexOf()
The indexOf() function is used to find the index of first occurence of specified value in an array.
if the value doesn't exist in the array , the index returned will be -1;

```
var arr = [1,2,3];
var index = arr.indexOf(2);
console.log(index); // 1

var index = arr.indexOf(8);
console.log(index); // -1
```

### Array.prototype.lastIndexOf()
The indexOf() function is used to find the index of first occurence of specified value in an array.
if the value doesn't exist in the array , the index returned will be -1;

```
var arr = [1,2,3,2];
var index = arr.lastIndexOf(2);
console.log(index); // 3

var index = arr.indexOf(8);
console.log(index); // -1
```

### Array.prototype.map()
The map() function iterates through the array and replaces the individual value in the array based on the returned value;

```
var arr = [1,2,3];
arr.map(function(val) {
    return val * val;  // replacing all values with its squares
});
console.log(arr); // [1,4,9]
```

### Array.prototype.reduce()
The reduce() method applies a function against an accumulator and each element in the array (from left to right) to reduce it to a single value.
```
var arr = [1,2,3];
var newArr = arr.reduce(function(accumulator, currentVal) {
    return currentVal * accumulator;
});

console.log(newArr); // 6
```

### Array.prototype.some()
The some() method tests whether at least one element in the array passes the test implemented by the provided function.

```
var arr = [1,2,3,4];
console.log(arr.some(function(val) {
    return val % 2 === 0; 
}));            // true;

```


# ECMAscript 6  

## Let and Const  
let is method of declaring a variable with block level scope.
```
{
    let a = 10;
    console.log(a);  10
    if (true)
    {
        let b = 12;
        console.log(b);  // 12
    }
    console.log(b);  // undefined
}
```
## Arrow Function
An arrow function expression has a shorter syntax than a function expression and does not have its own this, arguments, super, or new.target. These function expressions are best suited for non-method functions, and they cannot be used as constructors.

```
var materials = [
  'Hydrogen',
  'Helium',
  'Lithium',
  'Beryllium'
];

console.log(materials.map(material => material.length));
// expected output: Array [8, 6, 7, 9]

```

```
var arr = [1,2,3];
arr.forEach(() => console.log('hello'));
```

## Strings

### Methods
New methods introduced.

`let a = 'my string';`

a.startsWith('my');  // true
a.endsWith('ing');  // true
a.includes('str');  // true
a.repeat(3); //  my string my string my string

### Template Literals
```
let a = 'hello';
let b =  'Hey ${a}'; // Hey hello
```
To print a variable inside a string, ${} can be used .This helps inn avoiding the usage of concatenation operator(+) and joining the variable and strings.

Multiple lines of string can be displayed using the backtick (`) , without using the back slach(/) as mentioned in the ECMAscript 5.

```
let a = `First line 
second line
third line`;

```

## Arrays
New Array methods are introduced , such as : 

### Array.from()
The Array.from() method creates a new Array instance from an array-like or iterable object.

```
console.log(Array.from('foo'));
// expected output: Array ["f", "o", "o"]

console.log(Array.from([1, 2, 3], x => x + x));
// expected output: Array [2, 4, 6]
```

### Array.of()
The Array.of() method creates a new Array instance with a variable number of arguments, regardless of number or type of the arguments.

The difference between Array.of() and the Array constructor is in the handling of integer arguments: Array.of(7) creates an array with a single element, 7, whereas Array(7) creates an empty array with a length property of 7

```
Array.of(7);       // [7] 
Array.of(1, 2, 3); // [1, 2, 3]

Array(7);          // [ , , , , , , ]
Array(1, 2, 3);    // [1, 2, 3]
```

### Array.find()
The find() method returns the value of the first element in the array that satisfies the provided testing function. Otherwise undefined is returned.

```
var array1 = [5, 12, 8, 130, 44];

var found = array1.find(function(element) {
  return element > 10;
});

console.log(found);
// expected output: 12
```

### Array.fill()
The fill() method fills all the elements of an array from a start index to an end index with a static value.

```
var array1 = [1, 2, 3, 4];

// fill with 0 from position 2 until position 4
console.log(array1.fill(0, 2, 4));
// expected output: [1, 2, 0, 0]

// fill with 5 from position 1
console.log(array1.fill(5, 1));
// expected output: [1, 5, 5, 5]

console.log(array1.fill(6));
// expected output: [6, 6, 6, 6]
```

## Math
### Math.sign() 
The Math.sign() function returns the sign of a number, indicating whether the number is positive, negative or zero.
```
console.log(Math.sign(3));
// expected output: 1

console.log(Math.sign(-3));
// expected output: -1

console.log(Math.sign(0));
// expected output: 0

console.log(Math.sign('-3'));
// expected output: -1
```

### Math.trunc()
The Math.trunc() function returns the integer part of a number by removing any fractional digits.
```
console.log(Math.trunc(13.37));
// expected output: 13

console.log(Math.trunc(42.84));
// expected output: 42

console.log(Math.trunc(0.123));
// expected output: 0

console.log(Math.trunc(-0.123));
// expected output: 0
```
### Math.cbrt()
The Math.cbrt() function returns the cube root of a number.

```
console.log(Math.cbrt(-1));
// expected output: -1

console.log(Math.cbrt(1));
// expected output: 1

console.log(Math.cbrt(Infinity));
// expected output: Infinity

console.log(Math.cbrt(64));
// expected output: 4
```

## Spread Operator
Spread syntax allows an iterable such as an array expression or string to be expanded in places where zero or more arguments (for function calls) or elements (for array literals) are expected, or an object expression to be expanded in places where zero or more key-value pairs (for object literals) are expected.

```
function sum(x, y, z) {
  return x + y + z;
}

const numbers = [1, 2, 3];

console.log(sum(...numbers));
// expected output: 6

console.log(sum.apply(null, numbers));
// expected output: 6
```
## Destructuring
The destructuring assignment syntax is a ECMAscript expression that makes it possible to unpack values from arrays, or properties from objects, into distinct variables.
```
var a, b, rest;
[a, b] = [10, 20];

console.log(a);
// expected output: 10

console.log(b);
// expected output: 20

[a, b, ...rest] = [10, 20, 30, 40, 50];

console.log(rest);
// expected output: [30,40,50]
```

## Default parameters
Default parameters  can be used in the function , for if any parameters are not passed.
```
function f(x, y=12) {
  // y is 12 if not passed (or passed as undefined)
  return x + y;
}
console.log(f(3) == 15) // true
```

## Rest parameters
The rest parameter syntax allows us to represent an indefinite number of arguments as an array.
```
function sum(...theArgs) {
  return theArgs.reduce((previous, current) => {
    return previous + current;
  });
}

console.log(sum(1, 2, 3));
// expected output: 6

console.log(sum(1, 2, 3, 4));
// expected output: 10
```

### Using spread operator in passing parameters
Values can be passed to an array using the spread operator as well.
```
function sum(a , b, c) {
    console.log(a + b + c);
}
let a = [1,2];
sum(3, ...a);   // 6
```

## Class
ES6 classes are a simple sugar over the prototype-based OO pattern. Having a single convenient declarative form makes class patterns easier to use, and encourages interoperability. Classes support prototype-based inheritance, super calls, instance and static methods and constructors.

```
class Rectangle {
  constructor(height, width) {
    this.height = height;
    this.width = width;
  }
}
```

An important difference between function declarations and class declarations is that function declarations are hoisted and class declarations are not. You first need to declare your class and then access it, otherwise code like the following will throw a ReferenceError
```
var p = new Rectangle(); // ReferenceError

class Rectangle {}
```
A class expression is another way to define a class. Class expressions can be named or unnamed. The name given to a named class expression is local to the class's body. (it can be retrieved through the class's (not an instance's) .name property, though)

```
// unnamed
var Rectangle = class {
  constructor(height, width) {
    this.height = height;
    this.width = width;
  }
};

// named
var Rectangle = class Rectangle {
  constructor(height, width) {
    this.height = height;
    this.width = width;
  }
};
```

```
class Rectangle {
  constructor(height, width) {
    this.height = height;
    this.width = width;
  }
  // Getter
  get area() {
    return this.calcArea();
  }
  // Method
  calcArea() {
    return this.height * this.width;
  }
}

const square = new Rectangle(10, 10);

console.log(square.area); // 100
```
###### The extends keyword is used in class declarations or class expressions to create a class as a child of another class.

```
class Animal { 
  constructor(name) {
    this.name = name;
  }
  
  speak() {
    console.log(this.name + ' makes a noise.');
  }
}

class Dog extends Animal {
  speak() {
    console.log(this.name + ' barks.');
  }
}

var d = new Dog('Mitzie');
d.speak(); // Mitzie barks.
```
#### super() and super keyword.
super() is used to call the constructor of the super class. It can be called inside the constructor of the subclass.

```
class mainClass {
    constructor(name) {
        this.name = name;
    }
    
    printName() {
        console.og(this.name);
    }
}

class subClass extends mainClass {
    constructor() {
        super(prompt('Enter Name'));    
        this.age = prompt('enter age');
        super.printName(); // prints the name
    }
    printDetails(){
        console.log(this.name + ' ' + this.age);
    }
}
```
super key word can be used to call the function taht belongs to the mainClass.

## Generators
Generators are special types of functions in the sense that unlike a traditional function generators produce multiple values on a per request basis while suspending their execution between these requests.
The function*and yield keywords are unique to a generator. Generators are defined by adding an * at the end of a function keyword. This enables us to use the yield keyword within the body of the generator to produce values on request.

```
function* idMaker() {
  var index = 0;
  while(true)
    yield index++;
}

var gen = idMaker();

console.log(gen.next().value); // 0
console.log(gen.next().value); // 1
console.log(gen.next().value); // 2

```
```
let name,age;

function* getDetails() {
    yield prompt('Enter Name');
    yield prompt('Enter Age');
}
let gen = getDetails();
name = gen.next().value;
age = gen.next().value;
```

## Modules 
We can import classes and functions from exported modules.
Lets consder a file : 'name.js'
```
export class name {
    constructor() {
        this.name = '';
    }
    getName() {
        this.name = prompt('enter name');
    }
}

export function printHello() {
    console.log('Hello');
}
```
Now we import class name from 'name.js'.
```
import { name } from './name';

....
....
....

```

## Unicode
Non-breaking additions to support full Unicode, including new Unicode literal form in strings and new RegExp u mode to handle code points, as well as new APIs to process strings at the 21bit code points level. These additions support building global apps in ECMAscript.

```
// same as ES5.1
"𠮷".length == 2

// new RegExp behaviour, opt-in ‘u’
"𠮷".match(/./u)[0].length == 2

// new form
"\u{20BB7}"=="𠮷"=="\uD842\uDFB7"

// new String ops
"𠮷".codePointAt(0) == 0x20BB7

// for-of iterates code points
for(var c of "𠮷") {
  console.log(c);
}
```

## Symbols 
Symbols is the new data type in ECMAscript. Symbols has a function called symbol(), which generates a unique identifier.
The Symbol() function returns a value of type symbol, has static properties that expose several members of built-in objects, has static methods that expose the global symbol registry, and resembles a built-in object class but is incomplete as a constructor because it does not support the syntax "new Symbol()".  

```
const symbol1 = Symbol();
const symbol2 = Symbol(42);
const symbol3 = Symbol('foo');

console.log(typeof symbol1);
// expected output: "symbol"

console.log(symbol3.toString());
// expected output: "Symbol(foo)"

console.log(Symbol('foo') === Symbol('foo'));
// expected output: false
```

Symbols are not visible to iterations such as Object.keys(), for...in etc and also Object.getOwnPropertyNames().
Symbols can be viewd by using , Object.getOwnPropertySymbols().
```
class User {
    constructor() {
        this.id = Symbol('id');
        this.internalDetails[this.id] = { 'token': Symbol('token')};
    }
}
```

## Proxy
Proxy can be used to act as a inter-worker or a filterer between the accessor and the target object.
lets take an example : 
```
let target = {};
var p = new Proxy(target, handler);
function handler() {
    get: function(target,key){
        if (key === 'firstKey') {
            return target[key];
        } else return false;
    },
    set : function(target, key, value, reciever) {
        if (key === 'password') {
            if (value.length > 0 && value.length < 7) {
                target[key] = value;
            }
        } target[key] = value;
    }
}   // This returns value only if the key is 'firstKey' when user tries to access a value.
/* 
When we set a value to the object , it usually set the value for certain key except for a key called password, where it will check if the length of the value being set is greater than 0 and also less than 7.If the condition is true then it works or else it will not be set.
*/
```

## Map
The Map object holds key-value pairs. Any value (both objects and primitive values) may be used as either a key or a value.
```
var myMap = new Map();

var keyString = 'a string',
    keyObj = {},
    keyFunc = function() {};

// setting the values
myMap.set(keyString, "value associated with 'a string'");
myMap.set(keyObj, 'value associated with keyObj');
myMap.set(keyFunc, 'value associated with keyFunc');

myMap.size; // 3

// getting the values
myMap.get(keyString);    // "value associated with 'a string'"
myMap.get(keyObj);       // "value associated with keyObj"
myMap.get(keyFunc);      // "value associated with keyFunc"

myMap.get('a string');   // "value associated with 'a string'"
                         // because keyString === 'a string'
myMap.get({});           // undefined, because keyObj !== {}
myMap.get(function() {}) // undefined, because keyFunc !== function () {}
```

## WeakMap
The WeakMap object is a collection of key/value pairs in which the keys are weakly referenced.  The keys must be objects and the values can be arbitrary values.

```
var wm1 = new WeakMap(),
    wm2 = new WeakMap(),
    wm3 = new WeakMap();
var o1 = {},
    o2 = function() {},
    o3 = window;

wm1.set(o1, 37);
wm1.set(o2, 'azerty');
wm2.set(o1, o2); // a value can be anything, including an object or a function
wm2.set(o3, undefined);
wm2.set(wm1, wm2); // keys and values can be any objects. Even WeakMaps!

wm1.get(o2); // "azerty"
wm2.get(o2); // undefined, because there is no key for o2 on wm2
wm2.get(o3); // undefined, because that is the set value

wm1.has(o2); // true
wm2.has(o2); // false
wm2.has(o3); // true (even if the value itself is 'undefined')

wm3.set(o1, 37);
wm3.get(o1); // 37

wm1.has(o1); // true
wm1.delete(o1);
wm1.has(o1); // false
```

## Set 
The Set object lets you store unique values of any type, whether primitive values or object references.
```
var mySet = new Set();

mySet.add(1); // Set [ 1 ]
mySet.add(5); // Set [ 1, 5 ]
mySet.add(5); // Set [ 1, 5 ]
mySet.add('some text'); // Set [ 1, 5, 'some text' ]
var o = {a: 1, b: 2};
mySet.add(o);

mySet.add({a: 1, b: 2}); // o is referencing a different object so this is okay

mySet.has(1); // true
mySet.has(3); // false, 3 has not been added to the set
mySet.has(5);              // true
mySet.has(Math.sqrt(25));  // true
mySet.has('Some Text'.toLowerCase()); // true
mySet.has(o); // true

mySet.size; // 5

mySet.delete(5); // removes 5 from the set
mySet.has(5);    // false, 5 has been removed

mySet.size; // 4, we just removed one value
console.log(mySet);// Set [ 1, "some text", Object {a: 1, b: 2}, Object {a: 1, b: 2} ]
```

## WeakSet
WeakSet objects are collections of objects. An object in the WeakSet may only occur once; it is unique in the WeakSet's collection.

The main differences to the Set object are:

* In contrast to Sets, WeakSets are collections of objects only and not of arbitrary values of any type.
* The WeakSet is weak: References to objects in the collection are held weakly. If there is no other reference to an object stored in the WeakSet, they can be garbage collected. That also means that there is no list of current objects stored in the collection. WeakSets are not enumerable.

```
var ws = new WeakSet();
var obj = {};
var foo = {};

ws.add(window);
ws.add(obj);

ws.has(window); // true
ws.has(foo);    // false, foo has not been added to the set

ws.delete(window); // removes window from the set
ws.has(window);    // false, window has been removed
```

# References : 
*  https://www.ecma-international.org/publications/standards/Ecma-262-arch.htm
*  https://codeburst.io/generators-in-ECMAscript-1a7f9f884439
*  http://www.benmvp.com/learning-es6-history-of-ecmascript/
*  https://github.com/lukehoban/es6features#subclassable-built-ins
*  http://speakingjs.com/
*  https://developer.mozilla.org/en-US/
*  http://2ality.com
*  www.w3schools.com
*  https://ponyfoo.com/articles/
*  https://codeburst.io/
