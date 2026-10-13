---
layout: proof
title: "Pigeonhole Principle"
chapter: "Set Theory and Functions"
link_terms: ["pigeonhole principle", "pigeonhole"]
---

**Theorem:** Let $X$ be a [finite set](../D/finite-set) and $f : X \to Y$ any [function](../D/function). Then the [image](../D/image) $f(X)$ is finite and:

$$\# f(X) \leq \# X$$

with equality if and only if $f$ is [injective](../D/injective). Consequently:

1. **(Pigeonhole principle)** If $Y$ is finite and $\# X > \# Y$, then no function $X \to Y$ is injective.
2. If $\# X = \# Y$ is finite, then a function $X \to Y$ is injective if and only if it is [surjective](../D/surjective).

**Remark:** In words: if more than $n$ pigeons sit in $n$ holes, some hole holds two pigeons. Equality characterizes injectivity, not surjectivity onto an arbitrary codomain $Y$; it says that $f : X \to f(X)$ is a [bijection](../D/bijective). Part 2 fails for infinite sets: $n \mapsto n + 1$ is injective but not surjective on $\mathbb{N}$.

**Proof:** We use [induction](../T/induction) on $n = \# X$. If $n = 0$, then $f(X) = \varnothing$ and $f$ is injective.

Suppose the statement holds for sets with $n$ elements, and let $\# X = n + 1$. Choose $x \in X$ and let $X' = X \setminus \{x\}$, which has $n$ elements by the [uniqueness of finite cardinality](../T/finite-cardinality-unique) lemma. Then $f(X) = f(X') \cup \{f(x)\}$. By the induction hypothesis, $f(X')$ is finite with $\# f(X') \leq n$. If $f(x) \in f(X')$, then $\# f(X) = \# f(X') \leq n$; otherwise $\# f(X) = \# f(X') + 1 \leq n + 1$ by the [counting rules](../T/counting-rules).

Equality $\# f(X) = n + 1$ therefore holds exactly when $\# f(X') = n$ and $f(x) \notin f(X')$. By the induction hypothesis, the first condition means $f$ is injective on $X'$; the second means $f(x) \neq f(x')$ for every $x' \neq x$. Together they say exactly that $f$ is injective.

For (1), an injective $f$ would give $\# X = \# f(X) \leq \# Y$, since $f(X) \subseteq Y$. For (2), if $f$ is injective then $\# f(X) = \# X = \# Y$, and a [subset](../D/subset) of $Y$ with as many elements as $Y$ is all of $Y$ by the counting rules, so $f$ is surjective. If $f$ is surjective then $\# f(X) = \# Y = \# X$, so $f$ is injective.
