# Theory: Longest Common Subsequence

## Definition
The Longest Common Subsequence (LCS) of two sequences is the longest sequence that appears in the same relative order in both sequences, but not necessarily contiguously.

## Applications
- DNA sequence alignment in bioinformatics
- Version control systems (diff utility)
- Plagiarism detection
- Speech recognition

## Algorithmic Approaches

### 1. Standard Dynamic Programming
- Build DP table of size (n+1)×(m+1)
- Recurrence relation:
if A[i] == B[j]:
dp[i][j] = dp[i-1][j-1] + 1
else:
dp[i][j] = max(dp[i-1][j], dp[i][j-1])

### 2. Rolling Array Optimization
- Store only two rows at a time
- Reduces space from O(nm) to O(m)
- Can reconstruct LCS with additional steps

### 3. Hirschberg's Algorithm
- Divide-and-conquer approach
- Optimal O(nm) time, O(m) space
- Suitable for large sequences

## Complexity Analysis
| Algorithm | Time | Space |
|-----------|------|-------|
| Standard DP | O(nm) | O(nm) |
| Rolling Array | O(nm) | O(m) |
| Hirschberg | O(nm) | O(m) |