Sum of Squares of Special Elements
==================================

PROBLEM
Given a 1-indexed integer array nums of length n, an element nums[i] is
special if i divides n (n % i == 0). Return the sum of the squares of all
special elements.

EXAMPLES
Input:  nums = [1, 2, 3, 4]
Output: 21
Special positions: 1, 2, 4 -> 1^2 + 2^2 + 4^2 = 21

Input:  nums = [2, 7, 1, 19, 18, 3]
Output: 63
Special positions: 1, 2, 3, 6 -> 2^2 + 7^2 + 1^2 + 3^2 = 63

CONSTRAINTS
- 1 <= nums.length == n <= 50
- 1 <= nums[i] <= 50

APPROACH
Loop over the 1-indexed positions i from 1 to n. If n % i == 0, add
nums[i - 1] squared to the total. The "- 1" converts the 1-indexed
position to Python's 0-based indexing.

COMPLEXITY
- Time:  O(n)
- Space: O(1) extra

USAGE
    from sum_of_squares_of_special_elements import Solution

    s = Solution()
    print(s.sumOfSquares([1, 2, 3, 4]))             # 21
    print(s.sumOfSquares([2, 7, 1, 19, 18, 3]))     # 63

FILES
- sum_of_squares_of_special_elements.py : the solution

REFERENCE
LeetCode 2778 - Sum of Squares of Special Elements
