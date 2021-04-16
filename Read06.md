# Code 201 Reading Notes

## Problem Domain, Objects, and the DOM

### What is an object?
- Objects group together a set of variables and functions to create a model of something you would recognize  from the real world. 

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

### ***Document Object Model***
- The DOM tree is a model of a webpage. As a browser loads a web page, it creates a model of that page. 

### Working with the DOM Tree
- There are two steps with accessing and updating the DOM tree. 
1. Locate the node that represents the element you want to work with.
2. Use its text content, child elements, and attributes. 

Step 1: 
- Select an individual element node
- Select multiple elements
- Traversing between element nodes

Step 2: 
- Access/update text nodes
- Work with HTML content
- Access or update attribute values

### Caching DOM queries
- Methods that  find element in the DOM tree are calls DOM queries. 

### Accessing Elements
- DOM queries may return one element, or they may return a Nodelist, which is a collection of nodes. 

Methods that return a single element node
- getElementbyId
- querySelector

Methods that return one or more elements
- getElementsByClassName
- getElementsByTagName
- querySelectorAll

### NODELISTS: DOM Quries that return more than one element

Examples:
- getElementsByTagName('h1')
- getElementsbyClassName ('hot')
- querySelectorAll('li[id]')

### Looping Through A Nodelist
- When you start to use the same code over and over again, creating a loop to loop through a NodeList is a powerful technique.

### Traversing the DOM
- When you have an element node, you can select another element in relation to t using these five properties.

1. parentNode
2. previousSibling
3. nextSibling
4. firstChild
5. lastChild

- Traversing the DOM can be difficult because some browsers add a test node whenever they come across whitespace between elements.

### How to get/update element content 
- So far in this chapter has focus on finding elements in the DOM tree. The remainder of the chapter shows how to access/update element content. 


### Example of working with the DOM: 
1. Create a table body in HTML
var table = document.getElementById('table-body');

2. Creating a function to make a table head
function renderTableHead() {
  var tableHead = document.createElement('thead');
  table.appendChild(tableHead);// Table Body

  // Variable to start creation of table
  var openHours = ['6am', '7am', '8am', '9am', '10am', '11am', '12pm', '1pm', '2pm', '3pm', '4pm', '5pm', '6pm', '7pm', 'Totals'];
  var tableStart = document.createElement('th');
  tableStart.textContent = '';

  tableHead.appendChild(tableStart);
  for (var a = 0; a < openHours.length; a++) {
    var tableStart = document.createElement('th');
    tableStart.textContent = openHours[a];
    tableHead.appendChild(tableStart);
  }
}

3. Using a contstructor function to generate a set of stores, hours, the maximun, minimum, average, and total number of customers. 
// Constructor Function for Table and Rand Names
function Stores(store, minCust, maxCust, avgCookieSales) {
  this.name = store;
  this.minCust = minCust;
  this.maxCust = maxCust;
  this.avgCookieSales = avgCookieSales;
  this.totalcookiesPerday = 0
  this.array = [];
  storeLocations.push(this);
}

4. Creating two Arrays for the function to loop through. 
var openHours = ['6am', '7am', '8am', '9am', '10am', '11am', '12pm', '1pm', '2pm', '3pm', '4pm', '5pm', '6pm', '7pm', 'Totals'];
var storeLocations = [];

5. Creating the random set of numbers for customers per hour, total of all the stores per hour, and the total for end of day. 
// Function Prototype for Random
Stores.prototype.numOfcustomers = function () {
  // var totalcookiesPerday = 0;
  for (var i = 0; i < openHours.length - 1; i++) {
    var cookieshour = Math.floor((Math.random() * (this.maxCust - this.minCust + 1) + this.minCust) * this.avgCookieSales);
    this.totalcookiesPerday += cookieshour;
    this.array.push(cookieshour);
  }
  this.array.push(this.totalcookiesPerday);
}

6. Printing the values to a set of tables. 
// Print Table 
Stores.prototype.printTable = function () {
  this.numOfcustomers();
  var row = document.createElement('tr');
  var nameCell = document.createElement('td');
  table.appendChild(row);
  nameCell.textContent = this.name;
  row.append(nameCell);

  for (var i = 0; i < openHours.length; i++) {
    var dataCell = document.createElement('td');
    dataCell.textContent = this.array[i];
    row.appendChild(dataCell);
  }
}
// Declaring Functions and printing to the tables
var Seattle = new Stores('Seattle', 23, 65, 6.3);
var Tokyo = new Stores('Tokyo', 3, 24, 1.2);
var Dubai = new Stores('Dubai', 11, 38, 3.7);
var Paris = new Stores('Paris', 20, 38, 2.3);
var Lima = new Stores('Lima', 2, 16, 4.6);

7. Making the table come to life
function renderTable() {
  renderTableHead();
  for (var i = 0; i < storeLocations.length; i++) {
    storeLocations[i].printTable();
  }
  hourTotals();
}

console.log(Seattle.array);
console.log(Tokyo.array);
console.log(Dubai.array);
console.log(Paris.array);
console.log(Lima.array);
// var storeLocations = [Seattle, Tokyo, Dubai, Paris, Lima];

8. Using a function to create a table within HTML
function hourTotals() {
  var dayTot = 0
  // First cell is to have totals 
  var tablefoot = document.createElement('tfoot');
  var tablerow = document.createElement('tr');
  var tablehead = document.createElement('th');
  tablehead.textContent = 'Totals:';
  tablerow.appendChild(tablehead);
  tablefoot.appendChild(tablerow);

  for (var i = 0; i < openHours.length - 1; i++) {
    console.log(dayTot);
    var hourTot = 0
    for (var j = 0; j < storeLocations.length; j++) {
      // console.log(storeLocations);
      hourTot += storeLocations[j].array[i]
    }
    console.log(hourTot);
    var tabledata = document.createElement('td');
    tabledata.textContent = hourTot;
    tablerow.appendChild(tabledata);
    // were the hour append will live 
    // tablefoot.appendChild(hourTotals);
    dayTot += hourTot;
  }
  // daily total number to append
  var tabledata = document.createElement('td');
  tabledata.textContent = dayTot;
  tablerow.appendChild(tabledata);
  table.appendChild(tablefoot);
}
renderTable();

### Table of Contents
- [Read 01 Introductions to HTML and JavaScript](Read01.md)
- [Read 02 HTML CSS Javascript The Introduction](Read02.md)
- [Read 03 HTML List CSS Boxes JS Control Flow](Read03.md)
- [Read 04 HTML Links CSS Layout JS Functions](Read04.md)
- [Read 05 HTML Images CSS Color & Text](Read05.md)
- [Read 07 HTML Tables JS Constructor Functions](Read07.md)
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

### Link to Code 301
- [Reading Notes 301](jtaisey389.github.io/reading-notes301.md/)

### Link to Code 401
- [Reading Notes 401](jtaisey389.github.io/401_readingnotes.md/)

[<== Back_to_reading_notes](jtaisey389.github.io/reading-notes201.md/)
