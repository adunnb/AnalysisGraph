---
layout: proof
title: "Unions of Countable Sets"
chapter: "Set Theory and Functions"
link_terms: ["unions of countable sets"]
---

**Theorem:** If $A$ and $B$ are [disjoint](../D/union-intersection) [denumerable](../D/countable) sets, then $A \cup B$ is denumerable. By [induction](../T/induction), the union of any finite nonempty family of pairwise disjoint denumerable sets is denumerable.

**Remark:** Disjointness is only needed for the literal interleaving below. Using [subsets of countable sets](../T/countable-subsets), any union of two countable sets is countable, since $A \cup B = A \cup (B \setminus A)$.

**Proof:** Write $A = \{a_1, a_2, \ldots\}$ and $B = \{b_1, b_2, \ldots\}$ as lists without repetition, using [bijections](../D/bijective) $\mathbb{N} \to A$ and $\mathbb{N} \to B$. Interleave the two lists:

$$a_1,\ b_1,\ a_2,\ b_2,\ a_3,\ b_3,\ \ldots$$

that is, $h(2k - 1) = a_k$ and $h(2k) = b_k$. Every element of $A \cup B$ appears in this list, and since $A$ and $B$ are disjoint, no element appears twice. So $h : \mathbb{N} \to A \cup B$ is a bijection.
