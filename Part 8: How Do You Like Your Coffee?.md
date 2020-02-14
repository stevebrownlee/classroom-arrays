---


---

<h2 id="a-string-within-a-string">A String Within a String</h2>
<p>In this exercise, you will use a <code>for..of</code> loop and conditional logic with <code>if/else</code> blocks again. You will also use a new tool to find a smaller string value within a bigger string value. You will also use the logical OR operator <code>||</code>, which is similar to the logical AND operator <code>&amp;&amp;</code> you have used in previous exercises.</p>
<h4 id="quick-incrementing-review">Quick Incrementing Review</h4>
<p>If a variable has a numeric value, you can increase the value by 1 by putting two plus signs after the variable.</p>
<pre class=" language-js"><code class="prism  language-js"><span class="token keyword">let</span> pears <span class="token operator">=</span> <span class="token number">4</span>
pears<span class="token operator">++</span>
console<span class="token punctuation">.</span><span class="token function">log</span><span class="token punctuation">(</span>pears<span class="token punctuation">)</span>  <span class="token comment">// Will output 5</span>
</code></pre>
<h4 id="logical-operators-review">Logical Operators Review</h4>
<p>You have used <code>&amp;&amp;</code> before to check if BOTH conditions are true in order to run some logic.</p>
<pre class=" language-js"><code class="prism  language-js"><span class="token keyword">const</span> pineappleBelongsOnPizza <span class="token operator">=</span> <span class="token boolean">true</span>
<span class="token keyword">const</span> theyWereOnABreak <span class="token operator">=</span> <span class="token boolean">true</span>
<span class="token keyword">const</span> theOfficeIsFunny <span class="token operator">=</span> <span class="token boolean">false</span>

<span class="token keyword">if</span> <span class="token punctuation">(</span>pineappleBelongsOnPizza <span class="token operator">&amp;&amp;</span> theyWereOnABreak<span class="token punctuation">)</span> <span class="token punctuation">{</span>
	<span class="token comment">// Both variables are true, so this code runs</span>
	console<span class="token punctuation">.</span><span class="token function">log</span><span class="token punctuation">(</span><span class="token string">"Basic"</span><span class="token punctuation">)</span>
<span class="token punctuation">}</span>

<span class="token keyword">if</span> <span class="token punctuation">(</span>pineappleBelongsOnPizza <span class="token operator">&amp;&amp;</span> theOfficeIsFunny<span class="token punctuation">)</span> <span class="token punctuation">{</span>
	<span class="token comment">// Since both of the variables' values are not true, this won't run</span>
	console<span class="token punctuation">.</span><span class="token function">log</span><span class="token punctuation">(</span><span class="token string">"Bad"</span><span class="token punctuation">)</span>
<span class="token punctuation">}</span>
</code></pre>
<p>The OR <code>||</code> operator is for when you want to check if EITHER of the conditions are true. They both don’t need to be.</p>
<pre class=" language-js"><code class="prism  language-js"><span class="token keyword">const</span> pineappleBelongsOnPizza <span class="token operator">=</span> <span class="token boolean">true</span>
<span class="token keyword">const</span> theyWereOnABreak <span class="token operator">=</span> <span class="token boolean">true</span>
<span class="token keyword">const</span> theOfficeIsFunny <span class="token operator">=</span> <span class="token boolean">false</span>

<span class="token keyword">if</span> <span class="token punctuation">(</span>pineappleBelongsOnPizza <span class="token operator">||</span> theOfficeIsFunny<span class="token punctuation">)</span> <span class="token punctuation">{</span>
	<span class="token comment">// One of the variables' value is true, so this runs</span>
	console<span class="token punctuation">.</span><span class="token function">log</span><span class="token punctuation">(</span><span class="token string">"Basic"</span><span class="token punctuation">)</span>
<span class="token punctuation">}</span>

