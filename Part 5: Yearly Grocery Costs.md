---


---

<h2 id="using-the-length-of-an-array">Using the Length of an Array</h2>
<p>Arrays have a <code>.length</code> property that tells you how many items are in the array.</p>
<h2 id="rainfall">Rainfall</h2>
<p>You can perform whatever task you want inside a for loop. In the previous exercises, you have used the <code>.push()</code> methods to build up a new array based on the items in another array. Here is an example of building up a total value.</p>
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

