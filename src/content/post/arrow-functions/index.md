---
title: "6 Types of arrow functions"
description: "Bash Alias Directory - Use bash alias - directory - alias - alias directory."
publishDate: "30 Oct 2023"
tags: ["JavaScript"]
---

## 6 Types Of Arrow Functions

### No parameters

If The Function takes no parameters, you use empty parentheses.

```javascript
const greet = () => "Hello World!";
console.log(greet());
// Output: Hello World!
```

### Single Parameter

if there's only one parameter, parentheses are optional.

```javascript
const square = (x) => x * x;
console.log(square(4));
// Output: 16
```

### Multiple Parameters

If there's only one parameter, parentheses are optional.

```javascript
const add = (a, b) => a + b;
console.log(add(2, 3));
// Output: 5
```

### Function Body With Multiple Statements

If the function body has more than one statement, you need to use curly brackets and specify the return keyword. (if you want to return something).

```javascript
const greetPerson = (name) => {
 const greeting = "Hello, " + name + "!";
 return greeting;
};
console.log(greetPerson("Alice"));
// Output: Hello, Alice!
```

### Returning Object Literals

When directly returning an object literal, wrap the literal in parentheses to differentiate it from function block.

```javascript
const makePerson =(firstName, last: lastName) => ({ first: firstName, last: lastName});
console.log(makePerson("John", "Doe"));
// Output: { first: 'John', last: 'Doe' }
```

### Higher Order Functions and Callbacks

Arrow functions are particularluy popular when used as short callbacks.

```javascript
const numbers = [1, 2, 3, 4];
const doubled = numbers.map((num) => num * 2); 
console.log
// Output: [2, 4, 6, 8]
```
