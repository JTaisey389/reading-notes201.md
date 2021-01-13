### ***Lists***
What we will cover in this section:
 1. Numbered Lists
 2. Bullet Lists
 3. Defenition Lists

In HTML there are three types of lists that we can use.
- And ordered list where each item in the list is numbered. 
- Unordered list are lists with bullet points
- Definition Lists 

### Ordered Lists and Unordered Lists
- Examples: < li>< /li> List tag, '< ol> < /ol> Ordered list tag, < ul>< /ul> Unordered List tag

Ordered List
< ol>
 < li>Bagels< /li>
 < li>Cream cheese < /li>
< /ol>

<ol>
 <li>Bagels</li>
 <li>Cream cheese </li>
</ol>

Unordered List
< ul>
 < li>Bagels< /li>
 < li>Cream cheese < /li>
< /ul>

<ul>
 <li>Bagels</li>
 <li>Cream cheese </li>
</ul>

### Defenition Lists and Nested Lists
- Examples: < dl>< /dl> Defenition list tag, < dt>< /dt> DT contains the term being defined, < dd>< /dd> DD contains the defenition

< dl>
 < dt>Box< /dt>
 < dd>An object at which can contain items, or information within< /dd>
 < ul>
 < li>Used for moving< /li>
 < li>Used for storage
 < ul>
 < li>Information Storage< /li>
 < li>Contaninment of substance< /li>
 < /ul>
 < /li>
 < li>Boxes can be contained within one another< /li> 
 < /ul>
 
 <dl>
 <dt>Box</dt>
 <dd>An object at which can contain items, or information within</dd>
 <ul>
 <li>Used for moving</li>
 <li>Used for storage
 <ul>
 <li>Information Storage</li>
 <li>Contaninment of substance</li>
 </ul>
 </li>
 <li>Boxes can be contained within one another</li> 
 </ul>

## ***Boxes***
What we will cover in this section:
1. Controlling the size of boxes
2. Box model for borders, margin, and padding
3. Display and hiding boxes

### Box Dimensions & Limiting Width
- By default a box is sized just big enough to hold its contents. To set your dimensions for a box you can use the height and width properties. As with box dimensions which are just big enough to hold contents. You can limit the width of the actual content by applying a min or max-width. These commands take place in CSS.

Example: Box Dimensions - Width, Height
div { 
 height: 300px;
 width: 400px;
 background-color: #ee3e80;}
p { 
 height: 75%;
 width: 75%;
 background-color: elddda;}

Example: Limiting Width
td.description {
 min-width: 450px;
 max-width: 650px;
 text-align: left;
 padding: 5px;
 margin: 0px:}

### Limiting Height & Overflowing Content
- In the same token that you might want to limit the width of a box on a page, you might want to limit the height of a box on a page. When you constrain the height of a box what can happen is the box may not be big enough to hold the content. This is where overflowing content comes into play. You can either have the extra content hidden or you can provide the ability to scroll. 

Example: Min-hieght, Max-height
h2, p {
 width: 400px;
 font-size: 90%;
 line-height: 1.2em;}

h2 {
 color: #0088dd;
 border-bottomL 1px solid #0088dd;}

p {
 min-height: 10px;
 max-height: 30px; }

Example: Hidden, Scroll

p.one {
 overflow: hidden;}

p.two {
 overflow: scroll;}

### Border, Margin & Padding
- Every box has three available properties that can be adjusted to control its appearance.
1. Border: All boxes have a border even if it is not visible or specified. 
2. Margin: Margins sit outside the edge of the border. 
3. Padding: Padding is the space between the border of a box and any content contained within it.

- Within the padding and the margin, it is very helpful to add space between the various items on the page. This is white space and allows the user to read the page a little easier.

### Border Width:
- Border width property is used to control the width of a border.

Example: Border Width
p.one {
 border-width: 2px;}

p.two {
 border-width:thick}

p.three {border-width: 1px 4 px 12px 4px;}

### Border Style:
- Borders can be styled using the border-style property. 

Example: Border Style
p.one {border-style:solid: solid;}

p.two {border-style:solid: dotted;}

p.three {border-style:solid: dashed;}

p.four {border-style:solid: double;}

p.five {border-style:solid: groove;}

p.six {border-style:solid: ridge;}

p.seven {border-style:solid: inset;}

p. eight {border-style:solid: outset;}

### Border Color and Shorthand
- With borders, you can specify the color of a border using either RGB values; hex codes, or CSS color names. As with border color, shorthand allows the user to specify the width, style, and color of the border.

Example: Border Color

p.one {border-color: #0088dd;}

p.two {border-color: #bbbbaa #111111 #ee3e80 #0088dd;}

Example: Shorthand

p { width: 250px;
 border: 3px dotted #0088dd;}

### Padding & Margin
- Padding allows a user to specify how much space should appear between the content of an element and its border. As with padding you can control the space, margin properly controls the gap between boxes. 

Example: Padding

p { width:275px;
 border: 2px solid #0088dd;}
p.example {
 padding:10px;
}

Example: Margin
p {
 width: 200px;
 border: 2 px solid #0088dd;
 padding: 10px;}
p.example {
 margin: 20px;
} 

### Centering Content
- To center a box on a page you can set the left-margin and right-margin to auto.

Example: Centering Content
body {
 text-align: center;}
p {
 width: 300px;
 padding: 50px;
 border: 20px solid #0088dd;}

p.example {
 margin: 10px auto 10 px auto; text-align: left;}

### Change Inline/Block
- This display property allows you to turn an inline element into a block-level element. This also can be used to hide an element from the page.

Example:
1. Inline - Causes a block-level element to act like an inline element
2. Block - This causes an inline element to act like a block-level element 
3. Inline Block - This causes a block-level element to flow like an inline element. 

### Hiding Boxes
- This property allows you to hide boxes from users but it leaves a space where the element would have been.

Example: 
li {
 display: inline;
 margin-right: 10px;}
li.coming-soon {
 visibility: hidden;}

### CSS3 Border Images
- The border-image property applies an image to the border of any box. This can give your boxes added flair and emphasize certain parts of your website. In addition to border images, you can have box shadows. Box shadows allow you to add a drop shadow just like a text-shadow property.

### CSS3 Rounded Corners
- With the introduction of CSS3, introduced the ability to create rounded corners on any box. You have two options for doing rounded corners, you can either make it a constant radius or you can have elliptical.


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
- [Read 12 Documents for HTML Canvas Element & Chart JS](Read12.md)
- [Read 13 Local Storage](Read13.md)
- [Read 14a CSS Transforms Transitions and Animations](Read14A.md)
- [Read 14b What Google Learned About Teams](Read14A.md)

### Link to Code 102
- [Code 102 Reading Notes](https://jtaisey389.github.io/reading-notes/)

### <== Back to Code 201 Reading Notes
- [Reading Notes 201](https://jtaisey389.github.io/reading-notes201.md/)