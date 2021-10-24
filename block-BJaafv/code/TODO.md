1. What is the difference between the two `sum` function given below?

```js
// first
function sum(a, b) {
  return a + b;
}

// second
function sum(a, b) {
  console.log(a + b);
}
```

//answer:- In the first function output is return and give some value but in second case we did not get any value console.log only for the backend work or print the result in console.

2. If we store the returned value of both functions above in variable `first` and `second` what will be the value of `first` and `second`.
   // answer:- value will be store in both the variable but in second cash no value is return.

3. What will be the output when you call above `sum` function (first) with three parameter like `sum(12, 24, 35)`. Explain why?
   // answer:- because we have 2 parameter so the argument should b 2 if more then two it will not accept it.

4. Can you store the first `sum` function in a variable named `add`. If yes why? If no why?
   // answer:- Yes we can store it and use it's return value.

5. Declare a function named `sayHello` the accepts a parameter `name` and returns the name like `Hello Arya`.
   answer:-

```js
let name = `Arya`;
function sayHello(name) {
  return `Hello ${name}`;
}
```

6. What will be the output of the function below and why?

```js
let userName = "John";

function showMessage() {
  let message = "Hello, " + userName;
  return message;
}

showMessage(); // `Hello, john` (beacuse hello is difine in message variable and userName is define outside the funtion)
```

7. What will be the output for `Output1` `Output2` and `Output3` in the code below.

```js
let userName = "John";

function showMessage() {
  let message = "Hello, " + userName;
  return message;
}

alert(userName); // 'john'

showMessage(); // "Hello, John"

alert(userName); // "john"
```

8. What is a Anonymous Function give example of three functions.
   answer:-

```js
const add = function (a, b) {
  return a + b;
};
const sub = function (a, b) {
  return a - b;
};
const mul = function (a, b) {
  return a * b;
};
```

9. Can function declaration be a Anonymous Function? Explain
   // answer:- Yes function declaration can be anonymous , because in above examples we are doing same that is actually function declaration of anonymous.

10. Give 5 example of good naming convention for defining a function. You can read the details below to do that.

```md
Functions are actions. So their name is usually a verb. It should be brief, as accurate as possible and describe what the function does, so that someone reading the code gets an indication of what the function does.

It is a widespread practice to start a function with a verbal prefix which vaguely describes the action. There must be an agreement within the team on the meaning of the prefixes.

For instance, functions that start with "show" usually show something.

Function starting with…

"get…" – return a value,
"calc…" – calculate something,
"create…" – create something,
"check…" – check something and return a boolean, etc.
```

```js
function getGreaterNumber(a, b) {
  if (a > b) return a` is greater`;
  else return b` is greater`;
}

function calcTotal(a, b, c) {
  return a + b + c;
}

function create() {
  //create something,
}

function checkValue(value) {
  if (value % 2 === 0) return value` is even`;
  else return value` is odd`;
}
```
