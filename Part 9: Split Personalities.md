---


---

<h2 id="strings-into-arrays-into-strings">Strings into Arrays into Strings</h2>
<p>Now that you have worked with arrays and strings in various contexts, this chapter will cover how to convert strings into arrays, and vice versa.</p>
<h2 id="split-string-into-an-array">Split String into an Array</h2>
<p>Take a look at the following string. It represents a person’s full name, but in a very particular format. The first name, middle name, and last name are separated by commas. Juan is the first name. Carlos is the middle name. Rodriguez is the surname. You want to have each of those names stored in their own variable.</p>
<pre class=" language-js"><code class="prism  language-js"><span class="token keyword">const</span> fullName <span class="token operator">=</span> <span class="token string">"Juan,Carlos,Rodriguez"</span>
</code></pre>
<h3 id="split-into-multiple-variables">Split Into Multiple Variables</h3>
<p>You can use <code>.split()</code> method on any string to pull out sub-strings that are separated by a common character - also called the delimiter.  The following code both declares each variable, and assigns each a value all in one line of code.</p>
<p>Note that within the parenthesis after <code>.split</code>, there is a comma character.</p>
<pre class=" language-js"><code class="prism  language-js"><span class="token keyword">const</span> fullName <span class="token operator">=</span> <span class="token string">"Juan,Carlos,Rodriguez"</span>
<span class="token keyword">const</span> <span class="token punctuation">[</span> firstName<span class="token punctuation">,</span> middleName<span class="token punctuation">,</span> surName <span class="token punctuation">]</span> <span class="token operator">=</span> fullName<span class="token punctuation">.</span><span class="token function">split</span><span class="token punctuation">(</span><span class="token string">","</span><span class="token punctuation">)</span>

console<span class="token punctuation">.</span><span class="token function">log</span><span class="token punctuation">(</span>firstName<span class="token punctuation">)</span>  <span class="token comment">// Juan</span>
console<span class="token punctuation">.</span><span class="token function">log</span><span class="token punctuation">(</span>middleName<span class="token punctuation">)</span>  <span class="token comment">// Carlos</span>
console<span class="token punctuation">.</span><span class="token function">log</span><span class="token punctuation">(</span>surName<span class="token punctuation">)</span>  <span class="token comment">// Rodriguez</span>
</code></pre>
<p>If the sub-strings were separated by a colon instead, you would use that character inside the parenthesis.</p>
<pre class=" language-js"><code class="prism  language-js"><span class="token keyword">const</span> fullName <span class="token operator">=</span> <span class="token string">"Juan:Carlos:Rodriguez"</span>
<span class="token keyword">const</span> <span class="token punctuation">[</span> firstName<span class="token punctuation">,</span> middleName<span class="token punctuation">,</span> surName <span class="token punctuation">]</span> <span class="token operator">=</span> fullName<span class="token punctuation">.</span><span class="token function">split</span><span class="token punctuation">(</span><span class="token string">":"</span><span class="token punctuation">)</span>

console<span class="token punctuation">.</span><span class="token function">log</span><span class="token punctuation">(</span>firstName<span class="token punctuation">)</span>  <span class="token comment">// Juan</span>
console<span class="token punctuation">.</span><span class="token function">log</span><span class="token punctuation">(</span>middleName<span class="token punctuation">)</span>  <span class="token comment">// Carlos</span>
console<span class="token punctuation">.</span><span class="token function">log</span><span class="token punctuation">(</span>surName<span class="token punctuation">)</span>  <span class="token comment">// Rodriguez</span>
</code></pre>
<p>What if the names are separated by two colons, though?? Send two colons to the split method.</p>
<pre class=" language-js"><code class="prism  language-js"><span class="token keyword">const</span> fullName <span class="token operator">=</span> <span class="token string">"Juan::Carlos::Rodriguez"</span>
<span class="token keyword">const</span> <span class="token punctuation">[</span> firstName<span class="token punctuation">,</span> middleName<span class="token punctuation">,</span> surName <span class="token punctuation">]</span> <span class="token operator">=</span> fullName<span class="token punctuation">.</span><span class="token function">split</span><span class="token punctuation">(</span><span class="token string">"::"</span><span class="token punctuation">)</span>

