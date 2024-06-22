## 1. Two Sum
Given an array of integers `nums` and an integer `target`, return _indices of the two numbers such that they add up to `target`_.
You may assume that each input would have **_exactly_ one solution**, and you may not use the _same_ element twice.
You can return the answer in any order.
**Example 1:**
```Java
Input: nums = [2,7,11,15], target = 9
Output: [0,1]
Explanation: Because nums[0] + nums[1] == 9, we return [0, 1]
```
**Example 2:**
```Java
Input: nums = [3,2,4], target = 6
Output: [1,2]
```
**Example 3:**
```Java
Input: nums = [3,3], target = 6
Output: [0,1]
```
**Constraints:**
-   `2 <= nums.length <= 104`
-   `-109 <= nums[i] <= 109`
-   `-109 <= target <= 109`
-   **Only one valid answer exists.**

**Follow-up:** Can you come up with an algorithm that is less than `O(n2)` time complexity?

### [[Walkthrough 1#1. Two Sum|Answer]]

### Solution 1
```Java
public int[] twoSum(int[] nums, int target) {
        for ( int i = 0; i < nums.length; i++ ) {
            for( int j = i + 1; j < nums.length; j++ ){
                if (target == nums[i] + nums[j]) {
                    return new int[] {i, j};
                }
            }
        }
        return null;
    }
```

----
## 2. Add Two Numbers

You are given two **non-empty** linked lists representing two non-negative integers. The digits are stored in **reverse order**, and each of their nodes contains a single digit. Add the two numbers and return the sum as a linked list.

You may assume the two numbers do not contain any leading zero, except the number 0 itself.

**Example 1:**

