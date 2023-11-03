# JavaScript Quiz.

![Quiz image](https://www.bapugraphics.com/quiz/wp-content/uploads/2017/05/JavaScript-Quiz-Questions.jpg?x85292)

# 🧩 JavaScript Challenge: The Code Quiz

## Q-1: What's the output? 🤔

```js
const person = { name: 'Lydia' };

function sayHi(age) {
  return `${this.name} is ${age}`;
}

console.log(sayHi.call(person, 21));
console.log(sayHi.bind(person, 21));

```


- A: `undefined is 21`  `Lydia is 21`
- B: `function` `function`
- C: `Lydia is 21` `Lydia is 21` 
- D: `Lydia is 21` `function` 

**Answer:D**

With both, we can pass the object to which we want the **this** keyword to refer to. However, **.call** is also *executed immediately!*

**.bind.** returns a copy of the function, but with a bound context! It is not executed immediately.


## Q-2: Which of this values are falsy ?  🤖🔍
```js
0;
new Number(0);
('');
(' ');
new Boolean(false);
undefined;
```

- A: `0`, `''`, `undefined`
- B: `0`, `new Number(0)`, `''`, `new Boolean(false)`, `undefined`
- C: `0`, `''`, `new Boolean(false)`, `undefined`
- D: All of them are falsy


**Answer: A**

There are 8 falsy values:

- undefined
- null
- NaN
- false
-  '' (empty string)
- 0
- -0
- 0n (BigInt(0))

`Function constructors, like new Number and new Boolean are truthy.`

**I'll be revealing the answer next Friday! 📅 Stay tuned! 🤩**
