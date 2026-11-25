We will explore the mathematical foundations of the essential tools for solving optimization problems in economics.

# Unconstrained Maximization

We begin by examining the necessary conditions for a differentiable function to attain a local maximum.

However, before proceeding, it is important to note that theorem one and two establish **'necessary conditions'**, not 'sufficient conditions'.

The hypotheses of these theorems already contain the critical assuption **\"f attains local maximum at a.\"**

As a result, the following proof can be correct.

In other words, these theroems establish what must hold if a local maximum exist, rather than gurantee the existence of a local maximum.

<div class="math-center">
<p>With this distinction in mind, you need to learn...</p>
</div>

------------------------------------------------------------------------

<div class="math-theorem">
<p><strong>Theorem 1</strong>.  <em>(First-Order Necessary Conditions)<br />
Let <span class="math inline">\(U \subset \mathbb{R}^{n}\)</span> be open and <span class="math inline">\(f: U \rightarrow \mathbb{R}\)</span> be differentiale at <span class="math inline">\(a \in U\)</span>.</em></p>
<div class="math-center">
<p class="math-fbox-block"><span class="math-fbox math-fbox-wide">If <span class="math inline">\(f\)</span> attains a local maximum at <span class="math inline">\(a\)</span>, then <span class="math inline">\(Df(a)=0\)</span>.</span></p>
</div>
</div>
<div class="math-proof">
<p><em>Proof.</em> Let <span class="math inline">\(h \in \mathbb{R}^{n}\)</span> be arbitrary. Since <span class="math inline">\(U\)</span> is open and <span class="math inline">\(f\)</span> has local maximum at <span class="math inline">\(a\)</span>, there exists <span class="math inline">\(\varepsilon &gt; 0\)</span> such that <span class="math inline">\(a + th \in U\)</span> for all <span class="math inline">\(t \in (-\varepsilon, \varepsilon)\)</span>.</p>
<p>Define <span class="math inline">\(g:(-\varepsilon, \varepsilon) \rightarrow \mathbb{R}\)</span> by <span class="math inline">\(g(t)=f(a+th)\)</span></p>
<p>Therefore, <span class="math inline">\(g\)</span> has a local maximum at <span class="math inline">\(t=0\)</span> where <span class="math inline">\(\lvert t \rvert &lt; \varepsilon\)</span>. Thus, <span class="math inline">\(g(0)=f(a+0\cdot h)\)</span>.</p>
<p>Then, <span class="math inline">\(g(t) \leq g(0)\)</span> for every <span class="math inline">\(\lvert t \rvert &lt; \varepsilon\)</span>. Therefore, <span class="math inline">\(g\)</span> has local maximum at <span class="math inline">\(0\)</span>.</p>
<p>Since <span class="math inline">\(g\)</span> is differentiable at <span class="math inline">\(0\)</span> and by the chain rule, we get <span class="math display">\[g&#39;(0) = Df(a) h\]</span> The one-variable first-order necessary condition gives <span class="math inline">\(g&#39;(0)=0\)</span>. Since <span class="math inline">\(h\)</span> was arbitrary, <span class="math inline">\(Df(a)h=0\)</span> for every <span class="math inline">\(h \in \mathbb{R}^{n}\)</span>. Considering each standard basis vector <span class="math inline">\(e_j\)</span> for <span class="math inline">\(\mathbb{R}^{n}\)</span>, we get <span class="math display">\[Df(a)e_j=\frac{\partial f}{\partial x_j}(a)=0, \qquad j=1,\ldots,n.\]</span> Therefore, <span class="math inline">\(Df(a)=0\)</span>. ◻</p>
</div>
<div class="math-theorem">
<p><strong>Theorem 2</strong>.  <em>(Second Order Necessary conditions)<br />
Let <span class="math inline">\(U \subset \mathbb{R}^{n}\)</span> be open and <span class="math inline">\(a \in \operatorname{int}(U)\)</span> and <span class="math inline">\(f: U \rightarrow \mathbb{R}\)</span> be <span class="math inline">\(C^{2}\)</span> function.</em></p>
<div class="math-center">
<p class="math-fbox-block"><span class="math-fbox math-fbox-wide">If <span class="math inline">\(f\)</span> attains a local maximum at <span class="math inline">\(a\)</span>, then <span class="math inline">\(D^{2}f(a)\)</span> is negative semi-definite.</span></p>
</div>
</div>
<div class="math-proof">
<p><em>Proof.</em> Let <span class="math inline">\(h \in \mathbb{R}^{n}\)</span> be arbitrary. Since <span class="math inline">\(U\)</span> is open, there exists <span class="math inline">\(\varepsilon &gt; 0\)</span> such that <span class="math inline">\(a+th \in U\)</span> for all <span class="math inline">\(t \in (-\varepsilon, \varepsilon)\)</span>.</p>
<p>Define <span class="math inline">\(g: (-\varepsilon, \varepsilon) \rightarrow \mathbb{R}\)</span> by <span class="math inline">\(g(t)=f(a+th)\)</span>.</p>
<p>Since <span class="math inline">\(f\)</span> attains a local maximum at <span class="math inline">\(a\)</span>, we have <span class="math inline">\(g(t) \leq g(0)\)</span> for all sufficiently small <span class="math inline">\(\lvert t \rvert\)</span>, and the one-variable first-order necessary condition gives <span class="math inline">\(g&#39;(0)=0\)</span>.</p>
<p>By Taylor’s theorem, <span class="math display">\[g(t)-g(0)=g&#39;(0)t + \frac{1}{2}g&#39;&#39;(0)t^{2} + o(t^{2})\]</span></p>
<p>For all sufficiently small nonzero <span class="math inline">\(t\)</span>, the quitient <span class="math inline">\(2[g(t)-g(0)]/t^{2}\)</span> is nonpositive. Taking the limit as <span class="math inline">\(t \rightarrow 0\)</span> gives <span class="math display">\[g&#39;&#39;(0) = \lim_{t \to 0}\frac{2[g(t)-g(0)]}{t^2} \leq 0\]</span> By the chain rule, we get <span class="math inline">\(g&#39;&#39;(0) = h^{t}D^{2}f(a)h\)</span>.</p>
<p>Therefore, <span class="math display">\[h^{t}D^{2}f(a)h \leq 0\]</span> Since <span class="math inline">\(h \in \mathbb{R}^{n}\)</span> was arbitrary, <span class="math inline">\(D^{2}f(a)\)</span> is negative semi-definite. ◻</p>
</div>
