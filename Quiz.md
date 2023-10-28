# JavaScript Quiz.

![Quiz image](https://www.bapugraphics.com/quiz/wp-content/uploads/2017/05/JavaScript-Quiz-Questions.jpg?x85292)

# 🚀 JavaScript Rocket: The Code Quiz

## Q-1 : What's the outoput ??

```js
for (let i = 1; i < 5; i++) {
  if (i === 3) continue;
  console.log(i);
}
```

- A: `1` `2`
- B: `1` `2` `3`
- C: `1` `2` `4`
- D: `1` `3` `4`

**Answer:C**

The **continue** statement skips an iteration if a certain condition returns **true**.


## Q-2 : What's the ouput ??
```js
let a = 3;
let b = new Number(3);
let c = 3;

console.log(a == b);
console.log(a === b);
console.log(b === c);
```

- A: `true false true`
- B: `false false true`
- C: `true false false`
- D: `false true true`


**Answer: C**

**new Number()** is a built-in function constructor. Although it looks like a number, it's not really a number: it has a bunch of extra features and is an object.

When we use the **==** operator (Equality operator), it only checks whether it has the same value. They both have the value of **3**, so it returns **true**.

However, when we use the **===** operator (Strict equality operator), both value and type should be the same. It's not: **new Number()** is not a number, it's an object. Both return **false**.