<span class="token keyword">if</span> <span class="token punctuation">(</span>theyWereOnABreak <span class="token operator">||</span> theOfficeIsFunny<span class="token punctuation">)</span> <span class="token punctuation">{</span>
	<span class="token comment">// One of the variables' value is true, so this runs</span>
	console<span class="token punctuation">.</span><span class="token function">log</span><span class="token punctuation">(</span><span class="token string">"Bad"</span><span class="token punctuation">)</span>
<span class="token punctuation">}</span>
</code></pre>
<h2 id="includes-a-smaller-string">Includes a Smaller String</h2>
<p>As a software developer, you will often need to determine if a string contains a certain sub-string. For example, if you have an array where people filled out feedback for a play they attended, you want to determine how many people felt a certain emotion. You would look for the words “happy”, or “delight”, or “disappointed”, or “bored” anywhere in their feedback.</p>
<p>Their feedback won’t have those words in any predictable location in the entire string.</p>
<h4 id="example-feedback">Example Feedback</h4>
<pre class=" language-js"><code class="prism  language-js"><span class="token keyword">const</span> allFeedback <span class="token operator">=</span> <span class="token punctuation">[</span> 
    <span class="token string">"I don't regret coming, but I won't recommend it to a friend."</span><span class="token punctuation">,</span>
	<span class="token string">"I would say I was disappointed in the production."</span><span class="token punctuation">,</span>
	<span class="token string">"I was happy. The whole play had me smiling."</span><span class="token punctuation">,</span>
	<span class="token string">"What a delightful evening. Money well spent."</span><span class="token punctuation">,</span>
	<span class="token string">"Meh. It was fine."</span><span class="token punctuation">,</span>
	<span class="token string">"While there was nothing terrible, I was disappointed in the music."</span><span class="token punctuation">,</span>
	<span class="token string">"I was delighted by the fun music and the whimsical dances."</span><span class="token punctuation">,</span>
	<span class="token string">"I didn't hate it, but the last 20 minutes had me completely bored."</span>
<span class="token punctuation">]</span>
</code></pre>
<p>To find these keywords within the feedback, you can use the <code>String.includes()</code> method provided by JavaScript. Here is an example.</p>
<pre class=" language-js"><code class="prism  language-js"><span class="token keyword">let</span> happyCustomers <span class="token operator">=</span> <span class="token number">0</span>
<span class="token keyword">let</span> unhappyCustomers <span class="token operator">=</span> <span class="token number">0</span>

<span class="token keyword">for</span> <span class="token punctuation">(</span><span class="token keyword">const</span> feedback <span class="token keyword">of</span> allFeedback<span class="token punctuation">)</span> <span class="token punctuation">{</span>
	<span class="token comment">/*
		If the current feedback includes the string of "delight" or the string
		of "happy", increase the value of the happyCustomers variable by 1
	*/</span>
	<span class="token keyword">if</span> <span class="token punctuation">(</span>feedback<span class="token punctuation">.</span><span class="token function">includes</span><span class="token punctuation">(</span><span class="token string">"delight"</span><span class="token punctuation">)</span> <span class="token operator">||</span> feedback<span class="token punctuation">.</span><span class="token function">includes</span><span class="token punctuation">(</span><span class="token string">"happy"</span><span class="token punctuation">)</span><span class="token punctuation">)</span> <span class="token punctuation">{</span>
		happyCustomers<span class="token operator">++</span>
	<span class="token punctuation">}</span>
	<span class="token comment">/*
		If the current feedback includes the string of "disappointed" or 
		the string of "bored", increase the value of the unhappyCustomers
		variable by 1
	*/</span>
	<span class="token keyword">else</span> <span class="token keyword">if</span> <span class="token punctuation">(</span>feedback<span class="token punctuation">.</span><span class="token function">includes</span><span class="token punctuation">(</span><span class="token string">"disappointed"</span><span class="token punctuation">)</span> <span class="token operator">||</span> feedback<span class="token punctuation">.</span><span class="token function">includes</span><span class="token punctuation">(</span><span class="token string">"bored"</span><span class="token punctuation">)</span><span class="token punctuation">)</span> <span class="token punctuation">{</span>
		unhappyCustomers<span class="token operator">++</span>
	<span class="token punctuation">}</span>
<span class="token punctuation">}</span>

