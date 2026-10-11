---
layout: proof
title: "Maximal Elements in a Total Order"
chapter: "Set Theory and Functions"
link_terms: ["maximal elements in a total order"]
---

**Theorem:** In a [totally ordered set](../D/total-order) $(A, \preceq)$, a [maximal element](../D/maximal-element), if one exists, is a [greatest element](../D/greatest-element) and is unique. Likewise, a minimal element, if one exists, is a least element and is unique.

**Remark:** Existence and uniqueness are separate questions. Totality does not force a maximal element to exist: $\mathbb{N}$ and $[0, 1)$ are totally ordered and have none. It only says that a maximal element is unique *if* one exists. In a [partial order](../D/partial-order) that is not total, an element can be maximal without being greatest.

**Proof:** Let $m$ be maximal and let $a \in A$. Since the order is total, $a \preceq m$ or $m \preceq a$. In the second case, maximality gives $a = m$, so $a \preceq m$ by reflexivity. In either case $a \preceq m$, so $m$ is a greatest element. Greatest elements are unique by antisymmetry, so $m$ is unique.

The argument for a minimal element is the same with every inequality reversed.
