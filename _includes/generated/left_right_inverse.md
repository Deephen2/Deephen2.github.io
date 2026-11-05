# Conditions for the Existence of Left and Right Inverses

To establish the conditions for the existence of left and right inverses, we introduce the following notation:

Let $A \in M_{m\times n}$

<div class="math-definition">
<p><strong>Definition 1</strong>. <em><span
class="math display">$$\begin{aligned}
        \operatorname{Col}(A) &amp;= \left\{ {Ax\in \mathbb{R}^m :x \in
\mathbb{R}^n} \right\}
        \quad
        \operatorname{Col}(A)\subseteq \mathbb{R}^m \quad \text{then}
\quad  \operatorname{rank}(A) \leq m\\
        N(A) &amp;= \left\{ {x\in \mathbb{R}^n : Ax = 0 \in
\mathbb{R}^m} \right\}
        \quad
        N(A)\subseteq \mathbb{R}^n \quad \text{then} \quad nulity(A)
\leq n
    
\end{aligned}$$</span></em></p>
</div>
<div class="math-theorem">
<p><strong>Theorem 1</strong>. <em><span
class="math inline"><em>n</em> = rank (<em>A</em>) + <em>d</em><em>i</em><em>m</em>(<em>N</em>(<em>A</em>))</span></em></p>
</div>

which implies that

$$n = \operatorname{rank}(A) \leq m \impliedby nulity(A) = 0$$

$$\operatorname{rank}(A) = m \impliedby m \leq n$$

<div class="math-proposition">
<p><strong>Proposition 1</strong>. <em>A has left inverse <span
class="math inline"> ⟹ <em>N</em>(<em>A</em>) = {0}</span></em></p>
</div>
<div class="math-proof">
<p><em>Proof.</em> Suppose that <span
class="math inline"><em>A</em><sub><em>l</em></sub><sup>−1</sup> ∈ <em>M</em><sub><em>n</em> × <em>m</em></sub></span>
is a left inverse of <span class="math inline"><em>A</em></span>.
Then</p>
<p><span
class="math display"><em>A</em><sub><em>l</em></sub><sup>−1</sup><em>A</em> = <em>I</em><sub><em>n</em></sub>.</span></p>
<p>Let <span
class="math inline"><em>x</em> ∈ <em>N</em>(<em>A</em>)</span>. Since
<span class="math inline"><em>A</em><em>x</em> = 0</span>, it follows
that <span class="math display">$$\begin{aligned}
        x &amp;= I_nx \\
        &amp; = A_l^{-1}Ax \\
        &amp;= A_l^{-1}(0) \\
        &amp; = 0
    
\end{aligned}$$</span> Hence, <span
class="math display"><em>N</em>(<em>A</em>) = {0}.</span></p>
<p>Furthermore, by the rank-nullity theorem, <span
class="math display"><em>n</em> = rank (<em>A</em>) ≤ <em>m</em></span> ◻</p>
</div>
<div class="math-proposition">
<p><strong>Proposition 2</strong>. <em>If <span
class="math inline"><em>N</em>(<em>A</em>) = {0}</span>, then A has left
inverse</em></p>
</div>
<div class="math-proof">
<p><em>Proof.</em> Suppose that <span
class="math inline">$A^{T}Ax=\vec{0}$</span>, then, <span
class="math display">$$\begin{aligned}
        x^{T}A^{T}Ax&amp;=(Ax)^{T}Ax \\
        &amp;= {\lVert Ax\rVert}^2 \\
        &amp;= Ax \\
        &amp;= \vec{0}
    
