Understanding Scope and the difference between var, let and const

Guess the output:

```js
let firstName = "Arya";
const lastName = "Stark";
var knownAs = "no one";

console.log(window.firstName, window.lastName, window.knownAs); // undefined undefined 'no one'
```

Guess the output:

```js
let firstName = "Arya";
const lastName = "Stark";
var knownAs = "no one";

function fullName(a, b) {
  return a + b;
}

console.log(window.fullName(firstName, lastName)); // AryaStark
```

Make a Execution Context Diagram for the following JS and write the output.

```js
function addOne(num) {
  return num + 1;
}
var one = addOne(0);
var two = addOne(1);
console.log(one, two);
output; // 1 2
```

Make a Execution Context Diagram for the following JS and write the output.

```js
var one = addOne(0);
function addOne(num){
return num + 1;
}
var two = addOne(1);
console.log(one, two);
output will be // 1 2
```

Make a Execution Context Diagram for the following JS and write the output.

```js
console.log(addOne(0));
function addOne(num) {
  return num + 1;
}
var two = addOne(1);
console.log(two); // 2
```

Make a Execution Context Diagram for the following JS and write the output.

```js
var one = addOne(0);
const addOne = (num) => {
  return num + 1;
};
var two = addOne(1);
console.log(two);
// addOne is not defined
```

Make a Execution Context Diagram for the following JS and write the output.

```js
console.log(addOne(0));
const addOne = (num) => {
  return num + 1;
};
var two = addOne(1);
console.log(two);
// addOne is not defined
```

What will be the output of the following

```js
function isAwesome() {
  var awesome;
  if (false) {
    awesome = true;
  }
  console.log(awesome);
}
isAwesome();
// undefined
```

What will be the output of the following

```js
function isAwesome() {
  let awesome;
  if (true) {
    awesome = true;
  }
  console.log(awesome); // true
}
isAwesome();
```

What will be the output of the following

```js
function isAwesome() {
  let awesome;
  if (false) {
    awesome = true;
  }
  console.log(awesome);
}
isAwesome(); // undefined
```

What will be the output of the following

```js
let firstName = "Arya";
const lastName = "Stark";
var knownAs = "no one";

function fullName(a, b) {
  return a + b;
}
const name = fullName(firstName, lastName);
console.log(name); // AryaStark
```

Guess the output of the code below with a reason.

```js
function sayHello() {
  let name = "Arya Stark";
}
sayHello(); // undefined
```

Guess the output of the code below with a reason.

```js
if (true) {
  var name = "Arya Stark";
}
console.log(name);
// Arya Stark
```

Guess the output of the code below with a reason.

```js
if (true) {
  let name = "Arya Stark";
}
console.log(name);
// Arya Stark
```

Guess the output of the code below with a reason.

```js
for (var i = 0; i < 20; i++) {}
console.log(i);
// 20 as the value of i terminate last time with 20 and doesn't go for condition check
```

Guess the output of the code below with a reason.

```js
for (let i = 0; i < 20; i++) {
  //
}
console.log(i);
// i is not defined
```

Guess the output and the reason behind that.

```js
function sample() {
  if (true) {
    var username = "John Snow";
  }
  console.log(username);
}
sample();
// John Snow
```

Guess the output and the reason behind that.

```js
function sample() {
  if (true) {
    let username = "John Snow";
  }
  console.log(username);
}
sample();
// username is not defined
```

Guess the output and the reason behind that.

```js
function sample() {
  var username = "Arya Stark";
  if (true) {
    var username = "John Snow";
    console.log(username);
  }
  console.log(username, "second");
}
sample();
// John Snow John Snow second
```

Guess the output and the reason behind that.

```js
function sample() {
  let username = "Arya Stark";
  if (true) {
    let username = "John Snow";
    console.log(username, "first");
  }
  console.log(username, "second");
}
sample();
// John Snow first
// Arya Stark second
```

Guess the output and the reason behind that.

```js
function sample(...args) {
  for (let i = 0; i < args.length; i++) {
    let message = `Hello I am ${args[i]}`;
    console.log(message);
  }
}

sample("First", "Second", "Third");
// Hello I am First Hello I am Second Hello I am Third
```

Guess the output and the reason behind that.

```js
function sample(...args) {
  for (let i = 0; i < args.length; i++) {
    const message = `Hello I am ${args[i]}`;
    console.log(message);
  }
}

sample("First", "Second", "Third");
// Hello I am First Hello I am Second Hello I am Third
```

Guess the output and the reason behind that.

```js
if (true) {
  const myFunc = function () {
    console.log(username, "Second");
  };
  console.log(username, "First");
  let username = "Hello World!";
  myFunc();
}
// Cannot access 'username' before initialization
```

Guess the output and the reason behind that.

```js
function outer() {
  let movie = "Mad Max: Fury Road";
  function inner() {
    console.log(`I love this movie called ${movie.toUpperCase()}`);
  }
  inner();
}

outer();
// I love this movie called MAD MAX: FURY ROAD
```

Guess the output and the reason behind that.

```js
function outer() {
  let movie = "Mad Max: Fury Road";
  function inner() {
    let movie = "Before Sunrise";
    console.log(`I love this movie called ${movie.toUpperCase()}`);
  }
  inner();
}

outer();
// I love this movie called BEFORE SUNRISE
```

Guess the output and the reason behind that.

```js
function outer() {
  let movie = "Mad Max: Fury Road";
  function inner() {
    let movie = "Before Sunrise";
    function extraInner() {
      let movie = "Gone Girl";
      console.log(`I love this movie called ${movie.toUpperCase()}`);
    }
    extraInner();
  }
  inner();
}
outer();
// I love this movie called GONE GIRL
```

Using reduce find the final value when the initial value passed is 100. You have to pass the output of one function into the input of next function in the array allFunctions starts with addOne ends with half.

```js
const addOne = (num) => {
  return num + 1;
};
const subTwo = (num) => {
  return num - 2;
};
const multiplyThree = (num) => {
  return num * 3;
};
const half = (num) => {
  return num / 2;
};

let allFunctions = [addOne, subTwo, multiplyThree, addOne, multiplyThree, half];
allFunctions.reduce((acc, cv) => cv(acc), 100);
// Answer is:
```
