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

A second option wrather than writing the function yourself is to use Modernizr to detect support for HTML5 storage. 

`if (Modernizr.localstorage) {`
  `// window.localStorage is available!`
`} else {`
  `// no native support for HTML5 storage :(`
  `// maybe try dojox.storage or a third-party solution`
`}`

### Using HTML5 Storage
- HTML5 storage is based on named key/value pairs. You store data based on a named key, then you can retreive that data with the same key. The key is a string and the the data can be any type supported by JavaScript. Should you want to retreive anything other than strings, you will need to use functions like parseInt() or parseFloat().

`interface Storage {`
  `getter any getItem(in DOMString key);`
  `setter creator void setItem(in DOMString key, in any data);`
`};`

Calling setItem() with a named key that already exists will overwrite the previous value. Calling getItem() with a non-existent key will return null rather than throw an exception.

`var foo = localStorage.getItem("bar");`
`// ...`
`localStorage.setItem("bar", foo)`

This can also be re-written to use square bracket syntax instead. 

`var foo = localStorage["bar"];`
`// ...`
`localStorage["bar"] = foo;`

There are methods for removing the value for a given named key, and clearing the entire storage area. 

`interface Storage {`
  `deleter void removeItem(in DOMString key);`
  `void clear();`
`};`

Finally there is a property to get the total number of values in the storage area, and to iterate through all of the keys by index. 

`interface Storage {`
  `readonly attribute unsigned long length;`
  `getter DOMString key(in unsigned long index);`
`};`

### Tracking Changes to the HMTL5 Storage Area
- If you want to keep track programmatically of when the storage area changes,you an trap the storage event. The storage event is supported everywhere the localStorage object is supported, which includes Interenet Explorere 8. Trapping the storage event works the same as every other event you've ever trapped.

`if (window.addEventListener) {`
  `window.addEventListener("storage", handle_storage, false);`
`} else {`
  `window.attachEvent("onstorage", handle_storage);`
`};`

The handle storage callback function will be called with StorageEvent object.

`function handle_storage(e) {`
  `if (!e) { e = window.event; }`
`}`

### Storage Event Object
- Key: Is a string, the names key that was added, removed, or modified
- oldValue: any - The previous vaule, now overwritten a new item was added
- newValue: any - The new value, or null if an item was removed
- URL*: string - The page which called a method that triggered this change

### HTML5 Storage in action
- Lets take a look at HTML5 in action

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

### Link to Code 301
- [Reading Notes 301](jtaisey389.github.io/reading-notes301.md/)

### Link to Code 401
- [Reading Notes 401](jtaisey389.github.io/401_readingnotes.md/)

[<== Back_to_reading_notes](jtaisey389.github.io/reading-notes201.md/)
