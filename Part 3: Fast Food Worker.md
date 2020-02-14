## Fast Food

If you have ever had the pleasure of working in a fast food restaurant, you remember how important automation and repitition is. There is very little variation to the food offerings, and there are machines and processes set up to ensure that each product is produced in the same amount of time, with the exact same quantity of ingredients, in the exact same amount of time.

In this exercise, you are going to use the same processes as in the last chapter, but you are going to introduce an `if/else` code block inside the `for` loop. You will still have two arrays. The first contains the raw ingredients for food, and you will be using the `.push()` method to add the finished food product to the other array. However, what value gets inserted into the new array will depend on what the raw ingredient is.

As a review of `if/else` logic, here is a sample determining if the value of a variable is one of three possible states.

```js
const weather = "raining"

if (weather === "raining") {
	console.log("Remember your umbrella")
}
else if (weather === "snowing") {
	console.log("Remember your jacket and scarf")
}
else if (weather === "sunny") {
	console.log("Remember your sunscreen")
}
```

Now here is how you can use it inside a `for..of` loop.

```js
const 
```

## Exercise

There is some beginning code in the code editor. You need to complete it. You need to fill in the proper sections of the `for` loop to iterate the `rawIngredients` array. 

* If the current ingredient is "egg", then add "biscuit" to the finished foods array
* If the current ingredient is "beef patty", then add "burger" to the finished foods array
* If the current ingredient is "potato", then add "fries" to the finished foods array

Don't be shy about looking at the code in your last exercise to help out with this one.

```js
const rawIngredients = [ "beef patty", "egg", "potato", "egg", "potato", "beef patty", "beef patty", "potato" ]
const finishedFood = []

for (const ingredient of rawIngredients) {
	/* 
		Write your if/else code here. In each block use .push() to insert
		the correct item into the finishedFood array.
	*/
}

console.log(finishedFood)
```
<!--stackedit_data:
eyJoaXN0b3J5IjpbOTcxOTk0OTAzLC0xNzU3Mzc2MTcyXX0=
-->