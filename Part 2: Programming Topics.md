---


---

<h2 id="iterating-an-array">Iterating an Array</h2>
<p>In the last part, you targeted only specific items in an array. More often, you will need to perform a task on <strong>every item</strong> in an array. To do this, software developers write loops. A loop iterates an array - meaning it looks at every item.</p>
<p>You also often don’t know - or don’t care - how many items are in array. You just want to perform some task with each item.</p>
<h2 id="concise-for-loop-syntax">Concise For Loop Syntax</h2>
<p>In JavaScript, there is a specific kind of loop called a <code>for..of</code> loop that is designed specifically to iterate an array.</p>
<p>With a <code>for..of</code> loop, you don’t need to worry about accessing individual items using the <code>array[index]</code> syntax. All you need to do is declare a variable to store the current item, and the <code>for..of</code> loop will assign it the correct value as it iterates the array.</p>
<p>Go ahead and copy the following code into the code editor and run it. You will see each car model in the console output.</p>
<h2 id="cars">Cars</h2>
<p>Here’s a quick example.</p>
<pre class=" language-js"><code class="prism  language-js"><span class="token comment">// Inventory of a used car lot</span>
<span class="token keyword">const</span> carLot <span class="token operator">=</span> <span class="token punctuation">[</span> <span class="token string">"Pinto"</span><span class="token punctuation">,</span> <span class="token string">"F150"</span><span class="token punctuation">,</span> <span class="token string">"Cabriolet"</span><span class="token punctuation">,</span> <span class="token string">"Sentra"</span><span class="token punctuation">,</span> <span class="token string">"Xterra"</span><span class="token punctuation">,</span> <span class="token string">"Ram"</span> <span class="token punctuation">]</span>

<span class="token keyword">for</span> <span class="token punctuation">(</span><span class="token keyword">const</span> car <span class="token keyword">of</span> carLot<span class="token punctuation">)</span> <span class="token punctuation">{</span>
	console<span class="token punctuation">.</span><span class="token function">log</span><span class="token punctuation">(</span>car<span class="token punctuation">)</span>
<span class="token punctuation">}</span>
</code></pre>
<p>That would generate the following output in the console.</p>
<pre class=" language-html"><code class="prism  language-html">Pinto
F150
Cabriolet
Sentra
Xterra
Ram
</code></pre>
<h2 id="papers-to-copy">Papers to Copy</h2>
<p>Here’s a simple array of three pieces of paper. The variable of <code>paper</code> inside the <code>for</code> statement is where the variable is both declared and assigned a value as the code walks through the array one item at a time.</p>
<pre class=" language-js"><code class="prism  language-js"><span class="token keyword">const</span> originals <span class="token operator">=</span> <span class="token punctuation">[</span> <span class="token string">"Original paper 1"</span><span class="token punctuation">,</span> <span class="token string">"Original paper 2"</span><span class="token punctuation">,</span> <span class="token string">"Original paper 3"</span><span class="token punctuation">]</span>

<span class="token keyword">for</span> <span class="token punctuation">(</span><span class="token keyword">const</span> paper <span class="token keyword">of</span> originals<span class="token punctuation">)</span> <span class="token punctuation">{</span>
	console<span class="token punctuation">.</span><span class="token function">log</span><span class="token punctuation">(</span>paper<span class="token punctuation">)</span>
<span class="token punctuation">}</span>
</code></pre>
<p>That would generate the following output in the console.</p>
<pre class=" language-html"><code class="prism  language-html">"Original paper 1"
"Original paper 2"
"Original paper 3"
</code></pre>
<p>This will work on any array of items that you have in your code. Here is another example. Remember that you can name your variables anything you want, and make sure the name is relevant (i.e. provides context) for the value that is assigned to it.</p>
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
<h3 id="starter-code-to-provide">Starter code to provide</h3>
<pre class=" language-js"><code class="prism  language-js"><span class="token keyword">const</span> topics <span class="token operator">=</span> <span class="token punctuation">[</span>  <span class="token punctuation">]</span>

<span class="token keyword">for</span> <span class="token punctuation">(</span><span class="token punctuation">)</span> <span class="token punctuation">{</span>

<span class="token punctuation">}</span>
</code></pre>

