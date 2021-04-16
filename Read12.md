# Code 201 Reading Notes

## Charts and Canvas

### Easily Create Stunning Animated Charts 
- Charts are far better for displaying visually than tables and have the added benefit that no one is going to press-gang them into yse as a layout tool. A great way to get started with charts is with Chart.js a JavaScript plugin that uses HTML5's canvas element to draw the graph onto the page. 

### Setting it up
- First step is to download Chart.js. Copy the Chart.min.js out of the unzipped folder and into the directory you'll be working on. Then create a new html page and import the script.

HTML for the page 
`<!DOCTYPE html>`
`<html lang="en">`
    `<head>`
        `<meta charset="utf-8" />`
        `<title>Chart.js demo</title>`
        `<script src='Chart.min.js'>`

### Drawing a line chart
- To create a line chart, the first thing we need to do is create a canvas element in our HTML in which Chart.js can draw our chart. So we add this to the body of our HTML page.

`<canvas id="buyers" width="600" height="400"></canvas>`

- Moving on we write the script that will retreive the context of the canvas, so add this to the foot of your body element.

`<script>`
    `var buyers = document.getElementById('buyers').getContext('2d');`
    `new Chart(buyers).Line(buyerData);`


- Within the scrtip we needto create our data, in this instance it's an object that contains labels for the base of our chart and datasets. 

`var buyerData = {`
	`labels : ["January","February","March","April","May","June"],`
	`datasets : [`
		`{`
			`fillColor : "rgba(172,194,132,0.4)",`
			`strokeColor : "#ACC26D",`
			`pointColor : "#fff",`
			`pointStrokeColor : "#9DB86D",`
			`data : [203,156,99,251,305,247]`
		`}`
	`]`
`}`

- Finally we put it to the test by running it in our browser.

### Drawing a Pie Chart
- In similar fashion to a line chart you provide the data to be displayed. With a pie chart you supply some options to the chart. 

`<canvas id="countries" width="600" height="400"></canvas>`

- Next we input the Javascript data

`var countries= document.getElementById("countries").getContext("2d");`
`new Chart(countries).Pie(pieData, pieOptions);`

`var pieData = [`
	`{`
		`value: 20,`
		`color:"#878BB6"`
	`},`
	`{`
		`value : 40,`
		`color : "#4ACAB4"`
	`},`
	`{`
		`value : 10,`
		`color : "#FF8153"`
	`},`
	`{`
		`value : 30,`
		`color : "#FFEA88"`
	`}`
`];`

`var pieOptions = {`
	`segmentShowStroke : false,`
	`animateScale : true`
`}`

- Now we have ourselves a pie chart to display data

### Bar Chart
- Create the bar chart

`<canvas id="income" width="600" height="400"></canvas>`

`var income = document.getElementById("income").getContext("2d");`
`new Chart(income).Bar(barData);`

`var barData = {`
	`labels : ["January","February","March","April","May","June"],`
	`datasets : [`
		`{`
			`fillColor : "#48A497",`
			`strokeColor : "#48A4D1",`
			`data : [456,479,324,569,702,600]`
		`},`
		`{`
			`fillColor : "rgba(73,188,170,0.4)",`
			`strokeColor : "rgba(72,174,209,0.4)",`
			`data : [364,504,605,400,345,320]`
		`}`

	`]`
`}`

### Table of Contents
- [Read 01 Introductions to HTML and JavaScript](Read01.md)
- [Read 02 HTML CSS Javascript The Introduction](Read02.md)
- [Read 03 HTML List CSS Boxes JS Control Flow](Read03.md)
- [Read 04 HTML Links CSS Layout JS Functions](Read04.md)
- [Read 05 HTML Images CSS Color & Text](Read05.md)
- [Read 06 JS Object Literals And The DOM](Read06.md)
- [Read 07 HTML Tables JS Constructor Functions](Read07.md)
- [Read 08 Expanding CSS Layout](Read08.md)
- [Read 09 Forms & Events](Read09.md)
- [Read 10 Debugging JavaScript](Read10.md)
- [Read 11 Assorted Topics](Read11.md)
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
