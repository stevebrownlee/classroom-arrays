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

## Your Topics of Study

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



<!--stackedit_data:
eyJoaXN0b3J5IjpbMTE4Nzk1MDk1MiwtMzQyNzU2MDY5LDEwNz
cxMTgxMTcsMjk4MDkzMDIwLC0xODc3OTIzNDcwXX0=
-->