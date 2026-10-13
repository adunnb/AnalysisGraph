---
layout: proof
title: "Uniqueness of Finite Cardinality"
chapter: "Set Theory and Functions"
link_terms: ["uniqueness of finite cardinality"]
---

**Theorem:** If a set $X$ has the same [cardinality](../D/cardinality) as both $[n]$ and $[m]$, where $n, m \in \mathbb{N}_0$, then $n = m$.

**Remark:** This is what makes $\# X$ well defined for a [finite set](../D/finite-set). It is not merely a convention: the theorem rules out a set being in bijection with two different $[n]$.

**Lemma (deleting one element):** If $f : X \to [n]$ is a [bijection](../D/bijective) with $n \geq 1$, then for each $x \in X$ there is a bijection $X \setminus \{x\} \to [n - 1]$.

**Proof of the lemma:** Let $j = f(x)$. The [restriction](../D/function) of $f$ is a bijection $X \setminus \{x\} \to [n] \setminus \{j\}$. Composing with the relabeling:

$$h(t) = \begin{cases} t & \text{if } t < j \\ t - 1 & \text{if } t > j \end{cases}$$

which is a bijection $[n] \setminus \{j\} \to [n - 1]$, gives the result. For $n = 1$, both sets are empty and the empty map is a bijection.

**Proof of the theorem:** We use [induction](../T/induction) on $n$, proving the statement for all $m \in \mathbb{N}_0$ at once. If $n = 0$, then $X = \varnothing$; a map from $\varnothing$ cannot be onto a nonempty set, so $m = 0$.

Suppose the statement holds for $n$, and let $X \sim [n + 1]$ and $X \sim [m]$. Then $X$ is nonempty, so $m \geq 1$. Choose $x \in X$. By the lemma:

$$X \setminus \{x\} \sim [n], \qquad X \setminus \{x\} \sim [m - 1]$$

By the induction hypothesis, $n = m - 1$, so $m = n + 1$.
