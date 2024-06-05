# intro_to_algorithms 
## Computational Assignment

**1. Sorting Algorithms**

This document explores the implementation and performance analysis of Insertion Sort and Merge Sort algorithms. The algorithms are designed to sort an array `A[1..n]` in non-decreasing order. You can choose any programming language (Java, C/C++, Python, Julia, etc.) for implementation. Additionally, plots will be used to analyze the performance of these algorithms across various input sizes.

**1.1 Insertion Sort**

```
function Insertion-Sort(A)
  for j ← 2 to length[A]
    key ← A[j]
    i ← j - 1
    while i > 0 and A[i] > key
      A[i + 1] ← A[i]
      i ← i - 1
    A[i + 1] ← key
```

**1.2 Merge Sort**

```
function Merge-Sort(A, p, r)
  if p < r
    q ← floor((p + r) / 2)
    Merge-Sort(A, p, q)
    Merge-Sort(A, q + 1, r)
    Merge(A, p, q, r)
```

**2. Gale-Shapley Algorithm**

This section will implement the Gale-Shapley algorithm in a chosen programming language. The implementation will be analyzed to verify its properties for randomly generated assignment scenarios and instances designed to expose specific algorithm behaviors.

**3. Skip Lists**

This section dives into Skip Lists, a data structure introduced by William Pugh in his article "Skip Lists: a probabilistic alternative to balanced trees" (Communications of the ACM, Volume 33, Issue 6, June 1990, Pages 668-676). Skip Lists employ probabilistic balancing instead of enforcing strict balancing in search trees.

**3.a Implementation**

* Read and understand the Skip Lists concept from the aforementioned article by William Pugh.
* Implement Skip Lists in a programming language (Python, C, Pascal, Java, etc.).

**3.b Performance Analysis**

* Define sets `Sn` containing `n` elements, specifically `S256`, `S4096`, and `S65536`. Fill these sets with randomly generated integer keys.
* Measure and display the running time for inserting elements into these sets as a function of `n ∈ {256, 4096, 65536}`. Include sets with intermediate cardinalities to gain a clearer understanding of the computational complexity of Skip Lists.

**3.c Removal Analysis**

* Remove 20% of the keys from each set randomly.
* Display the computational cost associated with this removal operation.

This markdown text outlines the tasks and analysis for the respective sections. Remember to replace placeholders like `<chosen programming language>` with your specific choice. 
