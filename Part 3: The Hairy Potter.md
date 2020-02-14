---


---

<h2 id="ah..-push-it">Ah… Push It</h2>
<p>There is a classic hip hop song from the 1980’s that I always think of when I want to add a new value to an array. Arrays have a method on them named <code>.push()</code>. That method lets you add a new value as the last item in the array.</p>
<p>You will start off with this simple example where you have three pieces of paper that need to be copied. The original pieces of paper should not be touched. Therefore, you will end up with a new collection - or array - that will contain the copies.</p>
<p>Here’s how you can add a new piece of paper to the collection that needs to be copies.</p>
<pre class=" language-js"><code class="prism  language-js"><span class="token keyword">const</span> originals <span class="token operator">=</span> <span class="token punctuation">[</span> <span class="token string">"Original paper 1"</span><span class="token punctuation">,</span> <span class="token string">"Original paper 2"</span><span class="token punctuation">,</span> <span class="token string">"Original paper 3"</span> <span class="token punctuation">]</span>

originals<span class="token punctuation">.</span><span class="token function">push</span><span class="token punctuation">(</span><span class="token string">"Original paper 4"</span><span class="token punctuation">)</span>

console<span class="token punctuation">.</span><span class="token function">log</span><span class="token punctuation">(</span>originals<span class="token punctuation">)</span>

<span class="token comment">/*
This is the new contents of the array
	
[ "Original paper 1", "Original paper 2", "Original paper 3", "Original paper 4"]
*/</span>
</code></pre>
<h2 id="making-copies">Making Copies</h2>
<p>Now it is time to combine the <code>for</code> loop with the <code>push()</code> method on an array to make a copy for each item in the <code>originals</code> array.</p>
<pre class=" language-js"><code class="prism  language-js"><span class="token keyword">const</span> originals <span class="token operator">=</span> <span class="token punctuation">[</span> <span class="token string">"Original paper 1"</span><span class="token punctuation">,</span> <span class="token string">"Original paper 2"</span><span class="token punctuation">,</span> <span class="token string">"Original paper 3"</span> <span class="token punctuation">]</span>
<span class="token keyword">const</span> copies <span class="token operator">=</span> <span class="token punctuation">[</span><span class="token punctuation">]</span>  <span class="token comment">// Blank array that will contain the copies</span>

<span class="token keyword">for</span> <span class="token punctuation">(</span><span class="token keyword">const</span> paper <span class="token keyword">of</span> originals<span class="token punctuation">)</span> <span class="token punctuation">{</span>
	<span class="token keyword">const</span> copy <span class="token operator">=</span> <span class="token template-string"><span class="token string">`Copy of </span><span class="token interpolation"><span class="token interpolation-punctuation punctuation">${</span>paper<span class="token interpolation-punctuation punctuation">}</span></span><span class="token string">`</span></span>
	copies<span class="token punctuation">.</span><span class="token function">push</span><span class="token punctuation">(</span>copy<span class="token punctuation">)</span>
<span class="token punctuation">}</span>

console<span class="token punctuation">.</span><span class="token function">log</span><span class="token punctuation">(</span>copies<span class="token punctuation">)</span>
</code></pre>
<p>If you have anything in your code editor, go ahead and delete it all. Then take that code above and put it in the code editor and run it. You will see the new array displayed in the console below the editor.</p>
<h2 id="exercise-the-hairy-potter">Exercise: The Hairy Potter</h2>
<p>Delete everything that you currently have in the code editor. Copy and paste the following code into the editor. In this exercise, you are writing code to automate what a potter does: turn clay into pottery.</p>
<p>Your task is to iterate the array containing the chunks of clay and after your code is done, the <code>toFireInKiln</code> array should contain the string value “coffee mug” for every chunk of clay in the <code>clay</code> array.</p>
<blockquote>
<p>Reminder: You can make all of your variable names the same as the example, or you can change them if you want to be crazy. Just to remind you that JavaScript doesn’t care what you name your variables. For example, we chose the variable name <code>currentIndex</code> to represent the index of the array, but it doesn’t have to be that name. You could name it <code>index</code>, <code>idx</code>, <code>i</code>, or even <code>moonDust</code> if you like. It’s not a descriptive name, but you can do it anyway, as long as you use <code>moonDust</code> everywhere <code>currentIndex</code> is currently used.</p>
</blockquote>
<pre class=" language-js"><code class="prism  language-js"><span class="token keyword">const</span> clay <span class="token operator">=</span> <span class="token punctuation">[</span> <span class="token string">"Chunk of clay"</span><span class="token punctuation">,</span> <span class="token string">"Chunk of clay"</span><span class="token punctuation">,</span> <span class="token string">"Chunk of clay"</span><span class="token punctuation">,</span> <span class="token string">"Chunk of clay"</span> <span class="token punctuation">]</span>
<span class="token keyword">const</span> toFireInKiln <span class="token operator">=</span> <span class="token punctuation">[</span><span class="token punctuation">]</span>

<span class="token keyword">for</span> <span class="token punctuation">(</span><span class="token punctuation">)</span> <span class="token punctuation">{</span>
   <span class="token keyword">const</span> mug <span class="token operator">=</span> <span class="token string">"coffee mug"</span>
<span class="token punctuation">}</span>

console<span class="token punctuation">.</span><span class="token function">log</span><span class="token punctuation">(</span>toFireInKiln<span class="token punctuation">)</span>
</code></pre>

