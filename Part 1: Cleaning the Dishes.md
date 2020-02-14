---


---

<h2 id="position-of-items-in-an-array">Position of Items in an Array</h2>
<p>As mentioned in the introduction, the most common type of collection in JavaScript is the array. An array can be identified by use of square brackets.  The <code>[</code> and the <code>]</code> characters define an array. Here’s a simple definition of an array. Think of it as an empty basket.  Nothing is in it yet.</p>
<pre class=" language-js"><code class="prism  language-js"><span class="token keyword">const</span> appleBasket <span class="token operator">=</span> <span class="token punctuation">[</span><span class="token punctuation">]</span>
</code></pre>
<p>This is different than previous exercises where you assigned very concrete values to variables, like these.</p>
<pre class=" language-js"><code class="prism  language-js"><span class="token keyword">const</span> age <span class="token operator">=</span> <span class="token number">37</span>  <span class="token comment">// Clear, concrete numeric value</span>
<span class="token keyword">const</span> name <span class="token operator">=</span> <span class="token string">"Edward McKnight"</span> <span class="token comment">// Clear, concrete string value</span>
</code></pre>
<p>You can either declare a new array as empty, like above, or you can provide it with initial values upon declaration. For example, if you want some common color names to be in your array, you can provide those inside the square brackets.</p>
<pre class=" language-js"><code class="prism  language-js"><span class="token keyword">const</span> myFavoriteColors <span class="token operator">=</span> <span class="token punctuation">[</span> <span class="token string">"red"</span><span class="token punctuation">,</span> <span class="token string">"violet"</span><span class="token punctuation">,</span> <span class="token string">"pink"</span><span class="token punctuation">,</span> <span class="token string">"green"</span><span class="token punctuation">,</span> <span class="token string">"white"</span><span class="token punctuation">,</span> <span class="token string">"orange"</span> <span class="token punctuation">]</span>
</code></pre>
<p>The <code>myFavoriteColors</code> variable still has a single value, but it is more abstract. Its value is a collection of strings, or more specifically, an array of strings.</p>
<p>The placement of each number in that array is called its “index”. The indexing of an array starts at zero, not one. That is, the item at index 0 of the above array is the string value “red”.</p>
<ul>
<li>The item at index 0 is the string “red”</li>
<li>The item at index 1 is the string “violet”</li>
<li>The item at index 2 is the string “pink”</li>
<li>The item at index 3 is the string “green”</li>
<li>The item at index 4 is the string “white”</li>
<li>The item at index 5 is the string “orange”</li>
</ul>
<p>You can, if you need to, look at the item at a specific index by using the following syntax.</p>
<pre class=" language-js"><code class="prism  language-js">arrayVariable<span class="token punctuation">[</span>index number<span class="token punctuation">]</span>
</code></pre>
<p>So if you want to <code>console.log()</code> the color “white”, you would write the following code.</p>
<pre class=" language-js"><code class="prism  language-js"><span class="token keyword">const</span> whiteColor <span class="token operator">=</span> myFavoriteColors<span class="token punctuation">[</span><span class="token number">4</span><span class="token punctuation">]</span>
console<span class="token punctuation">.</span><span class="token function">log</span><span class="token punctuation">(</span>whiteColor<span class="token punctuation">)</span>
</code></pre>
<p>If you want to <code>console.log()</code> the color “violet”, you would write the following code.</p>
<pre class=" language-js"><code class="prism  language-js"><span class="token keyword">const</span> violetColor <span class="token operator">=</span> myFavoriteColors<span class="token punctuation">[</span><span class="token number">1</span><span class="token punctuation">]</span>
console<span class="token punctuation">.</span><span class="token function">log</span><span class="token punctuation">(</span>violetColor<span class="token punctuation">)</span>
</code></pre>
<h2 id="exercise-glass-scrubber">Exercise: Glass Scrubber</h2>
<p>You work in a fancy restaurant. You are in your first month, and everyone they hire starts in the kitchen as a dish cleaner. Your job, specifically, is to scrub the glasses clean. Over in the code editor, you will find an array of dirty dishes. This represents the large sink in the back of the restaurant where the waiter place all of the dirty dishes.</p>
<p>Your job is to identify the 3 dirty glasses by using the their index in the array and assign them to a corresponding variable. When you run the code, it should display the following.</p>
<pre class=" language-html"><code class="prism  language-html">I am cleaning the following glasses:
- Water glass
- Wine glass
- Whiskey glass
</code></pre>
<pre class=" language-js"><code class="prism  language-js"><span class="token keyword">const</span> dirtyDishes <span class="token operator">=</span> <span class="token punctuation">[</span> <span class="token string">"Whiskey glass"</span><span class="token punctuation">,</span> <span class="token string">"Dinner plate"</span><span class="token punctuation">,</span> <span class="token string">"Platter"</span><span class="token punctuation">,</span> <span class="token string">"Water glass"</span><span class="token punctuation">,</span> <span class="token string">"Salad plate"</span><span class="token punctuation">,</span> <span class="token string">"Wine glass"</span> <span class="token punctuation">]</span>


<span class="token keyword">const</span> waterGlass <span class="token operator">=</span> dirtyDishes<span class="token punctuation">[</span><span class="token number">0</span><span class="token punctuation">]</span>
<span class="token keyword">const</span> wineGlass <span class="token operator">=</span> dirtyDishes<span class="token punctuation">[</span><span class="token number">3</span><span class="token punctuation">]</span>
<span class="token keyword">const</span> whiskeyGlass <span class="token operator">=</span> dirtyDishes<span class="token punctuation">[</span><span class="token number">5</span><span class="token punctuation">]</span>

console<span class="token punctuation">.</span><span class="token function">log</span><span class="token punctuation">(</span><span class="token template-string"><span class="token string">`I am cleaning the following glasses:
* </span><span class="token interpolation"><span class="token interpolation-punctuation punctuation">${</span>waterGlass<span class="token interpolation-punctuation punctuation">}</span></span><span class="token string">
* </span><span class="token interpolation"><span class="token interpolation-punctuation punctuation">${</span>wineGlass<span class="token interpolation-punctuation punctuation">}</span></span><span class="token string">
* </span><span class="token interpolation"><span class="token interpolation-punctuation punctuation">${</span>whiskeyGlass<span class="token interpolation-punctuation punctuation">}</span></span><span class="token string">
`</span></span><span class="token punctuation">)</span>
</code></pre>

<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE4MzE5NjM1OTBdfQ==
-->