1. Convert the function below into different forms of function expression.

```js
function percentage(marks, total) {
  return (marks * 100) / total;
}

// function expression 

let percentage = function (marks,total) {
  return (marks * 100) / total;
}

let percentage = function getMarks(marks,total) {
  return (marks * 100) / total;
}

let percentage = (marks,total) => {
  return (marks * 100) / total;
} 

```

2. Write Function Declaration or Function Expression next to the function.

```js
function percentage(marks, total) {
  return (marks * 100) / total;
}
// function Declaration 
```
```js
let percentage = function percentage(marks, total) {
  return (marks * 100) / total;
};
// function Expression 
```

```js
let percentage = function (marks, total) {
  return (marks * 100) / total;
};
// function Expression 
```

```js
let percentage = (marks, total) => {
  return (marks * 100) / total;
};
// function Expression 
```

```js
let percentage = (marks, total) => (marks * 100) / total;
// function Expression 
```

3. Why is a function definition an expression in JavaScript? Give one example of function expression.
//
because function defition is a value and we can store it a variable it will  become an expression.
example:
<!-- let sum =  (a,b) => a + b; -->

example: let getEven = (num) => num % 2 == 0; 

4. Why is a function call  an expression in JavaScript?
 
// We know  that expression always return a value , so  here function call is also always return a value like undefined, number ,boolean etc hence funcyion call is an expression in javascript


5. Write VALID and INVALID next to each example below with the reason.

```js
function add(a, b) {
  return a + b;
}

let five = add(2, 3); // VALID bacause we can store  return value of function add after its execution or Call.
five = add; // VALID because the value five can be replaced by add funtion.
five = five(10, 11);// VALID because the value five can be replaced return value of five function.
five = function () {
  return 'Hello';
}; // VALID because the value five can be replaced by a new function.
```
6. What is the difference between function definition and function call? Explain with an example.

// function definition is just declaration of any function with a keyword function but on the other hand function call is a part of execution of code inside function when we call or execute the function.
example :  
<!-- function definition  -->
function getOdd(num){
  return num % 2 !== 0; 
}

<!-- function call  -->
getOdd(2) // false;
getOdd(3) // true;

7. What is the similarities between function definition and function call?
// The similarities between function definition and function call is that ,both are expression.
8. Is the code below valid or invalid. Explain with reason.

```js
function hello() {
  console.log('Hello World!');
}

hello.user = 'Sam'; 
// Valid because function is a type of object so we can treat it as a object so we can also add key inside hello object with value same.
```

9. What is higher order function explain with an example.

// A function which takes another function as an argument or return a function is known as a heigher order function.

<!-- let a = [1,2,3,4,5,6,7,8,9,10];

function getOdd(num){
  if (num % 2 == 0){
     return num;
  }
}

a.filter(getodd) -->

// So here filter is a heigher order function.
<!-- 
function heigher(){
  function main(){};
  return main;
} -->

// so here heigher is a  heigher order function.

10. Explain what is callback function. Why you can pass a function inside a function?

// A function that is passed in another function  as an argument is known as callback function. because callback function is an expression so we can pass it into another function as ans argument. 
