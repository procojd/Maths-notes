# Permutation Groups

## 1. Introduction
A **permutation** of a set is a bijective function (one-to-one and onto) from the set to itself.  
A **permutation group** is a set of permutations of a given set that forms a group under function composition.

---

## 2. Definition
Let \( S \) be a non-empty set.  
A **permutation group** \( G \) on \( S \) is a subgroup of the **symmetric group** \( Sym(S) \), which is the group of all bijections from \( S \) to \( S \) under composition.

- If \( |S| = n \), then the symmetric group on \( S \) is denoted by \( S_n \).
- \( S_n \) has \( n! \) elements.

---

## 3. Symmetric Group
- The **symmetric group** \( S_n \) is the group of all possible permutations of \( n \) objects.  
- Example:  
  For \( n = 3 \),  
  \[
  S_3 = \{ (1), (12), (13), (23), (123), (132) \}
  \]  
  where:
  - \((1)\) = identity permutation  
  - \((12)\) = swaps 1 and 2  
  - \((123)\) = sends \(1 \to 2, 2 \to 3, 3 \to 1\)

---

## 4. Cycle Notation
Permutations are often written in **cycle notation**:
- Example: \((123)\) means:
  \[
  1 \to 2, \quad 2 \to 3, \quad 3 \to 1
  \]
- Disjoint cycles can be written together:  
  \((12)(34)\) swaps 1 with 2, and 3 with 4.

---

## 5. Properties of Permutation Groups
1. **Closure**: The composition of two permutations is also a permutation.  
2. **Associativity**: Function composition is associative.  
3. **Identity**: The identity permutation exists.  
4. **Inverse**: Every permutation has an inverse.

Thus, permutation groups satisfy all group axioms.

---

## 6. Alternating Group
- The **alternating group** \( A_n \) is the subgroup of \( S_n \) consisting of **even permutations** (permutations that can be expressed as the product of an even number of transpositions).
- \( |A_n| = \frac{n!}{2} \).

Example:  
In \( S_3 \),  
\[
A_3 = \{ (1), (123), (132) \}
\]

---

## 7. Example
Consider \( S = \{1,2,3\} \).  
The symmetric group \( S_3 \) has 6 elements:  
- Identity: \((1)\)  
- Transpositions: \((12), (13), (23)\)  
- 3-cycles: \((123), (132)\)

These form a group under composition.

---

## 8. Applications
- Symmetry in geometry  
- Galois theory in algebra  
- Rubik’s cube solutions  
- Cryptography and coding theory

---

## 9. Summary
- A **permutation group** is a group formed by bijections of a set.  
- The **symmetric group** \( S_n \) contains all permutations of \( n \) elements.  
- The **alternating group** \( A_n \) contains only even permutations.  
- Permutation groups play a central role in group theory and many applications in mathematics and computer science.
