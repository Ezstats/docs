<h1 id="ezstats">EZstats</h1>
                        <p>So your a developer, who wants user data and see the usage of the app. Well then this is perfect for you! Continue below to install the library.</p>
                        <h1 id="installing">Installing</h1>
                        <p>
                            To get started, click this <a href="https://account.ezstats.app/home/library">link</a> to install the library.
                            Follow the tutorial below to integrate this to your applications
                        </p>
                        <h1 id="integration">Integration</h1>
                        <blockquote>
                            <p><b>TIP:</b>   Instead of adding a file one by one you can drag n’ drop them into visual studio code or Fitbit Studio</p>
                        </blockquote>
                        <p>Ok after you have the files installed import them into your code. A basic structure would look like</p>
<pre><code>File root
---
&gt; app
  &gt; index.js
  &gt; app_ezstats.js
&gt; companion
  &gt; index.js
  &gt; companion_ezstats.js
&gt; resources
</code></pre>
                        <br>
                        <blockquote>
                            <p><b>TIP:</b>  ​​​​‎‎‎You can refer to the <a href="https://dev.fitbit.com/build/guides/application/#folder-structure" target="_blank" title="Application Architecture Guide">Application Architecture Guide</a> for more info.</p>
                        </blockquote>
                        <hr>
                        <p>
                            Let’s get started!<br>
                            <br>
                            First, in your <code>app/index.js</code> we need to import the module, it can be done as simple as
                        </p>
<pre class=" language-javascript"><code class="prism  language-javascript"><span class="token keyword">import</span>  <span class="token operator">*</span>  <span class="token keyword">as</span>  ezstats  <span class="token keyword">from</span>  <span class="token string">"./app_ezstats.js"</span><span class="token punctuation">;</span>
</code></pre>
                        <p>
                            <br>
                            Now in the same file you need to initialize the module by calling the <code>initialize()</code> function. If you have imported Ezstats already then it would look something like this:
                        </p>
<pre class=" language-javascript"><code class="prism  language-javascript">ezstats<span class="token punctuation">.</span><span class="token function">initialize</span><span class="token punctuation">(</span><span class="token punctuation">)</span><span class="token punctuation">;</span>
</code></pre>
                        <br>
                        <blockquote>
                            <p><b>TIP:</b>  You can customize this function by modifying the <code>export function</code> in the <code>app_ezstats.js</code> ⚠️ Warning: If you mess up we are not responsible we recommend leaving the code as it is.</p>
                        </blockquote>
                        <hr>
                        <p>
                            <br>
                            Now for the companion part!
                        </p>
                        <p>In your <code>companion/index.js</code> we do basically the same thing as before, we import the companion module like this:</p>
<pre class=" language-javascript"><code class="prism  language-javascript"><span class="token keyword">import</span>  <span class="token operator">*</span>  <span class="token keyword">as</span>  ezstats  <span class="token keyword">from</span>  <span class="token string">"./companion_ezstats.js"</span><span class="token punctuation">;</span>
</code></pre>
                        <p>And initialize it with:</p>
<pre class=" language-javascript"><code class="prism  language-javascript">ezstats<span class="token punctuation">.</span><span class="token function">initialize</span><span class="token punctuation">(</span><span class="token punctuation">)</span><span class="token punctuation">;</span>
</code></pre>
                        <p>And boom! you now have EZstats running in your application. If you encounter any errors or problems email us at <abbr title="Email us at support@ezstats.app"><a style="cursor: help;" href="mailto:support@ezstats.app">support@ezstats.app</a></abbr> or send a message <a href="/home/support" title="Email us here!">here</a>. The specific lines of code is explained in comments in the ezstats files.</p>
                        <blockquote>
                            <p>⚠  Never modify the module without knowing what you are doing. As I mentioned this above we are not responsible for your mess up’s</p>
                        </blockquote>
