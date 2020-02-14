---


---

<h2 id="concise-for-loop-syntax">Concise For Loop Syntax</h2>
<p>The traditional <code>for</code> loop that you used in the past two exercises is the most basic way to perform the same task over and over again a certain number of times. In JavaScript, there is a specific kind of loop called a <code>for..of</code> loop that is designed specifically to iterate an array.</p>
<h2 id="cars">Cars</h2>
<p>Here’s a quick example.</p>
<pre class=" language-js"><code class="prism  language-js"><span class="token comment">// Inventory of a used car lot</span>
<span class="token keyword">const</span> carLot <span class="token operator">=</span> <span class="token punctuation">[</span> <span class="token string">"Pinto"</span><span class="token punctuation">,</span> <span class="token string">"F150"</span><span class="token punctuation">,</span> <span class="token string">"Cabriolet"</span><span class="token punctuation">,</span> <span class="token string">"Sentra"</span><span class="token punctuation">,</span> <span class="token string">"Xterra"</span><span class="token punctuation">,</span> <span class="token string">"Ram"</span> <span class="token punctuation">]</span>

<span class="token keyword">for</span> <span class="token punctuation">(</span><span class="token keyword">const</span> car <span class="token keyword">of</span> carLot<span class="token punctuation">)</span> <span class="token punctuation">{</span>
	console<span class="token punctuation">.</span><span class="token function">log</span><span class="token punctuation">(</span>car<span class="token punctuation">)</span>
<span class="token punctuation">}</span>
</code></pre>
<p>In this kind of loop, you don’t need to worry about accessing individual items using the <code>array[index]</code> syntax, and you don’t have to increment any variables. All you need to do is declare a variable to store the current item, and the <code>for..of</code> loop will assign it the correct value as it iterates the array.</p>
<p>Go ahead and copy that code into the code editor and run it. You will see each car model in the console output.</p>
<h2 id="flowers">Flowers</h2>
<p>Here’s another example.</p>
<pre class=" language-js"><code class="prism  language-js"><span class="token comment">// Inventory of a flower shop</span>
<span class="token keyword">const</span> flowerInventory <span class="token operator">=</span> <span class="token punctuation">[</span> <span class="token string">"Tulips"</span><span class="token punctuation">,</span> <span class="token string">"Roses"</span><span class="token punctuation">,</span> <span class="token string">"Daisies"</span><span class="token punctuation">,</span> <span class="token string">"Daffodils"</span><span class="token punctuation">,</span> <span class="token string">"Irises"</span><span class="token punctuation">,</span> <span class="token string">"Chrysanthemums"</span> <span class="token punctuation">]</span>

<span class="token keyword">for</span> <span class="token punctuation">(</span><span class="token keyword">const</span> flower <span class="token keyword">of</span> flowerInventory<span class="token punctuation">)</span> <span class="token punctuation">{</span>
	console<span class="token punctuation">.</span><span class="token function">log</span><span class="token punctuation">(</span>flower<span class="token punctuation">)</span>
<span class="token punctuation">}</span>
</code></pre>
<p>Put that code in the code editor and run it to see the output.</p>
<h2 id="rainfall">Rainfall</h2>
<p>You do perform whatever action you want inside a for loop. In the previous exercises, you have used the <code>.push()</code> methods to build up a new array based on the items in another array. Here is an example of building up a total value.</p>
<p>Reminder that arrays have a <code>.length</code> property that tells you how many items are in the array.</p>
<p>A meterologist wants to determine what the total rainfall for a year was, and then calculate the average rainfall per month.</p>
<pre class=" language-js"><code class="prism  language-js"><span class="token keyword">const</span> rainfallPerMonth <span class="token operator">=</span> <span class="token punctuation">[</span> <span class="token number">5</span><span class="token punctuation">,</span> <span class="token number">12</span><span class="token punctuation">,</span> <span class="token number">18</span><span class="token punctuation">,</span> <span class="token number">20</span><span class="token punctuation">,</span> <span class="token number">22</span><span class="token punctuation">,</span> <span class="token number">17</span><span class="token punctuation">,</span> <span class="token number">29</span><span class="token punctuation">,</span> <span class="token number">21</span><span class="token punctuation">,</span> <span class="token number">20</span><span class="token punctuation">,</span> <span class="token number">22</span><span class="token punctuation">,</span> <span class="token number">30</span><span class="token punctuation">,</span> <span class="token number">9</span> <span class="token punctuation">]</span>
<span class="token keyword">let</span> totalRainfall <span class="token operator">=</span> <span class="token number">0</span>  <span class="token comment">// Start at 0 and add to it in the loop</span>

