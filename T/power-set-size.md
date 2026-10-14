---
layout: proof
title: "Cardinality of the Power Set"
chapter: "Set Theory and Functions"
link_terms: ["cardinality of the power set"]
---

**Theorem:** If $X$ is a [finite set](../D/finite-set), then its [power set](../D/power-set) is finite and:

$$\# \mathcal{P}(X) = 2^{\# X}$$

**Example:** $\mathcal{P}(\{1, 2\}) = \{\varnothing, \{1\}, \{2\}, \{1, 2\}\}$ has $4 = 2^2$ elements, and a four-element set has $16$ subsets. For $X = \varnothing$, $\mathcal{P}(\varnothing) = \{\varnothing\}$ has $1 = 2^0$ element.

**Remark:** Informally, a subset of $\{x_1, \ldots, x_n\}$ is determined by $n$ independent yes-or-no choices, one for each $x_i$, so there are $2^n$ of them. For infinite sets the analogous statement is [Cantor's theorem](../T/cantor-theorem).

**Proof:** A [bijection](../D/bijective) $g : X \to [n]$ induces a bijection $\mathcal{P}(X) \to \mathcal{P}([n])$, $S \mapsto g(S)$, so it suffices to show $\# \mathcal{P}([n]) = 2^n$. We use [induction](../T/induction) on $n$. For $n = 0$, $\mathcal{P}(\varnothing) = \{\varnothing\}$ has one element.

Suppose $\# \mathcal{P}([n]) = 2^n$. The [subsets](../D/subset) of $[n + 1]$ split into two [disjoint](../D/union-intersection) families: those not containing $n + 1$, which are exactly the subsets of $[n]$, and those containing $n + 1$. The map $S \mapsto S \cup \{n + 1\}$ is a bijection from $\mathcal{P}([n])$ onto the second family, with inverse $T \mapsto T \setminus \{n + 1\}$. By the [counting rules](../T/counting-rules):

$$\# \mathcal{P}([n + 1]) = 2^n + 2^n = 2^{n+1}$$
