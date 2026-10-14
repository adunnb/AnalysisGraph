---
layout: proof
title: "The Integers Are Countable"
chapter: "Set Theory and Functions"
link_terms: ["integers are countable"]
---

**Theorem:** The set $\mathbb{Z}$ of integers is [denumerable](../D/countable). An explicit [bijection](../D/bijective) $f : \mathbb{N} \to \mathbb{Z}$ is:

$$f(2k + 1) = k \quad (k \in \mathbb{N}_0), \qquad f(2k) = -k \quad (k \in \mathbb{N})$$

**Remark:** The bijection lists the integers as $0, -1, 1, -2, 2, -3, 3, \ldots$: nonnegative integers at the odd positions and negative integers at the even positions. Although $\mathbb{N} \subsetneq \mathbb{Z}$, the two sets have the [same cardinality](../D/cardinality), which is impossible for [finite sets](../D/finite-set) by the [counting rules](../T/counting-rules).

**Proof:** Every $n \in \mathbb{N}$ is either odd, $n = 2k + 1$ with $k \in \mathbb{N}_0$, or even, $n = 2k$ with $k \in \mathbb{N}$, and in exactly one way, so $f$ is well defined. On the odd numbers, $f$ is a bijection onto $\mathbb{N}_0 = \{0, 1, 2, \ldots\}$, with inverse $k \mapsto 2k + 1$. On the even numbers, $f$ is a bijection onto the negative integers $\{-1, -2, \ldots\}$, with inverse $-k \mapsto 2k$. Since these two [images](../D/image) are [disjoint](../D/union-intersection) and together make up $\mathbb{Z}$, $f$ is a bijection $\mathbb{N} \to \mathbb{Z}$.
