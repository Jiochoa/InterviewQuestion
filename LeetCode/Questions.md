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

[[Walkthrough#1. Two Sum|Answer]]

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

[[Walkthrough#2. Add Two Numbers|Answer]]

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

[[Walkthrough#3. Longest Substring Without Repeating Characters|Answer]]

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

[[Walkthrough#4. Median of Two Sorted Arrays|Answer]]

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

[[Walkthrough#5. Longest Palindromic substring|Answer]]

### Solution 5