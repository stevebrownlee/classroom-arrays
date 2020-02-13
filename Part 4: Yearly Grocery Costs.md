## Concise For Loop Syntax

The traditional `for` loop that you used in the past two exercises is the most basic way to perform the same task over and over again a certain number of times. In JavaScript, there is a specific kind of loop called a `for..of` loop that is designed specifically to iterate an array. 

## Cars

Here's a quick example.

```js
// Inventory of a used car lot
const carLot = [ "Pinto", "F150", "Cabriolet", "Sentra", "Xterra", "Ram" ]

for (const car of carLot) {
	console.log(car)
}
```

In this kind of loop, you don't need to worry about accessing individual items using the `array[index]` syntax, and you don't have to increment any variables. All you need to do is declare a variable to store the current item, and the `for..of` loop will assign it the correct value as it iterates the array.

Go ahead and copy that code into the code editor and run it. You will see each car model in the console output.

## Flowers

Here's another example.

```js
// Inventory of a flower shop
const flowerInventory = [ "Tulips", "Roses", "Daisies", "Daffodils", "Irises", "Chrysanthemums" ]

for (const flower of flowerInventory) {
	console.log(flower)
}
```

Put that code in the code editor and run it to see the output.

## Rainfall

You do perform whatever action you want inside a for loop. In the previous exercises, you have used the `.push()` methods to build up a new array based on the items in another array. Here is an example of building up a total value.

Reminder that arrays have a `.length` property that tells you how many items are in the array.

A meterologist wants to determine what the total rainfall for a year was, and then calculate the average rainfall per month.

```js
const rainfallPerMonth = [ 5, 12, 18, 20, 22, 17, 29, 21, 20, 22, 30, 9 ]
let totalRainfall = 0  // Start at 0 and add to it in the loop

for (const rain of rainfallPerMonth) {
	totalRainfall += rain
}

// To find the average, you take the total and divide by the number of items
const averageRainfall = totalRainfall / rainfallPerMonth.length

console.log(`Total rainfall was ${totalRainfall} inches
Average rainfall was ${averageRainfall} inches
`)
```

Put that code into the code editor and run it to see the output.

## Exercise: Grocery Shopper

In this exercise, you will write code to calculate your average monthly grocery expenses. So far, you have collected five months' worth of expenses.

```js
const monthlyExpenses = [ 201.43, 189.22, 132.09,  238.85, 195.41 ]
let totalExpense = 0

for (const xxx of xxx) {
	// Add the current monthly cost to the value of totalExpense
}

// Calculate your average monthly food costs
const averageExpense = 

// Make sure you use backticks for multi-line string output
console.log()
```

Your ouput should look like format, with the correct values in it instead of the `xxx` placeholders.

```html
On average, I spend xxx dollars on groceries per month.
So far this year, I have spent xxx dollars on groceries.
```





Test output....

On average, I spend 191.4 dollars on groceries per month.
So far this year, I have spent 957 dollars on groceries.


<!--stackedit_data:
eyJoaXN0b3J5IjpbLTM3Nzc5NDg1OV19
-->