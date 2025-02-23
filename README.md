# Even-Odd Problem: Counting Violations in a Sequence

## Description
This project addresses the **Even-Odd Problem**, where we are given a sequence of requests with non-unique IDs. The goal is to process the requests in descending order of their IDs, but with a priority rule: requests with odd IDs must be processed before requests with even IDs. A **violation** occurs when, for any pair of indices `(i, j)` where `i < j`, the following conditions are met:
1. `a_i < a_j`
2. `a_i` is even
3. `a_j` is odd

The task is to count the number of such violations in a given sequence.

## Approaches
### 1. Brute Force Solution
The brute force approach involves iterating through all pairs of indices `(i, j)` where `i < j` and checking if the conditions for a violation are met. This approach has a time complexity of **O(n²)**.

### 2. Optimized Solution Using Merge Sort
To improve efficiency, the problem is solved using a modified **Merge Sort** algorithm. This approach reduces the time complexity to **O(n log n)** by leveraging the divide-and-conquer strategy and counting violations during the merge step.

## Key Features
- **Brute Force Implementation:** A straightforward solution to count violations by checking all pairs.
- **Optimized Merge Sort Implementation:** A more efficient solution using a modified merge sort algorithm.
- **Performance Comparison:** Demonstrates the significant performance improvement of the optimized solution over the brute force approach.

## Technologies Used
- Python
- NumPy (for generating random sequences)
