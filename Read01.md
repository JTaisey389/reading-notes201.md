# Code 201 Reading Notes
## Read 01 Notes & Information

### The Front End:
- The front end consists of HTML + CSS + JS
 - HTML is the content and the structure of the website. 
 - CSS is the presentation of the website
 - Java Script is the interaction 

### ***HTML Basics***
Q: What is HTML and what does it do?
A: HTML is the framework for all webpages and stores information within the content of the website.HTML is displayed very similar to a newspaper, for each story within a newspaper, you have a headline, some text, and occasionally an image. 

Within HTML we have a structure of the webpage that helps the user navigate through. Typically you have a heading, subheading, and so on. The goal is to establish a visual hierarchy within the web page. The larger heading is typically the most important information, followed by the lesser important subheadings. 

To structure your webpage you have to have a set of frameworks to contain the information. Here I have an example of the structure of a basic webpage: (Spaces were added in HTML to show the user)
 
 < html>

    < body>
 
    < h1>This is the Main Heading < /h1>
 
    < h2>This would be a sub-heading< /h2>
 
      < p> Text and content would go here. < /p>
 
    < h2>This would be an additional sub-heading< /h2>
 
      < p> Text and information to go here < /p>
 
    < /body>
 
 < /html> 

### Q: What is HTML? 
### A: HMTL stands for HyperText Markup Language and tells the browser **what** the content is. HTML often contains:
- Text
- Headlines
- Images
- Links
- Communicates **how** content should be organized
- Level of importance
- How to display content in blocks or boxes

### Q: Why do we write HTML?
### A: HMTL started in the late ’80s when the internet started
 - Invent a browser for the Web
 - Invent a language that the browsers could read
 - If there are words or things in angle brackets that tells the computer what to do

### Applying HTML in practice
- Content is wrapped in “tags”
- Tags tell the browser the meaning of the content
- Browsers display the content according to the rules of the tags
- This is called “marking up” the content
- Ergo: HyperText Markup Language

### HTML Tags
- Tags surround the content they describe. Like this:
- <p>My really cool block of text!</p>
- There are opening tags: <p>
- There are closing tags: </p>
- And there are self-closing tags: <img src=”puppies.jpg”>
- Browsers don’t care whether you use uppercase or lowercase characters

The HTML code consists of characters that live inside of angled brackets - these are known as elements. Elements are often made of two **tags**: an opening tag and a closing tag with a forward slash. Here is an example of an element.
 
 < html>< /html>

#### HTML Tags Continued: 
- Tags surround the content they describe. Like this:
- < p>My really cool block of text!< /p>
- There are opening tags: < p>
- There are closing tags: < /p>
- And there are self-closing tags: < img src=”puppies.jpg”>
 
 < html>< /html>

### ***Introductions to CSS***

### Q: What is CSS and what does it do?
### A: CSS works within the frameworks of the structures of the webpage. This tells the browser how the content should look

### Q: What can CSS do for you?
### A: CSS is a fantastic tool that you can give your webpage the little bit of flair that you were looking for. CSS can do a few things and more such as: 
- Change the Text color
- Change Font style and size
- Placement of content
- Size, type, and weight of borders
- Responsiveness: adapting the interface to the user’s screen size
- CSS Stands for: Cascading style sheets, and just as the name implies. CSS works from top to bottom. 

### CSS associates style rules with HTML elements:
- These rules govern how the content of specified elements should be displayed.
- CSS contains two parts: A selector and a declaration 
- Example: p {font-family: Arial;}
 -p is the selector and the font family is the declaration

### CSS properties affect how elements are displayed:
- CSS declarations sit inside curly brackets and each is made up of two parts: A property and a value. 
Example: h1, h2, h3 {font-family: Arial; color: yellow;}
 - This rule would apply to all headers in 1, 2, and 3. 
 - Within CSS you have a Margin, Border, and padding. The padding pushes the border away from the content. 

