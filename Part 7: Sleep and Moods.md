---


---

<h2 id="conditions-in-loops">Conditions in Loops</h2>
<p>You are going to practice your <code>for..of</code> loops some more. In this exercise, you are going to add a <code>if/else</code> code block inside the loop.</p>
<p>A quick example first.</p>
<pre class=" language-js"><code class="prism  language-js"><span class="token keyword">const</span> wines <span class="token operator">=</span> <span class="token punctuation">[</span> <span class="token string">"red"</span><span class="token punctuation">,</span> <span class="token string">"white"</span><span class="token punctuation">,</span> <span class="token string">"white"</span><span class="token punctuation">,</span> <span class="token string">"white"</span><span class="token punctuation">,</span> <span class="token string">"red"</span><span class="token punctuation">,</span> <span class="token string">"white"</span><span class="token punctuation">,</span> <span class="token string">"red"</span> <span class="token punctuation">]</span>
<span class="token keyword">const</span> wineCellar <span class="token operator">=</span> <span class="token punctuation">[</span><span class="token punctuation">]</span>
<span class="token keyword">const</span> wineRefrigerator <span class="token operator">=</span> <span class="token punctuation">[</span><span class="token punctuation">]</span>

<span class="token keyword">for</span> <span class="token punctuation">(</span><span class="token keyword">const</span> wine <span class="token keyword">of</span> wines<span class="token punctuation">)</span> <span class="token punctuation">{</span>
	<span class="token keyword">if</span> <span class="token punctuation">(</span>wine <span class="token operator">===</span> <span class="token string">"red"</span><span class="token punctuation">)</span> <span class="token punctuation">{</span>
		wineCellar<span class="token punctuation">.</span><span class="token function">push</span><span class="token punctuation">(</span>wine<span class="token punctuation">)</span>
	<span class="token punctuation">}</span>
	<span class="token keyword">else</span> <span class="token punctuation">{</span>
		wineRefrigerator<span class="token punctuation">.</span><span class="token function">push</span><span class="token punctuation">(</span>wine<span class="token punctuation">)</span>
	<span class="token punctuation">}</span>
<span class="token punctuation">}</span>

console<span class="token punctuation">.</span><span class="token function">log</span><span class="token punctuation">(</span><span class="token template-string"><span class="token string">`
Contents of wine cellar: </span><span class="token interpolation"><span class="token interpolation-punctuation punctuation">${</span>wineCellar<span class="token interpolation-punctuation punctuation">}</span></span><span class="token string">
Contents of wine refrigerator: </span><span class="token interpolation"><span class="token interpolation-punctuation punctuation">${</span>wineRefrigerator<span class="token interpolation-punctuation punctuation">}</span></span><span class="token string">
`</span></span><span class="token punctuation">)</span>
</code></pre>
<p>Feel free to copy that code into the editor and run it to see what happens.</p>
<p>In that example, you still iterate the entire array, but depending on the value of the <code>wine</code> variable, one of two different things could happen.</p>
<h2 id="exercise-sleep-mode">Exercise: Sleep Mode</h2>
<p>You decide to track how much your sleep affects your mood on a day-to-day basis. You notice that if you get less than 7 hours of sleep, you are grumpy all day long. If you get 7 or more hours of sleep, you are in a happy mood all day.</p>
<p>You start recording how many hours of sleep you get every night for two weeks. Based on the hours of sleep, you want to generate a readable report that shows you how many days you were grumpy and how many days you were happy.</p>
<p>There is an array already in the code editor of your tracked hours of sleep. You need to complete the code using the above code as an example. One thing you will do differently is instead of putting the array in the output like the example does, you need to display the number of items in <code>grumpyHours</code> and the number of items in the <code>happyHours</code> arrays.</p>
<h5 id="example-output">Example Output</h5>
<p>This is just an example. Your output will have different numbers.</p>
<pre class=" language-html"><code class="prism  language-html">I was grumpy on 14 days.
I was happy on 22 days.
</code></pre>
<h2 id="code-to-give">Code To Give</h2>
<pre class=" language-js"><code class="prism  language-js"><span class="token keyword">const</span> hours <span class="token operator">=</span> <span class="token punctuation">[</span> <span class="token number">6</span><span class="token punctuation">,</span> <span class="token number">9</span><span class="token punctuation">,</span> <span class="token number">7</span><span class="token punctuation">,</span> <span class="token number">8</span><span class="token punctuation">,</span> <span class="token number">6</span><span class="token punctuation">,</span> <span class="token number">6</span><span class="token punctuation">,</span> <span class="token number">8</span><span class="token punctuation">,</span> <span class="token number">5</span><span class="token punctuation">,</span> <span class="token number">9</span><span class="token punctuation">,</span> <span class="token number">8</span><span class="token punctuation">,</span> <span class="token number">7</span><span class="token punctuation">,</span> <span class="token number">6</span><span class="token punctuation">,</span> <span class="token number">7</span><span class="token punctuation">,</span> <span class="token number">7</span><span class="token punctuation">,</span> <span class="token number">8</span><span class="token punctuation">,</span> <span class="token number">6</span><span class="token punctuation">,</span> <span class="token number">9</span> <span class="token punctuation">]</span>
<span class="token keyword">const</span> grumpyHours <span class="token operator">=</span> <span class="token punctuation">[</span><span class="token punctuation">]</span>
<span class="token keyword">const</span> happyHours <span class="token operator">=</span> <span class="token punctuation">[</span><span class="token punctuation">]</span>

console<span class="token punctuation">.</span><span class="token function">log</span><span class="token punctuation">(</span><span class="token punctuation">)</span>
</code></pre>

