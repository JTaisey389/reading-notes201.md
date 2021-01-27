# Code 201 Reading Notes

## The Past, Present & Future Of Local Storage For Web Applications

Local storage is one of the areas where applications have held advantage over web aplications. Historically, web applications have had none of these luxuries. Thus cookies were invented in early in the webs history, and can be used for local storage of small amounts of data. There are three downsides with cookies.

1. Cookies are included with every HTTP request, thus showing down your web application
2. Cookies send unencrypted data over the internet
3. Cookies are limited to about 4 KB of data

Ideally what we want is: 
1. Storage Space, and lots of it
2. On the client
3. Data that persits beyond a page refresh
4. Does not transmit to the server

With HTML5 we have the capacity to do all of the requirements above

### Introducing HTML5 Storage
- HTML5 storage is a way for your web page to store key value pairs locally within the client web broswer. Similar to cookies this data persists even after you navigate away from the web site. 

- From your JavaScript, you can access the HTML5 support through the local storage object. 

Check for HTML5:
`function supports_html5_storage() {`
  `try {`
    `return 'localStorage' in window && window['localStorage'] !== null;`
  `} catch (e) {`
    `return false;`
  `}`
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
- [Read 12 Documents for HTML Canvas Element & Chart JS](Read12.md)
- [Read 14a CSS Transforms Transitions and Animations](Read14A.md)
- [Read 14b What Google Learned About Teams](Read14A.md)

### Link to Code 102
- [Code 102 Reading Notes](https://jtaisey389.github.io/reading-notes/)

### <== Back to Code 201 Reading Notes
- [Reading Notes 201](https://jtaisey389.github.io/reading-notes201.md/)
