# Code 201 Reading Notes

## Transforms
- With CC3 Came new ways to position and alter elements. Now layout techniques can be revisted with alternative ways to size, position, and change elements.

## Transforms Syntax
div {
  -webkit-transform: scale(1.5);
     -moz-transform: scale(1.5);
       -o-transform: scale(1.5);
          transform: scale(1.5);
}


## 2D Rotate

HTML:

`<figure class="box-1">Box 1</figure>`

`<figure class="box-2">Box 2</figure>`

CSS:

`.box-1 {`
  `transform: rotate(20deg);`
`}`
`.box-2 {`
  `transform: rotate(-55deg);`
`}`

## 2D Scale 
HTML:

`<figure class="box-1">Box 1</figure>`

`<figure class="box-2">Box 2</figure>`

CSS:
`.box-1 {`
  `transform: scale(.75);`
`}`
`.box-2 {`
  `transform: scale(1.25);`
`}`

## 2D Translate
HTML: 

`<figure class="box-1">Box 1</figure>`

`<figure class="box-2">Box 2</figure>`

`<figure class="box-3">Box 3</figure>`

CSS: 
`.box-1 {`
  `transform: translateX(-10px);`
`}`
`.box-2 {`
  `transform: translateY(25%);`
`}`
`.box-3 {`
  `transform: translate(-10px, 25%);`
`}`

## 2D Skew
HTML:

`<figure class="box-1">Box 1</figure>`

`<figure class="box-2">Box 2</figure>`

`<figure class="box-3">Box 3</figure>`

CSS:
`.box-1 {`
  `transform: skewX(5deg);`
`}`
`.box-2 {`
  `transform: skewY(-20deg);`
`}`
`.box-3 {`
  `transform: skew(5deg, -20deg);`
`}`

## Combining Transformers
HTML:

`<figure class="box-1">Box 1</figure>`

`<figure class="box-2">Box 2</figure>`

CSS:
`.box-1 {`
  `transform: rotate(25deg) scale(.75);`
`}`
`.box-2 {`
  `transform: skew(10deg, 20deg) translateX(20px);`
`}`

## 2D Cube Demo
HTML:
`<div class="cube">`
  `<figure class="side top">1</figure>`
  `<figure class="side left">2</figure>`
  `<figure class="side right">3</figure>`
`</div>`

CSS: 

.cube {
  position: relative;
}

.side {
  height: 95px;
  position: absolute;
  width: 95px;
}

.top {
  background: #9acc53;
  transform: rotate(-45deg) skew(15deg, 15deg);
}

.left {
  background: #8ec63f;
  transform: rotate(15deg) skew(15deg, 15deg) translate(-50%, 100%);
}

.right {
  background: #80b239;
  transform: rotate(-15deg) skew(-15deg, -15deg) translate(50%, 100%);
}

## Transform Origin
HTML:

`<figure class="box-1">Box 1</figure>`

`<figure class="box-2">Box 2</figure>`

`<figure class="box-3">Box 3</figure>`

`<figure class="box-4">Box 3</figure>`

CSS: 

.box-1 {
  transform: rotate(15deg);
  transform-origin: 0 0;
}

.box-2 {
  transform: scale(.5);
  transform-origin: 100% 100%;
}

.box-3 {
  transform: skewX(20deg);
  transform-origin: top left;
}

.box-4 {
  transform: scale(.75) translate(-10px, -10px);
  transform-origin: 20px 50px;
}








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
- [Read 14b What Google Learned About Teams](Read14A.md)

### Link to Code 102
- [Code 102 Reading Notes](https://jtaisey389.github.io/reading-notes/)

### Link to Code 301
- [Reading Notes 301](jtaisey389.github.io/reading-notes301.md/)

### Link to Code 401
- [Reading Notes 401](jtaisey389.github.io/401_readingnotes.md/)

[<== Back_to_reading_notes](jtaisey389.github.io/reading-notes201.md/)