console<span class="token punctuation">.</span><span class="token function">log</span><span class="token punctuation">(</span><span class="token template-string"><span class="token string">`Happy customers: </span><span class="token interpolation"><span class="token interpolation-punctuation punctuation">${</span>happyCustomers<span class="token interpolation-punctuation punctuation">}</span></span><span class="token string">
Unhappy customers: </span><span class="token interpolation"><span class="token interpolation-punctuation punctuation">${</span>unhappyCustomers<span class="token interpolation-punctuation punctuation">}</span></span><span class="token string">
`</span></span><span class="token punctuation">)</span>
</code></pre>
<h2 id="exercise-how-do-you-take-your-coffee">Exercise: How Do You Take Your Coffee?</h2>
<p>There is an array in the code editor of different coffee roasts around the world that you enjoy. Depending on the roast, you prepare the coffee differently. If it is a light roast, you drink it black. If it is a medium roast, you put cream in it. If it is a dark roast, you put cream and sugar in it.</p>
<p>Your job is to iterate the <code>coffees</code> array and output the following sentences for each coffee. Replace the <code>xxx</code> placeholder with the full name of the coffee.</p>
<p>For light roast, output <code>"I'll have the xxx and drink it black"</code><br>
For medium roast, output <code>"I'll have the xxx and add cream only"</code><br>
For dark roast, output <code>"I'll have the xxx and add cream and sugar"</code></p>
<pre class=" language-js"><code class="prism  language-js"><span class="token keyword">const</span> coffees <span class="token operator">=</span> <span class="token punctuation">[</span> 
    <span class="token string">"light colombian roast"</span><span class="token punctuation">,</span> <span class="token string">"hawaiian dark roast"</span><span class="token punctuation">,</span> <span class="token string">"guatemalan blend medium roast"</span><span class="token punctuation">,</span>
    <span class="token string">"dark madagascar blend"</span><span class="token punctuation">,</span> <span class="token string">"jamaican dark blue"</span><span class="token punctuation">,</span> <span class="token string">"jamaican medium roast"</span><span class="token punctuation">,</span>
    <span class="token string">"salvador robusto light"</span>
<span class="token punctuation">]</span>

<span class="token keyword">let</span> output <span class="token operator">=</span> <span class="token string">""</span>

<span class="token keyword">for</span> <span class="token punctuation">(</span><span class="token keyword">const</span> coffee <span class="token keyword">of</span> coffees<span class="token punctuation">)</span> <span class="token punctuation">{</span>
    <span class="token keyword">if</span> <span class="token punctuation">(</span>coffee<span class="token punctuation">.</span><span class="token function">includes</span><span class="token punctuation">(</span><span class="token string">"light"</span><span class="token punctuation">)</span><span class="token punctuation">)</span> <span class="token punctuation">{</span>
        output <span class="token operator">+=</span> <span class="token template-string"><span class="token string">`I'll have the </span><span class="token interpolation"><span class="token interpolation-punctuation punctuation">${</span>coffee<span class="token interpolation-punctuation punctuation">}</span></span><span class="token string"> and drink it black`</span></span>
    <span class="token punctuation">}</span>
    <span class="token keyword">else</span> <span class="token keyword">if</span> <span class="token punctuation">(</span>coffee<span class="token punctuation">.</span><span class="token function">includes</span><span class="token punctuation">(</span><span class="token string">"medium"</span><span class="token punctuation">)</span><span class="token punctuation">)</span> <span class="token punctuation">{</span>
        output <span class="token operator">+=</span> <span class="token template-string"><span class="token string">`I'll have the </span><span class="token interpolation"><span class="token interpolation-punctuation punctuation">${</span>coffee<span class="token interpolation-punctuation punctuation">}</span></span><span class="token string"> and add cream only`</span></span>
    <span class="token punctuation">}</span>
    <span class="token keyword">else</span> <span class="token keyword">if</span> <span class="token punctuation">(</span>coffee<span class="token punctuation">.</span><span class="token function">includes</span><span class="token punctuation">(</span><span class="token string">"dark"</span><span class="token punctuation">)</span><span class="token punctuation">)</span> <span class="token punctuation">{</span>
        output <span class="token operator">+=</span> <span class="token template-string"><span class="token string">`I'll have the </span><span class="token interpolation"><span class="token interpolation-punctuation punctuation">${</span>coffee<span class="token interpolation-punctuation punctuation">}</span></span><span class="token string"> and add cream and sugar`</span></span>
    <span class="token punctuation">}</span>
    output <span class="token operator">+=</span> <span class="token string">"\n"</span>
<span class="token punctuation">}</span>

console<span class="token punctuation">.</span><span class="token function">log</span><span class="token punctuation">(</span>output<span class="token punctuation">)</span>
</code></pre>

