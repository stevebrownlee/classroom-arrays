## Iterating an Array

In the last part, you targeted only specific items in an array. More often, you will need to perform a task on **every item** in an array. To do this, software developers write loops. A loop iterates an array - meaning it looks at every item.

You also often don't know - or don't care - how many items are in array. You just want to perform some task with each item.

## Concise For Loop Syntax

In JavaScript, there is a specific kind of loop called a `for..of` loop that is designed specifically to iterate an array. 

With a `for..of` loop, you don't need to worry about accessing individual items using the `array[index]` syntax. All you need to do is declare a variable to store the current item, and the `for..of` loop will assign it the correct value as it iterates the array.

Go ahead and copy the following code into the code editor and run it. You will see each car model in the console output.

## Cars

Here's a quick example.

```js
// Inventory of a used car lot
const carLot = [ "Pinto", "F150", "Cabriolet", "Sentra", "Xterra", "Ram" ]

for (const car of carLot) {
	console.log(car)
}
```

That would generate the following output in the console.

```html
Pinto
F150
Cabriolet
Sentra
Xterra
Ram
```

## Papers to Copy

Here's a simple array of three pieces of paper. The variable of `paper` inside the `for` statement is where the variable is both declared and assigned a value as the code walks through the array one item at a time.

```js
const originals = [ "Original paper 1", "Original paper 2", "Original paper 3"]

for (const paper of originals) {
	console.log(paper)
}
```

That would generate the following output in the console.

```html
Original paper 1
Original paper 2
Original paper 3
```

This will work on any array of items that you have in your code. Here is another example. Remember that you can name your variables anything you want, and make sure the name is relevant (i.e. provides context) for the value that is assigned to it.

```js
const teammates = [ "Susan", "Emory", "Seamus", "Adelaide" ]

for (const name of teammates) {
	console.log(name)
}
```

That would generate the following output in the console.

```html
Susan
Emory
Seamus
Adelaide
```

## Your Topics of Study

**Before you do the exercise, erase any code that you currently have in the code editor**

While you learn JavaScript, there are many topics that you will cover.

* Variables
* Loops
* Arrays
* Functions
* Objects
* Modules
* Events

Copy the code below into the editor. Then you need to take those topics above and put them in the `topics` array. Then, using the examples above, write a `for..of` loop that outputs them to the console.

```js
const topics = [  ]

for () {

}
```



