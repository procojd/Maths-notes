# Equivalence Relations and Partitions  

## 1. Relation (recap)  
A relation **R** on a set **A** is a subset of **A × A** (all ordered pairs from A).  
If (a, b) ∈ R, we say **a is related to b** and write **aRb**.  

**Example:**  
On A = {1,2,3}, let R = {(1,1), (2,2), (3,3), (1,3), (3,1)}.  
Here, 1R3 and 3R1.  

---

## 2. Equivalence Relation  
A relation R on a set A is called an **Equivalence Relation** if it satisfies:

- **Reflexive:** aRa for all a in A.  
- **Symmetric:** If aRb, then bRa.  
- **Transitive:** If aRb and bRc, then aRc.  

### Example 1: Congruence mod 3  
Let A = integers. Define aRb if a and b leave the same remainder when divided by 3.  
- Reflexive: a and a have the same remainder.  
- Symmetric: If a and b have same remainder, then b and a also do.  
- Transitive: If a and b have same remainder, and b and c have same remainder, then a and c also do.  

This is an **equivalence relation**.  

### Example 2: Same Length Strings  
Let S = {"cat", "dog", "fish", "ball"}.  
Define s1 R s2 if **length(s1) = length(s2)**.  
- "cat" R "dog" (both length 3).  
- "fish" R "ball" (both length 4).  

This relation is reflexive, symmetric, and transitive.  

---

## 3. Equivalence Class  
For a given a in A, the **equivalence class** of a is:  

[a] = { x in A | xRa }  

**Example (mod 3):**  
- [0] = {..., -6, -3, 0, 3, 6, ...}  
- [1] = {..., -5, -2, 1, 4, 7, ...}  
- [2] = {..., -4, -1, 2, 5, 8, ...}  

---

## 4. Partition of a Set  
A **partition** of a set A is a collection of subsets A1, A2, ..., Ak such that:  
1. None of the subsets are empty.  
2. The subsets are pairwise disjoint (no overlap).  
3. Their union is the whole set A.  

---

## 5. Connection  
- Every **equivalence relation** on a set A divides A into **equivalence classes**.  
- These equivalence classes form a **partition** of A.  

**Example:**  
Relation "same length" on S = {"cat","dog","fish","ball"}  
Partition of S = { {"cat","dog"}, {"fish","ball"} }  
