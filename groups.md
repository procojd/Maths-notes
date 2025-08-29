# Groups in Abstract Algebra

## 1. Introduction
A **Group** is a fundamental concept in abstract algebra.  
It is a set equipped with a binary operation that satisfies four conditions: **closure, associativity, identity, and invertibility**.

---

## 2. Formal Definition
A group is a pair **(G, *)**, where:
- **G** is a non-empty set.
- **\*** is a binary operation on G (`* : G × G → G`).

It satisfies the following axioms:

1. **Closure**  
   For all `a, b ∈ G`, `a * b ∈ G`.

2. **Associativity**  
   For all `a, b, c ∈ G`,  
   `(a * b) * c = a * (b * c)`.

3. **Identity Element**  
   There exists an element `e ∈ G` such that for all `a ∈ G`,  
   `e * a = a * e = a`.

4. **Inverse Element**  
   For each `a ∈ G`, there exists an element `a⁻¹ ∈ G` such that  
   `a * a⁻¹ = a⁻¹ * a = e`.

---

## 3. Examples of Groups

### Example 1: Integers under Addition
- Set: `ℤ`
- Operation: Addition `+`
- Identity: `0`
- Inverse: `-a` for each `a ∈ ℤ`
- Properties:
  - Closed under addition.
  - Associative: `(a + b) + c = a + (b + c)`.
  - Identity: `0`.
  - Inverse: `a + (-a) = 0`.

Thus, **(ℤ, +)** is a group.

---

### Example 2: Non-Zero Rational Numbers under Multiplication
- Set: `ℚ* = ℚ \ {0}`
- Operation: Multiplication `×`
- Identity: `1`
- Inverse: `1/a` for each `a ∈ ℚ*`
- Properties:
  - Closed under multiplication.
  - Associative: `(a × b) × c = a × (b × c)`.
  - Identity: `1`.
  - Inverse: `a × (1/a) = 1`.

Thus, **(ℚ*, ×)** is a group.

---

## 4. Types of Groups

1. **Abelian Group (Commutative Group)**  
   - If `a * b = b * a` for all `a, b ∈ G`, the group is **Abelian**.  
   - Example: `(ℤ, +)` is Abelian.

2. **Non-Abelian Group (Non-Commutative Group)**  
   - If commutativity does not hold for some elements, the group is **Non-Abelian**.  
   - Example: Group of 2×2 invertible matrices under multiplication.

3. **Finite and Infinite Groups**  
   - **Finite Group**: Number of elements is finite. The count is called the **order of the group**.  
     Example: Symmetry group of a triangle has 6 elements.  
   - **Infinite Group**: Infinite number of elements.  
     Example: `(ℤ, +)`.

---

## 5. Subgroups
A **subgroup** H of G is a subset of G such that:
- `(H, *)` itself forms a group under the same operation.  

### Example:
- `(2ℤ, +)` is a subgroup of `(ℤ, +)`.

---

## 6. Cyclic Groups
- A group is **cyclic** if there exists an element `g ∈ G` such that  
  every element of the group can be written as `gⁿ`.  
- `g` is called a **generator**.

Example:  
- `(ℤ, +)` is cyclic with generator `1` (or `-1`).

---

## 7. Cosets
- Given a subgroup `H ⊆ G` and an element `a ∈ G`, the **left coset** of H with respect to a is:  
  `aH = {a * h | h ∈ H}`.

- Similarly, the **right coset** is:  
  `Ha = {h * a | h ∈ H}`.

---

## 8. Normal Subgroups
- A subgroup `N` of `G` is **normal** if:  
  `gN = Ng` for all `g ∈ G`.

- Notation: `N ⊴ G`.

---

## 9. Quotient Groups
- If `N ⊴ G`, we can form the **quotient group** `G/N`.  
- Its elements are the cosets of N in G.

---

## 10. Applications of Groups
- **Symmetry** in geometry (rotations, reflections).
- **Cryptography** (RSA, elliptic curves).
- **Physics** (conservation laws, quantum mechanics).
- **Computer Science** (error correcting codes, automata).

---

## 11. Summary
- A group is a set with a binary operation that satisfies closure, associativity, identity, and inverse.  
- Groups can be Abelian or non-Abelian, finite or infinite.  
- Important concepts: subgroups, cyclic groups, cosets, normal subgroups, quotient groups.  
- Groups have wide applications in mathematics and science.
