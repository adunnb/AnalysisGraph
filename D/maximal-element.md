---
layout: definition
title: "Maximal and Minimal Elements"
chapter: "Set Theory and Functions"
link_terms: ["maximal element", "minimal element", "maximal", "minimal"]
---

**Definition:** Let $(A, \preceq)$ be a [partially ordered set](../D/partial-order). An element $m \in A$ is:

1. **maximal** if $m \preceq a$ implies $a = m$, that is, no element of $A$ is strictly larger than $m$;
2. **minimal** if $a \preceq m$ implies $a = m$, that is, no element of $A$ is strictly smaller than $m$.

**Example:** Order the [proper subsets](../D/subset) of $X = \{1, 2, 3\}$ by inclusion. Each of the three two-element sets $\{1, 2\}$, $\{1, 3\}$, $\{2, 3\}$ is maximal, since none is contained in another proper subset. None of them contains the other two.

**Example:** Ordered by inclusion, the family of all finite subsets of $\mathbb{N}$ has no maximal element: for any finite $E \subseteq \mathbb{N}$, choose $n \notin E$, and then $E \subsetneq E \cup \{n\}$ is still finite. Its only minimal element is $\varnothing$.

**Example:** With the usual order, $[0, 1)$ has no maximal element, since $x < \frac{x+1}{2} < 1$ for every $x < 1$. Likewise $\mathbb{N}$ has no maximal element, since $n < n + 1$.

**Remark:** A maximal element need not be [greatest](../D/greatest-element): being maximal only says nothing is strictly larger, while other elements may be incomparable with it, as in the first example. In a [total order](../D/total-order) the two notions coincide ([Maximal elements in a total order](../T/total-order-maximal)).
