# What Are Arrays in JavaScript? 

![JavaScript array](https://i.ytimg.com/vi/S2JVtEwa-kU/maxresdefault.jpg)

Arrays in JavaScript are the data type used to store a list of values. JavaScript array objects can be stored in variables and dealt with in the same way you deal with any other data type. The difference is that we can access each value inside the list individually, and perform various activities, such as looping over it.

## Declaration : 
There are two ways to creating an empty array.

```js
1. let arr = new Array();
2. let arr = [];
```
All most all the time we use `**let arr = []**` this syntax.

**Example :**
```js
    let fruits = ["Apple", "Orange", "Plum"];
```

You can easily access elements in an array by using square brackets with the element's position or index.

```js
let fruits = ["Apple", "Orange", "Plum"];

console.log(fruits[0]);
console.log(fruits[1]);
console.log(fruits[2]);
```
we can also replace the element.

```js
fruits[2] = 'Pear';
// now ["Apple", "Orange", "Pear"]
```
...Or we can add new item to the array.

```js
fruits[2] = 'Lemon';
// now ["Apple", "Orange", "Pear","Lemon"]
```

You can find out how many elements are in an array simply by looking at its **length** property in JavaScript.

```js
let fruits = ["Apple", "Orange", "Plum"];

console.log(fruits.length); // 3
```

In JavaScript, arrays are super flexible. You can store all sorts of elements in them, no matter what type those elements are.

```js
// mix of values
let arr = [ 'Apple', { name: 'Md: Miraz' }, true, function() { alert('hello'); } ];

// get the object at index 1 and then show its name
let name = arr[1].name;
console.log(name) 
// output : Md: Miraz

// get the function at index 3 and run it.
arr[3]();
// output: hello
```

## Get last elements with *''at''*

To access the last element in an array, you can simply use **`arrayName[arrayName.length - 1]`**.

```js
let fruits = ["Apple", "Orange", "Plum"];

console.log(fruits[fruits.length-1]) 
// output : Plum
```

You can get the last element of an array using this short and sweet syntax: **fruits.at(-1)**.

```js
let fruits = ["Apple", "Orange", "Plum"];

// same as fruits[fruits.length-1]
console.log(fruits.at(-1));
// output : Plum
```

## Methods pop/push, shift/unshift

### push():
JavaScript **push** method, Adds an element to the end of the array.

```js
let team = ['Mustakim al Mobin', 'Ruhi Jannt'];
// pushing data to the end of the array.
team.push('Kawsar Ahmed');

console.log(team);
// output: ['Mustakim al Mobin', 'Ruhi Jannt','Kawsar Ahmed'];
```

### pop():
JavaScript **pop** method, takes an element from the end of the array.
```js
let team = ['Mustakim al Mobin', 'Ruhi Jannt','Kawsar Ahmed'];
// Taking an element from the end of the array.
team.push();

console.log(team);
// output: ['Mustakim al Mobin', 'Ruhi Jannt']
```

### Shift() : 
In JavaScript **shift**  smoothly takes out the first element from an array.

```js
let team = ['Mustakim al Mobin', 'Ruhi Jannt','Kawsar Ahmed'];

let remove = team.shift(); 
// let's see the result
console.log(team); 
// ['Ruhi Jannt','Kawsar Ahmed'];
```

### unshift(): 
The **unshift** method is used to add elements to the front of the array and increases the index of every element by one.

```js
let team = ['Ruhi Jannt','Kawsar Ahmed'];

team.unshift("Gias uddin");
console.log(team);

// [Gias uddin,'Ruhi Jannt','Kawsar Ahmed'];
```

We've covered the basics of JavaScript arrays in this article. If you have any questions or feedback, please share them in the comments. Our experts are here to help and will respond quickly.




