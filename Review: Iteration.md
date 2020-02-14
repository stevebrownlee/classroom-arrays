---


---

<h2 id="review-of-iteration">Review of Iteration</h2>
<p>Things you used in this classroom.</p>
<ul>
<li><code>for..of</code> loops</li>
<li>Logical operators AND <code>&amp;&amp;</code> and OR <code>||</code></li>
<li>Arrays</li>
<li><code>if/else</code> code blocks for conditional logic</li>
<li><code>.push()</code> method for arrays</li>
<li><code>.length</code> property for arrays</li>
<li><code>.includes()</code> method for strings</li>
<li><code>+=</code> operator to add a any number to a variable’s existing value</li>
<li><code>++</code> operator to add 1 to a variable’s existing value</li>
<li>Division <code>/</code> operator to find averages</li>
</ul>
<p>That’s a lot. We also want to remind you that it’s expected for these concepts and skills to not be solidified just yet. You need a significant amount of practice to become proficient at determining when you need to use these tools when you write code.</p>
<p>Up next is going to be learning about JavaScript Objects. Before you go, we would like to present you with this optional challenge exercise. We won’t even test your submission. It’s up to you to work on this until you feel you have it right. If you want to just move on to Objects instead, that’s perfectly fine.</p>
<h2 id="optional-challenge-where-do-i-spend-my-money">Optional Challenge: Where Do I Spend My Money?</h2>
<p>Have you ever used online banking, or a service like Mint to track your monthly expenses? They can tell you in a concise report how much you spend on food, fuel, utilities, travel, clothing, and entertainment every month.</p>
<p>In the code editor, there is some sample code. It starts with an array filled with your monthly expenses. Each string in the array contains a <code>:</code> delimited string. On the left side of the colon is the vendor, and on the right is the amount of money you spent. Your job is to correctly categorize each expense and put the amount spent in the correct target array.</p>
<ul>
<li>If the vendor contains the sub-string of “Clothing” place the expense amount in the <code>clothing</code> array.</li>
<li>If the vendor contains the sub-string of “Movie” place the expense amount in the <code>entertainment</code> array.</li>
<li>If the vendor contains the sub-string of “Fuel” place the expense amount in the <code>fuel</code> array.</li>
<li>If the vendor contains the sub-string of “Utility” place the expense amount in the <code>utilities</code> array.</li>
<li>If the vendor contains the sub-string of “Groceries” or the sub-string of “Restaurant” place the expense amount in the <code>food</code> array.</li>
<li>If the vendor contains the sub-string of “Lyft” or the sub-string of “Uber” place the expense amount in the <code>travel</code> array.</li>
<li>If the expense amount is greater than 100.00, place the expense amount in the <code>largePurchases</code> array.</li>
</ul>
<h2 id="helpful-hints">Helpful Hints</h2>
<h3 id="turning-a-string-into-a-number">Turning a String into a Number</h3>
<p>To convert a string into a number, you can use the following code.</p>
<pre class=" language-js"><code class="prism  language-js"><span class="token keyword">const</span> accountBalance <span class="token operator">=</span> <span class="token string">"2551.30"</span>
console<span class="token punctuation">.</span><span class="token function">log</span><span class="token punctuation">(</span>accountBalance<span class="token punctuation">)</span>  <span class="token comment">// Output is "2551.30"</span>
console<span class="token punctuation">.</span><span class="token function">log</span><span class="token punctuation">(</span><span class="token function">parseFloat</span><span class="token punctuation">(</span>accountBalance<span class="token punctuation">)</span><span class="token punctuation">)</span>  <span class="token comment">// Output is 2551.30</span>
</code></pre>
<h3 id="logical-operators">Logical Operators</h3>
<p>You will need to use the logical OR <code>||</code> operator in some of your <code>if</code> conditions.</p>