console<span class="token punctuation">.</span><span class="token function">log</span><span class="token punctuation">(</span>firstName<span class="token punctuation">)</span>  <span class="token comment">// Juan</span>
console<span class="token punctuation">.</span><span class="token function">log</span><span class="token punctuation">(</span>middleName<span class="token punctuation">)</span>  <span class="token comment">// Carlos</span>
console<span class="token punctuation">.</span><span class="token function">log</span><span class="token punctuation">(</span>surName<span class="token punctuation">)</span>  <span class="token comment">// Rodriguez</span>
</code></pre>
<h3 id="split-into-array">Split Into Array</h3>
<h2 id="join-array-into-a-string">Join Array into a String</h2>
<p>You can do the complete opposite as well. If you have an existing array that contains string values, you can combine them into a single string with the <code>.join()</code> method.</p>
<p>Here is an example. A poem is currently stored in an array. Each line of the poem is one string value in the array. You want to combine all of them into one, single string to be displayed.</p>
<pre class=" language-js"><code class="prism  language-js"><span class="token keyword">const</span> sentences <span class="token operator">=</span> <span class="token punctuation">[</span>
	<span class="token string">"Praise the spells and bless the charms,"</span><span class="token punctuation">,</span>
	<span class="token string">"I found April in my arms."</span><span class="token punctuation">,</span>
	<span class="token string">"April golden, April cloudy,"</span><span class="token punctuation">,</span>
	<span class="token string">"Gracious, cruel, tender, rowdy;"</span>
<span class="token punctuation">]</span>

<span class="token keyword">const</span> wholePoem <span class="token operator">=</span> sentences<span class="token punctuation">.</span><span class="token function">join</span><span class="token punctuation">(</span><span class="token string">""</span><span class="token punctuation">)</span>

console<span class="token punctuation">.</span><span class="token function">log</span><span class="token punctuation">(</span>wholePoem<span class="token punctuation">)</span>
</code></pre>
<p>That output would be the following single string.</p>
<pre class=" language-html"><code class="prism  language-html">Praise the spells and bless the charms, I found April in my arms. April golden, April cloudy,  Gracious, cruel, tender, rowdy;
</code></pre>
<p>Much like the <code>.split()</code> method on a string, you can specify a character by which all the individual strings in the array will be joined. Another example below.</p>
<pre class=" language-js"><code class="prism  language-js"><span class="token keyword">const</span> surprises <span class="token operator">=</span> <span class="token punctuation">[</span> <span class="token string">"lions"</span><span class="token punctuation">,</span> <span class="token string">"tigers"</span><span class="token punctuation">,</span> <span class="token string">"bears"</span> <span class="token punctuation">]</span>
<span class="token keyword">const</span> exclamation <span class="token operator">=</span> surprises<span class="token punctuation">.</span><span class="token function">join</span><span class="token punctuation">(</span><span class="token string">" and "</span><span class="token punctuation">)</span>

console<span class="token punctuation">.</span><span class="token function">log</span><span class="token punctuation">(</span><span class="token template-string"><span class="token string">`</span><span class="token interpolation"><span class="token interpolation-punctuation punctuation">${</span>exclamation<span class="token interpolation-punctuation punctuation">}</span></span><span class="token string">, oh my`</span></span><span class="token punctuation">)</span>
</code></pre>
<p>The output would be the following string.</p>
<pre class=" language-html"><code class="prism  language-html">lions and tigers and bears, oh my
</code></pre>
<p>You could also wrap the strings in HTML elements.</p>
<pre class=" language-js"><code class="prism  language-js"><span class="token keyword">const</span> employees <span class="token operator">=</span> <span class="token punctuation">[</span> <span class="token string">"Mary Bulshear"</span><span class="token punctuation">,</span> <span class="token string">"Kelley Avignon"</span><span class="token punctuation">,</span> <span class="token string">"Brian Wellington"</span><span class="token punctuation">,</span> <span class="token string">"Cherie Midreaux"</span> <span class="token punctuation">]</span>
<span class="token keyword">const</span> listItems <span class="token operator">=</span> employees<span class="token punctuation">.</span><span class="token function">join</span><span class="token punctuation">(</span><span class="token string">"&lt;/li&gt;&lt;li&gt;"</span><span class="token punctuation">)</span>

