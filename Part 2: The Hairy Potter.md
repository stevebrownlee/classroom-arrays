> Break this up into two chapters. Push in next chapter.


# Iterating an Array

In the last part, you targeted only specific items in an array. More often, you will need to perform a task on **every item** in an array. To do this, software developers write loops. A loop iterates an array - meaning it looks at every item.

Here's a simple array of three pieces of paper.

```js
const originals = [ "Original paper 1", "Original paper 2", "Original paper 3"]
```

The problem software developers run into is that they often don't know how many items are in array. Some code that Bill wrote will build the array. Alice doesn't know how long that array is, but she definitely wants to do something with everything in it.

## Your First For Loop

In JavaScript, there are several ways to iterate through the items in an array.  The specific syntax you will be using is called a `for..of` loop that is designed specifically to iterate an array. You can start with a simple example. You can use a `for..of` loop to output each item in an array to the console.

```js
for (const paper of originals) {
	console.log(paper)
}
```

That would generate the following output in the console.

```html
"Original paper 1"
"Original paper 2"
"Original paper 3"
```

This will work on any array of items that you have in your code. Here is another example.

```js
const teammates = [ "Susan", "Emory", "Seamus", "Adelaide" ]
for (const name of teammates) {
	console.log(name)
}
```

That would generate the following output in the console.

```html
"Susan"
"Emory"
"Seamus"
"Adelaide"
```

## Ah.. Push It

There is a classic hip hop song from the 1980's that I always think of when I want to add a new value to an array. You have already seen that an array has a `.length` property. Arrays also have a method on then named `.push()`. That method lets you add a new value as the last item in the array.

However, we will start off with this simple example where you have three pieces of paper that need to be copied. The original pieces of paper should not be touched. Therefore, you will end up with a new collection - or array - that will contain the copies.

Here's how you can add a new piece of paper to the collection that needs to be copies.

```js
const originals = [ "Original paper 1", "Original paper 2", "Original paper 3" ]

originals.push("Original paper 4")

// This is the new contents of the array
const originals = [ "Original paper 1", "Original paper 2", "Original paper 3", "Original paper 4"]
```

## Making Copies

Now it is time to combine the `for` loop with the `push()` method on an array to make a copy for each item in the `originals` array.

```js
const originals = [ "Original paper 1", "Original paper 2", "Original paper 3" ]
const copies = []  // Blank array that will contain the copies
const numberOfPapers = originals.length

for (let currentIndex = 0; currentIndex < numberOfPapers; currentIndex++) {
	const copy = `Copy of ${originals[currentIndex]}`
	copies.push(copy)
}

console.log(copies)
```

If you have anything in your code editor, go ahead and delete it all. Then take that code above and put it in the code editor and run it. You will see the new array displayed in the console below the editor.

## Step By Step

Below you will see the values of each variable as the `for` loop iterates the collection.

First iteration.

```js
for (let currentIndex = 0; 0 < 3; currentIndex = 1) {
	const copy = `Copy of "Original paper 1"`
	copies.push(copy)
}
```

Second iteration.

```js
for (let currentIndex = 0; 1 < 3; currentIndex = 2) {
	const copy = `Copy of "Original paper 2"`
	copies.push(copy)
}
```

Third iteration.

```js
for (let currentIndex = 0; 2 < 3; currentIndex = 3) {
	const copy = `Copy of "Original paper 3"`
	copies.push(copy)
}
```

The evaluation after the third iteration evaluates to false, so the loop ends and the code inside the curly braces does not execute.

```js
for (let currentIndex = 0; 3 < 3; currentIndex = 3) {
}
```

## Exercise: The Hairy Potter

Delete everything that you currently have in the code editor. Copy and paste the following code into the editor. In this exercise, you are writing code to automate what a potter does: turn clay into pottery.

Your task is to iterate the array containing the chunks of clay and after your code is done, the `toFireInKiln` array should contain the string value "coffee mug" for every chunk of clay in the `clay` array.

> Reminder: You can make all of your variable names the same as the example, or you can change them if you want to be crazy. Just to remind you that JavaScript doesn't care what you name your variables. For example, we chose the variable name `currentIndex` to represent the index of the array, but it doesn't have to be that name. You could name it `index`, `idx`, `i`, or even `moonDust` if you like. It's not a descriptive name, but you can do it anyway, as long as you use `moonDust` everywhere `currentIndex` is currently used.

```js
const clay = [ "Chunk of clay", "Chunk of clay", "Chunk of clay", "Chunk of clay" ]
const toFireInKiln = []

for () {
   const mug = "coffee mug"
}

console.log(toFireInKiln)
```



<!--stackedit_data:
eyJoaXN0b3J5IjpbLTMxMzc3NzU2OSwtMzQyNzU2MDY5LDEwNz
cxMTgxMTcsMjk4MDkzMDIwLC0xODc3OTIzNDcwXX0=
-->