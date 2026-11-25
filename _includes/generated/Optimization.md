We will explore the mathematical foundations of the essential tools for solving optimization problems in economics.

# Unconstrained Maximization

We begin by examining the necessary conditions for a differentiable function to attain a local maximum.

<div class="math-theorem">
<p><strong>Theorem 1</strong>.  <em>(First-Order Necessary Conditions)<br />
Let <span class="math inline">\(U \subset \mathbb{R}^{n}\)</span> be open and <span class="math inline">\(f: U \rightarrow \mathbb{R}\)</span> be differentiale at <span class="math inline">\(a \in U\)</span>.</em></p>
<div class="center">

</div>
</div>
<div class="math-proof">
<p><em>Proof.</em> Let <span class="math inline">\(h \in \mathbb{R}^{n}\)</span> be arbitrary. Since <span class="math inline">\(U\)</span> is open and <span class="math inline">\(f\)</span> has local maximum at <span class="math inline">\(a\)</span>, there exists <span class="math inline">\(\varepsilon &gt; 0\)</span> such that <span class="math inline">\(a + th \in U\)</span> for all <span class="math inline">\(t \in (-\varepsilon, \varepsilon)\)</span>.</p>
<p>Define <span class="math inline">\(g:(-\varepsilon, \varepsilon) \rightarrow \mathbb{R}\)</span> by <span class="math inline">\(g(t)=f(a+th)\)</span>.</p>
<p>Since <span class="math inline">\(f\)</span> attains a local maximum at <span class="math inline">\(a\)</span>, <span class="math inline">\(g\)</span> has a local maximum at <span class="math inline">\(t=0\)</span> where <span class="math inline">\(\lvert t \rvert &lt; \varepsilon\)</span>. <span class="math inline">\(g(0)=f(a+0\cdot h)\)</span>. Then, <span class="math inline">\(g(t) \leq g(0)\)</span> for every <span class="math inline">\(\lvert t \rvert &lt; \varepsilon\)</span>. Therefore, <span class="math inline">\(g\)</span> has local maximum at <span class="math inline">\(0\)</span>.</p>
<p>Since <span class="math inline">\(g\)</span> is differentiable at <span class="math inline">\(0\)</span> and by the chain rule, we get <span class="math display">\[g&#39;(0) = Df(a) h\]</span> The one-variable first-order necessary condition gives <span class="math inline">\(g&#39;(0)=0\)</span>. Since <span class="math inline">\(h\)</span> was arbitrary, <span class="math inline">\(Df(a)h=0\)</span> for every <span class="math inline">\(h \in \mathbb{R}^{n}.\)</span> Taking <span class="math inline">\(h=\nabla f(a)\)</span> yields <span class="math display">\[0=Df(a)\nabla f(a) = {\lVert \nabla f(a) \rVert}^2\]</span> Hence, <span class="math inline">\(\nabla f(a)=0\)</span> and therefore, <span class="math inline">\(Df(a)=0\)</span> ◻</p>
</div>
<div class="math-theorem">
<p><strong>Theorem 2</strong>.  <em>(Second Order Necessary conditions)<br />
Let <span class="math inline">\(U \subset \mathbb{R}^{n}\)</span> be open and <span class="math inline">\(a \in \operatorname{int}(U)\)</span>. <span class="math inline">\(f: U \rightarrow \mathbb{R}\)</span> be <span class="math inline">\(C^{2}\)</span> function.</em></p>
<div class="center">

</div>
</div>
<div class="math-proof">
<p><em>Proof.</em> Let <span class="math inline">\(h \in \mathbb{R}^{n}\)</span> be arbitrary. Since <span class="math inline">\(U\)</span> is open, there exists <span class="math inline">\(\varepsilon &gt; 0\)</span> such that <span class="math inline">\(a+th \in U\)</span> for all <span class="math inline">\(t \in (-\varepsilon, \varepsilon)\)</span>.</p>
<p>Define <span class="math inline">\(g: (-\varepsilon, \varepsilon) \rightarrow \mathbb{R}\)</span> by <span class="math inline">\(g(t)=f(a+th)\)</span>.</p>
<p>Since <span class="math inline">\(f\)</span> attains a local maximum at <span class="math inline">\(a\)</span> and considering the first-order necessary condition, <span class="math display">\[\frac{dg(t)}{dt} = Df(a+th) \times h\]</span> <span class="math display">\[\frac{dg(0)}{dt} = Df(a) \times h = 0\]</span> Therefore, <span class="math display">\[g(0) \leq g(t) \qquad \text{where} \quad \lvert t \rvert &lt; \varepsilon\]</span> ◻</p>
</div>