![](https://assets.leetcode.com/uploads/2020/10/02/addtwonumber1.jpg)

```Java
Input: l1 = [2,4,3], l2 = [5,6,4]
Output: [7,0,8]
Explanation: 342 + 465 = 807.
```

**Example 2:**

```Java
Input: l1 = [0], l2 = [0]
Output: [0]
```

**Example 3:**

```Java
Input: l1 = [9,9,9,9,9,9,9], l2 = [9,9,9,9]
Output: [8,9,9,9,0,0,0,1]
```
**Constraints:**

- The number of nodes in each linked list is in the range `[1, 100]`.
- `0 <= Node.val <= 9`
- It is guaranteed that the list represents a number that does not have leading zeros.

### [[Walkthrough 1#2. Add Two Numbers|Answer]]

### Solution 2
```Java
public ListNode addTwoNumbers(ListNode l1, ListNode l2) {
       ListNode solution = new ListNode(0,null);
       ListNode solutionRoot = solution;
       boolean carry = false;
       // traverse both l1 and l2 until both are null
        while(l1 != null || l2 != null){
		// sum = both values. if values don't exist make it 0
            int valueOfL1 = 0;
            int valueOfL2 = 0;
            if(l1 != null) valueOfL1 = l1.val;
            if(l2 != null) valueOfL2 = l2.val;
            int sum = valueOfL1 + valueOfL2;
            // if there's a carry
            if(carry) {
                sum += 1;
                carry = false;
            }
            // if sum has carry
            if(sum > 9) {
                sum -= 10;
                carry = true;
            }
            // add new link with val = sum to the solution
            solution.val = sum;
            // iterate l1 and l2
            if(l1 != null) l1 = l1.next;
            if(l2 != null) l2 = l2.next;
            // if either value is not null, make another node for the next iteration
            if (l1 != null || l2 != null) {
                solution.next = new ListNode(0, null);
                solution = solution.next;
            } else if (carry) {
                solution.next = new ListNode(1);
            }
        }
        // return
        return solutionRoot;
    }
```

----

## 3. Longest Substring Without Repeating Characters

Given a string `s`, find the length of the **longest substring**without repeating characters.

**Example 1:**
```Java
Input: s = "abcabcbb"
Output: 3
Explanation: The answer is "abc", with the length of 3.
```

**Example 2:**
```Java
Input: s = "bbbbb"
Output: 1
Explanation: The answer is "b", with the length of 1.
```

**Example 3:**
```Java
Input: s = "pwwkew"
Output: 3
Explanation: The answer is "wke", with the length of 3.
Notice that the answer must be a substring, "pwke" is a subsequence and not a substring.
```

**Constraints:**
- `0 <= s.length <= 5 * 104`
- `s` consists of English letters, digits, symbols and spaces.

### [[Walkthrough 1#3. Longest Substring Without Repeating Characters|Answer]]

### Solution 3

----

## 4. Median of Two Sorted Arrays

Given two sorted arrays `nums1` and `nums2` of size `m` and `n` respectively, return **the median** of the two sorted arrays.

The overall run time complexity should be `O(log (m+n))`.

**Example 1:**

```Java
Input: nums1 = [1,3], nums2 = [2]
Output: 2.00000
Explanation: merged array = [1,2,3] and median is 2.
```

**Example 2:**

```Java
Input: nums1 = [1,2], nums2 = [3,4]
Output: 2.50000
Explanation: merged array = [1,2,3,4] and median is (2 + 3) / 2 = 2.5.
```

**Constraints:**

- `nums1.length == m`
- `nums2.length == n`
- `0 <= m <= 1000`
- `0 <= n <= 1000`
- `1 <= m + n <= 2000`
- `-106 <= nums1[i], nums2[i] <= 106`

### [[Walkthrough 1#4. Median of Two Sorted Arrays|Answer]]

### Solution 4

```Java
public double findMedianSortedArrays(int[] nums1, int[] nums2) {
        int index1 = 0;
        int index2 = 0;
        boolean isValidNums1 = false;
        boolean isValidNums2 = false;
        Stack<Integer> eleStack = new Stack<>();
        boolean isEven = false;
        int totalLength = 0;
        // add lenghts to total only if they exist
        totalLength = (nums1 != null)? nums1.length:0;
        totalLength += (nums2 != null)? nums2.length:0;
        double middle = (double) totalLength / 2;
        // find out if its an even number
        if(totalLength % 2 == 0) isEven = true;
        // iterate middle number of times because we just need to get to the center
        for (int i = 0; i <= (int)middle; i++) {
            // find out if values are comparable
            if(nums1 != null && index1 < nums1.length) {
                isValidNums1 = true;
            }
            if(nums2 != null && index2 < nums2.length) {
                isValidNums2 = true;
            }
            // both values are comparable
            if (isValidNums1  && isValidNums2){
                if (nums1[index1] < nums2[index2]) {
                    eleStack.push(nums1[index1]);
                    index1++;
                } else {
                    eleStack.push(nums2[index2]);
                    index2++;
                }
            // only nums1 is comparable
            } else if(isValidNums1 && !isValidNums2){
                eleStack.push(nums1[index1]);
                index1++;
            // only nums2 is comparable
            } else if(!isValidNums1 && isValidNums2) {
                eleStack.push(nums2[index2]);
                index2++;
            // none are comparable
            } else {
                System.out.println("Error: trying to push without a valid array");
            }
            // reset
            isValidNums1 = false;
            isValidNums2 = false;
        }
        // if even, pop latest values and divide by 2
        if (isEven) {
            double val1 = eleStack.pop();
            double val2 = eleStack.pop();
            return (val1 + val2) / 2;
        // id odd just return the frist pop
        } else {
            return (double) eleStack.pop();
        }
    }
```

---

## 5. Longest Palindromic substring

Given a string `s`, return _the longest_ 
_palindromic_
_substring_
 in `s`.

**Example 1:**
```Java
Input: s = "babad"
Output: "bab"
Explanation: "aba" is also a valid answer.
```
**Example 2:**
```Java
Input: s = "cbbd"
Output: "bb"
```

**Constraints:**
- `1 <= s.length <= 1000`
- `s` consist of only digits and English letters.

### [[Walkthrough 1#5. Longest Palindromic substring|Answer]]

### Solution 5

----
## 8. String to Integer (atoi)

Implement the `myAtoi(string s)` function, which converts a string to a 32-bit signed integer (similar to C/C++'s `atoi` function).

The algorithm for `myAtoi(string s)` is as follows:

1. Read in and ignore any leading whitespace.
2. Check if the next character (if not already at the end of the string) is `'-'` or `'+'`. Read this character in if it is either. This determines if the final result is negative or positive respectively. Assume the result is positive if neither is present.
3. Read in next the characters until the next non-digit character or the end of the input is reached. The rest of the string is ignored.
4. Convert these digits into an integer (i.e. `"123" -> 123`, `"0032" -> 32`). If no digits were read, then the integer is `0`. Change the sign as necessary (from step 2).
5. If the integer is out of the 32-bit signed integer range `[-231, 231 - 1]`, then clamp the integer so that it remains in the range. Specifically, integers less than `-231` should be clamped to `-231`, and integers greater than `231 - 1` should be clamped to `231 - 1`.
6. Return the integer as the final result.

**Note:**

- Only the space character `' '` is considered a whitespace character.
- **Do not ignore** any characters other than the leading whitespace or the rest of the string after the digits.

**Example 1:**

```Java
Input: s = "42"
Output: 42
Explanation: The underlined characters are what is read in, the caret is the current reader position.

Step 1: "42" (no characters read because there is no leading whitespace)
         ^
Step 2: "42" (no characters read because there is neither a '-' nor '+')
         ^
Step 3: "42" ("42" is read in)
           ^
The parsed integer is 42.
Since 42 is in the range [-231, 231 - 1], the final result is 42.
```

**Example 2:**

```Java
Input: s = "   -42"
Output: -42
Explanation:
Step 1: "   -42" (leading whitespace is read and ignored)
            ^
Step 2: "   -42" ('-' is read, so the result should be negative)
             ^
Step 3: "   -42" ("42" is read in)
               ^
The parsed integer is -42.
Since -42 is in the range [-231, 231 - 1], the final result is -42.
```

**Example 3:**

```Java
Input: s = "4193 with words"
Output: 4193
Explanation:
Step 1: "4193 with words" (no characters read because there is no leading whitespace)
         ^
Step 2: "4193 with words" (no characters read because there is neither a '-' nor '+')
         ^
Step 3: "4193 with words" ("4193" is read in; reading stops because the next character is a non-digit)
             ^
The parsed integer is 4193.
Since 4193 is in the range [-231, 231 - 1], the final result is 4193.
```

**Constraints:**

- `0 <= s.length <= 200`
- `s` consists of English letters (lower-case and upper-case), digits (`0-9`), `' '`, `'+'`, `'-'`, and `'.'`.
### [[Walkthrough 1#8. String to Integer (atoi)|Answer]]

### Solution 8


----

## 10. Regular Expression Matching

Given an input string `s` and a pattern `p`, implement regular expression matching with support for `'.'` and `'*'` where:
- `'.'` Matches any single character.​​​​
- `'*'` Matches zero or more of the preceding element.
The matching should cover the **entire** input string (not partial).

**Example 1:**
```Java
Input: s = "aa", p = "a"
Output: false
Explanation: "a" does not match the entire string "aa".
```
**Example 2:**
```Java
Input: s = "aa", p = "a*"
Output: true
Explanation: '*' means zero or more of the preceding element, 'a'. Therefore, by repeating 'a' once, it becomes "aa".
```
**Example 3:**
```Java
Input: s = "ab", p = ".*"
Output: true
Explanation: ".*" means "zero or more (*) of any character (.)".
```

**Constraints:**
- `1 <= s.length <= 20`
- `1 <= p.length <= 20`
- `s` contains only lowercase English letters.
- `p` contains only lowercase English letters, `'.'`, and `'*'`.
- It is guaranteed for each appearance of the character `'*'`, there will be a previous valid character to match.

### [[Walkthrough 1#10. Regular Expression Matching|Answer]]

### Solution 10


----

## 11. Container With Most Water

You are given an integer array `height` of length `n`. There are `n` vertical lines drawn such that the two endpoints of the `ith` line are `(i, 0)` and `(i, height[i])`.

Find two lines that together with the x-axis form a container, such that the container contains the most water.

Return _the maximum amount of water a container can store_.

**Notice** that you may not slant the container.

**Example 1:**
![](https://s3-lc-upload.s3.amazonaws.com/uploads/2018/07/17/question_11.jpg)

```Java
Input: height = [1,8,6,2,5,4,8,3,7]
Output: 49
Explanation: The above vertical lines are represented by array [1,8,6,2,5,4,8,3,7]. In this case, the max area of water (blue section) the container can contain is 49.
```

**Example 2:**
```Java
Input: height = [1,1]
Output: 1
```

**Constraints:**

- `n == height.length`
- `2 <= n <= 105`
- `0 <= height[i] <= 104`

### [[Walkthrough 1#11. Container With Most Water|Answer]]

### Solution 10


----

## 13. Roman to integer

Roman numerals are represented by seven different symbols: `I`, `V`, `X`, `L`, `C`, `D` and `M`.

**Symbol**       **Value**
I             1
V             5
X             10
L             50
C             100
D             500
M             1000

For example, `2` is written as `II` in Roman numeral, just two ones added together. `12` is written as `XII`, which is simply `X + II`. The number `27` is written as `XXVII`, which is `XX + V + II`.

Roman numerals are usually written largest to smallest from left to right. However, the numeral for four is not `IIII`. Instead, the number four is written as `IV`. Because the one is before the five we subtract it making four. The same principle applies to the number nine, which is written as `IX`. There are six instances where subtraction is used:

- `I` can be placed before `V` (5) and `X` (10) to make 4 and 9. 
- `X` can be placed before `L` (50) and `C` (100) to make 40 and 90. 
- `C` can be placed before `D` (500) and `M` (1000) to make 400 and 900.

Given a roman numeral, convert it to an integer.

**Example 1:**
```Java
Input: s = "III"
Output: 3
Explanation: III = 3.
```

**Example 2:**
```java
Input: s = "LVIII"
Output: 58
Explanation: L = 50, V= 5, III = 3.
```

**Example 3:**
```java
Input: s = "MCMXCIV"
Output: 1994
Explanation: M = 1000, CM = 900, XC = 90 and IV = 4.
```

**Constraints:**

- `1 <= s.length <= 15`
- `s` contains only the characters `('I', 'V', 'X', 'L', 'C', 'D', 'M')`.
- It is **guaranteed** that `s` is a valid roman numeral in the range `[1, 3999]`.

### [[Walkthrough 1#13. Roman to integer|Answer]]

### Solution 13

-----
## 20. Valid Parentheses

Given a string `s` containing just the characters `'('`, `')'`, `'{'`, `'}'`, `'['` and `']'`, determine if the input string is valid.

An input string is valid if:

1. Open brackets must be closed by the same type of brackets.
2. Open brackets must be closed in the correct order.
3. Every close bracket has a corresponding open bracket of the same type.

**Example 1:**
```java
Input: s = "()"
Output: true
```

**Example 2:**
```java
Input: s = "()[]{}"
Output: true
```

**Example 3:**
```java
Input: s = "(]"
Output: false
```

**Constraints:**

- `1 <= s.length <= 104`
- `s` consists of parentheses only `'()[]{}'`.


### [[Walkthrough 1#20. Valid Parentheses|Answer]]

### Solution 20

----