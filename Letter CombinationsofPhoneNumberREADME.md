# leet-day7

_**Letter Combinations of a Phone Number**_


**Problem Description**

Given a string containing digits from 2 to 9 inclusive, return all possible letter combinations that the number could represent. The mapping of digits to letters is the same as on a telephone keypad. Note that the digit '1' does not map to any letters.

You need to find all possible letter combinations that the input number could represent and return them in any order.

Examples

Input: digits = "23" 

Output: ["ad","ae","af","bd","be","bf","cd","ce","cf"]  

Explanation: The input "23" represents the digits 2 and 3 on a telephone keypad. The letter 'a' is mapped to digit 2, and 'b' and 'c' are mapped to digit 3. The output lists all possible letter combinations formed from these mappings.


Input: digits = ""

Output: []

Explanation: An empty input should return an empty output array since there are no letter combinations possible.


**Constraints**


The input string digits has a length between 0 and 4, inclusive.

Each character in digits is a digit in the range from '2' to '9'.


**Approach**

To solve this problem, we can use backtracking to generate all possible letter combinations. We can maintain a current string and iterate through each digit in the input digits. For each digit, we find the corresponding letters based on the keypad mapping and recursively generate all possible combinations.


**Time Complexity**

The time complexity of this approach is O(3^N * 4^M), where N is the number of digits with three letters ('7', '9') and M is the number of digits with four letters ('2', '3', '4', '5', '6', '8'). The reason is that each digit with three letters can have three possible letter combinations, and each digit with four letters can have four possible letter combinations. Since each digit is processed independently, we multiply the possibilities together.

**Space Complexity**

The space complexity of this approach is O(N+M), where N is the number of digits with three letters ('7', '9') and M is the number of digits with four letters ('2', '3', '4', '5', '6', '8'). The space is used to store the current string in the backtracking process.

_**Implementation**_

The solution to this problem can be implemented in C++ using the provided code in the previous response. It uses backtracking to generate all possible letter combinations. The letterCombinations function takes the input string digits and returns a vector of strings containing all the possible letter combinations.
