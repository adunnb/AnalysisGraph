---
layout: definition
title: "Equivalence Relation"
chapter: "Set Theory and Functions"
link_terms: ["equivalence relation", "equivalence class"]
---

**Definition:** An **equivalence relation** on a [set](../D/set) $A$ is a [relation](../D/relation) $\sim$ on $A$ that is reflexive, symmetric, and transitive:

1. $a \sim a$ for every $a \in A$;
2. $a \sim b$ implies $b \sim a$;
3. $a \sim b$ and $b \sim c$ imply $a \sim c$.

The **equivalence class** of $a \in A$ is the set $[a] = \{b \in A : b \sim a\}$.

**Example:** Equality is an equivalence relation on any set; each equivalence class is a single element.

**Example:** For a fixed $n \in \mathbb{N}$, **congruence mod $n$** on $\mathbb{Z}$, defined by $a \equiv b \pmod{n}$ when $a - b$ is a multiple of $n$, is an equivalence relation. Its equivalence classes are the $n$ remainder classes $[0], [1], \ldots, [n-1]$.

**Example:** Two sets have the [same cardinality](../D/cardinality) when there is a [bijection](../D/bijective) between them. On any family of sets, this is an equivalence relation: the identity is a bijection, the [inverse](../D/inverse-function) of a bijection is a bijection, and a [composition of bijections](../T/composition-bijections) is a bijection.

**Remark:** The equivalence classes of an equivalence relation partition $A$: every element lies in exactly one class, and two classes are either equal or [disjoint](../D/union-intersection). Compare a [partial order](../D/partial-order), which is antisymmetric instead of symmetric.
