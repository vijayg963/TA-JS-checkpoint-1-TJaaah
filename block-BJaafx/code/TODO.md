1. Using loops take 10 inputs from user and find the average of all the numbers.
   answer:-
   ```js
   function average() {
     let sum = 0;
     for (let i = 1; i <= 10; i++) {
       sum = prompt(`Enter ${i} value:`);
       sum += sum;
     }
     return sum / 10;
   }
   ```

````

2. What will be the output of the code below

```js
let i = 0;
while (i < 3) {
  println("hi");
  i++;
}
````

answer:- It will show error. because println is not defined.

3. Write a function named `getEvenSum` that accepts a parameter `max`. Return the sum of all even numbers. The value of max should default to 10.
   answer:-

```js
function getEvenSum(max = 10) {
  let sum = 0;
  for (let i = 0; i <= max; i++) {
    if (i % 2 === 0) {
      sum = sum + i;
    } else continue;
  }
  return sum;
}
```

4. Write a function named `getOddSum` that accepts a parameter `max`. Return the sum of all odd numbers. The value of max should default to 10.
   answer:-

```js
function getOddSum(max = 10) {
  let sum = 0;
  for (let i = 0; i <= max; i++) {
    if (i % 2 !== 0) {
      sum = sum + i;
    } else continue;
  }
  return sum;
}
```

5. Write a function named `getProductOfDigits` that accepts a parameter `num`. It returns the product of all the digits in the number.

- If the input value is less than 0 return `not a valid input`
- For example if the input is `123` output should be `6`.
  answer:-

```js
function getProductOfDigits(num) {
  let product = 1;
  if (num < 0) return `not a valid input`;
  else {
    while (num != 0) {
      product = product * (num % 10);
      num = Math.floor(num / 10);
    }
    return product;
  }
}
```

6. What will be the output of the following code below in multiple conditions? Explain with reason?

```js
function check(num) {
  if (num > 5) {
    return "Bigger than 5";
  }

  if (num < 5) {
    return "Smaller than 5";
  }

  return num;
}

check(10); // "Bigger than 5" as the value is greater than 5
check(1); // "Smaller than 5" as the value is smaller than 5
check(5); // 5 as there is no condition for it thus it returns the value of parameter
```

7. What will be the output of the following code given below? Explain the reason?

```js
function getOutput(name) {
  if (name === "Arya") return "You are arya";
  if (name === "John") return "You are john";
  return "Who are you";
}

getOutput("Arya"); // "You are arya" as per the given condition and the output is displayed
getOutput("John"); // "You are john" as per the given condition and the output is displayed
getOutput(); // "Who are you" as no value is passed so parameter the return statement is executed
```

8. What will be the output of the following code given below? Explain the reason?

```js
function getOutput(name) {
  if (name === "Arya") console.log("You are arya");
  if (name === "John") console.log("You are john");
  return "Who are you";
}

getOutput("Arya"); // "Who are you"
getOutput("John"); // "Who are you"
getOutput(); // "Who are you"
```

9. Can a function have multiple return statement? Give one example if possible and explain the reason.

```js
function getOutput(name) {
  if (name === "Arya") return "You are arya";
  if (name === "John") return "You are john";
  return "Who are you";
}
```

Here the return statements are indivisual to the if condition.

10. What is the difference between `for` loop and `while` loop. What are the different place you can use them? Explain with example.

answer:-The difference between for loop and while loop is that in for loop the number of iterations to be done is already known and is used to obtain a certain result whereas in while loop the command runs until a certain condition is reached and the statement is proved to be false. for loop is used when we know how many times the iterations is to be done, whereas, while loop is used until a statement is proven false.

//for loop

```js
function add(max) {
  let sum = 0;
  for (let i = max; i > 0; i--) {
    sum += i;
  }
  return sum;
}

//while loop
function add(max) {
  let sum = 0,
    i = max;
  while (i > 0) {
    sum += i;
    i--;
  }
  return sum;
}
```
