Create a execution context diagram of the following code on your notebook. Take a screenshot/photo and store it in the folder named img. Use ![](./img/image-name.png) to display it here.

Take in account the different phases of execution, different execution contexts

```js
1;
var firstName = "Arya";
var lastName = "Stark";

function getFullName(first, last) {
  return `${first} ${last}`;
}

function sayHelloToUser(name) {
  return `Hello ${name}, How are you doing?`;
}

var fullName = getFullName(firstName, lastName);
var jon = getFullName("John", "Snow");

console.log(fullName);

var userMessage = sayHelloToUser("Bran");
2;

function sayHi() {
  var name = "Lydia";
  var age = 21;
  console.log(name);
  console.log(age);
}

sayHi();
3;

function sayHi() {
  console.log(name);
  console.log(age);
  var name = "Lydia";
  var age = 21;
}

sayHi();
4;

console.log(arr); // undefined
console.log(username); // undefined
var usename = "Sam";
var arr = [1, 2, 3, 4, 5, 6];

function double(num) {
  return num * 2;
}
```
