# Code 201 Reading Notes
## Chapter 10 Reading

### ***Error Handling & Debugging***
- This chapter will help you learn how to find the errors in your code. It will also teach you how to write scripts that deal with potential errors gracefully.

### Order of execution
- To find the source of an error, it helps to know how scripts are processed. The order in which statements are executed can be complex; some tasks cannot complete until another statement or function has been run. 

### Execution Context
- Javascript interpreter uses the concept of execution contexts. There is one global execution context; plus, each function creates a new execution context. They correspond to a variable scope.

- Javascript interpreter processes one line of code at a time. When the statement needs data from another function it **stacks** or piles the new function on top of the current task.

### Execution context & Hoisting
- There are two phases of an activity:
1. Prepare new scope. Variables, functions, and arguments are created
2. Execute. Assign values to the variables, reference  functions and run their code, and finally  execute statements

### Understanding Scope
- Within the interpreter, each execution context has its own variables object. It hold the variables, functions, and parameters available within it.

### Understanding Errors
- If Javascript generates and error, then it throws and exception. 

Here are a variety of errors and what they mean.
    - Name: Type of error
    - Message: Description
    - fileNumber: Name of the Javascript
    - lineNumber: Line number of the error
  
Descriptions:
    - Error Generic Error -the other errors are all based upon this error
    - SyntaxError: Syntax has not been followed
    - Reference Error: Tried to reference a variable that is not declared/within scope.
    - TypeError: An unexpected data type that cannot be coerced
    - RangeError: Numbers not in an acceptable range
    - URI Error: encodeURI(), decodeURI(), and similar methods used incorrectly
    -EvalError: eval()function used incorrectly

### A Debugging Workflow
- Debugging is about deduction: Eliminating potential causes of an error. 

1. Where is the problem
2. What exactly is the problem

- A great way to review your code live is to use the DEV tools inside of the Javascript console

- Within your javascript code you can insert lines to inspect your code within the console. THere are a few different methods that be utilized to see where the errors in your code is taking place.

1. Console.info ()
2. Console.warn ()
3. Console.error ()

### Writing Tabular Data
- In browsers that support it, the console.table() method lets you output a table showing: objects, arrays that contain other objects or arrays

- You can also use the console.assert() method, you can test if a condition is met. 

### Handling Exceptions
- If you know your code might fail, use try, catch and finally.

1. Try - Will try to execute the code
2. Catch - If there is an exception, run this code
3. Finally - This always gets executed

### Throwing Errors
- If you know something might cause a problem for your script, you can generate your own errors before the interpreter creates them. 

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
- [Read 11 Assorted Topics](Read11.md)
- [Read 12 Documents for HTML Canvas Element & Chart JS](Read12.md)
- [Read 13 Local Storage](Read13.md)
- [Read 14a CSS Transforms Transitions and Animations](Read14A.md)
- [Read 14b What Google Learned About Teams](Read14A.md)

### Link to Code 102
- [Code 102 Reading Notes](https://jtaisey389.github.io/reading-notes/)

### <== Back to Code 201 Reading Notes
- [Reading Notes 201](https://jtaisey389.github.io/reading-notes201.md/)