console<span class="token punctuation">.</span><span class="token function">log</span><span class="token punctuation">(</span><span class="token template-string"><span class="token string">`&lt;li&gt;</span><span class="token interpolation"><span class="token interpolation-punctuation punctuation">${</span>listItems<span class="token interpolation-punctuation punctuation">}</span></span><span class="token string">&lt;/li&gt;`</span></span><span class="token punctuation">)</span>
</code></pre>
<p>That would generate the following HTML string.</p>
<pre><code>&lt;li&gt;Mary Bulshear&lt;/li&gt;
&lt;li&gt;Kelley Avignon&lt;/li&gt;
&lt;li&gt;Brian Wellington&lt;/li&gt;
&lt;li&gt;Cherie Midreaux&lt;/li&gt;
</code></pre>
<h2 id="exercise-split-personalities">Exercise: Split Personalities</h2>
<p>The Luminous Association of Personality Disorders (LAPD) has a yearly conference in Las Vegas where professional psychologists and cognitive scientists gather to discuss the latest research into aberrant mental disorders that affect people around the world. The software developer that maintain the entire list of known personality disorders have sent the you the list so that you can display them on the LAPD conference website. The format for the data is somewhat bizarre.</p>
<p>They sent them all in one large string, with each disorder separated by the following characters: <code>|$|</code>.</p>
<h3 id="original-disorders-string">Original Disorders String</h3>
<pre class=" language-js"><code class="prism  language-js"><span class="token string">"Depression|$|Bipolar|$|Manic|$|Anxiety|$|Anorexia|$|Posttraumtic Stress|$|Seasonal Affective|$|Bulimia"</span>
</code></pre>
<p>What you want to display on the web page is a series of <code>&lt;div&gt;</code> elements that contain the disorder names. That means you will first need to <code>split()</code> the string on the correct delimiter to generate an array of strings. Then you must <code>.join()</code> the array back into a single string, making sure each disorder name is surrounded by a <code>&lt;div&gt;</code> HTML tag.</p>
<h3 id="expected-final-output">Expected Final Output</h3>
<pre class=" language-html"><code class="prism  language-html"><span class="token tag"><span class="token tag"><span class="token punctuation">&lt;</span>div</span><span class="token punctuation">&gt;</span></span>Depression<span class="token tag"><span class="token tag"><span class="token punctuation">&lt;/</span>div</span><span class="token punctuation">&gt;</span></span>
<span class="token tag"><span class="token tag"><span class="token punctuation">&lt;</span>div</span><span class="token punctuation">&gt;</span></span>Bipolar<span class="token tag"><span class="token tag"><span class="token punctuation">&lt;/</span>div</span><span class="token punctuation">&gt;</span></span>
<span class="token tag"><span class="token tag"><span class="token punctuation">&lt;</span>div</span><span class="token punctuation">&gt;</span></span>Manic<span class="token tag"><span class="token tag"><span class="token punctuation">&lt;/</span>div</span><span class="token punctuation">&gt;</span></span>
<span class="token tag"><span class="token tag"><span class="token punctuation">&lt;</span>div</span><span class="token punctuation">&gt;</span></span>Anxiety<span class="token tag"><span class="token tag"><span class="token punctuation">&lt;/</span>div</span><span class="token punctuation">&gt;</span></span>
<span class="token tag"><span class="token tag"><span class="token punctuation">&lt;</span>div</span><span class="token punctuation">&gt;</span></span>Anorexia<span class="token tag"><span class="token tag"><span class="token punctuation">&lt;/</span>div</span><span class="token punctuation">&gt;</span></span>
<span class="token tag"><span class="token tag"><span class="token punctuation">&lt;</span>div</span><span class="token punctuation">&gt;</span></span>Posttraumtic Stress<span class="token tag"><span class="token tag"><span class="token punctuation">&lt;/</span>div</span><span class="token punctuation">&gt;</span></span>
<span class="token tag"><span class="token tag"><span class="token punctuation">&lt;</span>div</span><span class="token punctuation">&gt;</span></span>Seasonal Affective<span class="token tag"><span class="token tag"><span class="token punctuation">&lt;/</span>div</span><span class="token punctuation">&gt;</span></span>
<span class="token tag"><span class="token tag"><span class="token punctuation">&lt;</span>div</span><span class="token punctuation">&gt;</span></span>Bulimia<span class="token tag"><span class="token tag"><span class="token punctuation">&lt;/</span>div</span><span class="token punctuation">&gt;</span></span>
</code></pre>

