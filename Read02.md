# Code 201 Reading Notes
## Read 02 Notes & Informatiom

### ***Text in HTML***
What we will cover is this section:

  **1. Headings and Paragraphs**

  **2. Bold, Italic, Emphasis**

  **3. Structural and semantic markup**

### Headings & Paragraphs 
As you create a web page, you add tags known as markup to the contents of the page. Tags provide extra meaning and allow browsers to show users the appropriate structure for the page.
- *Structural markup*: Elements that you can use to describe both headings and paragraphs. 
- *Semantic markup*: This provides extra information; such as where the emphasis is placed in a sentence. That is something you have written is a quotation and who said it, the meaning of acronyms, and so on.

### Headings
- In html you have a choice of six different headings. H1 is only used for main headings, you will only have a main heading as a best practice. H2 through H6 headings are classified as subheadings and varrying in height. Example of headings:
 <h1>This is a main heading H1</h1>
 <h2>This is a level two heading</h2>
 <h3>Level three heading</h3>
 <h4>Level four heading</h4>
 <h5>Level five heading</h5>
 <h6>Level six heading</h6>

### Paragraphs
- In order to create a paragraph, you would surround the words that make up the paragraph with an opening < p> tag and a closing < /p> tag. By default, a browser would show you each paragraph on a new line with some space between it. 

Example of paragraphs:
<p>I'm gonna make him an offer he can't refuse. It's not personal. It's in business. Mr. Corleone is Johnny Fontane's godfather. Now Italians regard that as a very close, very sacred religious relationship. Very well. You want to do business with me. I will do business with you</p>
<p>What's the matter with you? Is this what you've become, a Hollywood finocchio who cries like a woman? "Oh, what do I do? What do I do?" What is that nonsense? Ridiculous! I don't like violence, Tom. I'm a businessman; blood is a big expense. Why do you hurt me, Michael? I've always been loyal to you. It's an old habit. I spent my whole life trying not to be careless.</p>

### Bold & Italic
- Once you have created a paragraph some users may want to add additional emphasis on words, sentences, or possibly the whole paragraph. These are just two options that you could use, but there are so many more at your disposal. As a reminder, you have to have an opening tag and a closing tag. 

Examples of using bold & italics: < b> & < /b> Bold Tag, < i> & < /i> Italic tag
<p>What's the matter with you? Is this what you've become, a Hollywood finocchio who cries like a woman? <b>"Oh, what do I do?</b> What do I do?" What is that nonsense? Ridiculous! I don't like violence, Tom.
<p>Augue neque gravida in fermentum et sollicitudin ac orci phasellus. <i> In pellentesque massa placerat duis ultricies lacus sed.</i> Amet volutpat consequat mauris nunc congue.

### Superscript & Subscript
- Superscript and subscripts are a wonderful way that you can increase the functionality of your text. For example, if you wanted to talk about E=MC2 a superscript would help you write that. The same would apply to subscript and as an example, we will use CO2.

Examples: < sup>< /sup> Superscript tag, < sub>< /sub> Subscript tag
<p>E=MC<sup>2</sup>
<p>CO<sub>2</sub>

### White Space
- For code to be easier to read, web page authors often add extra spaces or start some elements on new lines. 

Examples of white space: The whitespace will display each of the paragraphs and make it easier for the user to read. 
<p>Why is the grass green?</p>
<p>How does the wind blow?</p>
<p>Does Jim know his pumpkins are safe?</p>

### Line Breaks & Horizontal Rules
- Similar to white space line breaks and horizontal rules are a great tool for displaying the information to the user in a different way. 

Examples: < br /> Line breaks & < hr />
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. <br> Arcu odio ut sem nulla pharetra diam sit amet. <br/> Nulla malesuada pellentesque elit eget.

Rutrum tellus pellentesque eu tincidunt. Est ultricies integer quis auctor elit sed vulputate. In hendrerit gravida rutrum quisque non tellus orci ac.
<hr> Leo duis ut diam quam nulla porttitor massa id neque. Urna nunc id cursus metus aliquam eleifend mi. Faucibus pulvinar elementum integer enim. In arcu cursus euismod quis. Rutrum tellus pellentesque eu tincidunt tortor aliquam. Ut venenatis tellus in metus vulputate eu scelerisque felis.</hr>

### Visual Editors & Their Code Views
- Content management systems and HTML editors such as VS Code usually have two views of the page you are creating. A visual editor and a code view. 

Visual editors are similar to word processors. Each editor will differ slightly, there are some features that are common to most editors that allow you to control the presentation of text. 

Code views show you the code created by the visual editor so you can manually edit it, or so you can just enter new code yourself. All of the content on this page I have been editing in a code view and previewing with the visual editor. 

### Semantic Markup
- Some text elements are not affected by the structure of your webpages, but they do add extra information to the pages. They are known as semantic markup, the latter part will cover semantic markup. 

### Strong & Emphasis
- Thes are similar to bold and italics but differ with how they are applied and how they affect the text. 

Examples: < strong>< /strong> Strong tag, < em>< /em>
<p><strong>Beware:</strong> Squirrels are cute, but are nuts.</p>
<p>This vessle contains harmfull liquids <strong>do not consume this liquid, it will cause death</strong></p>

<p>I think <em>Marsha</em> broke her nose</p>

### Quotations
- Quotations consist of two elements used to markup quotations. 

Examples: < blockquote>< /blockquote> Blockquote tags, < q>< /q> Quote tag
<blockquote cite"http://en.wikipedia.org/wiki/Winnie-the-Pooh">
 <p>Did you ever stop to think, and forget to start again</p>
