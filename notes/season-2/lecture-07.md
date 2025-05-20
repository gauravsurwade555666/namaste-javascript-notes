## Currying in Java Script

Currying in JavaScript is a technique where a function, instead of taking all arguments at once, takes the first one and returns a new function that takes the next argument, and so on, until all arguments have been provided. 
The final function then executes with all the arguments.

## Why Use Currying?
- It helps create reusable and more flexible functions.
- It allows partial application of functions (pre-filling some arguments).

Example
Without Currying

```js
function add(a, b, c) {
  return a + b + c;
}

console.log(add(1, 2, 3)); // 6
```

With Currying
```js
function add(a) {
  return function(b) {
    return function(c) {
      return a + b + c;
    }
  }
}

console.log(add(1)(2)(3)); // 6
```



![image](https://github.com/user-attachments/assets/231354a0-5356-455b-bff3-5aa810bf5423)

![image](https://github.com/user-attachments/assets/830756fa-b84e-456a-9fa1-cb07e072c0d1)

