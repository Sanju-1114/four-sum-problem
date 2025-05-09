# Four Sum Problem

## Overview

This repository contains a C++ solution for the **Four Sum** problem. The goal of the problem is to find all unique quadruplets in an array of integers that sum to zero.

## Problem Description

Given an array `nums` of `n` integers, find all unique quadruplets `[nums[a], nums[b], nums[c], nums[d]]` such that:

- `0 <= a, b, c, d < n`
- `a`, `b`, `c`, and `d` are distinct
- `nums[a] + nums[b] + nums[c] + nums[d] == 0`

The solution must not contain duplicate quadruplets.


## Solution Approach

The provided solution uses a **Two Pointer Approach** to efficiently find the quadruplets. Here's a brief overview:

1. **Sort the Array**: Sorting helps in handling duplicates and enables the two-pointer technique.
2. **Nested Loops**: Two outer loops (`i` and `j`) select the first two numbers of the quadruplet.
3. **Two Pointers**: For each pair `(i, j)`, two pointers (`p` and `q`) are used to find the remaining two numbers such that their sum equals zero.
4. **Avoid Duplicates**: Skip duplicate values for `i`, `j`, and `p` to ensure unique quadruplets.
5. **Long Long for Sum**: Use `long long` to prevent integer overflow when calculating the sum of four numbers.

The time complexity is **O(n³)**, where `n` is the size of the input array.


## Code Explanation

- **Input**: A vector of integers (`nums`).
- **Output**: A vector of vectors, where each inner vector contains four integers that sum to zero.
- **Key Functions**:
  - `fourSum(vector<int>& nums)`: Implements the two-pointer approach to find all valid quadruplets.
  - `main()`: Demonstrates the solution with a sample input `{-2, -2, -1, -1, 1, 1, 2, 2}` and prints the resulting quadruplets.

## How to Run

1. **Clone the Repository**:

   ```bash
   git clone https://github.com/Sanju-1114/four-sum-problem.git
   ```
2. **Navigate to the Directory**:

   ```bash
   cd four-sum-problem
   ```
3. **Compile the Code**:

   ```bash
   g++ four_sum.cpp -o four_sum
   ```
4. **Run the Executable**:

   ```bash
   ./four_sum
   ```

## Example Output

For the input `{-2, -2, -1, -1, 1, 1, 2, 2}`, the program outputs:

```
-2  -1 1 2
-2  -1 1 2
```

## Dependencies

- C++ Standard Library (included with any standard C++ compiler)
- No external libraries required

## License

This project is open-source and available under the MIT License.


## Contact
For any questions or suggestions, feel free to reach out to Sanju-1114.
