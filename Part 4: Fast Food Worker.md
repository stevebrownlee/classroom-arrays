---


---

<h2 id="fast-food">Fast Food</h2>
<p>If you have ever had the pleasure of working in a fast food restaurant, you remember how important automation and repitition is. There is very little variation to the food offerings, and there are machines and processes set up to ensure that each product is produced in the same amount of time, with the exact same quantity of ingredients, in the exact same amount of time.</p>
<p>In this exercise, you are going to use the same processes as in the last chapter, but you are going to introduce an <code>if/else</code> code block inside the <code>for</code> loop. You will still have two arrays. The first contains the raw ingredients for food, and you will be using the <code>.push()</code> method to add the finished food product to the other array. However, what value gets inserted into the new array will depend on what the raw ingredient is.</p>
<p>As a review of <code>if/else</code> logic, here is a sample determining if the value of a variable is one of three possible states.</p>
<pre class=" language-js"><code class="prism  language-js"><span class="token keyword">const</span> weather <span class="token operator">=</span> <span class="token string">"raining"</span>

<span class="token keyword">if</span> <span class="token punctuation">(</span>weather <span class="token operator">===</span> <span class="token string">"raining"</span><span class="token punctuation">)</span> <span class="token punctuation">{</span>
	console<span class="token punctuation">.</span><span class="token function">log</span><span class="token punctuation">(</span><span class="token string">"Remember your umbrella"</span><span class="token punctuation">)</span>
<span class="token punctuation">}</span>
<span class="token keyword">else</span> <span class="token keyword">if</span> <span class="token punctuation">(</span>weather <span class="token operator">===</span> <span class="token string">"snowing"</span><span class="token punctuation">)</span> <span class="token punctuation">{</span>
	console<span class="token punctuation">.</span><span class="token function">log</span><span class="token punctuation">(</span><span class="token string">"Remember your jacket and scarf"</span><span class="token punctuation">)</span>
<span class="token punctuation">}</span>
<span class="token keyword">else</span> <span class="token keyword">if</span> <span class="token punctuation">(</span>weather <span class="token operator">===</span> <span class="token string">"sunny"</span><span class="token punctuation">)</span> <span class="token punctuation">{</span>
	console<span class="token punctuation">.</span><span class="token function">log</span><span class="token punctuation">(</span><span class="token string">"Remember your sunscreen"</span><span class="token punctuation">)</span>
<span class="token punctuation">}</span>
</code></pre>
<p>Now here is how you can use it inside a <code>for..of</code> loop.</p>
<pre class=" language-js"><code class="prism  language-js"><span class="token keyword">const</span> babies <span class="token operator">=</span> <span class="token punctuation">[</span> <span class="token string">"puppy"</span><span class="token punctuation">,</span> <span class="token string">"kitten"</span><span class="token punctuation">,</span> <span class="token string">"puppy"</span><span class="token punctuation">,</span> <span class="token string">"duckling"</span><span class="token punctuation">,</span> <span class="token string">"puppy"</span><span class="token punctuation">,</span> <span class="token string">"kitten"</span><span class="token punctuation">,</span> <span class="token string">"duckling"</span><span class="token punctuation">,</span> <span class="token string">"kitten"</span> <span class="token punctuation">]</span>
<span class="token keyword">const</span> grownAnimals <span class="token operator">=</span> <span class="token punctuation">[</span><span class="token punctuation">]</span>

<span class="token keyword">for</span> <span class="token punctuation">(</span><span class="token keyword">const</span> baby <span class="token keyword">of</span> babies<span class="token punctuation">)</span> <span class="token punctuation">{</span>
	<span class="token keyword">if</span> <span class="token punctuation">(</span>baby <span class="token operator">===</span> <span class="token string">"puppy"</span><span class="token punctuation">)</span> <span class="token punctuation">{</span>
		grownAnimals<span class="token punctuation">.</span><span class="token function">push</span><span class="token punctuation">(</span><span class="token string">"dog"</span><span class="token punctuation">)</span>
	<span class="token punctuation">}</span>
	<span class="token keyword">else</span> <span class="token keyword">if</span> <span class="token punctuation">(</span>baby <span class="token operator">===</span> <span class="token string">"kitten"</span><span class="token punctuation">)</span> <span class="token punctuation">{</span>
		grownAnimals<span class="token punctuation">.</span><span class="token function">push</span><span class="token punctuation">(</span><span class="token string">"cat"</span><span class="token punctuation">)</span>
	<span class="token punctuation">}</span>
	<span class="token keyword">else</span> <span class="token keyword">if</span> <span class="token punctuation">(</span>baby <span class="token operator">===</span> <span class="token string">"duckling"</span><span class="token punctuation">)</span> <span class="token punctuation">{</span>
		grownAnimals<span class="token punctuation">.</span><span class="token function">push</span><span class="token punctuation">(</span><span class="token string">"duck"</span><span class="token punctuation">)</span>
	<span class="token punctuation">}</span>
<span class="token punctuation">}</span>

console<span class="token punctuation">.</span><span class="token function">log</span><span class="token punctuation">(</span>grownAnimals<span class="token punctuation">)</span>
<span class="token comment">// [ "dog", "cat", "dog", "duck", "dog", "cat", "duck", "cat" ]</span>
</code></pre>
<h2 id="exercise">Exercise</h2>
<p>There is some beginning code in the code editor. You need to complete it. You need to fill in the proper sections of the <code>for</code> loop to iterate the <code>rawIngredients</code> array.</p>
<ul>
<li>If the current ingredient is “egg”, then add “biscuit” to the finished foods array</li>
<li>If the current ingredient is “beef patty”, then add “burger” to the finished foods array</li>
<li>If the current ingredient is “potato”, then add “fries” to the finished foods array</li>
</ul>
<p>Don’t be shy about looking at the code in your last exercise to help out with this one.</p>
<pre class=" language-js"><code class="prism  language-js"><span class="token keyword">const</span> rawIngredients <span class="token operator">=</span> <span class="token punctuation">[</span> <span class="token string">"beef patty"</span><span class="token punctuation">,</span> <span class="token string">"egg"</span><span class="token punctuation">,</span> <span class="token string">"potato"</span><span class="token punctuation">,</span> <span class="token string">"egg"</span><span class="token punctuation">,</span> <span class="token string">"potato"</span><span class="token punctuation">,</span> <span class="token string">"beef patty"</span><span class="token punctuation">,</span> <span class="token string">"beef patty"</span><span class="token punctuation">,</span> <span class="token string">"potato"</span> <span class="token punctuation">]</span>
<span class="token keyword">const</span> finishedFood <span class="token operator">=</span> <span class="token punctuation">[</span><span class="token punctuation">]</span>

<span class="token keyword">for</span> <span class="token punctuation">(</span><span class="token keyword">const</span> ingredient <span class="token keyword">of</span> rawIngredients<span class="token punctuation">)</span> <span class="token punctuation">{</span>
	<span class="token comment">/* 
		Write your if/else code here. In each block use .push() to insert
		the correct item into the finishedFood array.
	*/</span>
<span class="token punctuation">}</span>

console<span class="token punctuation">.</span><span class="token function">log</span><span class="token punctuation">(</span>finishedFood<span class="token punctuation">)</span>
</code></pre>

