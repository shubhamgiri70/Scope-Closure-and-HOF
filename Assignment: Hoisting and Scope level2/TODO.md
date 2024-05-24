For the given code below:

re-write the code in ways that system will understand
For Example:

```js
var username = 'Arya';
let brothers = ['John', 'Ryan', 'Bran'];

console.log(username, brothers[0]);

function sayHello(name) {
return `Hello ${name}`;
}

let message = sayHello(username);
var nextMessage = sayHello('Test');
// Declaration Phase
var username = undefined;
let brothers;

function sayHello(name) {
return `Hello ${name}`;
}

let message;
var nextMessage = undefined;

// Execution Phase

username = 'Arya';
brothers = ['John', 'Ryan', 'Bran'];

console.log(username, brothers[0]);

message = sayHello(username);
nextMessage = sayHello('Test');
console.log(username, numbers);

2.

var username = 'Arya';
let number = 21;

function sayHello(name) {
return `Hello ${name}`;
}

let message = sayHello(username);
var nextMessage = sayHello('Test');

// Declaration Phase


3.

console.log(username, numbers);
let username = 'Arya';
let number = 21;

let sayHello = function (name) {
return `Hello ${name}`;
};

let message = sayHello(username);
var nextMessage = sayHello('Test');

4.

let username = 'Arya';
console.log(username, numbers);

let number = 21;
let message = sayHello(username);

let sayHello = function (name) {
return `Hello ${name}`;
};

var nextMessage = sayHello('Test');


5.

console.log(name);
console.log(age);
var name = 'Lydia';
let age = 21;

6.

function sayHi(name) {
console.log(name);
console.log(age);
var name = 'Lydia';
let age = 21;
}

sayHi();


7.

sayHi();
function sayHi(name) {
console.log(name);
console.log(age);
var name = 'Lydia';
let age = 21;
}


8.

sayHi();
let sayHi = function sayHi(name) {
console.log(name);
console.log(age);
var name = 'Lydia';
let age = 21;
};


9.

let num1 = 21;
console.log(sum);
var sum = num1 + num2;
let num2 = 30;


10.

var num1 = 21;

let sum2 = addAgain(num1, num2, 4, 5, 6);

let add = (a, b, c, d, e) => {
return a + b + c + d + e;
};
function addAgian(a, b) {
return a + b;
}
let num2 = 200;

let sum = add(num1, num2, 4, 5, 6);
VM14000:3 Uncaught ReferenceError: addAgain is not defined
function test(a) {
let num1 = 21;
return add(a, num1);
}

let sum = test(100);

let add = (a, b) => {
return a + b;
};
VM14030:3 Uncaught ReferenceError: add is not defined

11.

function test(a) {
let num1 = 21;
return add(a, num1);
}

let sum = test(100);

function add(a, b) {
return a + b;
}
//declaration phase

12.

function test(a) {
let num1 = 21;
return add(a, num1);
}

let sum;

function add(a, b) {
return a + b;
}
// execution phase
function test(a) {
// declaration phase
a= 100
let num1;
// execution phase
num1 = 21;
return add(100, 21);
}

let sum = test(100);

function add(100, 21) {

return 100 + 21;
}
sum = 121

```