<span class="token keyword">for</span> <span class="token punctuation">(</span><span class="token keyword">const</span> rain <span class="token keyword">of</span> rainfallPerMonth<span class="token punctuation">)</span> <span class="token punctuation">{</span>
	totalRainfall <span class="token operator">+=</span> rain
<span class="token punctuation">}</span>

<span class="token comment">// To find the average, you take the total and divide by the number of items</span>
<span class="token keyword">const</span> averageRainfall <span class="token operator">=</span> totalRainfall <span class="token operator">/</span> rainfallPerMonth<span class="token punctuation">.</span>length

console<span class="token punctuation">.</span><span class="token function">log</span><span class="token punctuation">(</span><span class="token template-string"><span class="token string">`Total rainfall was </span><span class="token interpolation"><span class="token interpolation-punctuation punctuation">${</span>totalRainfall<span class="token interpolation-punctuation punctuation">}</span></span><span class="token string"> inches
Average rainfall was </span><span class="token interpolation"><span class="token interpolation-punctuation punctuation">${</span>averageRainfall<span class="token interpolation-punctuation punctuation">}</span></span><span class="token string"> inches
`</span></span><span class="token punctuation">)</span>
</code></pre>
<p>Put that code into the code editor and run it to see the output.</p>
<h2 id="exercise-grocery-shopper">Exercise: Grocery Shopper</h2>
<p>In this exercise, you will write code to calculate your average monthly grocery expenses. So far, you have collected five months’ worth of expenses.</p>
<pre class=" language-js"><code class="prism  language-js"><span class="token keyword">const</span> monthlyExpenses <span class="token operator">=</span> <span class="token punctuation">[</span> <span class="token number">201.43</span><span class="token punctuation">,</span> <span class="token number">189.22</span><span class="token punctuation">,</span> <span class="token number">132.09</span><span class="token punctuation">,</span>  <span class="token number">238.85</span><span class="token punctuation">,</span> <span class="token number">195.41</span> <span class="token punctuation">]</span>
<span class="token keyword">let</span> totalExpense <span class="token operator">=</span> <span class="token number">0</span>

<span class="token keyword">for</span> <span class="token punctuation">(</span><span class="token keyword">const</span> xxx <span class="token keyword">of</span> xxx<span class="token punctuation">)</span> <span class="token punctuation">{</span>
	<span class="token comment">// Add the current monthly cost to the value of totalExpense</span>
<span class="token punctuation">}</span>

<span class="token comment">// Calculate your average monthly food costs</span>
<span class="token keyword">const</span> averageExpense <span class="token operator">=</span> 

<span class="token comment">// Make sure you use backticks for multi-line string output</span>
console<span class="token punctuation">.</span><span class="token function">log</span><span class="token punctuation">(</span><span class="token punctuation">)</span>
</code></pre>
<p>Your output should look like format, with the correct values in it instead of the <code>xxx</code> placeholders.</p>
<pre class=" language-html"><code class="prism  language-html">On average, I spend xxx dollars on groceries per month.
So far this year, I have spent xxx dollars on groceries.
</code></pre>
<p>Test output…</p>
<p>On average, I spend 191.4 dollars on groceries per month.<br>
So far this year, I have spent 957 dollars on groceries.</p>

