---
layout: definition
title: "Greatest and Least Elements"
chapter: "Set Theory and Functions"
link_terms: ["greatest element", "least element"]
---

**Definition:** Let $(A, \preceq)$ be a [partially ordered set](../D/partial-order). An element $M \in A$ is:

1. a **greatest element** if $a \preceq M$ for every $a \in A$;
2. a **least element** if $M \preceq a$ for every $a \in A$.

**Example:** For any set $X$, under inclusion the [power set](../D/power-set) $\mathcal{P}(X)$ has greatest element $X$ and least element $\varnothing$.

**Example:** With the usual order, $0$ is the greatest element of $(-\infty, 0]$, while $(-\infty, 0)$ and $[0, 1)$ have no greatest element. Every nonempty [subset](../D/subset) of $\mathbb{N}$ has a least element; this is the well-ordering principle behind [mathematical induction](../T/induction).

**Remark:** A greatest element is [maximal](../D/maximal-element), but a maximal element need not be greatest. A greatest element, when it exists, is unique: if $M$ and $M'$ are both greatest, then $M \preceq M'$ and $M' \preceq M$, so $M = M'$ by antisymmetry. The same holds for least elements. In $\mathbb{R}$, a set's greatest element is also its [supremum](../D/supremum), but a supremum need not belong to the set.
