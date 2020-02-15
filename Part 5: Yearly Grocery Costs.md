## Using the Length of an Array

Arrays have a `.length` property that tells you how many items are in the array.

## Rainfall

You can perform whatever task you want inside a for loop. In the previous exercises, you have used the `.push()` methods to build up a new array based on the items in another array. Here is an example of building up a total value.

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

**Copy the following code into the code editor**

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

Your output should look like format, with the correct values in it instead of the `xxx` placeholders.

```html
On average, I spend xxx dollars on groceries per month.
So far this year, I have spent xxx dollars on groceries.
```





Test output....

On average, I spend 191.4 dollars on groceries per month.
So far this year, I have spent 957 dollars on groceries.