### Examples of CSS being applied:
Foreground Color:
- Color properly allows you to specify the color of text inside an element. Colors can be specified in one of three ways.
 1. RGB Values - RGB express colors in terms of how much *red, green, blue* area are used to make it up. RGB has values 0 to 255.
 2. Hex Codes -These are six-digit codes that represent the amount of red, green, and blue in a color. For hex code to work you have to have a # or hash sign proceed the code. Example #ee3e80
 3. Color names - 147 predefined color names are recognized by browsers. For example *DarkCyan*.

Background Color:
- CSS treats each HTML element as if it appears in a box, and the background-color property sets the color of the background for that box. A background color is easily specified by either calling: RGB values, Hex Codes, or Color Names
- If I did not specify a background color, the background would be transparent. Most web browser windows default to have a white background, but the browser's user can set a background color for their windows.

Understanding Color:
- Colors on a computer screen are created by mixing amounts of red, green, and blue. To find a color you want, you use a color picker. Color picking tools are available in imaged editing programs like photoshop and HIMP. The colors projected on your screen are composed of tiny squares that are called pixels. When your screen is not turned on the pixels display as black because it’s not emitting any light.
- RGB Values are expressed 0 - 255. Example rgb(102,205,170)
- Hex Codes are expressed in a hexadecimal code. Example #66cdaa
- Color names are represented by predefined names. Example MediumAuqaMarine
- Hue is near to the colloquial idea of color. 
- Saturation refers to the amount of gray color.
- Brightness refers to how much black is in a color. 

Contrast:
- When you pick foreground and background colors, it is important to ensure that there is enough contrast for the text to be legible. 
 - Low contrast can make text harder to read when there is low contrast between background and foreground
 - High contrast text is easier to read when there is high contrast between background and foreground color.
CSS3: Opacity
- CSS3 introduced the opacity property which allows you to specify the opacity of an element and any of its child elements. This property allows you to specify a color just like you would with an RGB value but adds a fourth value to indicate opacity. This is known as an alpha value and is a number between 0.0 and 1.0. For example, a value of .15 is 15% opacity.
CSS3: HSL Colors

- The introduction of CSS3 showcases an entirely new and intuitive way to specify colors using hue, saturation, and lightness value.
 - Hue is near to the colloquial idea of color. 
 - Saturation refers to the amount of gray color.
 - Lightness is the amount of white or black in a color. Lightness is represented as a percentage. 0% lightness is black, 100% lightness is white. 

CSS3: HSL & HSLA
- HSL color property has been introduced in CSS3 as an alternative way to specify colors. 
- (H)ue, (S)aturation, (L)ightness.
- (H)ue, (S)aturation, (L)ightness, (A)lpha

### ***JavaScript Basics***

### Q: What is Javascript?
### A: A programming language that allows dynamic interactions with the browser tells the browser what it should do when certain things happen 

### Why use Javascript?
- Javascript is a wonderful tool that you can further build upon the existing framework you have in place with HTML and CSS.
- Javascript provides the website with tools to have slideshows, Forms, filtering data, and so much more!

### The Nitty Gritty
- Javascript when you pull out a part of the word you have a script. A script is like a series of instructions to follow out in a one-by-one operation. To write a script you should first state your goal and then list the tasks that need to be completed to achieve it. 

- Though I did not touch that much on the actual code used for Javascript, I will go over that in a later topic and expand on that learning. At the heart of Javascript, you have expressions and operators. Both go hand in hand in telling the *script* you've created what order it should go.

### Table of Contents
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
- [Read 12 Documents for HTML Canvas Element & Chart JS](Read12.md)
- [Read 13 Local Storage](Read13.md)
- [Read 14a CSS Transforms Transitions and Animations](Read14A.md)
- [Read 14b What Google Learned About Teams](Read14A.md)

### Link to Code 102
- [Code 102 Reading Notes](https://jtaisey389.github.io/reading-notes/)

### <== Back to Code 201 Reading Notes
- [Reading Notes 201](https://jtaisey389.github.io/reading-notes201.md/)