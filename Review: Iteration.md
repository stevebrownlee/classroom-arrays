## Review of Iteration

Things you used in this classroom.

* `for..of` loops
* Logical operators AND `&&` and OR `||`
* Arrays
* `if/else` code blocks for conditional logic
* `.push()` method for arrays
* `.length` property for arrays
* `.includes()` method for strings
* `+=` operator to add a any number to a variable's existing value
* `++` operator to add 1 to a variable's existing value
* Division `/` operator to find averages

That's a lot. We also want to remind you that it's expected for these concepts and skills to not be solidified just yet. You need a significant amount of practice to become proficient at determining when you need to use these tools when you write code.

Up next is going to be learning about JavaScript Objects. Before you go, we would like to present you with this optional challenge exercise. We won't even test your submission. It's up to you to work on this until you feel you have it right. If you want to just move on to Objects instead, that's perfectly fine.

## Optional Challenge: Where Do I Spend My Money?

Have you ever used online banking, or a service like Mint to track your monthly expenses? They can tell you in a concise report how much you spend on food, fuel, utilities, travel, clothing, and entertainment every month.

Before you get to the challenge, you need to understand one of the lines of code in the starter code provided.

### Array Deconstruction and Split

In the sample code provided, you will see the following code. It uses array deconstruction, and the `.split()` method for strings.

```js
const  [ vendor,  amount ]  =  expense.split(":")
```

A brief explanation of `.split()`. Like its name, it splits a string into several smaller strings. You pass it an argument that is the character that splits the strings. Look at the string below. It's one string of names, and each one is separated by a comma. The comma is what you can use to split it into smaller strings.

Juan is the first name. Carlos is the middle name. Rodriguez is the surname. You want to have each of those names stored in their own variable.

```js
const fullName = [ "Juan,Carlos,Rodriguez" ]
```

You can use `.split()` to do this with the following code. It both declares each variable, and assigns each a value all in one line of code.

```js
const [ firstName, middleName, surName ] = fullName.split(",")

console.log(firstName)  // Juan
console.log(middleName)  // Carlos
console.log(surName)  // Rodriguez
```



### Helpful Hints

To convert a string into a number, you can use the following code.

```js
const accountBalance = "2551.30"
console.log(accountBalance)  // Output is "2551.30"
console.log(parseFloat(accountBalance))  // Output is 2551.30
```

You will need to use the logical OR `||` operator in some of your `if` conditions.

<!--stackedit_data:
eyJoaXN0b3J5IjpbOTUzODQxOTQ0XX0=
-->