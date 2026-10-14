---
layout: definition
title: "Power Set"
chapter: "Set Theory and Functions"
link_terms: ["power set"]
---

**Definition:** The **power set** of a set $A$ is the set of all [subsets](../D/subset) of $A$:

$$\mathcal{P}(A) = \{B : B \subseteq A\}$$

It is also written $2^A$.

**Example:** $\mathcal{P}(\{1, 2\}) = \{\varnothing, \{1\}, \{2\}, \{1, 2\}\}$ and $\mathcal{P}(\varnothing) = \{\varnothing\}$.

**Remark:** The elements of $\mathcal{P}(A)$ are themselves sets, and $\varnothing$ and $A$ always belong to $\mathcal{P}(A)$. A [finite set](../D/finite-set) with $n$ elements has $2^n$ subsets ([Cardinality of the power set](../T/power-set-size)), which explains the notation $2^A$. For every set $A$, the power set is strictly larger than $A$ ([Cantor's theorem](../T/cantor-theorem)).
