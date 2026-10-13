---
layout: definition
title: "Cardinality"
chapter: "Set Theory and Functions"
link_terms: ["cardinality", "same cardinality", "equinumerous"]
---

**Definition:** [Sets](../D/set) $A$ and $B$ have the **same cardinality**, written $A \sim B$, if there is a [bijection](../D/bijective) $A \to B$. We write $\operatorname{card}(A) \leq \operatorname{card}(B)$ if there is an [injection](../D/injective) $A \to B$.

**Example:** $\{a, b, c\} \sim \{1, 2, 3\}$, via $a \mapsto 1$, $b \mapsto 2$, $c \mapsto 3$. The map $n \mapsto 2n$ is a bijection from $\mathbb{N}$ onto the even natural numbers, so these two sets have the same cardinality even though one is a [proper subset](../D/subset) of the other.

**Remark:** Cardinality compares the sizes of sets without looking at what their elements are. On any family of sets, $\sim$ is an [equivalence relation](../D/equivalence-relation): the identity is a bijection, the [inverse](../D/inverse-function) of a bijection is a bijection, and a [composition of bijections](../T/composition-bijections) is a bijection. An injection $A \to B$ places the elements of $A$ inside $B$ without collisions, which is why it means "$A$ is no larger than $B$."
