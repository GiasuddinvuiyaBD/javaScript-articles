# JavaScript for...in loop
In the previous articles, we have coverd :
- [JavaScript while and do..while loop](https://web.facebook.com/groups/1773110546453636/permalink/1791177694646921/?mibextid=oMANbw)
- [JavaScript for...of loop](https://web.facebook.com/groups/1773110546453636/permalink/1795726244192066/?mibextid=oMANbw)
- [JavaScript for loop](https://web.facebook.com/groups/1773110546453636/permalink/1786581231773234/?mibextid=oMANbw)

Today we are going to learn **for...in** loop. 

In JavaScript **for...in** loop allowes you to iterate over all property keys of an object.

# Syntax: 
```js
for (key in object) {
    // body of for...in
}
```

In each iteration of the loop, a key is assigned to the **key** variable. The loop continues for all object properties.

> **Note :**  Once you get **keys**, you can easily find their corresponding values.

### Examples-1:  Iterate through an Object.

```js
const myInfo = {
    name : 'Gias Uddin',
    age : 19,
    profession : 'student'
}

// iterate by for..in 
for(let key in myInfo)
{
    console.log(`${key} => ${myInfo[key]}`);
}
```

**Output :** 
```
name => Gias Uddin
age => 19
profession => student
```

In the above program, the **for..in** loop is used to iterate over the **myInfo** objects and print all it's properties.

- The object key is assigned to the variable **key**.
- myInfo[key] is use to access the value of key.


### Examples-1: Update Values of Properties
```js
const team = {
    name1 : 'Mustakim al Mobin',
    name2 : 'Kawsar Ahmed'
}
// updating team member names.
for(let names in team)
{
    console.log(`${names} => Md : ${team[names]}`);
}
```
**Output :** 
```
name1  => Md : Mustakim al Mobin
name2  => Md : Kawsar Ahmed
```

### Iterate String by using for..in loop
```js
const str = 'coders';

for(let key in str)
{
    console.log(str[key])
}
```

**Output :** 
```
c
d
e
r
s
```

### for...in With Array

```js
const arr = ['JavaScript','Coders','Bangladesh'];

for(let key in arr)
{
    console.log(arr[key])
}
```

**Output :**
```
JavaScript
Coders
Bangladesh
```
You will learn more about the arrays later article.

> **Note :** You should not use **for..in** over an array where the index order is important.
On of the better way to iterate over the array using **for...of** loop. 

To learn more about **for..of** loop, visit [JavaScript for..of loop](https://web.facebook.com/groups/1773110546453636/permalink/1795726244192066/?mibextid=oMANbw)
