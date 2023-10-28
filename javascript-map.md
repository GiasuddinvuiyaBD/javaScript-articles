![javascript-map-img](https://i1.wp.com/www.cupcom.com.br/wp-content/uploads/2020/09/javascript-map.png?w=1200&ssl=1)

JavaScript map method provides easy way for manipulating arrays. In this article, we'll explore the basics of the map method in javascript, including syntax and use examples, so let's get started.🚀

## What Is JavaScript Map Method()
The map method allows us to create a new array based on an existing array. The new array is created by calling a callback function on each element of the original array. And, values returning by the callback function consists of the new array.🔄

## Syntex
The syntax of the **map()** method is straightforward. Here's what it looks like:

```js
array.map(function(currentValue, index, arr), thisValue)
```
The Javascript **map()** method takes a function as it's argument. The function as three parameters.

- **currentValue :** the current element being processed in the array.
- **index:** the index of the current element being processed.
- **arr:** the array itself
- **thisValue:** it is optional and is used to set the value of this when the function is called. **It is not commonly used.**🤷‍♂️

## Example of Javascript Map Method

### Mapping an array of numbers to an array of square roots. 
The following code takes an array of numbers and creates a new array containing the square roots of the numbers in the first array.🧮

```js
const number = [1,4,9];
const roots = number.map((num) => Math.sqrt(num));

// number is still :  [1, 4, 9]
// roots is now :  [1, 2, 3]
```
### Transforming an Array
The following code shows how map works when a function requiring one argument is used with it. The argument will automatically be assigned from each element of the array as map loops through the original array.🔄

```js
const numbers = [1, 4, 9];
const doubles = numbers.map((num) => num * 2);

console.log(doubles); // [2, 8, 18]
console.log(numbers); // [1, 4, 9]
```
### Mapped array contains undefined
```js
const numbers = [1, 2, 3, 4];
const filteredNumbers = numbers.map((num, index) => {
  if (index < 3) {
    return num;
  }
});

// index goes from 0, so the filterNumbers are 1,2,3 and undefined.
// filteredNumbers is [1, 2, 3, undefined]
// numbers is still [1, 2, 3, 4]

```

So, this is all for today. If you have any more questions or topics you'd like to explore related to JavaScript or any other subject, please don't hesitate to ask. Learning is a continuous journey, and I'm here to assist you in any way I can. Feel free to share your questions or topics of interest, and we can delve deeper into them together. Happy learning! 📚😊


