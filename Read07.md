# Code 201 Reading Notes
## Read 07
### ***Tables***
What we will cover in this section:
1. How to create tables
2. What information suits tables 
3. How to represent complex data in tables

## What is a table?
- A table represents information in a grid format. Examples include financial reports, TV Schedules, and sports results.

## Basic table structure
Example: 

`<table></table> is ues to create the table`
`<tr></tr> Is used to indicate the start of each row.`
`<td></td> Each of the cells is represented by the td`
`<th></th> Within rows you can have a table heading`

### Spanning Colums & Rows
- With columns, you may need to stretch entries in a table across more than one column. Additionally, you may also need to span a row with your entry. 

### Long Tables 
- Some elements help distinguish between the main content of the table. These elements help people who use screen readers and allow you to style these selections. 
Example:

`<thead></thead> The heading of a table:`
`<tbody></tbody> The body which sits inside the tbody`
`<tfoot></tfoot> The footer for your table

### Creating an Object
- You create a new object using a combination of the new keyword and the object () constructor function. After that created you can add properties and methods to it using dot notation.

`var hotel = new Object();`
`hotel .name = 'Quay';`
`hotel .rooms = 40;`
`hotel .booked = 25;`

`hotel.checkAvailability = function() {`
 `return this.rooms - this.booked;`
`};`

### Updating an Object
- To update a property, use the same technique that was shown above. 

`hotel.name = 'Park';` Update to new
`hotel['name'] = 'Park'; `

### Creating Many Objects
- A function called hotel will be used as a template. The function has three parameters. 

Example: 

`function Hotel(name, rooms, booked) {`
 `this.name = name;`
 `this.room = rooms;`
 `this.booked = booked;`

 `this.checkAvailability = function (){`
 `return this.rooms - this.booked;`
 `};`
`}`

### Recap: Ways to create objects
Literal Notations:

`var hotel = {}`

`hotel.name = 'Quay';`
`hotel.rooms = 40;`
`hotel.booked = 25;`
`hotel.checkAvailability = function () {`
 `return this.rooms - this.booked;`
`};`

Object Constructor Notation

`var hotel = new Object();`
`hotel.name = 'Quay';`
`hotel.rooms = 40;`
`hotel.booked = 25;`
`hotel.checkAvailability = function () {`
 `return this.rooms - this.booked;`
`};`

Literal Notation

`var hotel = {`
 `name = 'Quay',`
 `rooms = 40,`
 `booked = 25,`
 `checkAvailability: function () {`
 `return this.rooms - this.booked;`
 `}`
`};`

Object Constructor Notation

`function Hotel (name, rooms, booked){`
 `this.name = name;`
 `this.room = rooms;`
 `this.booked = booked;`

 `this.checkAvailability = function (){`
 `return this.rooms - this.booked;`
 `};`
`}`
`var quayHotel = new Hotel('Quay', 40, 25);`
`var parkHotel = new Hotel('Park', 120, 77);`

### This is a keyword
- The keyword "this" is frequently used inside of functions and objects. Where the function is declared alters what "this" means.

- A function in global scope: When a function is created at the top level of a script then it is in the global scope or global content. 
- Global Variables: All global variables become properties of the window object.
- A method of an object: When a function is defined inside an object, it becomes a method.
- Function expression as a method
- If a named function has been refined in the global scope, and it is then used as a method of an object, this refers to the object it is contained with.

### ***Recap***
- Variables: A variable has just one key and one value.

- Arrays: Arrays can store multiple pieces of information. Each piece of information is separated by a comma.

- Individual objects: Objects store sets of name/value pairs. They can be properties (variables) or methods (functions).

- Multiple Objects: When you need to create multiple objects on the same page, you should use an object constructor to provide a template for the objects.

### Arrays are objects
- Arrays are a special type of object. They hold a related set of key/value pairs. The key value for each is its index number. 

- You can combine arrays and objects to create a complete data structure: Arrays can store a series of objects and remember their order. 

### What are built-in Objects?
1. The browser object model: This contains the objects in the current browser window or tab. 

2. Document Object Model: The DOM uses an object to create a representation of the current page.

3. Global JavaScript Objects: The global JavaScript objects represent things that the JavaScript language needs to create a model of.

### The Window Object
- window.innerHeight
- window.innerWidth
- window.pageXOffset
- window.pageYOffset
- window.screenX
- window.screenY
- window.location
- window.document
- window.history
- window.history.length
- window.screen
- window.screen.width
- window.screen.height
- window.alert()
- window.open()
- window.print()

### The Document Object Model
- document.title
- document.lastModified
- document.URL
- document.domain
- document.write()
- document.getElementById()
- document.querySelectorAll()
- document.createdElement()
- document.createTextNode()

### String Objects
- length: Returns number of characters in the string in most cases
- toUpperCase(): Changes string to uppercase charecters
- toLowerCase(): Changes string lowercase characters
- chart(): Takes an index number as a parameter, and returns the character found at that position
- indexOf(): Returns index number of the first time a character or set of characters is found within the string
- lastIndexOf(): Returns index number of the last time a character or set of characters is found within the string
- substring(): Returns characters found between two index numbers. The first index number is included and the character for the last index number is not included. 
- split (): When a character is specified, it splits the string each time it is found. 
- trim (): Removes white space from start and end of a string
- replace(): Like find and replace, it takes one value that should be found, and another to replace it

Continued:
- saying.length; Home Sweet Home, Result "16"
- saying.toUpperCase(); Home Sweet Home, Result "HOME SWEET HOME"
- saying.toLowerCase(); Home Sweet Home, Result "home sweet home"
- saying.chartAt(12)); Home Sweet Home, Result "o"
- saying.indexOf('e,e'); Home Sweet Home, Result "7"
- saying.lastIndexOf('e'); Home Sweet Home, Result "14"
- saying.substring (8,14); Home Sweet Home, Result "et home"
- saying.split('')); Home Sweet Home, Result ['Home', 'Sweet', 'home', '']
- saying.trim(); Home Sweet Home, Result 'Home sweet home'
- saying.replace('me', 'w'); Home Sweet Home, Result 'How sweet home'

### Data Types Revisited
1. String
2. Number
3. Boolean
4. Undefined
5. Null
6. Object

### Number Objects
- isNaN() Checks the values to see if it is not a number
- toFixed() Rounds to specified number of decimal places(returns a string)
- toPrecision() Rounds to total number of places (returns a string)
- toExponential () Returns a string representing the number in exponential notation

### Math Objects
- Math.PI Returns PI
- Math.round ()Rounds number to the nearest integer
- Math.sqrt(n) Returns the square root of a positive number
- Math.ceil () Rounds number up to the nearest integer
- Math.floor () Rounds number down to the nearest integer
- Math. random() Generates a random number between 0 and 1

### Date Object & Time
- getDate()
- getDay()
- getFullYear()
- getHours()
- getMilliseconds()
- getMinutes()
- getMonth()
- getSeconds()
- getTime()
- getTimeZoneOffset()
- toDateString()
- totimeString()
- toString()

### Table of Contents
- [Read 01 Introductions to HTML and JavaScript](Read01.md)
- [Read 02 HTML CSS Javascript The Introduction](Read02.md)
- [Read 03 HTML List CSS Boxes JS Control Flow](Read03.md)
- [Read 04 HTML Links CSS Layout JS Functions](Read04.md)
- [Read 05 HTML Images CSS Color & Text](Read05.md)
- [Read 06 JS Object Literals And The DOM](Read06.md)
- [Read 08 Expanding CSS Layout](Read08.md)
- [Read 09 Forms & Events](Read09.md)
- [Read 10 Debugging JavaScript](Read10.md)
- [Read 11 Assorted Topics](Read11.md)
- [Read 12 Documents for HTML Canvas Element & Chart JS](Read12.md)
- [Read 13 Local Storage](Read13.md)
- [Read 14a CSS Transforms Transitions and Animations](Read14A.md)
- [Read 14b What Google Learned About Teams](Read14A.md)


### Link to Code 102
- [Code 102 Reading Notes](https://jtaisey389.github.io/reading-notes/)

### <== Back to Code 201 Reading Notes
- [Reading Notes 201](https://jtaisey389.github.io/reading-notes201.md/)