\end{aligned}$$</span></p>
<p>Therefore, <span
class="math inline"><em>N</em>(<em>A</em><sup><em>T</em></sup><em>A</em>) = <em>N</em>(<em>A</em>) = {0}</span>.</p>
<p>Since <span
class="math inline"><em>A</em><sup><em>T</em></sup><em>A</em></span> is
an <span class="math inline"><em>n</em> × <em>n</em></span> square
matrix, the rank-nullity theorem implies that <span
class="math inline">rank (<em>A</em><sup><em>T</em></sup><em>A</em>) = <em>n</em></span>.</p>
<p><span
class="math display">(<em>A</em><sup><em>T</em></sup><em>A</em>)<sup>−1</sup><em>A</em><sup><em>T</em></sup><em>A</em> = ((<em>A</em><sup><em>T</em></sup><em>A</em>)<sup>−1</sup><em>A</em><sup><em>T</em></sup>)<em>A</em> = <em>I</em><sub><em>n</em></sub></span></p>
<p>Therefore,</p>
<p><span
class="math display">(<em>A</em><sup><em>T</em></sup><em>A</em>)<sup>−1</sup><em>A</em><sup><em>T</em></sup>
is a left inverse of A</span> ◻</p>
</div>
<div class="math-proposition">
<p><strong>Proposition 3</strong>. <em>If <span
class="math inline">rank (<em>A</em>) = <em>m</em></span>, then A has a
right inverse.</em></p>
</div>
<div class="math-proof">
<p><em>Proof.</em> Let <span class="math inline"><em>y</em></span> be an
arbitrary vector in <span
class="math inline">ℝ<sup><em>m</em></sup></span>.</p>
<p>Since <span
class="math inline">rank (<em>A</em>) = <em>m</em></span>, there exists
<span class="math inline"><em>x</em> ∈ ℝ<sup><em>m</em></sup></span>
such that <span
class="math inline"><em>A</em><em>x</em> = <em>y</em></span>, which
means <span
class="math inline">Col (<em>A</em>) = ℝ<sup><em>m</em></sup></span>.</p>
<p>Since <span
class="math inline">rank (<em>A</em>) = rank (<em>A</em><sup><em>T</em></sup>) = <em>m</em></span>
and <span
class="math inline"><em>m</em> = rank (<em>A</em><sup><em>T</em></sup>) + <em>n</em><em>u</em><em>l</em><em>i</em><em>t</em><em>y</em><em>A</em><sup><em>T</em></sup></span>.</p>
<p><span
class="math display"><em>N</em>(<em>A</em><sup><em>T</em></sup>) = {0}</span></p>
<p>Suppose that <span
class="math inline"><em>A</em><em>A</em><sup><em>T</em></sup> = 0</span>.
Then</p>
<p><span
class="math display"><em>x</em><sup><em>T</em></sup><em>A</em><em>A</em><sup><em>T</em></sup> = ‖<em>A</em><sup><em>T</em></sup><em>x</em>‖<sup>2</sup> = 0</span></p>
<p><span
class="math display"><em>N</em>(<em>A</em><em>A</em><sup><em>T</em></sup>) ⊆ <em>N</em>(<em>A</em><sup><em>T</em></sup>)</span></p>
<p>Since <span
class="math inline"><em>N</em>(<em>A</em><sup><em>T</em></sup>) = {0}</span>
, it follows that <span
class="math inline"><em>N</em>(<em>A</em><em>A</em><sup><em>T</em></sup>) = {0}</span>.</p>
<p>By using the rank-nulity theorem,</p>
<p><span
class="math display">rank (<em>A</em><em>A</em><sup><em>T</em></sup>) = <em>m</em></span></p>
<p>Because <span
class="math inline"><em>A</em><em>A</em><sup><em>T</em></sup></span> is
a square matrix, it is therefore invertible.</p>
<p><span
class="math display"><em>A</em><em>A</em><sup><em>T</em></sup>(<em>A</em><em>A</em><sup><em>T</em></sup>)<sup>−1</sup> = <em>A</em>(<em>A</em><sup><em>T</em></sup>(<em>A</em><em>A</em><sup><em>T</em></sup>)<sup>−1</sup>) = <em>I</em><sub><em>m</em></sub></span></p>
<p>Hence, <span
class="math inline"><em>A</em><sup><em>T</em></sup>(<em>A</em><em>A</em><sup><em>T</em></sup>)<sup>−1</sup></span>
is right inverse of A ◻</p>
</div>
