Implement forEach array method using Array.reduce
forEach accepts two parameter array and callback
It does not return anything
It should work exactly like array forEach method

```js
function forEach(arr, cb) {
  arr.reduce((acc, cv, index, arr) => {
    cb(cv, index, arr);
  });
}

forEach(["Sam", "Jon", "Arya"], (name, i, arr) =>
  console.log(name + name, i, arr)
);
```

Implement map array method using Array.reduce
map accepts two parameter array and callback
It returns same size of array
It should work exactly like array map method

```js
function map(arr, cb) {
  return arr.reduce((acc, cv) => {
    acc.push(cb(cv));
    return acc;
  }, []);
}

map(["Sam", "Jon", "Arya"], (name) => name + name); // ['SamSam', 'JonJon', 'AryaArya']
```

Implement filter array method using Array.reduce
filter accepts two parameter array and callback
It returns same size or smaller array
It should work exactly like array filter method

```js
function filter(arr, cb) {
  return arr.reduce((acc, cv) => {
    if (cb(cv)) {
      acc.push(cv);
    }
    return acc;
  }, []);
}

filter(["Sam", "Jon", "Arya"], (name) => name.startsWith("S")); // ['Sam']
```


