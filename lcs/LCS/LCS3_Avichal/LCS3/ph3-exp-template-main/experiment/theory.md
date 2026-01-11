### Link your theory in here
# Theory: Longest Common Subsequence (LCS)

## 1. Introduction
The Longest Common Subsequence (LCS) problem is a classic computer science problem that finds applications in various domains including bioinformatics (DNA sequence alignment), version control systems (diff utility), and natural language processing.

## 2. Mathematical Definition
Given two sequences $X = x_1, x_2, \dots, x_m$ and $Y = y_1, y_2, \dots, y_n$, find the longest sequence $Z = z_1, z_2, \dots, z_k$ such that $Z$ is a subsequence of both $X$ and $Y$.

## 3. Dynamic Programming Approach

### 3.1 Recurrence Relation
Let $L[i][j]$ denote the length of LCS of prefixes $X[1..i]$ and $Y[1..j]$.

$$
L[i][j] =
\begin{cases}
0 & \text{if } i = 0 \text{ or } j = 0 \\
L[i-1][j-1] + 1 & \text{if } x_i = y_j \\
\max(L[i-1][j], L[i][j-1]) & \text{if } x_i \neq y_j
\end{cases}
$$

### 3.2 Time and Space Complexity
- **Time Complexity**: $O(mn)$ where $m$ and $n$ are lengths of sequences
- **Space Complexity**: $O(mn)$ for storing the DP table

## 4. Optimizations

### 4.1 Rolling Array Optimization
Instead of storing the entire $m \times n$ table, we can store only two rows at a time:
- Space complexity reduces to $O(\min(m, n))$
- Still maintains $O(mn)$ time complexity

### 4.2 Hirschberg's Algorithm
A divide-and-conquer approach that:
- Uses $O(mn)$ time
- Uses only $O(\min(m, n))$ space
- Can reconstruct the actual LCS

## 5. Applications
1. **Bioinformatics**: DNA and protein sequence alignment
2. **Version Control**: Comparing files in git/svn
3. **Plagiarism Detection**: Document similarity analysis
4. **Speech Recognition**: Word sequence alignment