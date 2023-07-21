# leet-day7

# **Wildcard Pattern Matching**


**Problem Description**

Given an input string s and a pattern p, implement wildcard pattern matching with support for '?' and '*' where:

'?' Matches any single character.

'*' Matches any sequence of characters (including the empty sequence).

The matching should cover the entire input string (not partial).


Example 1:

Input: s = "aa", p = "a"

Output: false

Explanation: "a" does not match the entire string "aa".


Example 2:

Input: s = "aa", p = "*"

Output: true

Explanation: '*' matches any sequence.


Example 3:

Input: s = "cb", p = "?a"

Output: false

Explanation: '?' matches 'c', but the second letter is 'a', which does not match 'b'.


**Approach**

To solve this problem efficiently, we can use a two-pointer approach. We will use two pointers, one for the input string s and one for the pattern p, to traverse both strings simultaneously. We will handle the special cases of '?' and '*' in the pattern, and try to match characters one by one.

**Complexity Analysis**

Time complexity: O(n), where n is the length of the input string s.

Space complexity: O(1), as we are not using any additional data structures.





