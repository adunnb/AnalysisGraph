---
layout: proof
title: "Extrema of Finite Totally Ordered Sets"
chapter: "Set Theory and Functions"
link_terms: ["extrema of finite totally ordered sets"]
---

**Theorem:** Every nonempty [finite](../D/finite-set) [totally ordered set](../D/total-order) $(A, \preceq)$ has a [greatest element and a least element](../D/greatest-element).

**Remark:** The hypotheses matter. The [empty set](../D/set) has no element that could be greatest or least, and infinite totally ordered sets such as $\mathbb{N}$ or $[0, 1)$ can fail to have a greatest element.

**Proof:** We prove the statement about greatest elements by [induction](../T/induction) on $n = \# A \geq 1$; for least elements, reverse every inequality.

If $n = 1$, the single element of $A$ is greatest, by reflexivity.

Suppose every totally ordered set with $n$ elements has a greatest element, and let $\# A = n + 1$. Choose a [bijection](../D/bijective) $f : [n+1] \to A$, write $a_i = f(i)$, and let $A' = \{a_1, \ldots, a_n\}$. Then $f$ restricts to a bijection $[n] \to A'$, so $A'$ is a totally ordered set with $n$ elements and has a greatest element $M'$. Since the order is total, $M' \preceq a_{n+1}$ or $a_{n+1} \preceq M'$. Let $M$ be $a_{n+1}$ in the first case and $M'$ in the second. Then $a \preceq M' \preceq M$ for every $a \in A'$ by transitivity, and $a_{n+1} \preceq M$, so $M$ is a greatest element of $A$.
