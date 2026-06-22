# Interpolation Search Algorithm

## Overview
This project implements the Interpolation Search algorithm in Python and compares its performance with Binary Search. Interpolation Search is an improved searching technique for uniformly distributed sorted data. Instead of always checking the middle element, it estimates the probable position of the target based on its value.

## Objective
- Implement the Interpolation Search algorithm.
- Compare its performance with Binary Search.
- Analyze execution time and number of comparisons for different input sizes.

## Algorithm
1. Initialize low and high indices.
2. Estimate the position of the target using the interpolation formula:
   
   pos = low + ((target - arr[low]) * (high - low)) / (arr[high] - arr[low])

3. If the target is found, return its index.
4. If the target is smaller, search the left subarray.
5. If the target is larger, search the right subarray.
6. Repeat until the element is found or the search range becomes invalid.

## Time Complexity
| Case | Complexity |
|--------|------------|
| Best Case | O(1) |
| Average Case | O(log log n) |
| Worst Case | O(n) |

## Space Complexity
- O(1)

## Features
- Efficient searching in uniformly distributed sorted arrays.
- Comparison with Binary Search.
- Measures execution time and number of comparisons.
- Performance analysis for different array sizes.

## Sample Output

```text
Array: [2, 5, 10, 15, 23, 35, 48, 60, 75, 90, 105, 120]
Searching for: 35

Found at index: 5
Comparisons: 2
```

## Applications
- Database indexing
- Searching in large sorted datasets
- Telephone directories
- Numerical data retrieval systems

## Conclusion
Interpolation Search performs faster than Binary Search when the data is uniformly distributed. It reduces the search space more effectively by predicting the likely position of the target element, making it suitable for large sorted datasets.
