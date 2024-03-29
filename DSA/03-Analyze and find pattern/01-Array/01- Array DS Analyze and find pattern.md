
### Source:
1. [Array](https://chat.openai.com/share/762f289f-108b-43bb-9ebb-f4070ab8f215)
2. [PDF-1](https://www.rose-hulman.edu/class/cs/csse120/Resources/C/Arrays/arrayPatterns.pdf)

### What type of problem i get in array:

1. **Prefix Sum Array Problems:**
	1. Store value of prefix sum of elements up to that position
		1. [Sum1](https://leetcode.com/problems/running-sum-of-1d-array/)
		2. [[724. Find Pivot Index]]
```
Input: [10, 2, -2, -20, 10], target = -10
Output: 3 (subarrays with sum -10: [10, 2, -2], [2, -2, -20, 10], [-20, 10])

```

2. **Two Pointer Technique**:
	1. It used to solving problems like finding pairs with certain property
	2. Finding subarrays that satisfy a specific condition
	3. Sums solved
		1. [[2108. Find First Palindromic String in the Array]]
```
Input: [2, 7, 11, 15], target = 9
Output: [2, 7] (indices 0 and 1)
```

3. **Sorting and Searching**:
	1. Sorting will help to solve many problems
	2. Searching will find elements that's in sorted array
	3. Sums solved
		1. [[1403. Minimum Subsequence in Non-Increasing Order]]
		2. [[2733. Neither Minimum nor Maximum]]

4. **Frequency Counting**:
	1. Counting occurrences of elements in the array or determining frequency of certain patterns within the array
```
Input: [4, 2, 8, 8, 4, 6, 8]
Output: 8 (appears 3 times)
```

5. **Sliding Window Technique**
	1. Find the maximum sum of a subarray of size k
```
Input: [2, 1, 5, 1, 3, 2], k = 3
Output: 9 (sum of subarray [5, 1, 3])
```

6. **Bit Manipulation:**
	1. Find single non-repeating element in an array where every other element appears twice
	2. Problems involving manipulating or transforming arrays in various ways.
```
Input: [4, 3, 6, 4, 3, 5, 6]
Output: 5
```

