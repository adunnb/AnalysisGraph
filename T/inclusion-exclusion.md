---
layout: proof
title: "Inclusion–Exclusion Principle"
chapter: "Set Theory and Functions"
link_terms: ["inclusion–exclusion", "inclusion-exclusion"]
---

**Theorem:** For [finite sets](../D/finite-set) $A$ and $B$:

$$\#(A \cup B) = \# A + \# B - \#(A \cap B)$$

**Example:** For $A = \{1, 2, 3\}$ and $B = \{1, 2, 4\}$: $\#(A \cup B) = 3 + 3 - 2 = 4$.

**Remark:** Subtracting $\#(A \cap B)$ corrects for the elements counted twice, once in $A$ and once in $B$. When $A$ and $B$ are disjoint the correction is zero.

**Proof:** The decompositions:

$$A \cup B = A \cup (B \setminus A), \qquad B = (A \cap B) \cup (B \setminus A)$$

are both unions of [disjoint](../D/union-intersection) sets. By the [counting rules](../T/counting-rules):

$$\#(A \cup B) = \# A + \#(B \setminus A), \qquad \# B = \#(A \cap B) + \#(B \setminus A)$$

Subtracting the second equation from the first eliminates $\#(B \setminus A)$ and gives the formula.
