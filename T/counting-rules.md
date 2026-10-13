---
layout: proof
title: "Counting Rules"
chapter: "Set Theory and Functions"
link_terms: ["counting rules"]
---

**Theorem:** Let $A$, $B$, $X$, $Y$ be [finite sets](../D/finite-set).

1. If $A$ and $B$ are [disjoint](../D/union-intersection), then $A \cup B$ is finite and $\#(A \cup B) = \# A + \# B$.
2. If $x \notin A$, then $\#(A \cup \{x\}) = \# A + 1$.
3. Every [subset](../D/subset) of a finite set is finite. If $A \subseteq B$, then $\# A \leq \# B$ and $\#(B \setminus A) = \# B - \# A$; if $A \subsetneq B$, then $\# A < \# B$.
4. $X \times Y$ is finite and $\#(X \times Y) = (\# X)(\# Y)$.

**Remark:** Part 3 fails for infinite sets: the even natural numbers form a proper subset of $\mathbb{N}$ with the [same cardinality](../D/cardinality).

**Proof of (1):** Let $f : A \to [n]$ and $g : B \to [m]$ be [bijections](../D/bijective). Since $A \cap B = \varnothing$, the map:

$$h(x) = \begin{cases} f(x) & \text{if } x \in A \\ n + g(x) & \text{if } x \in B \end{cases}$$

is well defined, and it is a bijection $A \cup B \to [n + m]$: $f$ fills $\{1, \ldots, n\}$ and $n + g$ fills $\{n + 1, \ldots, n + m\}$.

**Proof of (2):** Apply (1) with $B = \{x\}$.

**Proof of (3):** First, every subset $S$ of $[n]$ is finite with $\# S \leq n$, by [induction](../T/induction) on $n$. For $n = 0$, $S = \varnothing$. For the step, let $S \subseteq [n + 1]$ and $S' = S \setminus \{n + 1\} \subseteq [n]$, which is finite with $\# S' \leq n$. If $n + 1 \notin S$ then $S = S'$; otherwise $S = S' \cup \{n + 1\}$ and $\# S = \# S' + 1 \leq n + 1$ by (2).

In general, if $g : B \to [n]$ is a bijection and $A \subseteq B$, then $g$ restricts to a bijection from $A$ onto the subset $g(A)$ of $[n]$, so $A$ is finite and $\# A \leq n = \# B$. Since $B = A \cup (B \setminus A)$ is a disjoint union of finite sets, (1) gives $\# B = \# A + \#(B \setminus A)$. If $A \subsetneq B$, then $B \setminus A$ is nonempty, so $\#(B \setminus A) \geq 1$ and $\# A < \# B$.

**Proof of (4):** Bijections $X \to [n]$ and $Y \to [m]$ give a bijection $X \times Y \to [n] \times [m]$, so it suffices to count $[n] \times [m]$. If $n = 0$ or $m = 0$ the product is empty. Otherwise the map:

$$(i, j) \mapsto (i - 1)m + j$$

is a bijection $[n] \times [m] \to [nm]$: it lists the $m$ pairs with first coordinate $1$, then the $m$ pairs with first coordinate $2$, and so on. Its inverse is given by division with remainder.
