# Conditions for the Existence of Left and Right Inverses

To establish the conditions for the existence of left and right inverses, we introduce the following notation:

Let $A \in M_{m\times n}$

<div class="math-definition">
<p><strong>Definition 1</strong>.  <em><span class="math display">\[\begin{aligned}
        \operatorname{Col}(A) &amp;= \left\{ {Ax\in \mathbb{R}^m :x \in \mathbb{R}^n} \right\}
        \quad 
        \operatorname{Col}(A)\subseteq \mathbb{R}^m \quad \text{then} \quad  \operatorname{rank}(A) \leq m\\
        N(A) &amp;= \left\{ {x\in \mathbb{R}^n : Ax = 0 \in \mathbb{R}^m} \right\} 
        \quad
        N(A)\subseteq \mathbb{R}^n \quad \text{then} \quad nulity(A) \leq n
    
\end{aligned}\]</span></em></p>
</div>
<div class="math-theorem">
<p><strong>Theorem 1</strong>.  <em><span class="math inline">\(n = \operatorname{rank}(A) + dim(N(A))\)</span></em></p>
</div>

which implies that

$$n = \operatorname{rank}(A) \leq m \impliedby nulity(A) = 0$$

$$\operatorname{rank}(A) = m \impliedby m \leq n$$

<div class="math-proposition">
<p><strong>Proposition 1</strong>.  <em>A has left inverse <span class="math inline">\(\implies N(A) = \left\{0\right\}\)</span></em></p>
</div>
<div class="math-proof">
<p><em>Proof.</em> Suppose that <span class="math inline">\(A^{\scriptscriptstyle -1}_{l}\in{M_{n\times m}}\)</span> is a left inverse of <span class="math inline">\(A\)</span>. Then</p>
<p><span class="math display">\[A_l^{\scriptscriptstyle -1}A = I_n.\]</span></p>
<p>Let <span class="math inline">\(x \in N(A)\)</span>. Since <span class="math inline">\(Ax=0\)</span>, it follows that <span class="math display">\[\begin{aligned}
        x &amp;= I_nx \\
        &amp; = A_l^{\scriptscriptstyle -1}Ax \\
        &amp;= A_l^{\scriptscriptstyle -1}(0) \\
        &amp; = 0
    
\end{aligned}\]</span> Hence, <span class="math display">\[N(A)=\{0\}.\]</span></p>
<p>Furthermore, by the rank-nullity theorem, <span class="math display">\[n = \operatorname{rank}(A) \leq m\]</span> ◻</p>
</div>
<div class="math-proposition">
<p><strong>Proposition 2</strong>.  <em>If <span class="math inline">\(N(A)=\{0\}\)</span>, then A has left inverse</em></p>
</div>
<div class="math-proof">
<p><em>Proof.</em> Suppose that <span class="math inline">\(A^{\scriptscriptstyle T}Ax=\vec{0}\)</span>, then, <span class="math display">\[\begin{aligned}
        x^{\scriptscriptstyle T}A^{\scriptscriptstyle T}Ax&amp;=(Ax)^{\scriptscriptstyle T}Ax \\
        &amp;= {\lVert Ax\rVert}^{\scriptscriptstyle 2} \\
        &amp;= Ax \\
        &amp;= \vec{0}
    
\end{aligned}\]</span></p>
<p>Therefore, <span class="math inline">\(N(A^{\scriptscriptstyle T}A)=N(A)=\left\{0\right\}\)</span>.</p>
<p>Since <span class="math inline">\(A^{\scriptscriptstyle T}A\)</span> is an <span class="math inline">\(n \times n\)</span> square matrix, the rank-nullity theorem implies that <span class="math inline">\(\operatorname{rank}(A^{\scriptscriptstyle T}A)=n\)</span>.</p>
<p><span class="math display">\[(A^{\scriptscriptstyle T}A)^{\scriptscriptstyle -1}A^{\scriptscriptstyle T}A = ((A^{\scriptscriptstyle T}A)^{\scriptscriptstyle -1}A^{\scriptscriptstyle T})A = I_n\]</span></p>
<p>Therefore,</p>
<p><span class="math display">\[(A^{\scriptscriptstyle T}A)^{\scriptscriptstyle -1}A^{\scriptscriptstyle T} \text{ is a left inverse of A}\]</span> ◻</p>
</div>
<div class="math-proposition">
<p><strong>Proposition 3</strong>.  <em>If <span class="math inline">\(\operatorname{rank}(A) = m\)</span>, then A has a right inverse.</em></p>
</div>
<div class="math-proof">
<p><em>Proof.</em> Let <span class="math inline">\(y\)</span> be an arbitrary vector in <span class="math inline">\(\mathbb{R}^m\)</span>.</p>
<p>Since <span class="math inline">\(\operatorname{rank}(A) = m\)</span>, there exists <span class="math inline">\(x \in \mathbb{R}^m\)</span> such that <span class="math inline">\(Ax = y\)</span>, which means <span class="math inline">\(\operatorname{Col}(A) = \mathbb{R}^m\)</span>.</p>
<p>Since <span class="math inline">\(\operatorname{rank}(A) = \operatorname{rank}(A^{\scriptscriptstyle T}) = m\)</span> and <span class="math inline">\(m = \operatorname{rank}(A^{\scriptscriptstyle T}) + nulity A^{\scriptscriptstyle T}\)</span>.</p>
<p><span class="math display">\[N(A^{\scriptscriptstyle T}) = \left\{0\right\}\]</span></p>
<p>Suppose that <span class="math inline">\(AA^{\scriptscriptstyle T}x = 0\)</span>. Then</p>
<p><span class="math display">\[x^{\scriptscriptstyle T}AA^{\scriptscriptstyle T}x = {\lVert A^{\scriptscriptstyle T}x \rVert}^{\scriptscriptstyle 2} = 0\]</span></p>
<p><span class="math display">\[N(AA^{\scriptscriptstyle T}) \subseteq N(A^{\scriptscriptstyle T})\]</span></p>
<p>Since <span class="math inline">\(N(A^{\scriptscriptstyle T}) = \left\{0\right\}\)</span> , it follows that <span class="math inline">\(N(AA^{\scriptscriptstyle T}) = \left\{0\right\}\)</span>.</p>
<p>By using the rank-nulity theorem,</p>
<p><span class="math display">\[\operatorname{rank}(AA^{\scriptscriptstyle T}) = m\]</span></p>
<p>Because <span class="math inline">\(AA^{\scriptscriptstyle T}\)</span> is a square matrix, it is therefore invertible.</p>
<p><span class="math display">\[AA^{\scriptscriptstyle T}(AA^{\scriptscriptstyle T})^{\scriptscriptstyle -1} = A(A^{\scriptscriptstyle T}(AA^{\scriptscriptstyle T})^{\scriptscriptstyle -1}) = I_m\]</span></p>
<p>Hence, <span class="math inline">\(A^{\scriptscriptstyle T}(AA^{\scriptscriptstyle T})^{\scriptscriptstyle -1}\)</span> is right inverse of A ◻</p>
</div>
