# for...of
Assalamu alaikum, Everyone. Today i we are going to learn javascirpt **for of** loop statement.

<!-- ![for..of](https://i.ytimg.com/vi/virQjbYVvjM/maxresdefault.jpg) -->

The `for...of` statement executes a loop that operates on a sequenc of value of an **iterable object**. Iterable objects includes build-ins such as Array,String,Type Array,Map,Set as well as argument object from a functions.

# Syntax
```js
for(variable of iterable)
{
    //statement
}
```
Here i will explain how it's work.

**variable** : It receive a value from the sequence on each iteration.

**iterable** : An iterable object is the source of squence of values on which the loop operates.

**statement** : The statement block is the code enclosed within the curly braces. It's the code that gets executed repeatedly as long as the loop's condition is true.

# Examples : 

**Iterating over an array:**
```js
const team = ["Mustakim Al Mubin", "Kawsar Ahmed", "Rohi Jannat"];

for(let names of team)
{
    console.log(names)
}

/* output:
    1.Mustakim Al Mubin
    2.Kawsar Ahmed
    3.Rohi Jannat
*/
```
Inside the loop, this line uses the console.log function to print the value of the names variable to the console. In each iteration of the loop, names will take on the value of each element in the team array.

**Iterating over a string**
```js
const instructor = "Samim Ahmed";

for(let value of instructor)
{
    console.log(value)
}

/*Output:
    1. S
    2. a
    3. m
    4. i
    5. m
    6. ''
    7. A
    8. h
    9. m
    10. e
    11. d

*/
```
As the code runs, it iterates through the characters of the "Samim Ahmed" string one by one, and it prints each character to the console. So, you will see the individual characters `"S," "a," "m," "i," "m," " ," "A," "h," "m," "e," "d"` printed on separate lines in the console.

I appreciate your enthusiasm for learning and discussing JavaScript! If you have any more questions or topics you'd like to explore related to JavaScript or any other subject, please don't hesitate to ask. Learning is a continuous journey, and I'm here to assist you in any way I can. Feel free to share your questions or topics of interest, and we can delve deeper into them together. Happy learning!