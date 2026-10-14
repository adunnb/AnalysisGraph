---
layout: proof
title: "Products of Countable Sets"
chapter: "Set Theory and Functions"
link_terms: ["products of countable sets"]
---

**Theorem:** The set $\mathbb{N} \times \mathbb{N}$ is [denumerable](../D/countable). Consequently, if $A$ and $B$ are denumerable, then so is their [Cartesian product](../D/cartesian-product) $A \times B$, and by [induction](../T/induction) so is any finite product of denumerable sets.

**Remark:** The idea is to list the pairs diagonal by diagonal, by increasing $i + j$:

$$(1,1);\quad (1,2),\ (2,1);\quad (1,3),\ (2,2),\ (3,1);\quad \ldots$$

Each diagonal is finite, so every pair is reached after finitely many steps. The formula below makes this precise.

**Proof:** For $d \in \mathbb{N}_0$ let $T(d) = \frac{d(d+1)}{2}$, so $T(0) = 0 < T(1) < T(2) < \cdots$ and $T(d) - T(d-1) = d$. Define:

$$f(i, j) = T(i + j - 2) + j$$

The pairs with $i + j - 1 = d$ are $(d, 1), (d - 1, 2), \ldots, (1, d)$, with $j = 1, \ldots, d$, and $f$ sends them to $T(d - 1) + 1, \ldots, T(d)$, one each. As $d$ runs through $\mathbb{N}$, these blocks of integers are [disjoint](../D/union-intersection) and cover all of $\mathbb{N}$. So $f : \mathbb{N} \times \mathbb{N} \to \mathbb{N}$ is a [bijection](../D/bijective): given $m \in \mathbb{N}$, the unique $d$ with $T(d - 1) < m \leq T(d)$ and then $j = m - T(d - 1)$, $i = d + 1 - j$ recover the only pair sent to $m$.

For denumerable $A$ and $B$, bijections $a : \mathbb{N} \to A$ and $b : \mathbb{N} \to B$ give a bijection $\mathbb{N} \times \mathbb{N} \to A \times B$, $(i, j) \mapsto (a(i), b(j))$. Its [composition](../D/composition) with $f^{-1}$ is a bijection $\mathbb{N} \to A \times B$.
