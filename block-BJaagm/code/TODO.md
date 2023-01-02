1. What does thread of execution means in JavaScript?

<!-- // For execution of code javascript engine takes the code and execute it line by line so it is known as thread of execution.  -->

2. Where the JavaScript code gets executed?

<!-- // JavaScript executed the whole code in Global Execution Context.  -->

3. What does context means in Global Execution Context?

<!-- // The Environment where our code is execute is known as Context in global Execution. -->

4. When do you create a global execution context.

<!--  When we have to execute some code of snippets so we create a global execution of context. -->

5. Execution context consists of what all things?

<!-- // Execution context consists of some section like memory where our whole data is stored and in another section all the computation or execution of our code is happendes. -->

6. What are the different types of execution context?

<!-- // There are two types of execution context :  -->
<!-- 1. Global Execution Context. that creates only once in throughout the code.
2. Function Execution ConText. that creates whenever we call any function. -->

7. When global and function execution context gets created?

8. Function execution gets created during function execution or while declaring a function.

<!-- //Function execution gets created only when the function is executed or call.  -->


9. Create a execution context diagram of the following code on your notebook. Take a screenshot/photo and store it in the folder named `img`. Use `![](./img/image-name.png)` to display it here.



```js
var user = "Arya";

function sayHello(){
  return `Hello ${user}`;
}

var userMsg = sayHello(user);
```

<!-- Put your image here -->

![](./img/image-name.jpg)



```js
var marks = 400;
var total = 500;

function getPercentage(amount, totalAmount){
  return (amount * 100) / totalAmount;
}

var percentageMarks = getPercentage(marks, total);
var percentageProfit = getPercentage(400, 200);
```

<!-- Put your image here -->

![](./img/image-name.jpg)



```js
var age = 21;

function customeMessage(userAge){
  if(userAge > 18){
    return `You are an adult`;
  }else {
    return `You are a kid`;
  }
}

var whoAmI = customeMessage(age);
var whoAmIAgain = customeMessage(12);
```

<!-- Put your image here -->

![](./img/image-name.jpg)