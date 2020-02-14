---


---

<h2 id="arrays-a.k.a.-collections-of-things">Arrays (a.k.a. collections of things)</h2>
<p>In software, values don’t only have to be assigned individually to variables.</p>
<pre class=" language-js"><code class="prism  language-js"><span class="token keyword">const</span> flower1 <span class="token operator">=</span> <span class="token string">"Tulip"</span>
<span class="token keyword">const</span> flower2 <span class="token operator">=</span> <span class="token string">"Rose"</span>
<span class="token keyword">const</span> flower3 <span class="token operator">=</span> <span class="token string">"Daffodil"</span>
<span class="token keyword">const</span> flower4 <span class="token operator">=</span> <span class="token string">"Daisy"</span>
</code></pre>
<p>Since you have four strings that are all describing a similar type of thing - flowers - you can put those four strings in a collection called an array in JavaScript. You can spot an array in code by seeing some comma-delimited values separated by commas, which are all surrounded by two square brackets: the <code>[</code> and the <code>]</code> characters.</p>
<p>Here is an array of those four flowers.</p>
<pre class=" language-js"><code class="prism  language-js"><span class="token keyword">const</span> flowers <span class="token operator">=</span> <span class="token punctuation">[</span> <span class="token string">"Tulip"</span><span class="token punctuation">,</span> <span class="token string">"Rose"</span><span class="token punctuation">,</span> <span class="token string">"Daffodil"</span><span class="token punctuation">,</span> <span class="token string">"Daisy"</span> <span class="token punctuation">]</span>
</code></pre>
<p>When you assign an array as a value to a variable, it is recommended that you name the variable as a plural form of what the items in the array are. Here are some more examples.</p>
<pre class=" language-js"><code class="prism  language-js"><span class="token keyword">const</span> dogs <span class="token operator">=</span> <span class="token punctuation">[</span> <span class="token string">"Schnauzer"</span><span class="token punctuation">,</span> <span class="token string">"Labrador Retriever"</span><span class="token punctuation">,</span> <span class="token string">"Bulldog"</span><span class="token punctuation">,</span> <span class="token string">"Poodle"</span><span class="token punctuation">,</span> <span class="token string">"Collie"</span> <span class="token punctuation">]</span>
<span class="token keyword">const</span> studentAges <span class="token operator">=</span> <span class="token punctuation">[</span> <span class="token number">24</span><span class="token punctuation">,</span> <span class="token number">54</span><span class="token punctuation">,</span> <span class="token number">32</span><span class="token punctuation">,</span> <span class="token number">27</span><span class="token punctuation">,</span> <span class="token number">29</span><span class="token punctuation">,</span> <span class="token number">40</span><span class="token punctuation">,</span> <span class="token number">35</span> <span class="token punctuation">]</span>
<span class="token keyword">const</span> professions <span class="token operator">=</span> <span class="token punctuation">[</span> <span class="token string">"Mechanic"</span><span class="token punctuation">,</span> <span class="token string">"Plumber"</span><span class="token punctuation">,</span> <span class="token string">"Musician"</span><span class="token punctuation">,</span> <span class="token string">"Engineer"</span> <span class="token punctuation">]</span>
<span class="token keyword">const</span> expenses <span class="token operator">=</span> <span class="token punctuation">[</span> <span class="token number">71.54</span><span class="token punctuation">,</span> <span class="token number">401.03</span><span class="token punctuation">,</span> <span class="token number">89.59</span><span class="token punctuation">,</span> <span class="token number">145.62</span> <span class="token punctuation">]</span>
<span class="token keyword">const</span> months <span class="token operator">=</span> <span class="token punctuation">[</span> <span class="token string">"April"</span><span class="token punctuation">,</span> <span class="token string">"July"</span><span class="token punctuation">,</span> <span class="token string">"October"</span><span class="token punctuation">,</span> <span class="token string">"December"</span> <span class="token punctuation">]</span>
</code></pre>
<p>As a software developer, you will constantly be working with collections of related data stored in arrays like the ones above.</p>
<p>In the exercise in this chapter, you will learn how to access specific items in an array, how to add items to an array, and how to automate the process of targeting each item in the array - in sequence - and doing something with each item.</p>
<h2 id="exercise-your-first-array">Exercise: Your First Array</h2>
<p>Some sample code is provided in the editor. Take the 5 values assigned to the 5 variables and store them in the provided blank array instead.</p>
<h3 id="code-to-provide">Code to Provide</h3>
<pre class=" language-js"><code class="prism  language-js"><span class="token keyword">const</span> yellowFruit <span class="token operator">=</span> <span class="token string">"Banana"</span>
<span class="token keyword">const</span> orangeFruit <span class="token operator">=</span> <span class="token string">"Orange"</span>
<span class="token keyword">const</span> redFruit <span class="token operator">=</span> <span class="token string">"Apple"</span>
<span class="token keyword">const</span> greenFruit <span class="token operator">=</span> <span class="token string">"Watermelon"</span>
<span class="token keyword">const</span> blueFruit <span class="token operator">=</span> <span class="token string">"Blueberry"</span>

<span class="token keyword">const</span> fruits <span class="token operator">=</span> <span class="token punctuation">[</span><span class="token punctuation">]</span>

console<span class="token punctuation">.</span><span class="token function">log</span><span class="token punctuation">(</span>fruits<span class="token punctuation">)</span>
</code></pre>