</blockquote>
<p>As A.A. Milne said, <q>Some people talk to animals. Not many listent though. That's the problem</q></p>

### Abbreviations
- Abbreviations are a way that the user can show the title of an attribute. For this example, I will spell the code out followed by demonstrating the code. 

Example: Spelled out
< p>< abbr title="Professor">Prof< /abbr> Stephen Hawking is a theoretical physicist and cosmologist.< /p>
< p>< acronym title="National Aeornautics and Space Administration">NASA< /acronym> do some crazy space stuff.< /p>

Example: In Use
<p><abbr title="Professor">Prof</abbr> Stephen Hawking is a theoretical physicist and cosmologist.</p>
<p><acronym title="National Aeornautics and Space Administration">NASA</acronym> do some crazy space stuff.</p>

### Citations & Defenitions
- Building upon the framework of HTML, citations, and definitions are great attributes to format your webpage. Cite allows you to reference someone's work like that of a book, and dfn terminology to a user.

Example: < cite>< /cite> Citation tags, < dfn>< /dfn> tags
<p><cite>A Brief History of Time</cite> by Stephen Hawking has sold over ten million copies worldwide. </p>

<p>A <dfn>black hole</dfn> is a region of space from which nothing, not even light, can escape.</p>

### Author Details
- The < address> element has a specific use: to contain contact details for the author of the page.

Example: < address>< /address> Address tag
<address>
 <p><a href="mailto:homer@example.org">
 homer@example.org</a></p>
 <p>742 Evergreen Terrace, Springfield.</p>
</address>

### Changes to content
- Changing content in HTML also gives you the functionality to insert or delete elements within a document. These are < ins> and < del> elements, which are insert and delete. 

Example: < ins>< /ins> Insert tag, < del>< /del> Delete tag
<p>It was the <del>worst</del> <ins>best</best> idea she ever had.</p>

- In addition to those elements a < s> element indicates something that is no longer accurate or relevant.
Example: < s>< /s> Strikethrough tag

<p>Laptop computer: Apple MacBook Pro</p>
<p><s>Was $2,995</s></p>
<p>Now only $2,994</p>

### ***Introductions to CSS***
What we will cover in this section:

 1. What CSS Does**

 2. How CSS Works**

 3. Rules, Properties, and Values**

### Understanding CSS: Thinking within the box
- To understand how CSS works is to imagine there is an invisible box around every HTML element. With CSS this allows you to create rules that control the way that each individual box and the content of that box is presented.

### CSS Associates Style with rules and elements in HTML
- CSS will contain a selector and a declaration. 

Example: p {font-family: times;}
 - P is the selector and within the currly brackets is the declaration

Within declarations, you have a property and a value. 
Example: {font-family: Arial; color: yellow;}
 - The property is the font family with the value being Arial.

### External CSS
- With CSS you can link external documents to CSS. If you have an HTML page you would need to link your CSS to that sheet. 

Example: < link href="css/style.css" type="text/css" rel="stylesheet"/>
You are probably asking yourself what did I just type. Well here is the explanation!
 The link to tell your browser where to find the CSS files to be used. href specifies the path to the CSS files, type refers to the type of document. Finally, rel specifies the relationship between the HTML page and the file it's linked to. 

### Using Internal CSS
- Just like external CSS you have the option to use internal CSS. Internal CSS works, in the same way, external CSS and it will apply a style to a selector you have chosen. 

### CSS Selectors
- There are multiple types of selectors that allow you to target specific rules to an HTML element.

Overview of Selectors:
 - Universal Selector: * {} These target all elements on a page
 - Type Selector: h1, h2,h3, {} Targets specific elements
 - Class Selector: .note {} Targets any element whose class attribute has a value of note
 p.note {} Targets only < p> elements whose class attribute has a value of note
 - ID Selector: #introduction {} Targets elements whose id attribute has a value of introduction
 - Child Selector: li>a {} Targets any < a> elements that are children of an < li> element
 - Descendant Selector: p a {} Targets and < a> elements that sit inside a < p> element, even if there are other elements nested between them
 - Adjacent Sibiling Selector: hl+p {} Targets the first < p> element after any < h1> element, but not other < p> elements
 - General Sibling Selector: hl~p {} If you had two < p> elements that are sibilings of an < h1> element, this rule would apply.

### How CSS Rules Cascade
- If there are two or more rules that apply to the same element, it is important to understand which will take place. 
- If the two selectors are identical, the latter of the two will take precedence.
- If there is a selector that is more specific than the others, the more specific rule will take precedence over more general ones.

### Inheritance
- If you specify the font-family or color properties on a body element they will apply to most child elements. That is because the value of the font-family property is inherited by child elements. 

### ***Introduction to JavaScript***
What we will cover in this section:
1. The language syntax and grammar
2. Giving instructions 

### Statements
- A script is a series of instructions that a computer can follow one-by-one. Each individual instruction or step is known as a statement.

### Comments
- Wiriting comments to explain what your code does is a good practice. It's a great way for you to navigate the written code and understand what you have written. 

### What is a variable
- A script will have to temporarily store the bits of information it needs to do its job. It can sotre this data in variables, variables change or vary each time a script runs. 

### Data Types
- JavaScript destinguishes between number, strings, and true or false values known as booleans. These are all data types which include, numbers, strings and booleans.
### Arrays
- An array is a special type of variable. It doesn't just store one value; it stores a list of values. Within arrays you have values that are accessed as if they are in a numbered list. 

### Table of Contents
- [Read 01 Introductions to HTML and JavaScript](Read01.md)
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