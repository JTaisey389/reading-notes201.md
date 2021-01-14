# Code 201 Reading Notes

## Read 04 Notes & Informatiom

### ***Links***
What we will cover in this section:
 1. Creating links between pages
 2. Linking to other sites
 3. Email links

Links are the future of the web. They allow a user to move from one web page to another, this enables the very idea of browsing or surfing.

### Writing Links
- A link is created using the `<a>` element. Users can click on anything between the opening tag and the closing tag. The great part about a link is you can specify which page you want by using the href attribute.

Example: `<a href="https://www.youtube.com/">Youtube</a>`

### Linking to other sites
- Building upon the ability to create a link, the user can link to other sites also using the `<a>` element. This element has an attribute called href, href allows you to call a value. This value is the page that you want people to go to when they click on the link. 

Example:

`<p>Movie Reviews</p>`
 `<ul>`
 `<li><a href="https://www.rottentomatoes.com/">Rotten Tomatoes</a></li>`
 `</ul>`
`</p>`


### Linking to other pages within the same site
- As you create your web page you will likely have multiple pages on the same site. For this link, you would just need a relative URL to the other page on your website.

Example: 

`<p>`
 `<ul>`
 `<li><a href="index.html">Home</a></li>`
 `</ul>`
`</p>`

### Directory Structure
- With larger webpages, it is a good idea to organize your code by placing the pages for each different section of the site into a new folder. Folders on a website are sometimes referred to as directories.

 1. Structure: The top-level folder is known as the root folder. The root folder contains all of the other files and folders for a website. 
 2. Relationships: The relationship between files and folders on a website is described using the same terminology as a family tree. This starts with Grandparent, Parent, Child and finally Grandchild
 3. Homepages: The main homepage of a website written in HTML and each of the sections in a child folder are called *index.html.*

### Realative URLS
- A relative URL can be used when linking to pages within your website. They are a shorthand way of telling the browser where to find your files. 

### Email links
- Email links that start up the user's email program and address and email to a specified email address. This is a `mailto:` link that uses the `<a>` element. 

Example:
`<a href ="mailto:jdtaisey89@icloud.com">Email Jason</a>`

### Opening a new link to a new window
- To have a link open a new browser window you would use a target attribute.

Example: 
`<a href="https://www.imdb.com/" target="_blank">IMDB</a>`

### Linking to a specific part of the same page
- Linking to a specific part of the same page is a simple way to ass a list of content. When you have a long webpage this helps the user avoid having to constantly scroll to find information.

Example:
`<a href="arc_shot>Arc Shot</a><br />`

- This linking can also be used to go to a specific part of another page.

### ***Layout***
What we will cover in this section:
 1. Controlling the position of elements
 2. Creating site layouts
 3. Designing for different sized screens

### Concepts in positioning elements
- CSS treats each part of HTML as an element. These elements are essentially contained in a box that displays information.

Example:
Block-level elements start on a new line, while inline elements flow between surrounding text.

When one block-level element sits inside another block-level, the outer box is known as the containing or parent element.

### Controlling elements positions
- Within CSS there are positioning schemes that allow you to control the layout of a page. 

Examples:

Normal Flow - Each block-level element appears on a new line, causing each item to appear lower down on the page than the previous one. 

Relative Positioning - This will move the element from the position it would be in normal flow. This shift text to the top, right, bottom, or left of where it would have been placed.

Fixed Positioning - This is a form of absolute positioning that positions the element about the browser window. 

Floating elements - Floating an element allows you to take that element out of the normal flow and position it into the far left or right of a containing box.

### Positions
- With normal flow, each block-level elements sit on top of the next one. This would appear as a normal body of text within the normal flow. What positions ultimately do is change where the text is displayed within your viewport.

Position - Static: 

`body {`
 `width: 400px;` 
 `font-family: Arial, Verdana, sans-serif;`
 `color: #665544;}`
`h1 {`
 `background-color: #efefef;`
 `padding: 10px;}`
