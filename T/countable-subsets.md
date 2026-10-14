---
layout: proof
title: "Subsets of Countable Sets"
chapter: "Set Theory and Functions"
link_terms: ["subsets of countable sets"]
---

**Theorem:** Every [subset](../D/subset) of $\mathbb{N}$ is [countable](../D/countable). More generally, every subset of a countable set is countable, and if there is an [injection](../D/injective) from $S$ into a countable set, then $S$ is countable.

**Remark:** An injection only shows that a set is *at most* countable. To conclude that it is denumerable, one must also show it is infinite. This is the strategy for the rationals.

**Proof:** Let $A \subseteq \mathbb{N}$. If $A$ is [finite](../D/finite-set) there is nothing to prove, so suppose $A$ is infinite. Choose its elements in increasing order, using the well-ordering principle:

$$a_1 = \min A, \qquad a_{k+1} = \min\bigl(A \setminus \{a_1, \ldots, a_k\}\bigr)$$

The set $A \setminus \{a_1, \ldots, a_k\}$ is nonempty, since otherwise $A$ would be finite. Each $a_{k+1}$ lies in the set from which $a_k$ was the [least element](../D/greatest-element) and differs from $a_k$, so $a_1 < a_2 < a_3 < \cdots$. In particular the $a_k$ are distinct, and by [induction](../T/induction) $a_k \geq k$ for every $k$.

Every element of $A$ is eventually chosen. If some $a \in A$ were never chosen, then $a \in A \setminus \{a_1, \ldots, a_k\}$ for every $k$, so $a_{k+1} \leq a$ for every $k$. Taking $k = a$ gives $a + 1 \leq a_{a+1} \leq a$, a contradiction. Hence $k \mapsto a_k$ is a [bijection](../D/bijective) $\mathbb{N} \to A$.

For a subset $S$ of a denumerable set $T$, a bijection $g : T \to \mathbb{N}$ restricts to a bijection from $S$ onto $g(S) \subseteq \mathbb{N}$, which is countable; a set in bijection with a countable set is countable. For a subset of a finite set, use the [counting rules](../T/counting-rules). Finally, an injection $f : S \to T$ is a bijection from $S$ onto the subset $f(S)$ of $T$.
