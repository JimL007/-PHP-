---


---

<h1 id="php学习之旅">PHP学习之旅</h1>
<hr>
<h2 id="目录基础语法">目录(基础语法)</h2>
<ul>
<li>语法</li>
<li>变量</li>
<li>Echo/Print</li>
<li>数据类型</li>
<li>字符串函数</li>
<li>常量</li>
<li>运算符</li>
<li>分支语句</li>
<li>循环语句</li>
<li>函数</li>
<li>数组</li>
<li>数组排序</li>
<li>超全局</li>
</ul>
<h2 id="表单">表单</h2>
<ul>
<li>表单处理</li>
<li>表单验证</li>
<li>表单必填</li>
<li>表单 URL/E-mail</li>
<li>表单完成</li>
</ul>
<hr>
<h3 id="语句">语句</h3>
<ul>
<li>大小写敏感
<ul>
<li>在PHP中,所有用户定义的<strong>函数,类,关键词</strong>都对大小写不敏感</li>
<li>但是,所有的<strong>变量名</strong>都对大小写敏感</li>
</ul>
</li>
</ul>
<h3 id="变量">变量</h3>
<ul>
<li>所有的变量名都对大小写敏感</li>
<li>命名规则: $str  = “hello word!” ($符+变量名;如果变量被赋的值是文本,请用引号包围该值)</li>
<li>PHP是一门类型松散的语言,我们无需规定变量的类型,PHP会自动转换合适的类型</li>
<li><strong>变量作用域(php有三种变量作用域)</strong>
<ul>
<li>global (全局),在函数之外声明的变量,只能在函数之外进行访问.</li>
<li>local (局部),在函数之内声明的变量,只能在函数之内访问</li>
<li>static (静态); 通常,当函数完成/执行后,会删除所有变量.如若不想删除该变量,则在首次声明该变量时使用 static 关键词</li>
</ul>
<pre class=" language-php"><code class="prism  language-php"><span class="token keyword">function</span> <span class="token function">myTest</span><span class="token punctuation">(</span><span class="token punctuation">)</span> <span class="token punctuation">{</span>
	<span class="token keyword">static</span> <span class="token variable">$x</span><span class="token operator">=</span><span class="token number">0</span><span class="token punctuation">;</span>
	<span class="token keyword">echo</span> <span class="token variable">$x</span><span class="token punctuation">;</span>
    <span class="token variable">$x</span><span class="token operator">++</span><span class="token punctuation">;</span>
    <span class="token punctuation">}</span>
<span class="token function">myTest</span><span class="token punctuation">(</span><span class="token punctuation">)</span><span class="token punctuation">;</span>
<span class="token function">myTest</span><span class="token punctuation">(</span><span class="token punctuation">)</span><span class="token punctuation">;</span>
<span class="token function">myTest</span><span class="token punctuation">(</span><span class="token punctuation">)</span><span class="token punctuation">;</span>
</code></pre>
</li>
</ul>

