# Code 201 Reading Notes
## Forms and JS Events 

### ***Forms***
What we will cover in this section:
1. How to collect information from visitors
2. Different kinds of  form controls 
3. New HTML5 form controls

- Traditionally the form has refered to a printed document that contains space for your to fill in information. 

### Form Controls
Examples: Text Input, Password Input, Text Area

- Making choices: Buttons, Check boxes, Drop-down boxes

- Submitting forms: Subscribe, Image Buttons, Uploading files

### How forms work
1. A user fills in a form and then presses a button to submit information to the server
2. The Name of each from control is sent to the server along with the values 
3. The server processes the information using a programing language such as PHP, C#, VB.net, or Java
4. The server creates a new page to send back to the browser based on the information received

### Form Structure
Examples: `<form></form>` Form controls live inside the form element. The element should always carry an action attribute and will usually have a method and id attribute too. 

### Text Input
Examples: `<input></input> The input element is used to create several different form controls. The value of the type=text attribute determines what kind of input you will be creating. With inputs there are three key peices of code you will need. The name, the size and the maxlength, the maxlength will control the number of charecters a user may enter in the feild.

### Password Input
Example: When the type attribute has a value of password it created a text box that acts just like a single line text input, except the charecters are blocked out. As mentioned earlier the name attribute indicated the name of the password input, secondly it can also cary the size or the maxlenght attribute.

### Text Area
-Example: `<textarea></textarea>` The textarea element is used to create a multi-line text input. Unlike other inpout elements this is not an empty element. It should not have an opening and closing tag.

### Buttons
Example: A button is a type of input and allows the user to pick just one of a number of options. Within the button you will have a name to set the value for the options, the value which is sent to the server, and finally checked which is used to indicate which value is to be selected.

Note: Once a button has been selected it cannot be deslected. The user can only select a different option. 

### Checkbox
Example: Similar to the button the checkbox allows users to select and unselect more than option. 

### Drop Down List Box
- Drop down list boxs also known as slect box allows users to select one option from a drop down list. The function of a drop down list box is similar to that of the radio button.

### Multiple Select Box
- With multiple select boxes you can set up the box to select different options. Its values should be the nubmer of options you want to show at once.

### File input box
- If you want to allow users to upload a file (for example and image, video, mp3, or pdf). With file input you need to have a type="file" followed by a browse botton. The browse button opens a window that allows the user to select a file from their computer. 

### Submit Button
- The submit button is used to send a form to the server. With the submit button you can use a name attribute to give your sumbit button a name. The value attribute is used to control the text that appears on a button. 

### Image Button
- If you want to use an image for the submit button, you can give the type attribute a value image. This is done with a type="image".

### Button & Hidden Controls
- The `<button>` element was introducted to allow users more control over how their buttons appear. To create a hidden form control with type="hidden". This allows a web page author to add values to forms that user cannot see.

### Labelling Form Controls
- When introducing form controls, the code was kept simple by indicating the pourpose of each one in  text next to it. The "for" attributes states which form control the label belongs to. 

### Grouping Form Elements
- You can group relates form controls together inside the `<feildset>` element. The `<legend>` element can come directly after the opening `<feildset>`. 

### Form Validation
- You have probably seen forms on the web that give users messages. This is known as form validation. 

### Date input
- With HTML5 you have the option for the user to put in a date. You would do a `<input type="date">`. 

### Other inputs with HTML 5
- You can set up a `<input type="email>` for the user to input their email into a text box.
-You also can set up `<input type="url">`, this gives the functionality to ask the user for their webpage.

### ***Lists, Tables and Forms***
What we will cover in this section:
1. Specifying bullet point styles
2. Adding borders and backgrounds to tables
3. Changing the appearance of form elements

### Bullet Point Styles 
Examples: Unordered Lists: None, Disc, Circle, Square

Examples: Ordered Lists:

Decimal - 1 2 3
Decimal-leading Zero - 01 02 03
lower-alpha - abcde
upper-alpha - ABCDE
lower-roman - i. ii. ii.
upper-roman = I II II

With bullet point styles you can also use an image to act as a bullt point using list-style-image property.

### Positioning the marker
- Lists are indented into the page by default and the list-style-position indicates whether the marker should appear on the inside or the outside of the box containing the main points. You specify the location by calling outside or inside. This list for example is sitting inside of the marker. 

### Table Properties
Width - to set the width of a table
Padding - Sets the space between the border of each table cell and its content
Text-transform - Converts the content of the table headers to uppercase
Letter-Spacing, Font-Size - Adds additional styling to the content of the table headers
Border-top, border-bottom - Sets the borders above and bellow the table headers
Text-Align - To align the wirting to theleft of some table caells and to the right of others
Background-color - Changes the background color of the alternating table rows
:Hover - Highlights a table row when a user's mouse goes over it. 

- With table properties you should add some styling to ensure they are clean and easy to follow.
1. Give Ceels Padding
2. Distinguish Headings
3. Shade ALternate rows
4. Align Numerals
5. Online Extra

### Border on Empty Cells 
- If you have empty cells in your table, then you can use the empty-cells property to specifiy whether or not their borders should be shown.

Example: Show will show the borders of any empty cells

Example: Hide will hide the borders of any empty cells

Example: Inherit. If you have one table nested inside of another, the inherit value instructs the table cells to obey the ruls of the containing table. 

### ***Events***
- When you browse the web, your browser registers different types of events. This is your way of the browsers saying, "Hey, this just happened".

UI Events: Load, Unload, Erroe, Resize, Scroll

Keyboard Events: Keydown, Keyup, Keypress

Mouse Events: Click, dbClick, mousedown, mouseup, mousemove, mouseover, mouseout

Event: Focus/Focusin, blur/focusout

Form Event: Input, Change, Submit, Reset, Cut, Copy, Paste, Select

### How Events Trigger Javascript
- When the user interacts with the HTML on a webpage, there are three steps involved in getting it to trigger some JavaScript code. 
1. Select the element
2. Indicate which event will trigger response
3. State the code you want to run

### There are three ways to bind an element
1. HTML Handler Events (no longer used)
2. Traditional DOM event handlers
3. DOM lvel 2 event listeners

### Event Listeners
- Event listeners are a more recent approash to handling events. They can deal with more than one function at a time, but they are not supported in older browsers.

### Event Flow
- HTLM Elements nest inside of other elements. If you hover or click on a link, you will also be hovering or clicking on its parent element.

- Why flow matters: Flows of events only really matters when your code has event handlers on an element and one of its ancestors or decendant elements. 

### The event object
- When an event occcirs, the event object tells you information about the event, and the element it happened upon.

### Different types of Events
1. W3C Dom events, which looks after other specifications including, HTML, CSS and XML.
2. HTML 5 Events
3. BOM Events

### User Interface Events
- UI events occur as a result of interaction with the browser window rather than the HTML page contained within it. 

### Table of Contents
- [Read 01 Introductions to HTML and JavaScript](Read01.md)
- [Read 02 HTML CSS Javascript The Introduction](Read02.md)
- [Read 03 HTML List CSS Boxes JS Control Flow](Read03.md)
- [Read 04 HTML Links CSS Layout JS Functions](Read04.md)
- [Read 05 HTML Images CSS Color & Text](Read05.md)
- [Read 06 JS Object Literals And The DOM](Read06.md)
- [Read 07 HTML Tables JS Constructor Functions](Read07.md)
- [Read 08 Expanding CSS Layout](Read08.md)
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
