---


---

<blockquote>
<p>Break this up into two chapters. Push in next chapter.</p>
</blockquote>
<h1 id="iterating-an-array">Iterating an Array</h1>
<p>In the last part, you targeted only specific items in an array. More often, you will need to perform a task on <strong>every item</strong> in an array. To do this, software developers write loops. A loop iterates an array - meaning it looks at every item.</p>
<p>Here’s a simple array of three pieces of paper.</p>
<pre class=" language-js"><code class="prism  language-js"><span class="token keyword">const</span> originals <span class="token operator">=</span> <span class="token punctuation">[</span> <span class="token string">"Original paper 1"</span><span class="token punctuation">,</span> <span class="token string">"Original paper 2"</span><span class="token punctuation">,</span> <span class="token string">"Original paper 3"</span><span class="token punctuation">]</span>
</code></pre>
<p>The problem software developers run into is that they often don’t know how many items are in array. Some code that Bill wrote will build the array. Alice doesn’t know how long that array is, but she definitely wants to do something with everything in it.</p>
<h2 id="your-first-for-loop">Your First For Loop</h2>
<p>In JavaScript, there are several ways to iterate through the items in an array.  The specific syntax you will be using is called a <code>for..of</code> loop that is designed specifically to iterate an array. You can start with a simple example. You can use a <code>for..of</code> loop to output each item in an array to the console.</p>
<pre class=" language-js"><code class="prism  language-js"><span class="token keyword">for</span> <span class="token punctuation">(</span><span class="token keyword">const</span> paper <span class="token keyword">of</span> originals<span class="token punctuation">)</span> <span class="token punctuation">{</span>
	console<span class="token punctuation">.</span><span class="token function">log</span><span class="token punctuation">(</span>paper<span class="token punctuation">)</span>
<span class="token punctuation">}</span>
</code></pre>
<p>That would generate the following output in the console.</p>
<pre class=" language-html"><code class="prism  language-html">"Original paper 1"
"Original paper 2"
"Original paper 3"
</code></pre>
<p>This will work on any array of items that you have in your code. Here is another example.</p>
<pre class=" language-js"><code class="prism  language-js"><span class="token keyword">const</span> teammates <span class="token operator">=</span> <span class="token punctuation">[</span> <span class="token string">"Susan"</span><span class="token punctuation">,</span> <span class="token string">"Emory"</span><span class="token punctuation">,</span> <span class="token string">"Seamus"</span><span class="token punctuation">,</span> <span class="token string">"Adelaide"</span> <span class="token punctuation">]</span>
<span class="token keyword">for</span> <span class="token punctuation">(</span><span class="token keyword">const</span> name <span class="token keyword">of</span> teammates<span class="token punctuation">)</span> <span class="token punctuation">{</span>
	console<span class="token punctuation">.</span><span class="token function">log</span><span class="token punctuation">(</span>name<span class="token punctuation">)</span>
<span class="token punctuation">}</span>
</code></pre>
<p>That would generate the following output in the console.</p>
<pre class=" language-html"><code class="prism  language-html">"Susan"
"Emory"
"Seamus"
"Adelaide"
</code></pre>
<h2 id="your-topics-of-study">Your Topics of Study</h2>
<p>While you learn JavaScript, there are many topics that you will cover.</p>
<ul>
<li>Variables</li>
<li>Loops</li>
<li>Arrays</li>
<li>Functions</li>
<li>Objects</li>
<li>Modules</li>
<li>Events</li>
</ul>
<p>Copy the code below into the editor. Then you need to take those topics above and put them in the <code>topics</code> array. Then, using the examples above, write a <code>for..of</code> loop that outputs them to the console.</p>
<pre class=" language-js"><code class="prism  language-js"><span class="token keyword">const</span> topics <span class="token operator">=</span> <span class="token punctuation">[</span>  <span class="token punctuation">]</span>

<span class="token keyword">for</span> <span class="token punctuation">(</span><span class="token punctuation">)</span> <span class="token punctuation">{</span>

<span class="token punctuation">}</span>
</code></pre>

