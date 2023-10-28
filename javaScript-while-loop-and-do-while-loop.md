## While Loop 

A while loop will continue when the condition is true. 

For example, the below code will loop while “i” is less than the Array size:
```
let i = 0;
let tempMembers = ["Mustakim All Mobin", "Kawser Ahamed", "Ruhi Jannat"]

while(i < tempMembers.length)
{
    console.log(tempMembers[i])
}
```

We are doing the same thing as we were in the previous article For loop:

- i = 0 creating an index variable and setting it to 0.
- i < tempMembers.length looping while i is less then tempMembers.length
- console.log(tempMembers[i]) printing each teamp members name into the console.
- i++ incrementing the index by 1 on each loop.

This code will print all the team members name without me  😂.

**Now Question is why would you use a While loop over a For loop?**

Frankly speaking you will not see While loops very often in JavaScript code. But they can be useful. For example, say we are not sure what position the our other team member is in. We want to loop until we see other team member.

Let's see. 

```
let i = 0;
let notSeeOther = true;
let tempMembers = ["Mustakim All Mobin", "Kawser Ahamed", "Gias uddin Vuiya", "Ruhi Jannat"].


while(notSeeOther)
{
    console.log(tempMembers[i])
    i++
    if(tempMembers[i] === "Gias uddin Vuiya")
    {
        notSeeOther = false;
    }
}
```

For each loop, we check the condition **‘notSeeOther’** when it's **'true',** then the loop continues. As soon as **‘notSeeOther’** is set to false the loop will stop. This like break statement.

So, this is all about **While loop**. If you have any question or need clarification about this topic, Please😐 Don't hesitate to ask🗣️. 

Your question will not only help you but also inspire me to write more article about **JavaScript**,**React**,**DSA** and **NextJs**. So, making your learning journy more interactive. Till then, Allah Hafiz.😊