`p {`
 `width: 450px;}`

Position - Relative: Relative positioning moves an element in relation to where it would have been in normal flow.

`p.example {`
 `position: relative;`
 `top: 10px;`
 `left: 100px;}`

Position - Absolute: Absolute position takes the box out of the normal flow and no longer affects the position of other elements on the page.

`h1 {`
 `position: absolute ;`
 `top: 0px;`
 `left: 500px;`
 `width: 250px;}`
`p {`
 `width: 450px;}`

Position - Fixed: Fizex positioning is a type of absolute positioning that requires the position property to have a value of fixed.

`h1 {`
 `position: fixed ;`
 `top: 0px;`
 `left: 500px;`
 `padding: 10px;`
 `margin: 0px;`
 `width: 100%;}`
 `background-color: #efefef;}`
`p.example {`
 `margin-top: 100px;}`

### Elements
- Elements are usually made up of two tags. An opening `<` and a closing tag `>`.

Z-Index: As you use relative, fixed, or absolute positioning, boxes can overlap. If your boxes do overlap, the elements that appear later in the HTML code sit on top. 

`h1 {`
 `position: fixed ;`
 `top: 0px;`
 `left: 0px;`
 `padding: 10px;`
 `margin: 0px;`
 `width: 100%;}`
 `background-color: #efefef;`
 `z-index: 10;}`
`p {`
 `position: relative;`
 `top: 70px;`
 `left: 70px;}`

Float: A float property allows you to take an element in normal flow and place it as far to the left or right of the containing element as possible.

`blockqoute {`
 `float: right;`
 `width: 275px;`
 `font-size: 130%;`
 `font-style: italic;`
 `font-family: Georiga, Times, Serif; `
 `margin: 0px 0px 10 px 10px;`
 `padding: 10px;`
 `border-top: 1px solid #66ff44;`
 `border-bottom: 1px solid #665544;}`

Using float to place elements side-by-side. A lot of layouts place boxes next to each other. A floating element is commonly used to achieve this. 

Example:

`body {`
 `width: 750px;`
 `font-family: Arial, Verdana, sans-serif;`
 `color: #665544;}`
`p {
 `width: 230px;`
 `float: left;`
 `margin: 5px;`
 `padding: 5px`
 `background-color: #efefef;}`

The clear property allows you to say that no element within the same containing element should touch the left or right-hand sides of a box.

`body {`
 `width: 750px;`
 `font-family: Arial, Verdana, sans-serif;`
 `color: #665544;}`
`p {
 `width: 230px;`
 `float: left;`
 `margin: 5px;`
 `padding: 5px`
 `background-color: #efefef;}`
 `.clear {`
 `clear: left;}`
 
Types of clearing floats: Left, Right, Both, and none

### ***Functions Methods & Objects***
- Functions & Methods: Functions consist of a series of statements that have been grouped because they perform a specific task. 
- Objects: In chapter one, you say that programmers use objects to create models of the world using data and that objects are made up of properties and methods.
- Built-in objects: The browser comes with a set of objects that act as a toolkit for creating interactive web pages.

### What is a function?
- Functions let you group a series of statements to perform a specific task. If different parts of a script repeat the same task, you can reuse the function.

Example: A basic function

`var msg = 'Sign up to receive our newsletter for 10% off!';`
`function updateMessage () {`
 `var el = document.getElementById('message');`
 `el.textContent =msg;`
`}`
`updateMessage();`


### Table of Contents
- [Read 01 Introductions to HTML and JavaScript](Read01.md)
- [Read 02 HTML CSS Javascript The Introduction](Read02.md)
- [Read 03 HTML List CSS Boxes JS Control Flow](Read03.md)
- [Read 05 HTML Images CSS Color & Text](Read05.md)
- [Read 06 JS Object Literals And The DOM](Read06.md)
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

### <== Back to Code 201 Reading Notes
- [Reading Notes 201](https://jtaisey389.github.io/reading-notes201.md/)
