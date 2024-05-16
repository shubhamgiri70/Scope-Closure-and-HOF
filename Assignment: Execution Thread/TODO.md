1. What does thread of execution means in JavaScript?
   // in javascript, the "thread of execution" refers to the secquence in which statements within a script are executed. for eg.

```js
var user = "Arya";

function sayHello() {
  return `Hello ${user}`;
}

var userMessage = sayHello(user);
```

2 - Where the JavaScript code gets executed?

// javascript engine

3 - What does context means in Global Execution Context?

// the global execution context is a fundamental concept in understending how the code excuted. talking about "context", the surrounding in which a particular peice of code is executed.

4 - When do you create a global execution context.

// A global execution context is created whenever javascript code is executed. this happens in mant situations like Initial page load, script execution, executing a javascript file nad using a developer tools console etc.

5 - Execution context consists of what all things?

An execution context in javascript consists of several component that together create an environment of the execution of code. these component includes -
Variable environment, Lexical environment, scope chain, outer enviroment refrence and code execution etc

6 - What are the different types of execution context?

global execution context - this is the outermost context and is created when your script is executed. it represents the defult enviroment in which your javascript code runs. in web browsers, the global execution context is associated with the global object (window)

7 - When global and function execution context gets created?

the global and function execution context gets created under different circumstances like
The global execution context creation - the GEC is created when the javascript engine is first encounters your script. For web browesers, when an HTML page is loded, the browser starts parsing the HTML and encounters the `<script>` tags or external script files.
Function Execution context creation - the FEC is created whenever a funtion is called or invocked. When a function is called, a new execution context for that function is created and pushed onto the excution stack.

Create a execution context diagram of the following code on your notebook. Take a screenshot/photo and store it in the folder named img. Use ![](./img/Screenshot%202024-05-16%20at%2011.50.35 AM.png) to display it here.

```js
var user = "Arya";

function sayHello() {
  return `Hello ${user}`;
}

var userMsg = sayHello(user);
```

```js
var marks = 400;
var total = 500;

function getPercentage(amount, totalAmount){
return (amount \* 100) / totalAmount;
}

var percentageMarks = getPercentage(marks, total);
var percentageProfit = getPercentage(400, 200);
```

```js
var age = 21;

function customeMessage(userAge) {
  if (userAge > 18) {
    return `You are an adult`;
  } else {
    return `You are a kid`;
  }
}

var whoAmI = customeMessage(age);
var whoAmIAgain = customeMessage(12);
```
