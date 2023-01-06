Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

Example:

```js
function hello() {
  var username = 'Arya';
}
console.log(useranme); // output
```

In above code we are looking for the variable named `usename`. There is no variable named `username` in the global scope. The variable is inside the function named `hello` and we can't access the variable defined inside a function from outside.

The above code will throw an error `Reference Error username is not defined`.

2. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
{
  const username = 'Arya';
}
console.log(useranme); // output
```

In above code we are looking for the variable named `usename`. There is no variable named `username` in the global scope. The variable is inside the block scope and we can't access the variable defined inside a block scope from outside.

The above code will throw an error `Reference Error username is not defined`.

3. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
if (true) {
  let username = 'Arya';
}
console.log(useranme); // output
```

In above code we are looking for the variable named `usename`. There is no variable named `username` in the global scope. The variable is inside the function scope and we can't access the variable defined inside a function scope from outside.

The above code will throw an error `Reference Error username is not defined`.



4. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
if (true) {
  var username = 'Arya';
}
console.log(username); // output
```

In above code we are looking for the variable named `username`. There is no variable named `username` in the global scope. The variable is inside the block scope but declared by keyword var so it doesn't create scope  we can access the variable defined by var keyword inside a block scope from outside.

The above code output is "Arya"`.

5. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John';
if (true) {
  var username = 'Arya';
}
console.log(username); // output
```
In above code we are looking for the variable named `username`. There is a variable declared by let, named `username` in the global scope. The variable declared inside the block scope having the same name username by var keyword and var does't create scope in block and we can not redeclare any variable using let keyword. so it'll throw an Error.

The above code will throw an error `Syntax Error username has already been declared`.


6. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John';
if (true) {
  let username = 'Arya';
}
console.log(username); // output
```
In above code we are looking for the variable named `username`. There is a variable declared by let, named `username` in the global scope. The variable declared inside the block scope having the same name username by let keyword and let  creates its own scope in block so we can declare any variable using let keyword in each scope.

The code output is "John"

7. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John';
function sayHello() {
  let username = 'Arya';
}
sayHello();
console.log(username); // output
```

In above code we are looking for the variable named `username`. There is a variable declared by let, named `username` in the global scope. The variable declared inside the functional scope having the same name username by let keyword and let creates its own scope in function also so we can declare any variable using let keyword in each scope. but when function execution context completed it'll be deleted. 

The code output is "John"

8. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
for (var i = 0; i < 10; i++) {
  console.log(i, 'First'); // output
}
console.log(i, 'Second'); // output
```
The output of first console is the value of i till the loop end and the output of second console is 10 because i is declared by var keyword so it is accessible outside the block scope.

9. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
for (let i = 0; i < 10; i++) {
  console.log(i, 'First'); // output
}
console.log(i, 'Second'); // output
```
The output of first console is the value of i till the loop end and the output of second console is  "refrence error i is not defined" because i is declared by let keyword so it creates the block scope so it is not accessible outside the block scope.
