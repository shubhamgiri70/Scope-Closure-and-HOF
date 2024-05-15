// Convert the function below into different forms of function expression.

```js
function percentage(marks, total) {
return (marks * 100) / total;
};

// Your code goes here

function expression //
let percentage = function percentage(marks, total){
   return (marks * 100) / total;
}; // with name

let percentage = function (marks, total){
   return (marks * 100) / total;
}; // without name

let percentage = (marks, total) => {
   return (marks * 100) / total;
}; // Arrow function

let percentage = (marks, total) => (marks * 100) / total; // Arrow function

// Write Function Declaration or Function Expression next to the function.

function percentage(marks, total) {
return (marks * 100) / total;
};
// function declaration

let percentage = function percentage(marks, total) {
  return (marks * 100) / total;
};
// function expression


let percentage = function (marks, total) {
  return (marks * 100) / total;
};
// function expression

let percentage = (marks, total) => {
  return (marks * 100) / total;
};
// function expression

let percentage = (marks, total) => (marks * 100) / total;
// function expression


// Why is a function definitation an expression in JavaScript? Give an example of function expression.

// A function defination is an expression in javascript because it evaluates to a value.
 for example -
 function add(a, b){
    return a + b;
 };

let add = function (a, b){
    return a + b;
}

// Why is a function call an expression in JavaScript?

// function call always returns a value that's why it is an expression.

// Write VALID and INVALID next to each example below with the reason.

function add(a, b) {
return a + b;
}

let five = add(2, 3); // valid
five = add; // valid
five = five(10, 11); // valid
five = function () {
return 'Hello';
}; // valid


// What is the difference between function definition and function call? Explain with an example.

// A function definition defines the structure and behaviour of a function. it specifies the name of the function, its parameter(if any), and the code to be executed when the function is called. the function definition is where we write the logic that the function will perform.

// A function call is the action of actually running the code defined within a function. function is called with the name along with parenthesis.

// What is the similarities between function definition and function call?

// function definition is an expression (function is an object).
// function call is an expression (it always returns a value).


// Is the code below valid or invalid. Explain with reason.

function hello() {
console.log('Hello World!');
}

hello.user = 'Sam'; // valid

// What is higher order function explain with an example.

// it is a function which accepts a function defination and returns a function defination. for eg.

function add(cb){
   cb()
}

function add(){
 function main(){}
 return main
}

// Explain what is callback function. Why you can pass a function inside a function?

// beacause function is an expression in javascript we can pass a function inside another function.

```
