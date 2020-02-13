# Iterating an Array

In the last part, you targeted only specific items in an array. More often, you will need to perform a task on **every item** in an array. To do this, software developers write loops. A loop iterates an array - meaning it looks at every item.

Here's a simple array of three pieces of paper.

```js
const originals = [ "Original paper", "Original paper", "Original paper"]
```

The problem software developers run into is that they often don't know how many items are in array. Some code that Bill wrote will build the array. Alice doesn't know how long that array is, but she definitely wants to do something with everything in it.

However, we will start off with this simple example where you have three pieces of paper that need to be copied. The original pieces of paper should not be touched. Therefore, you will end up with a new collection - or array - that will contain the copies.

```js
const originals = [ "Original paper 1", "Original paper 2", "Original paper 3"]
const copies = []  // Blank array that will contain the copies
```

## Your First For Loop

The task we want to perform is to put a copy into the `copies` array for every piece of paper in the `originals` array.

The first step is to determine how many piece of paper are in the `originals` array. JavaScript provides you a property on any array you create named `length`. To access a property of something in JavaScript, you use a period - developers call it a "dot" - and then the name of the property.

```js
// Length property of originals array
const numberOfPapers = originals.length
```

Since there are three items in the originals array, JavaScript turns that code above into the following code.

```js
// Length property of originals array
const numberOfPapers = 3
```

Ok, now that you have the number of times you need to perform the task of making copies, you can write a `for` loop. The syntax is daunting when you first see it, but after enough practice, it will become automatic. In later chapters, you will also learn more concise syntax.

```js
for (let currentIndex = 0; currentIndex < numberOfPapers; currentIndex++) {
	console.log(originals[currentIndex])
}
```

The first part of the for loop is the initalizer: `let currentIndex = 0`

This is where you specify which index you want to look at first. Remember in the last chapter that the index is the position of a certain value in an array. Array indexing starts with 0. So in the for loop, we are letting JavaScript know the we want to start with the very first item in the array.

The second part is the evaluation section: `currentIndex < numberOfPapers`

If the condition in this section evaluates to true, all of the code inside the curly braces `{ }` will execute. When this condition is first evaluated, JavaScript sees the following condition: `0 < 3`. Is 0 less than 3? Of course, so it evaluates to `true` and the code executes.

The third part is the incrementor: `currentIndex++`

After the code inside the curly braces executes, the code you write here will execute. It's where you can specify what to do with your initialized variable. In this case, you are incrementing its value by 1.  The `++` operator after a variable with a numeric value will add 1 to its current value.

## Ah.. Push It

There is a classic hip hop song from the 1980's that I always think of when I want to add a new value to an array. You have already seen that an array has a `.length` property. Arrays also have a method on then named `.push()`. That method lets you add a new value as the last item in the array.

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
   const mug = "Dried mug"
}

console.log(toFireInKiln)
```



<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE4Nzc5MjM0NzBdfQ==
-->