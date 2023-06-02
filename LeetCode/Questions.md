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
