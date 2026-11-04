# Dimension Theorem

<div class="math-lemma">

**Lemma.**

**Lemma 1** (Replacement Lemma). *Let $V$ be a vector space spanned by $n$ vectors. Then every linearly independent subset of $V$ contains at most $n$ vectors.*

</div>
<div class="math-theorem">

**Theorem.**

**Theorem 1** (Dimension Theorem). *Let $V$ be a finite-dimensional vector space. Then any two bases of $V$ have the same number of elements.*

</div>
<div class="math-proof">

**Proof.**

*Proof.* Let $$B_1 = \{v_1,v_2,\ldots,v_m\}$$ and $$B_2 = \{w_1,w_2,\ldots,w_n\}$$ be two bases of $V$.

Since $B_1$ is linearly independent and $B_2$ spans $V$, the Replacement Lemma implies that $$m \leq n.$$

Similarly, since $B_2$ is linearly independent and $B_1$ spans $V$, we obtain $$n \leq m.$$

Combining these inequalities, $$m \leq n
\quad \text{and} \quad
n \leq m,$$ we conclude that $$\boxed{m=n}.$$

Therefore, any two bases of $V$ have the same number of elements. ◻

</div>
<div class="math-definition">

**Definition.**

**Definition 1** (Dimension). *The dimension of a finite-dimensional vector space $V$ is the number of vectors in any basis of $V$.*

*It is denoted by $$\dim(V)=n.$$*

</div>
