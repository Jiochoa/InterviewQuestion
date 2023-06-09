---

excalidraw-plugin: parsed
tags: [excalidraw]

---
==⚠  Switch to EXCALIDRAW VIEW in the MORE OPTIONS menu of this document. ⚠==


# Text Elements
## 1. TwoSum

 ^IhXGGchF

nums ^EJQayqUG

2 ^NGmD7BIz

7 ^kdrNEY7K

11 ^4H8SMuN4

15 ^WTqYGFSg

target ^uxewmC0E

9 ^HM9Et0i7

INFO ^CuJHrOKm

- int[] nums: Array of integers
- int target: integer
- One solution
- don't use same element twice

> int[] twoSum (int[] nums, int target) <  ^4bKTrt45

EXAMPLE ^KtihYIHC

WALKTHROUGH ^xwmves8c

t ^5UZHxEyp

f ^UFySeXJW

return new int[] {i, j} ^GpTQ957t

return NULL ^dSX0TpvP

loop the nums (i = 0) ^riUQ2AqO

loop the nums (j = i + 1) ^jb8P1ZSP

if target == nums[i] + nums[j] ^MoAtt0Bz

BRUTEFORCE ^SiIIpeqI

- loop nums
    - loop nums (start one after the i )
        - if both nums are == target return them ^m0e83AsJ

OPTIMIZATION ^XL5Rzdin

O(n^2) ^96FkyxdY

I could use a hash map ^ul926vVY

loop nums ^7H3OK7CO

if current nums < target ^nVmcb4mY

temp = target - nums[i] ^2y7BvpjY

F ^TYh0V5nE

return NULL ^878P6nha

T ^slumvpno

Hash Table 
(key is number, 
value is the index) ^Bi68HoJB

nums ^lKkt4Gor

2 ^YXqfO2u9

7 ^tbAje1NO

11 ^ZiV4kI59

15 ^yFpW2N2s

target ^hBZ6nfIL

9 ^UXkpt7rV

if temp is in Hash   ^mc5mqui5

T ^RDR4NTGb

return temp index 
and current nums index ^hBSxODRt

F ^Qm2SjL3F

2 ^jy3f26ZR

0 ^TUHynmNq

O (n)  ^TDki9nQu

IMPLEMENTATION ^v4OfmmPE

[[LeetCode/Questions#Solution 1]] ^4DszYKaL

## 2. Add Two Numbers
 ^CjwqNKbu

INFO ^k7qRZbC9

- given two reversed non-negative integers made into Link List
    -  ex. 234 => 4-> 3-> 2
- return the sum of these numbers in reverse
- no leading zeros
    - ex. 034 ^YiC895uq

EXAMPLE ^SnaKSG0t

Input: l1 = [2,4,3], l2 = [5,6,4]
Output: [7,0,8]
Explanation: 342 + 465 = 807. ^3mh7wTWn

WALKTHROUGH ^oDIhD1vm

2 ^bQ9Kjc4G

4 ^LrJzMGg3

3 ^BY3tMLOh

5 ^q7xmGnTH

6 ^y3MQq29Y

4 ^RqHOIK5i

7 ^RzKJ3NZ7

0 ^W1G5e9CW

8 ^ebTfCNkg

- traverse both l1 and l2 (while either is not null)
    - sum = add the number
    - if carry
        - sum =+ 1
        - carry = false
    - if sum > 9 (has carry)
        - sum -= 10
        - carry = true
    - soliution.val = sum
    - iterrate l1 and l2
    - if either value is not null, make a link
    - if no next link but carry
        - add node with carry at the end
- return solutionRoot  ^UqLjPF1c

BRUTEFORCE ^4pQSL374

while l1 != null || l2 != null ^ejtyfHdN

valueOfL1 = 0 ^cuC54Pzm

valueOfL2 = 0 ^Jl3JxABL

if l1 != null ^EKYLN7r9

if l2 != null ^M9Fk06V7

T ^YUriF5yq

T ^5XJJAhkQ

valueOfL1 = l1.val ^CsbpHz1e

valueOfL2 = l2.val ^yISwYhXp

sum = valueOfL1 + valueOfL2 ^ZxNinOT2

if carry ^bdU8Spka

sum += 1
carry = false ^bAUMH9eb

T ^GSuPrClY

if sum > 9 ^LJhTz5ci

T ^tHHhdcrH

sum -= 10
carry = true ^wVwIqg3n

if l1 != null ^XTNcHyqj

if l2 != null ^UJkg4XXO

l1 = l1.next ^3eceJrTA

l2 = l2.next ^PUoVTY2C

T ^WyDR98C8

T ^eTMXarA5

if l1 != null || l2 != null ^RGZeWxgw

solution.next = new LL(0)
solution = solution.next ^21X7o51b

T ^Yhg6cteH

else if carry ^aM0MnguH

F ^VbZv4or5

solution.next = new LL(1) ^zhRP7JL5

T ^AqBeoXcy

return solutionRoot ^vMLPktr1

OPTIMIZATION ^VCCU9bsz

- Save space by overwriting l1 to place the results
 ^WzD1RNLk

IMPLEMENTATION ^KHAjE5i0

[[LeetCode/Questions#Solution 2]] ^8HEJKyGR

## 3. Longest Substring Without Repeating Characters
 ^xhM5EUUD

IMPLEMENTATION ^roA8ufOK

[[LeetCode/Questions#Solution 3]] ^NNWqlJlc

INFO ^GMHL0rQL

- String s: some string with size
- find the length (int) of the longest substring without repeated characters

 > int lenghtOfLongestSubstring(String s) < ^ZaCZwczy

EXAMPLE ^HLDADPi9

Input: s = "abcabcbb"
Output: 3
Explanation: The answer is "abc", with the length of 3. ^bHKtblkx

s =  ^Hcpkd9il

a b c a b c b b ^O9WPDf8g

answer = 3 ^LrTy4VPp

Input: s = "bbbbb"
Output: 1
Explanation: The answer is "b", with the length of 1. ^qsfNyCd1

s =  ^Cjhf1DmE

b b b b b ^8LchyRmr

answer = 1 ^DuNZWEmW

WALKTHROUGH ^d97KNsgQ

BRUTEFORCE ^awDk0lBX

- HM map = new HM()
- maxSize = 0
- for i=0; i < s.size; i++
    - char c = s.charAt(i)
    - if char not in map
        - add char to map, index
    - else
        - if size of map > maxSize
            - maxSize = map.size
        - i = map.get(c)
        - reset map
- return math.max maxSize, HM.size ^TJzEns7o

HashMap hp
maxSize = 0 ^6O8ooDM9

for i = 0; i < s.size; i++ ^mIdyLAej

char c = s.charAt(i) ^t4sY6wXv

if char not in map ^5GbI1Dya

add char to map ^MBRee8Me

T ^kVdmDfZi

else ^r3CyvYMt

if map.size >= maxSize ^l7Vr1W1T

maxSize = map.size ^3ZO2W5dZ

F ^OexmKV6X

T ^dg3ZClGf

i = map.get(c)
reset map ^IFmFOM5C

return math.max maxSize, HM.size ^acF9zMYQ

## 4. Median of Two Sorted Arrays
 ^5iylbkuX

INFO ^r4cG85MX

- two sorted arrays size <= 1000
    - nums1: int[] size m
    - nums2: int[] size n
- get the median of the two arrays
- time complexity has to be O (log (n+m))

 > double findMedianSortedArrays(int[] nums1, int[] nums2 < ^a2b23STU

EXAMPLE ^zFhOJ4IL

Input: nums1 = [1,3], nums2 = [2]
Output: 2.00000
Explanation: merged array = [1,2,3] and median is 2. ^1DmY6bW3

nums1 =  ^WD8Nvqq3

nums2 =  ^yerdBEBp

Input: nums1 = [1,2], nums2 = [3,4]
Output: 2.50000
Explanation: merged array = [1,2,3,4] and median is (2 + 3) / 2 = 2.5. ^Fq6dwvk2

nums1 =  ^9dS3OjAn

nums2 =  ^gxNuMUtL

WALKTHROUGH ^2W2MNvNT

BRUTEFORCE ^39LNsojw

- index1 = 0
- index2 = 0
- isValidn1 = false
- isValidn2 = false
- eleStack
- isEven = false
- totalLenght = 0
- add lenghts to total if exist
- middle = totalLen / 2
- if totalLen is even
    - isEven = true 
- traverse middle number of times
    -  push lowest number to the stack if exist
       // if statements checking valid entries
- if isEven
    - return eleQu.pop +eleQ.pop / 2
- else // its odd
    - return eleQ.pop ^Q1wWuBcj

int index1 = 0
int index2 = 0
bool isValidn1 = false
bool isValidn2 = false
Stack eleStack
bool isEven = false
double totalLenght = 0 ^KhqMIAub

totalLen =  ^VhgxddiH

totalLen += ^3v2udqof

if nums1 != null ^xX0dtknE

? ^yggfoPQl

nums1.len; 0 ^eAUcrbGd

if nums2 != null ^26z4DY0E

? ^5AAk21cK

nums2.len; 0 ^lAzkYAHh

double middle = totalLen / 2 ^FEp81Olq

if totalLen % 2 ^iXFgkvIs

T ^8lVrTGXP

isEven = true ^HgAyVWZA

for i = 0; i <= middle; i++ ^yHM1IhuC

if nums1 != null && index1 < nums1.len ^ryXRNAEw

if nums2 != null && index2 < nums2.len ^CO8SUKbN

T ^RkcFzKen

isValidn1 = true ^ufQY7RpN

T ^7o0IcGUM

isValidn2 = true ^F5Gj3LdF

if both are valid ^RBLxe1zd

elseif nums1 is valid only ^6xdptmqX

elseif nums2 is valid only ^P8WmMKNf

elseif none are valid ^jOCb8bFq

T ^riqi57Pn

eleStack.push(nums1[index1])
index1++ ^FfAoqAbR

eleStack.push(nums2[index2])
index2++ ^xAtyoG4x

if nums1[index] < nums2[index] ^XtkzbQgg

else ^ywBQiAMy

eleStack.push(nums1[index1])
index1++ ^j7MZjHWE

eleStack.push(nums2[index2])
index2++ ^wkFv7olp

shouldn't reach here ^r1sCVGVw

isValudn1 = false
isvaludn2 = false ^WjtWYwuI

if isEven ^LQuSoN04

else ^tjyHz7s2

return stack.pop + stack.pop / 2 ^ykpUG89g

return stack.pop ^78kTVTN0

T ^WAyHZxe1

IMPLEMENTATION ^PhwtVNwT

[[LeetCode/Questions#Solution 4]] ^Dy4mZlvk

## 5. Longest Palindromic substring
 ^g10tFFxD

IMPLEMENTATION ^0nS4OByO

[[LeetCode/Questions#Solution 5]] ^Q4qt0CVq

INFO ^XL6MFY2i

- Get the longest palindrome out of the given string
- s: String
    - between 1 and 1000 chars
    - only digits and English letters

> String longestPalindrome(String s) < ^iPySBb4F

EXAMPLE ^6OXOtOz9

Input: s = "babad"
Output: "bab"
Explanation: "aba" is also a valid answer. ^uTeXJ0gs

s = ^ME505CXW

Input: s = "cbbd"
Output: "bb" ^iwtpZdPp

s = ^mXhtfKSp

WALKTHROUGH ^C5VKkpwl

BRUTEFORCE ^w5bjdWB9

- curLongest = " "
- if s.len < 2, return s
- iterate string 
    - iterate string (from i to end)
        - if len i to j is shorter than 
          curLong, skip
        - curSub = all chars from i tp j
        - if curSub isPalindrome
            - curLongest = curSub
            - j = curLongest.len - 1  ^Rgp0ljmA

String curLongest = null ^ySQtmyjD

if s.len < 2 ^gDEJ3UsG

T ^WPxyK0Ph

return s ^taMMKozs

for i = 0; i < s.len; i++ ^yncwLfvN

for j = i; j < s.len; j++ ^VVdoI2YW

if isPalindrome(curSub) ^yezUe9A6

T ^xyh2wMIt

if curSub.len > curLongest.len ^z41nsNAC

T ^F5JbdS1y

curLongest = curSub ^PK7kNpnW

return curLongest ^0zl7uVyB

// isPalindrome s: String
- Dequeue = new dequeu()
- if str < 2 return s
- iterate s
    - add all chars to the deque
- loop s.len times / 2
    - if start of dequeue != end of dequeue
        - return false
- return true ^VZYUFZyh

- iterate s
    - iterate sIndex = i - 1; eIndex = i + 1; 
      not stIndex >= 0 && not enIndex <= s.len - 1
        - check substring (i - 1, i)
        - curSub = s.substring (startIndex, endIndex)
        - if curSub > curLongest
            - if isPal(curSub)
                - curLongest = curSub
    - reset start and end index ^Q58zagls

SecondSolution? ^gR6wU2vO

## 8. String to Integer (atoi)
 ^Rur1RGNw

IMPLEMENTATION ^txKTVQEb

[[LeetCode/Questions#Solution 10]] ^qFvkk2O0

INFO ^1XLVD5Xb

Implement a function which converts a 
string to a 32-bit signed integer
- ignore whitespaces
- check for + and -
- null answer is 0
- max is 2^31 min is -2^31 - 1
    - if bigger than that make it max
    - if smaller than that make it min
- ignore anything before and after the 
  number string ^hbY9mC6m

Input: s = "4193 with words"
Output: 4193
Explanation:
The parsed integer is 4193.
Since 4193 is in the range [-231, 231 - 1], the final result is 4193. ^TPHEztcL

EXAMPLE ^gvcG0D3u

WALKTHROUGH ^C94UUQqM

BRUTEFORCE ^fTXnsmfZ

- long result
- isValid = notLetter AND 
           notWhitespace AND ...
- iterate the string
    - if NOT isValid (str[i]), skip
    - if +, positive = true
    - if -, negative = true
    - if isNumers(str[i]) 
        - Stack.push (str[i])
- iterate stack i = 0
    - result += stack.pop * (10 * i)
    - if result < -2^31
        - return -2^31
    - if result > 2^31 - 1
        - return 2^31 - 1
- return result ^bC6w54eJ

## 10. Regular Expression Matching
 ^FC6Kc4U1

INFO ^EaF72K9B

Implement a regular expression matching 
with support for . and *
    - s :String 1 <= s.length <= 20 
    - p :String pattern 1 <= p.length <= 20
    - . Matches any single character
    - * Matches zero or more of the 
        preceding element 

> boolean isMatch(String  s, String p) <
 ^QS6xixLZ

EXAMPLE ^iC30sz9z

Input: s = "aa", p = "a"
Output: false
Explanation: "a" does not match the entire string "aa". ^bv4ytyYR

Input: s = "aa", p = "a*"
Output: true
Explanation: '*' means zero or more of the preceding element, 
'a'. Therefore, by repeating 'a' once, it becomes "aa". ^VuknZj0n

Input: s = "ab", p = ".*"
Output: true
Explanation: ".*" means "zero or more (*) of any character (.)". ^3ErbVFPg

WALKTHROUGH ^DQp9SlhM

BRUTEFORECE ^OKLnofNr

## 11. Container With Most Water
 ^7E6maRv2

IMPLEMENTATION ^TsBS2I7U

[[LeetCode/Questions#Solution 11]] ^xcIGUIFU

INFO ^1wV7KCko

Find two lines that together with 
the x-axis form a container, this 
container must contain the most water.
- height: int[]      (
- n:      int length ( n== heght.len )
- return the max water a container can store

>  int maxArea (int[] height) < ^BC6F8C7t

EXAMPLE ^lMxKPcvf

Input: height = [1,8,6,2,5,4,8,3,7]
Output: 49
Explanation: The above vertical lines are represented 
by array [1,8,6,2,5,4,8,3,7]. In this case, the max area 
of water (blue section) the container can contain is 49. ^zEW3vNBp

WALKTHROUGH ^JFj5GE8o

BRUTEFORECE ^DNPxkTHc

// iterate heights (start at the ends)
- maxArea = 0
- while startIndex < endIndex 
    - currArea = endIndex - startIndex 
      * min(heights[startIndex], heights[endIndex])
    - if currArea > currMaxArea
        - maxAea = currArea
- return MaxArea ^M0prJgM1

maxArea = 0
startIndex = 0
endIndex = height.len - 1 ^FvKJ5cc8

while startIndex < endIndex  ^ri3wmAZC

curArea = (endIndex - startIndex) 
* min (height[startIndex], height[endIndex]) ^knDqSQjd

if curArea > maxArea ^lnfT11Nh

T ^Qpaygbid

maxArea = cueArea ^eTlcueKy

return maxArea ^IGDlEbPR

%%
# Drawing
```json
{
	"type": "excalidraw",
	"version": 2,
	"source": "https://github.com/zsviczian/obsidian-excalidraw-plugin/releases/tag/1.9.2",
	"elements": [
		{
			"type": "text",
			"version": 351,
			"versionNonce": 81936755,
			"isDeleted": false,
			"id": "IhXGGchF",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -559.6654872866029,
			"y": -475.67393803200866,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 137,
			"height": 75,
			"seed": 1924285551,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159298,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "## 1. TwoSum\n\n",
			"rawText": "## 1. TwoSum\n\n",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "## 1. TwoSum\n\n",
			"lineHeight": 1.25,
			"baseline": 67
		},
		{
			"type": "text",
			"version": 347,
			"versionNonce": 1651704637,
			"isDeleted": false,
			"id": "EJQayqUG",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -391.1198087897546,
			"y": -103.07727531466043,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 44,
			"height": 25,
			"seed": 1616377135,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159298,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "nums",
			"rawText": "nums",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "nums",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 339,
			"versionNonce": 1956616979,
			"isDeleted": false,
			"id": "FiWL2YO1VzV_xeQZUHGcW",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -323.3367581776827,
			"y": -114.27259007375031,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 26,
			"height": 35,
			"seed": 325666703,
			"groupIds": [],
			"roundness": null,
			"boundElements": [
				{
					"type": "text",
					"id": "NGmD7BIz"
				}
			],
			"updated": 1686311159298,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 315,
			"versionNonce": 1527354269,
			"isDeleted": false,
			"id": "NGmD7BIz",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -317.3367581776827,
			"y": -109.27259007375031,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 14,
			"height": 25,
			"seed": 2029441889,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159298,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "2",
			"rawText": "2",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "FiWL2YO1VzV_xeQZUHGcW",
			"originalText": "2",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 391,
			"versionNonce": 1656799411,
			"isDeleted": false,
			"id": "zDHlMnqcHXMrV0u50XrF2",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -293.8872586636882,
			"y": -114.66843588433912,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 26,
			"height": 35,
			"seed": 1971712047,
			"groupIds": [],
			"roundness": null,
			"boundElements": [
				{
					"type": "text",
					"id": "kdrNEY7K"
				},
				{
					"id": "CnB5otnVuEgzDG631R5YZ",
					"type": "arrow"
				}
			],
			"updated": 1686311159298,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 359,
			"versionNonce": 925833213,
			"isDeleted": false,
			"id": "kdrNEY7K",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -286.3872586636882,
			"y": -109.66843588433912,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 11,
			"height": 25,
			"seed": 1517194305,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159298,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "7",
			"rawText": "7",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "zDHlMnqcHXMrV0u50XrF2",
			"originalText": "7",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 433,
			"versionNonce": 1760309843,
			"isDeleted": false,
			"id": "rkt3uCzL2oWP-p0x6MDZW",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -268.43820960932237,
			"y": -112.08415172272666,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 26,
			"height": 35,
			"seed": 502407855,
			"groupIds": [],
			"roundness": null,
			"boundElements": [
				{
					"type": "text",
					"id": "4H8SMuN4"
				},
				{
					"id": "BFTbNg_M66aA2y4hoE_uo",
					"type": "arrow"
				}
			],
			"updated": 1686311159298,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 406,
			"versionNonce": 283447389,
			"isDeleted": false,
			"id": "4H8SMuN4",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -260.43820960932237,
			"y": -107.08415172272666,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 10,
			"height": 25,
			"seed": 827794913,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159298,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "11",
			"rawText": "11",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "rkt3uCzL2oWP-p0x6MDZW",
			"originalText": "11",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 443,
			"versionNonce": 670593011,
			"isDeleted": false,
			"id": "FAOXESuV29GL_0CHR1u0i",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -236.78145364125982,
			"y": -113.48086825147325,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 30,
			"height": 35,
			"seed": 882437345,
			"groupIds": [],
			"roundness": null,
			"boundElements": [
				{
					"type": "text",
					"id": "WTqYGFSg"
				}
			],
			"updated": 1686311159298,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 544,
			"versionNonce": 1174207677,
			"isDeleted": false,
			"id": "WTqYGFSg",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -230.28145364125982,
			"y": -108.48086825147325,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 17,
			"height": 25,
			"seed": 916062415,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159298,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "15",
			"rawText": "15",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "FAOXESuV29GL_0CHR1u0i",
			"originalText": "15",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 348,
			"versionNonce": 1642854803,
			"isDeleted": false,
			"id": "uxewmC0E",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -399.0807124728254,
			"y": -30.35200978274642,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 65,
			"height": 25,
			"seed": 217392847,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159298,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "target",
			"rawText": "target",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "target",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 410,
			"versionNonce": 2115525917,
			"isDeleted": false,
			"id": "5QmiUL92ITl3Zz4BrG41N",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -321.7020339322637,
			"y": -35.49806572259976,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 26,
			"height": 35,
			"seed": 994610433,
			"groupIds": [],
			"roundness": null,
			"boundElements": [
				{
					"type": "text",
					"id": "HM9Et0i7"
				},
				{
					"id": "CnB5otnVuEgzDG631R5YZ",
					"type": "arrow"
				},
				{
					"id": "BFTbNg_M66aA2y4hoE_uo",
					"type": "arrow"
				}
			],
			"updated": 1686311159298,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 375,
			"versionNonce": 1409109811,
			"isDeleted": false,
			"id": "HM9Et0i7",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -314.7020339322637,
			"y": -30.498065722599762,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 12,
			"height": 25,
			"seed": 968744641,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159299,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "9",
			"rawText": "9",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "5QmiUL92ITl3Zz4BrG41N",
			"originalText": "9",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "arrow",
			"version": 1012,
			"versionNonce": 1890103677,
			"isDeleted": false,
			"id": "CnB5otnVuEgzDG631R5YZ",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -308.2518951552612,
			"y": -77.48328042542553,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 2.511507745943163,
			"height": 40.901881369492436,
			"seed": 452691183,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159299,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "zDHlMnqcHXMrV0u50XrF2",
				"gap": 14.529889397880822,
				"focus": 1.8583821215132086
			},
			"endBinding": {
				"elementId": "5QmiUL92ITl3Zz4BrG41N",
				"gap": 1.0833333333333357,
				"focus": -0.22753439483329485
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					-2.511507745943163,
					40.901881369492436
				]
			]
		},
		{
			"type": "arrow",
			"version": 1045,
			"versionNonce": 1351807187,
			"isDeleted": false,
			"id": "BFTbNg_M66aA2y4hoE_uo",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -283.09204473102034,
			"y": -76.79886657009571,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 15.346590229362391,
			"height": 36.65503954286624,
			"seed": 1266628655,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159299,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "rkt3uCzL2oWP-p0x6MDZW",
				"gap": 14.65661186605621,
				"focus": 0.9941323058245162
			},
			"endBinding": {
				"elementId": "5QmiUL92ITl3Zz4BrG41N",
				"gap": 4.645761304629708,
				"focus": 0.04877775537656524
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					-15.346590229362391,
					36.65503954286624
				]
			]
		},
		{
			"type": "text",
			"version": 105,
			"versionNonce": 1794079197,
			"isDeleted": false,
			"id": "CuJHrOKm",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -554.5396738556567,
			"y": -396.61323598885326,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 50,
			"height": 25,
			"seed": 434069263,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159299,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "INFO",
			"rawText": "INFO",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "INFO",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 210,
			"versionNonce": 423845491,
			"isDeleted": false,
			"id": "4bKTrt45",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -444.9856304112999,
			"y": -358.1043352305556,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 413,
			"height": 150,
			"seed": 517726095,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159299,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "- int[] nums: Array of integers\n- int target: integer\n- One solution\n- don't use same element twice\n\n> int[] twoSum (int[] nums, int target) < ",
			"rawText": "- int[] nums: Array of integers\n- int target: integer\n- One solution\n- don't use same element twice\n\n> int[] twoSum (int[] nums, int target) < ",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "- int[] nums: Array of integers\n- int target: integer\n- One solution\n- don't use same element twice\n\n> int[] twoSum (int[] nums, int target) < ",
			"lineHeight": 1.25,
			"baseline": 142
		},
		{
			"type": "text",
			"version": 154,
			"versionNonce": 368981565,
			"isDeleted": false,
			"id": "KtihYIHC",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -556.4790496334896,
			"y": -181.50516753104876,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 91,
			"height": 25,
			"seed": 456646927,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159299,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "EXAMPLE",
			"rawText": "EXAMPLE",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "EXAMPLE",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 209,
			"versionNonce": 2027231251,
			"isDeleted": false,
			"id": "xwmves8c",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -552.8953058104684,
			"y": 42.936096154295626,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 149,
			"height": 25,
			"seed": 1094953775,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159299,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "WALKTHROUGH",
			"rawText": "WALKTHROUGH",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "WALKTHROUGH",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "line",
			"version": 1074,
			"versionNonce": 2092328605,
			"isDeleted": false,
			"id": "dlS8imdeP0k3kycqSFfTH",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -179.47882849663927,
			"y": 297.460723252034,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 366.533661067454,
			"height": 4.981324613249598,
			"seed": 1319166241,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159299,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					366.533661067454,
					-4.981324613249598
				]
			]
		},
		{
			"type": "line",
			"version": 835,
			"versionNonce": 490642867,
			"isDeleted": false,
			"id": "txKxmfTfuBQOg7ATVZ3cy",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -395.0718674488796,
			"y": 320.95845572109965,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 8.735878069171008,
			"height": 359.0188239320661,
			"seed": 123772993,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159299,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					8.735878069171008,
					359.0188239320661
				]
			]
		},
		{
			"type": "line",
			"version": 1102,
			"versionNonce": 1372162813,
			"isDeleted": false,
			"id": "XQImxjhxOWmTOe5CMRHns",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -383.59694728786127,
			"y": 677.7256490541802,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 563.4640244467452,
			"height": 4.747235000088494,
			"seed": 1438969889,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159299,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					563.4640244467452,
					4.747235000088494
				]
			]
		},
		{
			"type": "line",
			"version": 1000,
			"versionNonce": 832991059,
			"isDeleted": false,
			"id": "9BmXa4NG8BjSJvAM4erAc",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 185.16316686484697,
			"y": 290.79340775983735,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 6.233647334111254,
			"height": 386.1240786597841,
			"seed": 383009793,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159299,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					-6.233647334111254,
					386.1240786597841
				]
			]
		},
		{
			"type": "line",
			"version": 914,
			"versionNonce": 1975067485,
			"isDeleted": false,
			"id": "DGQrYgaW43VoNaSOhaKSQ",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -84.35321054190473,
			"y": 355.7407828756984,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 211.33620489211296,
			"height": 7.012994939630687,
			"seed": 1210190849,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159299,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					211.33620489211296,
					-7.012994939630687
				]
			]
		},
		{
			"type": "line",
			"version": 666,
			"versionNonce": 946015475,
			"isDeleted": false,
			"id": "TFkFHAQnVG0OOWzN3lwvS",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -335.56214671204987,
			"y": 383.3103975387811,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 2.7531056589894547,
			"height": 257.8759285622688,
			"seed": 214484769,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159299,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					2.7531056589894547,
					257.8759285622688
				]
			]
		},
		{
			"type": "line",
			"version": 858,
			"versionNonce": 1020702653,
			"isDeleted": false,
			"id": "OgHWfvqjlDYvnNEcYM5wT",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -336.5954190630713,
			"y": 642.8946904363677,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 467.6825765854695,
			"height": 10.701254312094193,
			"seed": 222640897,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159299,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					467.6825765854695,
					-10.701254312094193
				]
			]
		},
		{
			"type": "line",
			"version": 767,
			"versionNonce": 620426899,
			"isDeleted": false,
			"id": "LCYkJH50xZJ-4c4sW35wN",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 127.36420014801283,
			"y": 350.8659523016722,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 3.948047192065758,
			"height": 280.2539947641877,
			"seed": 1372074721,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159299,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					3.948047192065758,
					280.2539947641877
				]
			]
		},
		{
			"type": "arrow",
			"version": 1420,
			"versionNonce": 1967370269,
			"isDeleted": false,
			"id": "6t8aj0MUHgWY9fKxB8VRh",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -177.22987819083946,
			"y": 467.29386447111244,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 82.44677534042441,
			"height": 80.64649089246268,
			"seed": 769551567,
			"groupIds": [],
			"roundness": null,
			"boundElements": [
				{
					"type": "text",
					"id": "5UZHxEyp"
				}
			],
			"updated": 1686311159300,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "JTZRIt2Y5cDlp-qvhpqCX",
				"focus": 0.3494710927465274,
				"gap": 3.6449508109811006
			},
			"endBinding": {
				"elementId": "Dfix6sAsR1VhBaBMTqXmh",
				"focus": -0.4183084931000283,
				"gap": 2.420947514159252
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					82.44677534042441,
					80.64649089246268
				]
			]
		},
		{
			"type": "text",
			"version": 539,
			"versionNonce": 908373043,
			"isDeleted": false,
			"id": "5UZHxEyp",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -201.789987839444,
			"y": 505.2989233431757,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 11,
			"height": 25,
			"seed": 204864239,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159300,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "t",
			"rawText": "t",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "6t8aj0MUHgWY9fKxB8VRh",
			"originalText": "t",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "arrow",
			"version": 1592,
			"versionNonce": 754033789,
			"isDeleted": false,
			"id": "cqUWUZEJVpqLiJUTBeqw1",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -197.02709558544174,
			"y": 468.91419777725423,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 1.507524729718341,
			"height": 256.25976958832166,
			"seed": 1891026191,
			"groupIds": [],
			"roundness": null,
			"boundElements": [
				{
					"type": "text",
					"id": "UFySeXJW"
				}
			],
			"updated": 1686311159300,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "JTZRIt2Y5cDlp-qvhpqCX",
				"focus": 0.35788178244374014,
				"gap": 5.265284117122889
			},
			"endBinding": {
				"elementId": "FwdlBuDUi3WJGjtlstv8g",
				"focus": -0.15572228809590177,
				"gap": 4.3562189968378675
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					1.507524729718341,
					256.25976958832166
				]
			]
		},
		{
			"type": "text",
			"version": 442,
			"versionNonce": 264678867,
			"isDeleted": false,
			"id": "UFySeXJW",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -189.22938856052195,
			"y": 518.0463315068437,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 10,
			"height": 25,
			"seed": 987319087,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159300,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "f",
			"rawText": "f",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "cqUWUZEJVpqLiJUTBeqw1",
			"originalText": "f",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 377,
			"versionNonce": 933367005,
			"isDeleted": false,
			"id": "GpTQ957t",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -122.2680231979117,
			"y": 557.9976332221947,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 213,
			"height": 25,
			"seed": 1022196225,
			"groupIds": [],
			"roundness": null,
			"boundElements": [
				{
					"id": "6t8aj0MUHgWY9fKxB8VRh",
					"type": "arrow"
				}
			],
			"updated": 1686311159300,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "return new int[] {i, j}",
			"rawText": "return new int[] {i, j}",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "return new int[] {i, j}",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 416,
			"versionNonce": 351763315,
			"isDeleted": false,
			"id": "dSX0TpvP",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -244.29385930028582,
			"y": 745.5302196543173,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 121,
			"height": 25,
			"seed": 1708245487,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159300,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "return NULL",
			"rawText": "return NULL",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "return NULL",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 435,
			"versionNonce": 1961257277,
			"isDeleted": false,
			"id": "PqXL3UQz1zymvXBMyO0J8",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -252.29390368949038,
			"y": 740.4392217849993,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 140.36365855823863,
			"height": 32.727272727272634,
			"seed": 1518163567,
			"groupIds": [],
			"roundness": null,
			"boundElements": [
				{
					"id": "cqUWUZEJVpqLiJUTBeqw1",
					"type": "arrow"
				}
			],
			"updated": 1686311159300,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 421,
			"versionNonce": 33395987,
			"isDeleted": false,
			"id": "FwdlBuDUi3WJGjtlstv8g",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -266.8393582349449,
			"y": 729.5301863624138,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 169.45445667613632,
			"height": 55.272716175426126,
			"seed": 317980015,
			"groupIds": [],
			"roundness": null,
			"boundElements": [
				{
					"id": "cqUWUZEJVpqLiJUTBeqw1",
					"type": "arrow"
				}
			],
			"updated": 1686311159300,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 381,
			"versionNonce": 1444952477,
			"isDeleted": false,
			"id": "Dfix6sAsR1VhBaBMTqXmh",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -127.72245767944577,
			"y": 550.3613028777344,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 226.90906871448863,
			"height": 42.181840376420496,
			"seed": 628040655,
			"groupIds": [],
			"roundness": null,
			"boundElements": [
				{
					"id": "6t8aj0MUHgWY9fKxB8VRh",
					"type": "arrow"
				}
			],
			"updated": 1686311159301,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 397,
			"versionNonce": 1179613875,
			"isDeleted": false,
			"id": "v5AP22sI9IQ3bDfhywC5x",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -142.31992686065513,
			"y": 542.2055157937247,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 256.72729492187506,
			"height": 61.09092018821025,
			"seed": 1421509761,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159301,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 447,
			"versionNonce": 612433405,
			"isDeleted": false,
			"id": "riUQ2AqO",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -401.34887256111153,
			"y": 286.50601292073395,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 208,
			"height": 25,
			"seed": 982089188,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159301,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "loop the nums (i = 0)",
			"rawText": "loop the nums (i = 0)",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "loop the nums (i = 0)",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 522,
			"versionNonce": 512994387,
			"isDeleted": false,
			"id": "fHq7OIetBX62YCq5O0n4S",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -420.2060328568705,
			"y": 280.22028555605766,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 236.0001046316964,
			"height": 33.14285278320312,
			"seed": 981544036,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159301,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 409,
			"versionNonce": 118109789,
			"isDeleted": false,
			"id": "jb8P1ZSP",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -344.7773044807545,
			"y": 352.22025503847954,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 239,
			"height": 25,
			"seed": 316465252,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159301,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "loop the nums (j = i + 1)",
			"rawText": "loop the nums (j = i + 1)",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "loop the nums (j = i + 1)",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 448,
			"versionNonce": 1856023027,
			"isDeleted": false,
			"id": "5CYchF1Py6XLSce_09y1J",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -364.20584103209376,
			"y": 341.3631034620287,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 278.28569684709817,
			"height": 47.42858886718749,
			"seed": 299829852,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159301,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 470,
			"versionNonce": 1217225405,
			"isDeleted": false,
			"id": "MoAtt0Bz",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -293.63463916267415,
			"y": 431.64887878289926,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 305,
			"height": 25,
			"seed": 171347676,
			"groupIds": [],
			"roundness": null,
			"boundElements": [
				{
					"id": "6t8aj0MUHgWY9fKxB8VRh",
					"type": "arrow"
				},
				{
					"id": "cqUWUZEJVpqLiJUTBeqw1",
					"type": "arrow"
				}
			],
			"updated": 1686311159301,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "if target == nums[i] + nums[j]",
			"rawText": "if target == nums[i] + nums[j]",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "if target == nums[i] + nums[j]",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 385,
			"versionNonce": 1534915475,
			"isDeleted": false,
			"id": "JTZRIt2Y5cDlp-qvhpqCX",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -301.3488725611116,
			"y": 419.07751124662684,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 324.5714460100446,
			"height": 44.57140241350447,
			"seed": 211537500,
			"groupIds": [],
			"roundness": null,
			"boundElements": [
				{
					"id": "6t8aj0MUHgWY9fKxB8VRh",
					"type": "arrow"
				},
				{
					"id": "cqUWUZEJVpqLiJUTBeqw1",
					"type": "arrow"
				}
			],
			"updated": 1686311159301,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 238,
			"versionNonce": 1571554077,
			"isDeleted": false,
			"id": "SiIIpeqI",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -547.9862898618289,
			"y": 220.61059825391885,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 138,
			"height": 25,
			"seed": 231449188,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159301,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "BRUTEFORCE",
			"rawText": "BRUTEFORCE",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "BRUTEFORCE",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 247,
			"versionNonce": 626985267,
			"isDeleted": false,
			"id": "m0e83AsJ",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -401.90933626732806,
			"y": 103.61066985285231,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 495,
			"height": 75,
			"seed": 727554916,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159301,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "- loop nums\n    - loop nums (start one after the i )\n        - if both nums are == target return them",
			"rawText": "- loop nums\n    - loop nums (start one after the i )\n        - if both nums are == target return them",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "- loop nums\n    - loop nums (start one after the i )\n        - if both nums are == target return them",
			"lineHeight": 1.25,
			"baseline": 67
		},
		{
			"type": "text",
			"version": 150,
			"versionNonce": 718772093,
			"isDeleted": false,
			"id": "XL5Rzdin",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -504.0344336295474,
			"y": 829.9166964026304,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 165,
			"height": 25,
			"seed": 1077618788,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159301,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "OPTIMIZATION",
			"rawText": "OPTIMIZATION",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "OPTIMIZATION",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 116,
			"versionNonce": 1101884115,
			"isDeleted": false,
			"id": "96FkyxdY",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 242.3578252346349,
			"y": 426.32431198041184,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 64,
			"height": 25,
			"seed": 1353488484,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159302,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "O(n^2)",
			"rawText": "O(n^2)",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "O(n^2)",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 112,
			"versionNonce": 173121501,
			"isDeleted": false,
			"id": "ul926vVY",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -412.8421259372401,
			"y": 889.1243608085368,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 235,
			"height": 25,
			"seed": 54661340,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159302,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "I could use a hash map",
			"rawText": "I could use a hash map",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "I could use a hash map",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 149,
			"versionNonce": 889100403,
			"isDeleted": false,
			"id": "7H3OK7CO",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -394.68835490358606,
			"y": 998.1705268617218,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 91,
			"height": 25,
			"seed": 2092580708,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159302,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "loop nums",
			"rawText": "loop nums",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "loop nums",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 232,
			"versionNonce": 304847933,
			"isDeleted": false,
			"id": "8oKLcmYMx75VGs4D-hrfZ",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -404.19473379683086,
			"y": 989.6363591089819,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 111.38465294471149,
			"height": 35.076904296875,
			"seed": 1852297052,
			"groupIds": [],
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1686311159302,
			"link": null,
			"locked": false
		},
		{
			"type": "line",
			"version": 244,
			"versionNonce": 756617747,
			"isDeleted": false,
			"id": "IuNDU5yD09qmydcycbKDB",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -285.8346011588175,
			"y": 1009.5353318154847,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 461.74270293910104,
			"height": 3.1066484909061955,
			"seed": 1946864612,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159302,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					461.74270293910104,
					-3.1066484909061955
				]
			]
		},
		{
			"type": "line",
			"version": 260,
			"versionNonce": 440863901,
			"isDeleted": false,
			"id": "kMpnfB5MAthWBqcf5mDGs",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -381.17956675629483,
			"y": 1024.3343204861023,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 3.0967718232328707,
			"height": 387.43642352472057,
			"seed": 1998020580,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159302,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					3.0967718232328707,
					387.43642352472057
				]
			]
		},
		{
			"type": "text",
			"version": 208,
			"versionNonce": 1525897139,
			"isDeleted": false,
			"id": "nVmcb4mY",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -350.8284882054311,
			"y": 1061.396006961061,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 245,
			"height": 25,
			"seed": 1699247972,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159302,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "if current nums < target",
			"rawText": "if current nums < target",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "if current nums < target",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 264,
			"versionNonce": 39153917,
			"isDeleted": false,
			"id": "pK2PggBh-u4FBUcRijrGl",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -351.555046959417,
			"y": 1045.5980630535976,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 260.9230393629807,
			"height": 46.76922137920678,
			"seed": 1220959588,
			"groupIds": [],
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"id": "-xJwKt573SZ2Uv0MaJgUI",
					"type": "arrow"
				},
				{
					"id": "dtACra8UrPNTnwTlTLRz6",
					"type": "arrow"
				}
			],
			"updated": 1686311159302,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 437,
			"versionNonce": 213117267,
			"isDeleted": false,
			"id": "2y7BvpjY",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -225.85668032296985,
			"y": 1148.3418598836988,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 238,
			"height": 25,
			"seed": 1918569060,
			"groupIds": [],
			"roundness": null,
			"boundElements": [
				{
					"id": "dtACra8UrPNTnwTlTLRz6",
					"type": "arrow"
				}
			],
			"updated": 1686311159302,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "temp = target - nums[i]",
			"rawText": "temp = target - nums[i]",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "temp = target - nums[i]",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "arrow",
			"version": 242,
			"versionNonce": 936921437,
			"isDeleted": false,
			"id": "-xJwKt573SZ2Uv0MaJgUI",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -272.55120737978507,
			"y": 1093.972759137751,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 13.371686670385714,
			"height": 365.478161627123,
			"seed": 961112292,
			"groupIds": [],
			"roundness": null,
			"boundElements": [
				{
					"type": "text",
					"id": "TYh0V5nE"
				}
			],
			"updated": 1686311159302,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "pK2PggBh-u4FBUcRijrGl",
				"focus": 0.39881423822309403,
				"gap": 1.6054747049466869
			},
			"endBinding": {
				"elementId": "vAR2Lxc9Aytd4NLKmB_nu",
				"focus": -0.2708361124227557,
				"gap": 7.342903003375
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					13.371686670385714,
					365.478161627123
				]
			]
		},
		{
			"type": "text",
			"version": 93,
			"versionNonce": 129058547,
			"isDeleted": false,
			"id": "TYh0V5nE",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -260.22791154584513,
			"y": 1270.5837689945529,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 11,
			"height": 25,
			"seed": 1475606372,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159302,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "F",
			"rawText": "F",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "-xJwKt573SZ2Uv0MaJgUI",
			"originalText": "F",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 157,
			"versionNonce": 2082543037,
			"isDeleted": false,
			"id": "878P6nha",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -300.45958656920845,
			"y": 1473.4645953014178,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 121,
			"height": 25,
			"seed": 827673564,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1686311159302,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "return NULL",
			"rawText": "return NULL",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "return NULL",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 149,
			"versionNonce": 577892499,
			"isDeleted": false,
			"id": "v9tkPj0Yql7GmhemJLLHS",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -308.61362052353536,
			"y": 1472.233938750937,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 148.30772986778845,
			"height": 27.692307692307622,
			"seed": 954874468,
			"groupIds": [],
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1686311159302,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 180,
			"versionNonce": 1783715357,
			"isDeleted": false,
			"id": "vAR2Lxc9Aytd4NLKmB_nu",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -322.31449850760094,
			"y": 1466.793823768249,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 176.6153658353365,
			"height": 42.46150090144215,
			"seed": 610779356,
			"groupIds": [],
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"id": "scb1boLLkfHTdVRKN9sxV",
					"type": "arrow"
				},
				{
					"id": "-xJwKt573SZ2Uv0MaJgUI",
					"type": "arrow"
				}
			],
			"updated": 1686311159302,
			"link": null,
			"locked": false
		},
		{
			"type": "arrow",
			"version": 620,
			"versionNonce": 514614835,
			"isDeleted": false,
			"id": "dtACra8UrPNTnwTlTLRz6",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -240.0080427718694,
			"y": 1100.732079996543,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 64.81510075118817,
			"height": 43.282446169043396,
			"seed": 1141327708,
			"groupIds": [],
			"roundness": null,
			"boundElements": [
				{
					"type": "text",
					"id": "slumvpno"
				}
			],
			"updated": 1686311159302,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "pK2PggBh-u4FBUcRijrGl",
				"focus": 0.40273462289337625,
				"gap": 8.364795563738767
			},
			"endBinding": {
				"elementId": "2y7BvpjY",
				"focus": -0.31322897663026605,
				"gap": 4.327333718112413
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					64.81510075118817,
					43.282446169043396
				]
			]
		},
		{
			"type": "text",
			"version": 91,
			"versionNonce": 1029343869,
			"isDeleted": false,
			"id": "slumvpno",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -159.88939364767964,
			"y": 1123.4970064323716,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 16,
			"height": 25,
			"seed": 659142500,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159303,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "T",
			"rawText": "T",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "dtACra8UrPNTnwTlTLRz6",
			"originalText": "T",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 326,
			"versionNonce": 1128736723,
			"isDeleted": false,
			"id": "Bi68HoJB",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 222.54760446597334,
			"y": 958.7656576264268,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 180,
			"height": 75,
			"seed": 1145456740,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159303,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Hash Table \n(key is number, \nvalue is the index)",
			"rawText": "Hash Table \n(key is number, \nvalue is the index)",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Hash Table \n(key is number, \nvalue is the index)",
			"lineHeight": 1.25,
			"baseline": 67
		},
		{
			"type": "rectangle",
			"version": 278,
			"versionNonce": 1442722525,
			"isDeleted": false,
			"id": "IRVSZ2qmNZabne7yEPSfC",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 253.28937813733648,
			"y": 1066.2413082121468,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 38,
			"height": 49,
			"seed": 1602777188,
			"groupIds": [],
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "jy3f26ZR"
				},
				{
					"id": "sppZD67UEWgvTdiblcFGx",
					"type": "arrow"
				}
			],
			"updated": 1686311159303,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 173,
			"versionNonce": 911783283,
			"isDeleted": false,
			"id": "jy3f26ZR",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 265.2893781373365,
			"y": 1078.2413082121468,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 14,
			"height": 25,
			"seed": 980416100,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159303,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "2",
			"rawText": "2",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "IRVSZ2qmNZabne7yEPSfC",
			"originalText": "2",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 270,
			"versionNonce": 13487933,
			"isDeleted": false,
			"id": "6_CpFmJ-6n3IoKWhWlYXC",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 253.33235111187253,
			"y": 1116.9652904112725,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 41.70561372948623,
			"height": 44.86518251434086,
			"seed": 1618757092,
			"groupIds": [],
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1686311159303,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 292,
			"versionNonce": 388468499,
			"isDeleted": false,
			"id": "jjyoht0DF1C2WeXzwaLch",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 253.96419737420229,
			"y": 1166.2538306560436,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 46.76096235361991,
			"height": 41.70571015040173,
			"seed": 695692900,
			"groupIds": [],
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1686311159303,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 320,
			"versionNonce": 2083184541,
			"isDeleted": false,
			"id": "uypJAkn3c3R2uWFBiSQs_",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 256.4918716862694,
			"y": 1208.5913870687752,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 42.33745999181576,
			"height": 48.024654878279044,
			"seed": 1116507236,
			"groupIds": [],
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1686311159303,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 390,
			"versionNonce": 1479161011,
			"isDeleted": false,
			"id": "lKkt4Gor",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2.422308106485218,
			"y": 818.0056439573889,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 44,
			"height": 25,
			"seed": 661829724,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159303,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "nums",
			"rawText": "nums",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "nums",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 382,
			"versionNonce": 1044833277,
			"isDeleted": false,
			"id": "NOJVZojRpvyLmofwSomJM",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 70.20535871855708,
			"y": 806.810329198299,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 26,
			"height": 35,
			"seed": 28527836,
			"groupIds": [],
			"roundness": null,
			"boundElements": [
				{
					"type": "text",
					"id": "YXqfO2u9"
				}
			],
			"updated": 1686311159303,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 358,
			"versionNonce": 1493640787,
			"isDeleted": false,
			"id": "YXqfO2u9",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 76.20535871855708,
			"y": 811.810329198299,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 14,
			"height": 25,
			"seed": 1609388380,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159303,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "2",
			"rawText": "2",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "NOJVZojRpvyLmofwSomJM",
			"originalText": "2",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 437,
			"versionNonce": 2065914973,
			"isDeleted": false,
			"id": "hOTa5S22WBDTFqGNgO_EB",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 99.65485823255159,
			"y": 806.4144833877101,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 26,
			"height": 35,
			"seed": 1634911708,
			"groupIds": [],
			"roundness": null,
			"boundElements": [
				{
					"type": "text",
					"id": "tbAje1NO"
				}
			],
			"updated": 1686311159303,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 402,
			"versionNonce": 1083499507,
			"isDeleted": false,
			"id": "tbAje1NO",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 107.15485823255159,
			"y": 811.4144833877101,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 11,
			"height": 25,
			"seed": 1800776284,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159303,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "7",
			"rawText": "7",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "hOTa5S22WBDTFqGNgO_EB",
			"originalText": "7",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 476,
			"versionNonce": 1787939005,
			"isDeleted": false,
			"id": "TIH1Pre1OWqzbGBvFoRNe",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 125.10390728691743,
			"y": 808.9987675493226,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 26,
			"height": 35,
			"seed": 1885863644,
			"groupIds": [],
			"roundness": null,
			"boundElements": [
				{
					"type": "text",
					"id": "ZiV4kI59"
				}
			],
			"updated": 1686311159303,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 449,
			"versionNonce": 383380883,
			"isDeleted": false,
			"id": "ZiV4kI59",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 133.10390728691743,
			"y": 813.9987675493226,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 10,
			"height": 25,
			"seed": 960217948,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159303,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "11",
			"rawText": "11",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "TIH1Pre1OWqzbGBvFoRNe",
			"originalText": "11",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 486,
			"versionNonce": 1312008477,
			"isDeleted": false,
			"id": "dXPRAC-lcS2kuLQ3zgdME",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 156.76066325498,
			"y": 807.602051020576,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 30,
			"height": 35,
			"seed": 740489180,
			"groupIds": [],
			"roundness": null,
			"boundElements": [
				{
					"type": "text",
					"id": "yFpW2N2s"
				}
			],
			"updated": 1686311159303,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 587,
			"versionNonce": 520930099,
			"isDeleted": false,
			"id": "yFpW2N2s",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 163.26066325498,
			"y": 812.602051020576,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 17,
			"height": 25,
			"seed": 355441756,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159303,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "15",
			"rawText": "15",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "dXPRAC-lcS2kuLQ3zgdME",
			"originalText": "15",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 391,
			"versionNonce": 930774397,
			"isDeleted": false,
			"id": "hBZ6nfIL",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -5.538595576585578,
			"y": 890.7309094893027,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 65,
			"height": 25,
			"seed": 1848881372,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159304,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "target",
			"rawText": "target",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "target",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 456,
			"versionNonce": 1905517779,
			"isDeleted": false,
			"id": "JuCM8rOGYXGZPjgsr6scv",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 71.8400829639761,
			"y": 885.5848535494493,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 26,
			"height": 35,
			"seed": 650196316,
			"groupIds": [],
			"roundness": null,
			"boundElements": [
				{
					"type": "text",
					"id": "UXkpt7rV"
				}
			],
			"updated": 1686311159304,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 418,
			"versionNonce": 229098973,
			"isDeleted": false,
			"id": "UXkpt7rV",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 78.8400829639761,
			"y": 890.5848535494493,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 12,
			"height": 25,
			"seed": 1814702556,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159304,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "9",
			"rawText": "9",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "JuCM8rOGYXGZPjgsr6scv",
			"originalText": "9",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 289,
			"versionNonce": 1443222131,
			"isDeleted": false,
			"id": "mc5mqui5",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -218.31108503565747,
			"y": 1200.2124787709379,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 192,
			"height": 25,
			"seed": 406100060,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159304,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "if temp is in Hash  ",
			"rawText": "if temp is in Hash  ",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "if temp is in Hash  ",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 297,
			"versionNonce": 1405944381,
			"isDeleted": false,
			"id": "eMHWvECDTrZ9FSBc8DYsK",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -226.83298806807858,
			"y": 1190.5089870045424,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 200.35401683399994,
			"height": 42.93371188716312,
			"seed": 783194844,
			"groupIds": [],
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"id": "Ljj_2ckprSDwpFCmBBzPr",
					"type": "arrow"
				},
				{
					"id": "scb1boLLkfHTdVRKN9sxV",
					"type": "arrow"
				}
			],
			"updated": 1686311159304,
			"link": null,
			"locked": false
		},
		{
			"type": "arrow",
			"version": 917,
			"versionNonce": 1562971155,
			"isDeleted": false,
			"id": "Ljj_2ckprSDwpFCmBBzPr",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -144.20015430959842,
			"y": 1246.4613058120192,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 98.2938199460512,
			"height": 67.57184021647413,
			"seed": 1009591772,
			"groupIds": [],
			"roundness": null,
			"boundElements": [
				{
					"type": "text",
					"id": "RDR4NTGb"
				}
			],
			"updated": 1686311159304,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "eMHWvECDTrZ9FSBc8DYsK",
				"gap": 13.018606920313625,
				"focus": 0.5169351683436475
			},
			"endBinding": {
				"elementId": "W0fYSikoJVYpEvcY4nqQ5",
				"gap": 8.264791195805438,
				"focus": 0.019738788419738734
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					98.2938199460512,
					67.57184021647413
				]
			]
		},
		{
			"type": "text",
			"version": 152,
			"versionNonce": 785101469,
			"isDeleted": false,
			"id": "RDR4NTGb",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -15.246109557767113,
			"y": 1341.9237259226666,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 16,
			"height": 25,
			"seed": 1069812316,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159304,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "T",
			"rawText": "T",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "Ljj_2ckprSDwpFCmBBzPr",
			"originalText": "T",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 466,
			"versionNonce": 989073843,
			"isDeleted": false,
			"id": "hBSxODRt",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -100.73112382196629,
			"y": 1321.0870802039237,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 223,
			"height": 50,
			"seed": 1139605732,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159304,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "return temp index \nand current nums index",
			"rawText": "return temp index \nand current nums index",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "return temp index \nand current nums index",
			"lineHeight": 1.25,
			"baseline": 42
		},
		{
			"type": "rectangle",
			"version": 473,
			"versionNonce": 727013117,
			"isDeleted": false,
			"id": "W0fYSikoJVYpEvcY4nqQ5",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -128.58332980757356,
			"y": 1322.2979372242987,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 262.77999469601934,
			"height": 55.09902965578616,
			"seed": 1478894692,
			"groupIds": [],
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"id": "Ljj_2ckprSDwpFCmBBzPr",
					"type": "arrow"
				}
			],
			"updated": 1686311159304,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 515,
			"versionNonce": 1619878739,
			"isDeleted": false,
			"id": "nqHVvZELRRaXthEwK_XG_",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -144.32594930473428,
			"y": 1315.0321945701828,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 286.999444841466,
			"height": 69.63056115877679,
			"seed": 66265564,
			"groupIds": [],
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1686311159304,
			"link": null,
			"locked": false
		},
		{
			"type": "arrow",
			"version": 468,
			"versionNonce": 1139502941,
			"isDeleted": false,
			"id": "scb1boLLkfHTdVRKN9sxV",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -198.00736313498498,
			"y": 1240.0511541318435,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 25.266996844704977,
			"height": 225.00585892588083,
			"seed": 2124364764,
			"groupIds": [],
			"roundness": null,
			"boundElements": [
				{
					"type": "text",
					"id": "Qm2SjL3F"
				}
			],
			"updated": 1686311159304,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "eMHWvECDTrZ9FSBc8DYsK",
				"focus": 0.6648948290580529,
				"gap": 6.608455240138028
			},
			"endBinding": {
				"elementId": "vAR2Lxc9Aytd4NLKmB_nu",
				"focus": 0.08990138264333106,
				"gap": 1.7368107105245372
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					-25.266996844704977,
					225.00585892588083
				]
			]
		},
		{
			"type": "text",
			"version": 163,
			"versionNonce": 1447788787,
			"isDeleted": false,
			"id": "Qm2SjL3F",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -221.80171967946387,
			"y": 1305.844185330824,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 11,
			"height": 25,
			"seed": 1468227676,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159304,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "F",
			"rawText": "F",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "scb1boLLkfHTdVRKN9sxV",
			"originalText": "F",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "arrow",
			"version": 855,
			"versionNonce": 652180413,
			"isDeleted": false,
			"id": "sppZD67UEWgvTdiblcFGx",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 305.43636512784025,
			"y": 1086.4378735113175,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 45.01416984635853,
			"height": 3.814865257069414,
			"seed": 462310108,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1686311159304,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "IRVSZ2qmNZabne7yEPSfC",
				"gap": 14.146986990503763,
				"focus": -0.27240599512453634
			},
			"endBinding": {
				"elementId": "9SVlOQDu_CfefLuBnZXhs",
				"gap": 2.3726969208560718,
				"focus": -0.32684790034440436
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					45.01416984635853,
					3.814865257069414
				]
			]
		},
		{
			"type": "rectangle",
			"version": 320,
			"versionNonce": 1437919891,
			"isDeleted": false,
			"id": "9SVlOQDu_CfefLuBnZXhs",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 352.82323189505485,
			"y": 1068.9454328565919,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 60,
			"height": 35,
			"seed": 1588637404,
			"groupIds": [],
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "TUHynmNq"
				},
				{
					"id": "sppZD67UEWgvTdiblcFGx",
					"type": "arrow"
				}
			],
			"updated": 1686311159304,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 244,
			"versionNonce": 1012071453,
			"isDeleted": false,
			"id": "TUHynmNq",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 375.82323189505485,
			"y": 1073.9454328565919,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 14,
			"height": 25,
			"seed": 1700343260,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159304,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "0",
			"rawText": "0",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "9SVlOQDu_CfefLuBnZXhs",
			"originalText": "0",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "line",
			"version": 202,
			"versionNonce": 595599411,
			"isDeleted": false,
			"id": "GJpmioqMK6gZCHbVe9y-w",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 177.79167515024972,
			"y": 1008.6572127097395,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 0,
			"height": 412.94010055281956,
			"seed": 193354852,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1686311159304,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					0,
					412.94010055281956
				]
			]
		},
		{
			"type": "line",
			"version": 156,
			"versionNonce": 1815572605,
			"isDeleted": false,
			"id": "N-gFzPTkcTdpHHFqGd-Rn",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -379.2535532361107,
			"y": 1424.624686787291,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 560.6780766160391,
			"height": 1.8164703095981167,
			"seed": 1491299036,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1686311159304,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					560.6780766160391,
					-1.8164703095981167
				]
			]
		},
		{
			"type": "text",
			"version": 224,
			"versionNonce": 697541075,
			"isDeleted": false,
			"id": "TDki9nQu",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 114.80044499782196,
			"y": 1523.6988404208091,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 59,
			"height": 25,
			"seed": 391623780,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159305,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "O (n) ",
			"rawText": "O (n) ",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "O (n) ",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "freedraw",
			"version": 249,
			"versionNonce": 609114333,
			"isDeleted": false,
			"id": "HnETVQPpmXOiXvxZTL3uj",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 135.99247542377736,
			"y": 1484.9479049671302,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 112.61995813135783,
			"height": 93.8500113042237,
			"seed": 1667421532,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159305,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-10.293300957883957,
					-4.238415324142807
				],
				[
					-13.32072067737505,
					-4.238415324142807
				],
				[
					-18.164518316946555,
					-3.6328944244373815
				],
				[
					-27.852298375125145,
					0.6054747049465732
				],
				[
					-36.329036633893054,
					10.293208568366254
				],
				[
					-45.41129579236633,
					25.43030716582166
				],
				[
					-57.5209746703307,
					55.70450436073247
				],
				[
					-55.70459675025029,
					67.81418323869684
				],
				[
					-53.28260554094675,
					72.05259856283965
				],
				[
					-38.75102784319665,
					82.95128183615225
				],
				[
					-33.90713781410733,
					86.58417626058986
				],
				[
					-19.98098862654473,
					89.61159598008089
				],
				[
					1.8163779200804129,
					86.58417626058986
				],
				[
					15.137098597455463,
					80.52933682160756
				],
				[
					27.852205985607327,
					73.86902267767891
				],
				[
					38.145414553973495,
					64.7867635192058
				],
				[
					47.83319461215214,
					47.83324080691091
				],
				[
					55.09898346102713,
					27.85225218036635
				],
				[
					55.09898346102713,
					18.16451831694667
				],
				[
					50.86061433164318,
					9.68773386341968
				],
				[
					44.80577489266099,
					4.843843834330528
				],
				[
					34.51256632429488,
					3.632894424437609
				],
				[
					19.98089623702697,
					4.843843834330528
				],
				[
					3.6328482296786433,
					9.082259158473335
				],
				[
					-10.898729468071508,
					14.53162389250906
				],
				[
					-26.641348965232282,
					19.980942431785934
				],
				[
					-31.48523899432155,
					23.00836215127697
				],
				[
					-34.51265871381264,
					27.246777475419776
				],
				[
					-32.0906675045091,
					48.43871551185748
				],
				[
					-32.0906675045091,
					48.43871551185748
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.1923828125,
				0.2587890625,
				0.29296875,
				0.33203125,
				0.3916015625,
				0.4326171875,
				0.4541015625,
				0.48046875,
				0.482421875,
				0.482421875,
				0.4794921875,
				0.4765625,
				0.4697265625,
				0.4697265625,
				0.48046875,
				0.484375,
				0.4931640625,
				0.4990234375,
				0.5068359375,
				0.5107421875,
				0.5126953125,
				0.5126953125,
				0.5126953125,
				0.5166015625,
				0.5146484375,
				0.5126953125,
				0.5263671875,
				0.5283203125,
				0.505859375,
				0.0146484375,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 147,
			"versionNonce": 1359343475,
			"isDeleted": false,
			"id": "UqqEP7fCYm26ENnYdmO4U",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 211.75210815838625,
			"y": 1502.2103282618496,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 88.01566384197258,
			"height": 45.8039734697918,
			"seed": 1027736796,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159305,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.8980365138916113,
					0
				],
				[
					-2.6943836257627254,
					2.694383625762839
				],
				[
					-4.490593695589951,
					8.083013835244401
				],
				[
					-8.083013835244401,
					26.045388617604658
				],
				[
					-5.388630209481562,
					28.739772243367497
				],
				[
					0,
					28.739772243367497
				],
				[
					12.573744572878354,
					23.35114203388548
				],
				[
					33.23036593895722,
					12.573607530834579
				],
				[
					49.39653065148991,
					0
				],
				[
					66.46086891995822,
					-8.981187391179901
				],
				[
					79.93265000672818,
					-17.064201226424302
				],
				[
					79.93265000672818,
					-17.064201226424302
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.333984375,
				0.37890625,
				0.4150390625,
				0.4482421875,
				0.4951171875,
				0.5078125,
				0.5185546875,
				0.521484375,
				0.53515625,
				0.529296875,
				0.486328125,
				0.0166015625,
				0
			]
		},
		{
			"type": "text",
			"version": 201,
			"versionNonce": 506017085,
			"isDeleted": false,
			"id": "v4OfmmPE",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -285.3397859619897,
			"y": -474.94622474661014,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 189,
			"height": 25,
			"seed": 629827804,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159305,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "IMPLEMENTATION",
			"rawText": "IMPLEMENTATION",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "IMPLEMENTATION",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 263,
			"versionNonce": 471697683,
			"isDeleted": false,
			"id": "4DszYKaL",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -301.96972547402777,
			"y": -428.6887445871282,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 366,
			"height": 25,
			"seed": 1529320804,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159305,
			"link": "[[LeetCode/Questions#Solution 1]]",
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "📍[[LeetCode/Questions#Solution 1]]",
			"rawText": "[[LeetCode/Questions#Solution 1]]",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "📍[[LeetCode/Questions#Solution 1]]",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "line",
			"version": 245,
			"versionNonce": 1697219997,
			"isDeleted": false,
			"id": "DH_WuPOl-JKlWhLwQVF0h",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 437.9410657702914,
			"y": 1551.1974648262046,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 0,
			"height": 2090.6667073567705,
			"seed": 2029670492,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1686311159305,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					0,
					-2090.6667073567705
				]
			]
		},
		{
			"type": "text",
			"version": 126,
			"versionNonce": 5303987,
			"isDeleted": false,
			"id": "CjwqNKbu",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 475.9731760753506,
			"y": -510.4535700587774,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 243,
			"height": 50,
			"seed": 1132479324,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159305,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "## 2. Add Two Numbers\n",
			"rawText": "## 2. Add Two Numbers\n",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "## 2. Add Two Numbers\n",
			"lineHeight": 1.25,
			"baseline": 42
		},
		{
			"type": "text",
			"version": 87,
			"versionNonce": 478202365,
			"isDeleted": false,
			"id": "k7qRZbC9",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 479.8122001072645,
			"y": -417.6088748577599,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 50,
			"height": 25,
			"seed": 752181604,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159305,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "INFO",
			"rawText": "INFO",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "INFO",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 250,
			"versionNonce": 4628563,
			"isDeleted": false,
			"id": "YiC895uq",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 647.4789278090873,
			"y": -379.27554152442656,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 607,
			"height": 125,
			"seed": 2050461540,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159305,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "- given two reversed non-negative integers made into Link List\n    -  ex. 234 => 4-> 3-> 2\n- return the sum of these numbers in reverse\n- no leading zeros\n    - ex. 034",
			"rawText": "- given two reversed non-negative integers made into Link List\n    -  ex. 234 => 4-> 3-> 2\n- return the sum of these numbers in reverse\n- no leading zeros\n    - ex. 034",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "- given two reversed non-negative integers made into Link List\n    -  ex. 234 => 4-> 3-> 2\n- return the sum of these numbers in reverse\n- no leading zeros\n    - ex. 034",
			"lineHeight": 1.25,
			"baseline": 117
		},
		{
			"type": "text",
			"version": 93,
			"versionNonce": 87065181,
			"isDeleted": false,
			"id": "SnaKSG0t",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 482.47892780908796,
			"y": -233.27553135190055,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 91,
			"height": 25,
			"seed": 1934118364,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159305,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "EXAMPLE",
			"rawText": "EXAMPLE",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "EXAMPLE",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 80,
			"versionNonce": 97852915,
			"isDeleted": false,
			"id": "3mh7wTWn",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 651.1456148208067,
			"y": -168.608885030286,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 314,
			"height": 75,
			"seed": 53993316,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159305,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Input: l1 = [2,4,3], l2 = [5,6,4]\nOutput: [7,0,8]\nExplanation: 342 + 465 = 807.",
			"rawText": "Input: l1 = [2,4,3], l2 = [5,6,4]\nOutput: [7,0,8]\nExplanation: 342 + 465 = 807.",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Input: l1 = [2,4,3], l2 = [5,6,4]\nOutput: [7,0,8]\nExplanation: 342 + 465 = 807.",
			"lineHeight": 1.25,
			"baseline": 67
		},
		{
			"type": "text",
			"version": 137,
			"versionNonce": 1141518013,
			"isDeleted": false,
			"id": "oDIhD1vm",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 496.11084142599555,
			"y": 44.5610362131203,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 149,
			"height": 25,
			"seed": 610995556,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159305,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "WALKTHROUGH",
			"rawText": "WALKTHROUGH",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "WALKTHROUGH",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 1445,
			"versionNonce": 2080565139,
			"isDeleted": false,
			"id": "UqLjPF1c",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 531.0371979710019,
			"y": 92.43413590659083,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 549,
			"height": 392.29178922024084,
			"seed": 681778618,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159305,
			"link": null,
			"locked": false,
			"fontSize": 22.41667366972805,
			"fontFamily": 1,
			"text": "- traverse both l1 and l2 (while either is not null)\n    - sum = add the number\n    - if carry\n        - sum =+ 1\n        - carry = false\n    - if sum > 9 (has carry)\n        - sum -= 10\n        - carry = true\n    - soliution.val = sum\n    - iterrate l1 and l2\n    - if either value is not null, make a link\n    - if no next link but carry\n        - add node with carry at the end\n- return solutionRoot ",
			"rawText": "- traverse both l1 and l2 (while either is not null)\n    - sum = add the number\n    - if carry\n        - sum =+ 1\n        - carry = false\n    - if sum > 9 (has carry)\n        - sum -= 10\n        - carry = true\n    - soliution.val = sum\n    - iterrate l1 and l2\n    - if either value is not null, make a link\n    - if no next link but carry\n        - add node with carry at the end\n- return solutionRoot ",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "- traverse both l1 and l2 (while either is not null)\n    - sum = add the number\n    - if carry\n        - sum =+ 1\n        - carry = false\n    - if sum > 9 (has carry)\n        - sum -= 10\n        - carry = true\n    - soliution.val = sum\n    - iterrate l1 and l2\n    - if either value is not null, make a link\n    - if no next link but carry\n        - add node with carry at the end\n- return solutionRoot ",
			"lineHeight": 1.25,
			"baseline": 384
		},
		{
			"type": "ellipse",
			"version": 616,
			"versionNonce": 1739542301,
			"isDeleted": false,
			"id": "exilHY7MVp5lul_mthCmu",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1069.5113051877756,
			"y": -221.03114056806646,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 46,
			"height": 49,
			"seed": 1954994802,
			"groupIds": [
				"9hX1u_x2ljBZy_eVTNM85",
				"0kGMhlqkWxAculZoYF0Dc"
			],
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "bQ9Kjc4G"
				},
				{
					"id": "0b4tR5q7vjmysYkD2HHcQ",
					"type": "arrow"
				}
			],
			"updated": 1686311159305,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 458,
			"versionNonce": 688291123,
			"isDeleted": false,
			"id": "bQ9Kjc4G",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1085.747849220485,
			"y": -208.85525670713687,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 14,
			"height": 25,
			"seed": 1307528622,
			"groupIds": [
				"9hX1u_x2ljBZy_eVTNM85",
				"0kGMhlqkWxAculZoYF0Dc"
			],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159305,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "2",
			"rawText": "2",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "exilHY7MVp5lul_mthCmu",
			"originalText": "2",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "ellipse",
			"version": 554,
			"versionNonce": 781280125,
			"isDeleted": false,
			"id": "qD1dnyM8cY5Fi9I6jbduK",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1167.7450225029113,
			"y": -226.35588166317126,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 46,
			"height": 49,
			"seed": 266420722,
			"groupIds": [
				"9hX1u_x2ljBZy_eVTNM85",
				"0kGMhlqkWxAculZoYF0Dc"
			],
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "LrJzMGg3"
				},
				{
					"id": "0b4tR5q7vjmysYkD2HHcQ",
					"type": "arrow"
				},
				{
					"id": "krEjcblc8Oo_g-wRpnRTJ",
					"type": "arrow"
				}
			],
			"updated": 1686311159305,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 444,
			"versionNonce": 1212571347,
			"isDeleted": false,
			"id": "LrJzMGg3",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1184.4815665356207,
			"y": -214.17999780224167,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 13,
			"height": 25,
			"seed": 6240370,
			"groupIds": [
				"9hX1u_x2ljBZy_eVTNM85",
				"0kGMhlqkWxAculZoYF0Dc"
			],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159306,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "4",
			"rawText": "4",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "qD1dnyM8cY5Fi9I6jbduK",
			"originalText": "4",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "ellipse",
			"version": 506,
			"versionNonce": 217181149,
			"isDeleted": false,
			"id": "IJJojCOaSu6BXOfooL_LH",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1267.4388307481072,
			"y": -218.65468502313746,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 47,
			"height": 49,
			"seed": 1311385202,
			"groupIds": [
				"9hX1u_x2ljBZy_eVTNM85",
				"0kGMhlqkWxAculZoYF0Dc"
			],
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "BY3tMLOh"
				}
			],
			"updated": 1686311159306,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 418,
			"versionNonce": 1683557491,
			"isDeleted": false,
			"id": "BY3tMLOh",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1283.8218213902232,
			"y": -206.47880116220787,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 14,
			"height": 25,
			"seed": 1126797358,
			"groupIds": [
				"9hX1u_x2ljBZy_eVTNM85",
				"0kGMhlqkWxAculZoYF0Dc"
			],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159306,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "3",
			"rawText": "3",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "IJJojCOaSu6BXOfooL_LH",
			"originalText": "3",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "arrow",
			"version": 1321,
			"versionNonce": 1927440445,
			"isDeleted": false,
			"id": "0b4tR5q7vjmysYkD2HHcQ",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1117.840065323369,
			"y": -199.36028900055095,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 45.46624147751163,
			"height": 1.3730368957216967,
			"seed": 876922990,
			"groupIds": [
				"9hX1u_x2ljBZy_eVTNM85",
				"0kGMhlqkWxAculZoYF0Dc"
			],
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1686311159306,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "exilHY7MVp5lul_mthCmu",
				"gap": 2.4692869157360597,
				"focus": -0.1466371121836409
			},
			"endBinding": {
				"elementId": "qD1dnyM8cY5Fi9I6jbduK",
				"gap": 4.68303500486099,
				"focus": -0.19164758936026255
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					45.46624147751163,
					1.3730368957216967
				]
			]
		},
		{
			"type": "arrow",
			"version": 797,
			"versionNonce": 1896154643,
			"isDeleted": false,
			"id": "krEjcblc8Oo_g-wRpnRTJ",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1215.2527012324904,
			"y": -200.62267839588787,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 54.54898531140566,
			"height": 4.545757033411434,
			"seed": 2062249646,
			"groupIds": [
				"9hX1u_x2ljBZy_eVTNM85",
				"0kGMhlqkWxAculZoYF0Dc"
			],
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1686311159306,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "qD1dnyM8cY5Fi9I6jbduK",
				"gap": 1.5352178855322194,
				"focus": -0.032924178754431405
			},
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					54.54898531140566,
					4.545757033411434
				]
			]
		},
		{
			"type": "ellipse",
			"version": 731,
			"versionNonce": 1380210845,
			"isDeleted": false,
			"id": "4ktnhSsKOpNCwK4cOKRVh",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1079.313281166852,
			"y": -124.4961707344041,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 47,
			"height": 49,
			"seed": 1131699566,
			"groupIds": [
				"rfh2hC-4_wjn4UI5_wHT5",
				"0kGMhlqkWxAculZoYF0Dc"
			],
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "q7xmGnTH"
				}
			],
			"updated": 1686311159306,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 676,
			"versionNonce": 625003443,
			"isDeleted": false,
			"id": "q7xmGnTH",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1096.696271808968,
			"y": -112.32028687347452,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 12,
			"height": 25,
			"seed": 338239858,
			"groupIds": [
				"rfh2hC-4_wjn4UI5_wHT5",
				"0kGMhlqkWxAculZoYF0Dc"
			],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159306,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "5",
			"rawText": "5",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "4ktnhSsKOpNCwK4cOKRVh",
			"originalText": "5",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "ellipse",
			"version": 663,
			"versionNonce": 1690909949,
			"isDeleted": false,
			"id": "Y1xH8USbSnljmuMKGFIcC",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1166.0331881676393,
			"y": -129.69133462951416,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 45,
			"height": 49,
			"seed": 1643053106,
			"groupIds": [
				"rfh2hC-4_wjn4UI5_wHT5",
				"0kGMhlqkWxAculZoYF0Dc"
			],
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "y3MQq29Y"
				},
				{
					"id": "Zf8jKqqcGJBrzgJsSwvVm",
					"type": "arrow"
				}
			],
			"updated": 1686311159306,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 636,
			"versionNonce": 355654995,
			"isDeleted": false,
			"id": "y3MQq29Y",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1182.123285590942,
			"y": -117.51545076858457,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 13,
			"height": 25,
			"seed": 582260146,
			"groupIds": [
				"rfh2hC-4_wjn4UI5_wHT5",
				"0kGMhlqkWxAculZoYF0Dc"
			],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159306,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "6",
			"rawText": "6",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "Y1xH8USbSnljmuMKGFIcC",
			"originalText": "6",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "ellipse",
			"version": 733,
			"versionNonce": 837981533,
			"isDeleted": false,
			"id": "y1g7qtk355waWdqEx29nd",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1258.0137714415205,
			"y": -130.54025624906862,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 51,
			"height": 49,
			"seed": 1776940334,
			"groupIds": [
				"rfh2hC-4_wjn4UI5_wHT5",
				"0kGMhlqkWxAculZoYF0Dc"
			],
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "RqHOIK5i"
				}
			],
			"updated": 1686311159306,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 687,
			"versionNonce": 204585715,
			"isDeleted": false,
			"id": "RqHOIK5i",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1276.9825485212634,
			"y": -118.36437238813903,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 13,
			"height": 25,
			"seed": 1935575150,
			"groupIds": [
				"rfh2hC-4_wjn4UI5_wHT5",
				"0kGMhlqkWxAculZoYF0Dc"
			],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159306,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "4",
			"rawText": "4",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "y1g7qtk355waWdqEx29nd",
			"originalText": "4",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "arrow",
			"version": 617,
			"versionNonce": 1427235261,
			"isDeleted": false,
			"id": "4BpZhqcvHudFxTghtgYue",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1124.567986625965,
			"y": -108.91077813858337,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 48.70447572382659,
			"height": 1.2987662014001558,
			"seed": 2030321266,
			"groupIds": [
				"rfh2hC-4_wjn4UI5_wHT5",
				"0kGMhlqkWxAculZoYF0Dc"
			],
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1686311159306,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					48.70447572382659,
					-1.2987662014001558
				]
			]
		},
		{
			"type": "arrow",
			"version": 1251,
			"versionNonce": 650372243,
			"isDeleted": false,
			"id": "Zf8jKqqcGJBrzgJsSwvVm",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1213.5525712847007,
			"y": -102.38023734687991,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 48.68661447986928,
			"height": 4.5822924000937455,
			"seed": 753478770,
			"groupIds": [
				"rfh2hC-4_wjn4UI5_wHT5",
				"0kGMhlqkWxAculZoYF0Dc"
			],
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1686311159306,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "Y1xH8USbSnljmuMKGFIcC",
				"gap": 2.65453483841355,
				"focus": 0.21006876647029296
			},
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					48.68661447986928,
					-4.5822924000937455
				]
			]
		},
		{
			"type": "ellipse",
			"version": 602,
			"versionNonce": 55091741,
			"isDeleted": false,
			"id": "NEjY1Xn_YKnNmMlzzZv5o",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1074.4934139098473,
			"y": -33.463227722622804,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 57,
			"height": 49,
			"seed": 1539496238,
			"groupIds": [
				"Ajld6Asjms0H9O_g9IwNA",
				"0kGMhlqkWxAculZoYF0Dc"
			],
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "RzKJ3NZ7"
				},
				{
					"id": "-y-piyUZ_HAiYpXFSxj5t",
					"type": "arrow"
				}
			],
			"updated": 1686311159306,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 560,
			"versionNonce": 748673587,
			"isDeleted": false,
			"id": "RzKJ3NZ7",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1097.3408706460307,
			"y": -21.28734386169322,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 11,
			"height": 25,
			"seed": 1976927150,
			"groupIds": [
				"Ajld6Asjms0H9O_g9IwNA",
				"0kGMhlqkWxAculZoYF0Dc"
			],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159306,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "7",
			"rawText": "7",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "NEjY1Xn_YKnNmMlzzZv5o",
			"originalText": "7",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "ellipse",
			"version": 619,
			"versionNonce": 1367889533,
			"isDeleted": false,
			"id": "vxvUoabl2P81si07C7P1B",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1165.9861865354621,
			"y": -38.781824597105555,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 58,
			"height": 50,
			"seed": 1564053678,
			"groupIds": [
				"Ajld6Asjms0H9O_g9IwNA",
				"0kGMhlqkWxAculZoYF0Dc"
			],
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "W1G5e9CW"
				}
			],
			"updated": 1686311159306,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 597,
			"versionNonce": 715922387,
			"isDeleted": false,
			"id": "W1G5e9CW",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1187.9800898810522,
			"y": -26.459494126769243,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 14,
			"height": 25,
			"seed": 776435438,
			"groupIds": [
				"Ajld6Asjms0H9O_g9IwNA",
				"0kGMhlqkWxAculZoYF0Dc"
			],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159306,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "0",
			"rawText": "0",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "vxvUoabl2P81si07C7P1B",
			"originalText": "0",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "ellipse",
			"version": 606,
			"versionNonce": 982679261,
			"isDeleted": false,
			"id": "H-a6zWexNz3TrcXhni8xB",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1266.7915852215801,
			"y": -38.23609334745046,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 50,
			"height": 49,
			"seed": 1705974126,
			"groupIds": [
				"Ajld6Asjms0H9O_g9IwNA",
				"0kGMhlqkWxAculZoYF0Dc"
			],
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "ebTfCNkg"
				}
			],
			"updated": 1686311159306,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 585,
			"versionNonce": 1291790707,
			"isDeleted": false,
			"id": "ebTfCNkg",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1284.1139156919164,
			"y": -26.06020948652088,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 15,
			"height": 25,
			"seed": 1306406386,
			"groupIds": [
				"Ajld6Asjms0H9O_g9IwNA",
				"0kGMhlqkWxAculZoYF0Dc"
			],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159307,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "8",
			"rawText": "8",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "H-a6zWexNz3TrcXhni8xB",
			"originalText": "8",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "arrow",
			"version": 1091,
			"versionNonce": 1694014269,
			"isDeleted": false,
			"id": "-y-piyUZ_HAiYpXFSxj5t",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1132.5148903037893,
			"y": -17.826890964724853,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 35.722710220804856,
			"height": 3.897062575745977,
			"seed": 16711858,
			"groupIds": [
				"Ajld6Asjms0H9O_g9IwNA",
				"0kGMhlqkWxAculZoYF0Dc"
			],
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1686311159307,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "NEjY1Xn_YKnNmMlzzZv5o",
				"gap": 2.722846203825558,
				"focus": -0.22849828739977
			},
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					35.722710220804856,
					-3.897062575745977
				]
			]
		},
		{
			"type": "arrow",
			"version": 556,
			"versionNonce": 2027914003,
			"isDeleted": false,
			"id": "Z62sIMhULBsARu8kHIw_b",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1217.5915088938755,
			"y": -13.931207697805718,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 57.795938223137,
			"height": 1.2987662014001558,
			"seed": 1720661678,
			"groupIds": [
				"Ajld6Asjms0H9O_g9IwNA",
				"0kGMhlqkWxAculZoYF0Dc"
			],
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1686311159307,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					57.795938223137,
					1.2987662014001558
				]
			]
		},
		{
			"type": "freedraw",
			"version": 311,
			"versionNonce": 689712029,
			"isDeleted": false,
			"id": "JYbW3pt0BdHclVRA8koSN",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1084.7816031428877,
			"y": -155.34362884245132,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 15.104210435800269,
			"height": 1.4384753274795798,
			"seed": 886065082,
			"groupIds": [
				"0kGMhlqkWxAculZoYF0Dc"
			],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159307,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.7192376637397047,
					0
				],
				[
					-1.4384753274794093,
					-0.7192376637397615
				],
				[
					-0.7192376637397047,
					0
				],
				[
					0.719237663739932,
					0
				],
				[
					2.1577678655357886,
					0.7192376637398183
				],
				[
					4.31548085675513,
					0.7192376637398183
				],
				[
					5.7540110585509865,
					0.7192376637398183
				],
				[
					7.192486386030396,
					0.7192376637398183
				],
				[
					8.631016587826252,
					0.7192376637398183
				],
				[
					10.069491915305662,
					0
				],
				[
					10.788729579045594,
					0
				],
				[
					11.507967242785298,
					0
				],
				[
					12.946497444581155,
					0
				],
				[
					13.66573510832086,
					0.7192376637398183
				],
				[
					0,
					0
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.138671875,
				0.158203125,
				0.1728515625,
				0.2724609375,
				0.265625,
				0.2724609375,
				0.2763671875,
				0.2763671875,
				0.283203125,
				0.296875,
				0.2998046875,
				0.2998046875,
				0.3017578125,
				0.3037109375,
				0.2880859375,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 309,
			"versionNonce": 650356915,
			"isDeleted": false,
			"id": "7I1mkONXzL9x8zNGMjYRx",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1092.693327192658,
			"y": -163.25535289222137,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 1.4385302017956292,
			"height": 16.542685763279906,
			"seed": 341812858,
			"groupIds": [
				"0kGMhlqkWxAculZoYF0Dc"
			],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159307,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.7192925380559245,
					2.1577129912193413
				],
				[
					0.7192925380559245,
					4.315480856754903
				],
				[
					0.7192925380559245,
					5.034718520494664
				],
				[
					0.7192925380559245,
					7.192486386030282
				],
				[
					0.7192925380559245,
					8.630961713509862
				],
				[
					0.7192925380559245,
					10.069491915305662
				],
				[
					0.7192925380559245,
					11.507967242785185
				],
				[
					0.7192925380559245,
					12.946442570264765
				],
				[
					0.7192925380559245,
					14.384972772060564
				],
				[
					0.7192925380559245,
					15.104210435800383
				],
				[
					0.7192925380559245,
					15.823448099540144
				],
				[
					0.7192925380559245,
					16.542685763279906
				],
				[
					1.4385302017956292,
					16.542685763279906
				],
				[
					1.4385302017956292,
					16.542685763279906
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.181640625,
				0.2470703125,
				0.2802734375,
				0.29296875,
				0.3349609375,
				0.3583984375,
				0.3671875,
				0.376953125,
				0.3818359375,
				0.3837890625,
				0.3837890625,
				0.3837890625,
				0.314453125,
				0.0283203125,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 311,
			"versionNonce": 1462677501,
			"isDeleted": false,
			"id": "uWYz5vgAez8sEmtMk54vG",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1177.5646884975417,
			"y": -163.25535289222137,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 17.981215965075762,
			"height": 2.8770055292753796,
			"seed": 1147518778,
			"groupIds": [
				"0kGMhlqkWxAculZoYF0Dc"
			],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159307,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.7192376637397047,
					0.7192376637397615
				],
				[
					0,
					0.7192376637397615
				],
				[
					1.4384753274796367,
					0.7192376637397615
				],
				[
					2.8770055292754932,
					1.438475327479523
				],
				[
					5.034718520494835,
					1.438475327479523
				],
				[
					7.9117240497701005,
					0.7192376637397615
				],
				[
					9.350254251565957,
					0.7192376637397615
				],
				[
					10.788729579045366,
					0.7192376637397615
				],
				[
					12.227204906525003,
					0.7192376637397615
				],
				[
					15.104210435800496,
					0.7192376637397615
				],
				[
					15.823448099540201,
					0
				],
				[
					16.542740637596353,
					0.7192376637397615
				],
				[
					17.261978301336057,
					0.7192376637397615
				],
				[
					17.261978301336057,
					1.438475327479523
				],
				[
					17.261978301336057,
					2.1577129912193413
				],
				[
					17.261978301336057,
					2.8770055292753796
				],
				[
					17.261978301336057,
					2.8770055292753796
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.1533203125,
				0.2353515625,
				0.3056640625,
				0.3427734375,
				0.37890625,
				0.3955078125,
				0.4111328125,
				0.4130859375,
				0.4130859375,
				0.4130859375,
				0.4130859375,
				0.4130859375,
				0.4130859375,
				0.4130859375,
				0.3828125,
				0.2763671875,
				0.13671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 311,
			"versionNonce": 2085755475,
			"isDeleted": false,
			"id": "OO1tmDxqkL176mlWKmGld",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1188.353418076587,
			"y": -169.7286016145119,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 2.8770055292754932,
			"height": 19.419691292555285,
			"seed": 1879754406,
			"groupIds": [
				"0kGMhlqkWxAculZoYF0Dc"
			],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159307,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					0.7192376637397615
				],
				[
					-0.7192376637397047,
					0.7192376637397615
				],
				[
					-0.7192376637397047,
					1.438475327479523
				],
				[
					-0.7192376637397047,
					2.8770055292753796
				],
				[
					-0.7192376637397047,
					5.754011058550759
				],
				[
					-0.7192376637397047,
					7.911724049770044
				],
				[
					-0.7192376637397047,
					10.069491915305662
				],
				[
					0,
					12.227204906525003
				],
				[
					0,
					13.665735108320803
				],
				[
					0,
					15.823448099540144
				],
				[
					0.719237663739932,
					16.542740637596182
				],
				[
					0.719237663739932,
					17.261978301335944
				],
				[
					0.719237663739932,
					17.981215965075705
				],
				[
					0.719237663739932,
					18.700453628815524
				],
				[
					0.719237663739932,
					19.419691292555285
				],
				[
					2.1577678655357886,
					18.700453628815524
				],
				[
					2.1577678655357886,
					18.700453628815524
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.1552734375,
				0.2509765625,
				0.33203125,
				0.35546875,
				0.3671875,
				0.3984375,
				0.4208984375,
				0.43359375,
				0.4384765625,
				0.44140625,
				0.453125,
				0.45703125,
				0.45703125,
				0.4482421875,
				0.400390625,
				0.3837890625,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 304,
			"versionNonce": 1026664541,
			"isDeleted": false,
			"id": "k80UYxhW6bttIREVupGWG",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1261.716812138686,
			"y": -151.74738564943618,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 25.17370235110593,
			"height": 0.7192376637397615,
			"seed": 1847876986,
			"groupIds": [
				"0kGMhlqkWxAculZoYF0Dc"
			],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159307,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.7191827894234848,
					0
				],
				[
					4.315425982438683,
					0
				],
				[
					10.788729579045366,
					0
				],
				[
					15.823448099540201,
					-0.7192376637397615
				],
				[
					19.4196912925554,
					-0.7192376637397615
				],
				[
					22.296641947514217,
					-0.7192376637397615
				],
				[
					24.454409813050006,
					-0.7192376637397615
				],
				[
					24.454409813050006,
					0
				],
				[
					25.17370235110593,
					0
				],
				[
					25.17370235110593,
					0
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.1865234375,
				0.3466796875,
				0.3671875,
				0.392578125,
				0.39453125,
				0.3974609375,
				0.3994140625,
				0.3994140625,
				0.3994140625,
				0.328125,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 308,
			"versionNonce": 643913715,
			"isDeleted": false,
			"id": "_dLI0lfkxxZEiXspOynQe",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1278.2595527762821,
			"y": -161.09763990100203,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 3.596243193015198,
			"height": 23.735227023626464,
			"seed": 1671592442,
			"groupIds": [
				"0kGMhlqkWxAculZoYF0Dc"
			],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159307,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.7192925380559245,
					0.7192925380560382
				],
				[
					-0.7192925380559245,
					2.157767865535561
				],
				[
					-0.7192925380559245,
					2.8770055292753227
				],
				[
					0,
					5.034773394810941
				],
				[
					0.7191827894234848,
					7.192486386030282
				],
				[
					1.4384753274794093,
					8.631016587826082
				],
				[
					2.157658116902894,
					10.788729579045423
				],
				[
					2.157658116902894,
					14.384972772060564
				],
				[
					2.157658116902894,
					17.261978301335944
				],
				[
					2.157658116902894,
					17.981215965075705
				],
				[
					2.157658116902894,
					18.700508503131744
				],
				[
					2.157658116902894,
					21.577459158090846
				],
				[
					2.8769506549592734,
					23.735227023626464
				],
				[
					2.8769506549592734,
					23.735227023626464
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.189453125,
				0.275390625,
				0.37890625,
				0.3935546875,
				0.4443359375,
				0.4638671875,
				0.4677734375,
				0.4697265625,
				0.4697265625,
				0.4697265625,
				0.4697265625,
				0.45703125,
				0.275390625,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 388,
			"versionNonce": 1828099261,
			"isDeleted": false,
			"id": "5swRSC-RLEuFI0p7kCGEP",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1206.334579167347,
			"y": -258.19620611241095,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 15.823448099539974,
			"height": 18.700453628815467,
			"seed": 946692090,
			"groupIds": [
				"iBiC3j3T-vAH101jNuO21",
				"0kGMhlqkWxAculZoYF0Dc"
			],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159307,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.7192925380559245,
					-1.4385027646376898
				],
				[
					1.4384753274794093,
					-2.1577404283774513
				],
				[
					0.7192925380559245,
					-2.1577404283774513
				],
				[
					-1.4384753274796367,
					-1.4385027646376898
				],
				[
					-3.596243193015198,
					0
				],
				[
					-5.034718520494835,
					0.7192651008979283
				],
				[
					-8.630961713510032,
					2.1577404283774513
				],
				[
					-10.06943704098967,
					3.596243193015141
				],
				[
					-11.508022117101518,
					5.034745957652831
				],
				[
					-12.227204906525003,
					7.192486386030282
				],
				[
					-11.508022117101518,
					9.350226814407733
				],
				[
					-11.508022117101518,
					10.069491915305662
				],
				[
					-10.06943704098967,
					11.507994679943351
				],
				[
					-9.350254251566184,
					11.507994679943351
				],
				[
					-7.911778924086548,
					12.946470007422874
				],
				[
					-5.7540110585509865,
					14.384972772060564
				],
				[
					-5.034718520494835,
					14.384972772060564
				],
				[
					-2.8769506549592734,
					15.104237872958493
				],
				[
					-1.4384753274796367,
					15.823475536698254
				],
				[
					0.7192925380559245,
					15.823475536698254
				],
				[
					1.4384753274794093,
					15.823475536698254
				],
				[
					2.157767865535334,
					15.104237872958493
				],
				[
					2.8769506549588186,
					15.104237872958493
				],
				[
					2.8769506549588186,
					15.823475536698254
				],
				[
					3.5962431930149705,
					16.542713200438016
				],
				[
					3.5962431930149705,
					16.542713200438016
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.1640625,
				0.1943359375,
				0.2197265625,
				0.271484375,
				0.2783203125,
				0.283203125,
				0.291015625,
				0.32421875,
				0.3408203125,
				0.359375,
				0.369140625,
				0.3837890625,
				0.390625,
				0.3974609375,
				0.3994140625,
				0.396484375,
				0.3974609375,
				0.3974609375,
				0.3974609375,
				0.3974609375,
				0.41015625,
				0.4140625,
				0.4140625,
				0.4033203125,
				0.2822265625,
				0.142578125,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 400,
			"versionNonce": 1928847763,
			"isDeleted": false,
			"id": "tEWOUY-xl-rbWpUZVMyN-",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1217.1233087463922,
			"y": -258.9154437761507,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 17.262033175652277,
			"height": 13.665735108320803,
			"seed": 143131258,
			"groupIds": [
				"iBiC3j3T-vAH101jNuO21",
				"0kGMhlqkWxAculZoYF0Dc"
			],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159307,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-1.4384753274794093,
					-0.7192651008979283
				],
				[
					-1.4384753274794093,
					0
				],
				[
					-2.157767865535334,
					0.7192376637397615
				],
				[
					-3.5962431930149705,
					2.1577404283774513
				],
				[
					-4.315535731071122,
					4.315480856754903
				],
				[
					-4.315535731071122,
					7.192486386030282
				],
				[
					-4.315535731071122,
					9.350226814407733
				],
				[
					-4.315535731071122,
					10.069464478147495
				],
				[
					-3.5962431930149705,
					10.788729579045423
				],
				[
					-3.5962431930149705,
					11.507967242785185
				],
				[
					-2.8769506549588186,
					11.507967242785185
				],
				[
					-2.157767865535334,
					11.507967242785185
				],
				[
					-1.4384753274794093,
					12.227232343683113
				],
				[
					-0.7192925380559245,
					11.507967242785185
				],
				[
					0,
					11.507967242785185
				],
				[
					1.4384753274796367,
					11.507967242785185
				],
				[
					2.1577678655357886,
					10.788729579045423
				],
				[
					2.8769506549592734,
					9.350226814407733
				],
				[
					2.8769506549592734,
					7.192486386030282
				],
				[
					2.8769506549592734,
					5.753983621392592
				],
				[
					2.8769506549592734,
					5.034745957652831
				],
				[
					2.8769506549592734,
					3.596243193015141
				],
				[
					2.1577678655357886,
					2.1577404283774513
				],
				[
					2.8769506549592734,
					2.876978092117213
				],
				[
					2.8769506549592734,
					4.315480856754903
				],
				[
					3.596243193015198,
					6.473221285132354
				],
				[
					3.596243193015198,
					7.192486386030282
				],
				[
					4.31553573107135,
					7.911724049770044
				],
				[
					5.034718520494835,
					8.630989150667972
				],
				[
					6.473193847974471,
					10.069464478147495
				],
				[
					7.192486386030396,
					10.788729579045423
				],
				[
					8.630961713509805,
					10.788729579045423
				],
				[
					9.350254251566184,
					11.507967242785185
				],
				[
					10.06943704098967,
					11.507967242785185
				],
				[
					10.788729579045594,
					12.227232343683113
				],
				[
					11.508022117101518,
					12.227232343683113
				],
				[
					12.946497444581155,
					12.946470007422874
				],
				[
					12.946497444581155,
					12.946470007422874
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.130859375,
				0.18359375,
				0.236328125,
				0.2490234375,
				0.271484375,
				0.294921875,
				0.318359375,
				0.3330078125,
				0.337890625,
				0.33984375,
				0.3505859375,
				0.357421875,
				0.3623046875,
				0.3623046875,
				0.3623046875,
				0.3623046875,
				0.3662109375,
				0.3662109375,
				0.3662109375,
				0.3681640625,
				0.3701171875,
				0.373046875,
				0.373046875,
				0.373046875,
				0.3681640625,
				0.373046875,
				0.39453125,
				0.3984375,
				0.3984375,
				0.4033203125,
				0.408203125,
				0.412109375,
				0.4150390625,
				0.4150390625,
				0.4150390625,
				0.4111328125,
				0.396484375,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 386,
			"versionNonce": 1109325085,
			"isDeleted": false,
			"id": "m7bvV-JKA2KRfCC4JLkml",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1237.2622925770036,
			"y": -263.2309520700638,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 9.350254251566184,
			"height": 14.384972772060564,
			"seed": 543605114,
			"groupIds": [
				"iBiC3j3T-vAH101jNuO21",
				"0kGMhlqkWxAculZoYF0Dc"
			],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159307,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					1.4385027646376898
				],
				[
					0,
					3.596243193015141
				],
				[
					0,
					6.473248722290521
				],
				[
					0.7191827894234848,
					7.91175148692821
				],
				[
					0.7191827894234848,
					11.507994679943351
				],
				[
					1.438475327479864,
					12.227232343683113
				],
				[
					1.438475327479864,
					12.946497444581041
				],
				[
					1.438475327479864,
					13.665735108320803
				],
				[
					2.1577678655357886,
					14.384972772060564
				],
				[
					2.8769506549592734,
					14.384972772060564
				],
				[
					2.8769506549592734,
					12.946497444581041
				],
				[
					3.596243193015198,
					10.788729579045423
				],
				[
					3.596243193015198,
					8.630989150667972
				],
				[
					3.596243193015198,
					6.473248722290521
				],
				[
					3.596243193015198,
					4.315508293913069
				],
				[
					4.315425982438683,
					2.157767865535618
				],
				[
					5.034718520494835,
					0.7192651008979283
				],
				[
					5.7540110585509865,
					0
				],
				[
					6.473193847974471,
					0
				],
				[
					7.192486386030396,
					0
				],
				[
					7.911669175453881,
					0.7192651008979283
				],
				[
					9.350254251566184,
					0
				],
				[
					0,
					0
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.1630859375,
				0.2060546875,
				0.2197265625,
				0.2373046875,
				0.2451171875,
				0.2724609375,
				0.28125,
				0.28125,
				0.298828125,
				0.3095703125,
				0.3603515625,
				0.3701171875,
				0.3720703125,
				0.3720703125,
				0.3720703125,
				0.3720703125,
				0.369140625,
				0.369140625,
				0.359375,
				0.3466796875,
				0.34375,
				0.3134765625,
				0.0126953125,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 384,
			"versionNonce": 726415155,
			"isDeleted": false,
			"id": "6Bi6RTSTRq6NKF-_lsI5T",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1250.9279728110082,
			"y": -265.38869249844123,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 15.823448099540201,
			"height": 17.261950864177777,
			"seed": 963132218,
			"groupIds": [
				"iBiC3j3T-vAH101jNuO21",
				"0kGMhlqkWxAculZoYF0Dc"
			],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159307,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					5.034745957652831
				],
				[
					0,
					8.630989150667972
				],
				[
					0,
					10.788729579045423
				],
				[
					-0.7191827894234848,
					12.946470007422874
				],
				[
					0,
					13.665735108320803
				],
				[
					0,
					14.384972772060564
				],
				[
					0.7192925380561519,
					14.384972772060564
				],
				[
					1.4384753274796367,
					12.946470007422874
				],
				[
					1.4384753274796367,
					12.227232343683113
				],
				[
					2.157767865535561,
					10.069491915305662
				],
				[
					2.877060403591713,
					7.192486386030282
				],
				[
					2.877060403591713,
					3.596243193015141
				],
				[
					3.596243193015198,
					1.4385027646376898
				],
				[
					5.034718520494835,
					0
				],
				[
					6.473303596606684,
					-1.4385027646376898
				],
				[
					9.350254251565957,
					-2.1577404283774513
				],
				[
					10.788729579045366,
					-2.876978092117213
				],
				[
					12.227204906525003,
					-2.1577404283774513
				],
				[
					12.946497444581155,
					-2.1577404283774513
				],
				[
					13.66578998263708,
					-2.1577404283774513
				],
				[
					15.104265310116716,
					-2.1577404283774513
				],
				[
					15.104265310116716,
					-2.1577404283774513
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.138671875,
				0.201171875,
				0.2353515625,
				0.244140625,
				0.2744140625,
				0.2998046875,
				0.3193359375,
				0.3310546875,
				0.3681640625,
				0.373046875,
				0.373046875,
				0.3828125,
				0.3828125,
				0.3828125,
				0.3828125,
				0.3759765625,
				0.3740234375,
				0.3701171875,
				0.3671875,
				0.369140625,
				0.3212890625,
				0.0322265625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 373,
			"versionNonce": 672942461,
			"isDeleted": false,
			"id": "wBUUqaxDQOqLcqjHgKAed",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1271.7862491796757,
			"y": -268.26567059055844,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 4.31553573107135,
			"height": 10.788729579045423,
			"seed": 895382586,
			"groupIds": [
				"iBiC3j3T-vAH101jNuO21",
				"0kGMhlqkWxAculZoYF0Dc"
			],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159307,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					0.7192376637397615
				],
				[
					-0.7192925380561519,
					2.1577404283774513
				],
				[
					-0.7192925380561519,
					4.315480856754903
				],
				[
					-0.7192925380561519,
					7.192486386030282
				],
				[
					-1.4385850761123038,
					9.350226814407733
				],
				[
					-0.7192925380561519,
					10.788729579045423
				],
				[
					0,
					10.788729579045423
				],
				[
					2.157658116902894,
					9.350226814407733
				],
				[
					2.876950654959046,
					7.911724049770044
				],
				[
					0,
					0
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.1630859375,
				0.2626953125,
				0.2841796875,
				0.310546875,
				0.328125,
				0.33984375,
				0.3427734375,
				0.21484375,
				0.0595703125,
				0.0126953125,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 372,
			"versionNonce": 767875283,
			"isDeleted": false,
			"id": "AAb2Sn83EekvMn6jfiS2Z",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1278.2594430276497,
			"y": -266.8271952630789,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 12.227204906524776,
			"height": 27.331470216641605,
			"seed": 872710118,
			"groupIds": [
				"iBiC3j3T-vAH101jNuO21",
				"0kGMhlqkWxAculZoYF0Dc"
			],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159307,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-2.157767865535334,
					2.8770055292753796
				],
				[
					-2.8769506549588186,
					4.315508293913069
				],
				[
					-4.315535731071122,
					7.192486386030282
				],
				[
					-5.754011058550532,
					10.069491915305662
				],
				[
					-6.4731938479740165,
					12.946497444581041
				],
				[
					-7.192486386030168,
					14.384972772060564
				],
				[
					-7.91177892408632,
					17.981215965075705
				],
				[
					-9.35025425156573,
					21.577459158090846
				],
				[
					-12.227204906524776,
					27.331470216641605
				],
				[
					-12.227204906524776,
					27.331470216641605
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2060546875,
				0.267578125,
				0.3017578125,
				0.380859375,
				0.423828125,
				0.42578125,
				0.42578125,
				0.4052734375,
				0.3017578125,
				0.013671875,
				0
			]
		},
		{
			"type": "text",
			"version": 179,
			"versionNonce": 540021213,
			"isDeleted": false,
			"id": "4pQSL374",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 511.4006114802078,
			"y": 537.3445202128366,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 138,
			"height": 25,
			"seed": 1148148090,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159307,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "BRUTEFORCE",
			"rawText": "BRUTEFORCE",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "BRUTEFORCE",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 342,
			"versionNonce": 1207453299,
			"isDeleted": false,
			"id": "d9X1RfJfkqxGJwoHJiJNp",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 495.8865995412334,
			"y": 605.7398207605368,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 288,
			"height": 46,
			"seed": 1754863174,
			"groupIds": [],
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "ejtyfHdN"
				}
			],
			"updated": 1686311159307,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 350,
			"versionNonce": 124505661,
			"isDeleted": false,
			"id": "ejtyfHdN",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 518.3865995412334,
			"y": 616.2398207605368,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 243,
			"height": 25,
			"seed": 864078406,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159308,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "while l1 != null || l2 != null",
			"rawText": "while l1 != null || l2 != null",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "d9X1RfJfkqxGJwoHJiJNp",
			"originalText": "while l1 != null || l2 != null",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "line",
			"version": 356,
			"versionNonce": 1353515027,
			"isDeleted": false,
			"id": "f09sfmSR4JlgGwG0bnpGX",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 788.7471488556644,
			"y": 620.7197477397001,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 293.2502468535715,
			"height": 2.0554870105383145,
			"seed": 1174467738,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1686311159308,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					293.2502468535715,
					-2.0554870105383145
				]
			]
		},
		{
			"type": "line",
			"version": 579,
			"versionNonce": 481361565,
			"isDeleted": false,
			"id": "n47qNGUJIGC8Nfl5MgvyE",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 518.3290668335276,
			"y": 648.3279884040182,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 10.521493436012861,
			"height": 769.0450317408596,
			"seed": 1282397446,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1686311159308,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					10.521493436012861,
					769.0450317408596
				]
			]
		},
		{
			"type": "text",
			"version": 187,
			"versionNonce": 31032755,
			"isDeleted": false,
			"id": "cuC54Pzm",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 570.8649507260234,
			"y": 672.7921550384985,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 138,
			"height": 25,
			"seed": 1133234502,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159308,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "valueOfL1 = 0",
			"rawText": "valueOfL1 = 0",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "valueOfL1 = 0",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 222,
			"versionNonce": 1186013949,
			"isDeleted": false,
			"id": "Jl3JxABL",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 571.5501566244288,
			"y": 713.2168461724722,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 147,
			"height": 25,
			"seed": 1347553734,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159308,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "valueOfL2 = 0",
			"rawText": "valueOfL2 = 0",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "valueOfL2 = 0",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 350,
			"versionNonce": 312760147,
			"isDeleted": false,
			"id": "xNRJO5pObfQ37Nv0Hp4iD",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 574.7584974985546,
			"y": 755.0118968293854,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 156,
			"height": 35,
			"seed": 1494687962,
			"groupIds": [],
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "EKYLN7r9"
				},
				{
					"id": "-KMLbaVZeNzJVe1BumxrU",
					"type": "arrow"
				}
			],
			"updated": 1686311159308,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 322,
			"versionNonce": 435010397,
			"isDeleted": false,
			"id": "EKYLN7r9",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 601.7584974985546,
			"y": 760.0118968293854,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 102,
			"height": 25,
			"seed": 1175401178,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159308,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "if l1 != null",
			"rawText": "if l1 != null",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "xNRJO5pObfQ37Nv0Hp4iD",
			"originalText": "if l1 != null",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 434,
			"versionNonce": 291763443,
			"isDeleted": false,
			"id": "57zzzR6sVb7XRKg_ID8mm",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 582.2788839853263,
			"y": 810.2553886294816,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 156,
			"height": 35,
			"seed": 334797574,
			"groupIds": [],
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "M9Fk06V7"
				},
				{
					"id": "TaZOEZc8gBVct_0Rr_2EC",
					"type": "arrow"
				}
			],
			"updated": 1686311159308,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 409,
			"versionNonce": 515393469,
			"isDeleted": false,
			"id": "M9Fk06V7",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 604.7788839853263,
			"y": 815.2553886294816,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 111,
			"height": 25,
			"seed": 1106725446,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159308,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "if l2 != null",
			"rawText": "if l2 != null",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "57zzzR6sVb7XRKg_ID8mm",
			"originalText": "if l2 != null",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "arrow",
			"version": 1103,
			"versionNonce": 2107563667,
			"isDeleted": false,
			"id": "-KMLbaVZeNzJVe1BumxrU",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 733.2489211603236,
			"y": 766.9930904750827,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 69.88650608443118,
			"height": 0.730594076940406,
			"seed": 686149190,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "YUriF5yq"
				}
			],
			"updated": 1686311159308,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "xNRJO5pObfQ37Nv0Hp4iD",
				"gap": 2.4904236617690003,
				"focus": -0.2553782948557581
			},
			"endBinding": {
				"elementId": "CsbpHz1e",
				"gap": 13.703490681653875,
				"focus": 0.323121873875478
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					69.88650608443118,
					-0.730594076940406
				]
			]
		},
		{
			"type": "text",
			"version": 284,
			"versionNonce": 1462913053,
			"isDeleted": false,
			"id": "YUriF5yq",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 784.5155199275378,
			"y": 756.5577813647571,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 16,
			"height": 25,
			"seed": 2117996614,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159308,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "T",
			"rawText": "T",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "-KMLbaVZeNzJVe1BumxrU",
			"originalText": "T",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "arrow",
			"version": 1055,
			"versionNonce": 571184179,
			"isDeleted": false,
			"id": "TaZOEZc8gBVct_0Rr_2EC",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 741.9315392398969,
			"y": 827.6934285184791,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 74.68263373004208,
			"height": 2.1097151585148595,
			"seed": 1850228954,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "5XJJAhkQ"
				}
			],
			"updated": 1686311159308,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "57zzzR6sVb7XRKg_ID8mm",
				"gap": 3.652655254570618,
				"focus": 0.11392188859613891
			},
			"endBinding": {
				"elementId": "yISwYhXp",
				"gap": 14.613023345560123,
				"focus": 0.30194330768510536
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					74.68263373004208,
					-2.1097151585148595
				]
			]
		},
		{
			"type": "text",
			"version": 342,
			"versionNonce": 88947837,
			"isDeleted": false,
			"id": "5XJJAhkQ",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 779.1522534717392,
			"y": 813.426342446102,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 16,
			"height": 25,
			"seed": 1073681818,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159308,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "T",
			"rawText": "T",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "TaZOEZc8gBVct_0Rr_2EC",
			"originalText": "T",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 404,
			"versionNonce": 781227475,
			"isDeleted": false,
			"id": "CsbpHz1e",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 816.8389179264086,
			"y": 757.0674099768589,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 167,
			"height": 25,
			"seed": 828274266,
			"groupIds": [],
			"roundness": null,
			"boundElements": [
				{
					"id": "-KMLbaVZeNzJVe1BumxrU",
					"type": "arrow"
				}
			],
			"updated": 1686311159308,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "valueOfL1 = l1.val",
			"rawText": "valueOfL1 = l1.val",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "valueOfL1 = l1.val",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 325,
			"versionNonce": 818586845,
			"isDeleted": false,
			"id": "yISwYhXp",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 831.227196315499,
			"y": 814.6211508196736,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 185,
			"height": 25,
			"seed": 463168902,
			"groupIds": [],
			"roundness": null,
			"boundElements": [
				{
					"id": "TaZOEZc8gBVct_0Rr_2EC",
					"type": "arrow"
				}
			],
			"updated": 1686311159308,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "valueOfL2 = l2.val",
			"rawText": "valueOfL2 = l2.val",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "valueOfL2 = l2.val",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 244,
			"versionNonce": 306471795,
			"isDeleted": false,
			"id": "ZxNinOT2",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 590.734771754614,
			"y": 860.5271232237923,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 293,
			"height": 25,
			"seed": 1736075738,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159308,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "sum = valueOfL1 + valueOfL2",
			"rawText": "sum = valueOfL1 + valueOfL2",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "sum = valueOfL1 + valueOfL2",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 406,
			"versionNonce": 1832649021,
			"isDeleted": false,
			"id": "eZVwsKdXIoJPBaRieskpX",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 593.1428902722946,
			"y": 912.1561300620273,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 120,
			"height": 35,
			"seed": 1062845702,
			"groupIds": [],
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "bdU8Spka"
				},
				{
					"id": "qUQcWFz0gpX1wVrDguZWR",
					"type": "arrow"
				}
			],
			"updated": 1686311159308,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 392,
			"versionNonce": 359496979,
			"isDeleted": false,
			"id": "bdU8Spka",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 616.1428902722946,
			"y": 917.1561300620273,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 74,
			"height": 25,
			"seed": 829836678,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159309,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "if carry",
			"rawText": "if carry",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "eZVwsKdXIoJPBaRieskpX",
			"originalText": "if carry",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "arrow",
			"version": 1340,
			"versionNonce": 1610797469,
			"isDeleted": false,
			"id": "qUQcWFz0gpX1wVrDguZWR",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 716.402561426599,
			"y": 935.5900411737042,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 86.67278073538887,
			"height": 4.504562590415958,
			"seed": 960179206,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "GSuPrClY"
				}
			],
			"updated": 1686311159309,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "eZVwsKdXIoJPBaRieskpX",
				"gap": 3.259671154304442,
				"focus": 0.1283409864640767
			},
			"endBinding": {
				"elementId": "bAUMH9eb",
				"gap": 7.535865254514874,
				"focus": -0.040706662784510586
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					86.67278073538887,
					4.504562590415958
				]
			]
		},
		{
			"type": "text",
			"version": 235,
			"versionNonce": 864182963,
			"isDeleted": false,
			"id": "GSuPrClY",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 712.17000830195,
			"y": 965.2386136892826,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 16,
			"height": 25,
			"seed": 919190426,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159309,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "T",
			"rawText": "T",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "qUQcWFz0gpX1wVrDguZWR",
			"originalText": "T",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 532,
			"versionNonce": 105944573,
			"isDeleted": false,
			"id": "bAUMH9eb",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 810.6112074165028,
			"y": 917.7591170909844,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 132,
			"height": 50,
			"seed": 1534811546,
			"groupIds": [],
			"roundness": null,
			"boundElements": [
				{
					"id": "qUQcWFz0gpX1wVrDguZWR",
					"type": "arrow"
				}
			],
			"updated": 1686311159309,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "sum += 1\ncarry = false",
			"rawText": "sum += 1\ncarry = false",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "sum += 1\ncarry = false",
			"lineHeight": 1.25,
			"baseline": 42
		},
		{
			"type": "rectangle",
			"version": 446,
			"versionNonce": 891917395,
			"isDeleted": false,
			"id": "9csucsP1cwLrechuyz5eg",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 587.2688576247663,
			"y": 977.6310797333465,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 125,
			"height": 35,
			"seed": 727826010,
			"groupIds": [],
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "LJhTz5ci"
				},
				{
					"id": "o5dWcZpOfd8tTUGDTdX3k",
					"type": "arrow"
				}
			],
			"updated": 1686311159309,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 394,
			"versionNonce": 992398941,
			"isDeleted": false,
			"id": "LJhTz5ci",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 599.2688576247663,
			"y": 982.6310797333465,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 101,
			"height": 25,
			"seed": 1964178118,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159309,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "if sum > 9",
			"rawText": "if sum > 9",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "9csucsP1cwLrechuyz5eg",
			"originalText": "if sum > 9",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "arrow",
			"version": 1518,
			"versionNonce": 171545075,
			"isDeleted": false,
			"id": "o5dWcZpOfd8tTUGDTdX3k",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 719.7565285344406,
			"y": 996.610141604968,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 86.19391104442684,
			"height": 5.459771652610016,
			"seed": 684809030,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "tHHhdcrH"
				}
			],
			"updated": 1686311159309,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "9csucsP1cwLrechuyz5eg",
				"gap": 7.487670909674307,
				"focus": 0.2755162152991135
			},
			"endBinding": {
				"elementId": "wVwIqg3n",
				"gap": 13.18554660274458,
				"focus": 0.5141509228041106
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					86.19391104442684,
					-5.459771652610016
				]
			]
		},
		{
			"type": "text",
			"version": 287,
			"versionNonce": 2102852285,
			"isDeleted": false,
			"id": "tHHhdcrH",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 775.164767470176,
			"y": 1126.487267456974,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 16,
			"height": 25,
			"seed": 1464993990,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159309,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "T",
			"rawText": "T",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "o5dWcZpOfd8tTUGDTdX3k",
			"originalText": "T",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 486,
			"versionNonce": 1673059219,
			"isDeleted": false,
			"id": "wVwIqg3n",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 819.135986181612,
			"y": 976.2608770320192,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 124,
			"height": 50,
			"seed": 1768108442,
			"groupIds": [],
			"roundness": null,
			"boundElements": [
				{
					"id": "o5dWcZpOfd8tTUGDTdX3k",
					"type": "arrow"
				}
			],
			"updated": 1686311159309,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "sum -= 10\ncarry = true",
			"rawText": "sum -= 10\ncarry = true",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "sum -= 10\ncarry = true",
			"lineHeight": 1.25,
			"baseline": 42
		},
		{
			"type": "freedraw",
			"version": 142,
			"versionNonce": 1971493661,
			"isDeleted": false,
			"id": "Srq4gzxwOmgx2lrilIHNb",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1121.7364627538389,
			"y": 937.9507373690682,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 39.73943296169773,
			"height": 66.46089478337285,
			"seed": 1079323398,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159309,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-13.703281586169169,
					16.443948358177295
				],
				[
					-20.554922379253867,
					43.85051153051597
				],
				[
					-18.49951377952175,
					53.442819095608684
				],
				[
					-11.64787298643705,
					58.92415263962471
				],
				[
					-2.0555131474736754,
					60.979613513227605
				],
				[
					10.277461189627047,
					56.86863949215103
				],
				[
					19.184510582443863,
					47.27633192705832
				],
				[
					17.81420333337519,
					24.665948674201445
				],
				[
					14.38838293683284,
					10.277461189626933
				],
				[
					9.592255291222045,
					0.6852058984051155
				],
				[
					2.7406144981373473,
					-5.481281270145246
				],
				[
					-3.425820396542349,
					-3.425820396542349
				],
				[
					-4.796232193352353,
					5.4813335440160245
				],
				[
					0,
					15.073641109108735
				],
				[
					0,
					15.073641109108735
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2490234375,
				0.357421875,
				0.45703125,
				0.46875,
				0.46875,
				0.4560546875,
				0.4228515625,
				0.4228515625,
				0.494140625,
				0.5,
				0.5087890625,
				0.533203125,
				0.54296875,
				0.2900390625,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 134,
			"versionNonce": 232649011,
			"isDeleted": false,
			"id": "cV2O9ty0H9AlxhulDJIfM",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1166.2721279088892,
			"y": 929.7287893269148,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 25.351154572606447,
			"height": 65.09058753430429,
			"seed": 2027026010,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159310,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-17.814307881116747,
					26.721409547804342
				],
				[
					-25.351154572606447,
					53.442819095608684
				],
				[
					-19.184615130185193,
					61.66476713776194
				],
				[
					-15.0736933829794,
					64.40543390976995
				],
				[
					-11.64787298643705,
					65.09058753430429
				],
				[
					-8.907153940558374,
					65.09058753430429
				],
				[
					-8.907153940558374,
					65.09058753430429
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.23046875,
				0.3125,
				0.43359375,
				0.455078125,
				0.455078125,
				0.43359375,
				0.0126953125,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 142,
			"versionNonce": 1008414589,
			"isDeleted": false,
			"id": "6IBpe-HEBq7QdHeiyg1Ni",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1166.2721279088892,
			"y": 968.097967313415,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 22.610435526727542,
			"height": 26.036203649399226,
			"seed": 1317757254,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159310,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.6852058984050018,
					8.907153940558374
				],
				[
					-1.3704117968100036,
					19.184615130185307
				],
				[
					-0.6852058984050018,
					24.665896400330553
				],
				[
					6.851640793084698,
					15.073641109108735
				],
				[
					12.332869789359165,
					3.4258203965422354
				],
				[
					13.703281586169396,
					0.6851536245342231
				],
				[
					15.07358883523807,
					-1.3703072490686736
				],
				[
					15.758690185901514,
					-1.3703072490686736
				],
				[
					17.81420333337519,
					0.6851536245342231
				],
				[
					18.49940923178042,
					14.38843521070362
				],
				[
					19.184510582443863,
					17.12910198271163
				],
				[
					19.869716480849092,
					19.184615130185307
				],
				[
					20.554922379254094,
					19.869768754719644
				],
				[
					21.24002372991754,
					19.869768754719644
				],
				[
					21.24002372991754,
					19.869768754719644
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.234375,
				0.2470703125,
				0.2763671875,
				0.32421875,
				0.4345703125,
				0.44921875,
				0.4521484375,
				0.4658203125,
				0.4892578125,
				0.50390625,
				0.5205078125,
				0.515625,
				0.453125,
				0.2666015625,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 135,
			"versionNonce": 168776403,
			"isDeleted": false,
			"id": "-ie4Fhwybh_U9igYVaYbc",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1190.937972035349,
			"y": 922.1919949092959,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 26.72146182167512,
			"height": 75.36804872393134,
			"seed": 242713626,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159310,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					10.962667088032049,
					13.01812796163506
				],
				[
					20.554922379254094,
					32.887844442483924
				],
				[
					26.72146182167512,
					61.66476713776194
				],
				[
					20.554922379254094,
					71.25707470285465
				],
				[
					15.758794733643072,
					74.682895099397
				],
				[
					13.018180235505952,
					75.36804872393134
				],
				[
					3.425820396542349,
					73.99768920099189
				],
				[
					3.425820396542349,
					73.99768920099189
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2646484375,
				0.30859375,
				0.3759765625,
				0.419921875,
				0.4814453125,
				0.4921875,
				0.484375,
				0.0146484375,
				0
			]
		},
		{
			"type": "rectangle",
			"version": 262,
			"versionNonce": 1600272349,
			"isDeleted": false,
			"id": "i_c62OAKmwCyc1MA7ILGX",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 592.5859724854554,
			"y": 1049.668703073489,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 130,
			"height": 35,
			"seed": 642212130,
			"groupIds": [],
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "XTNcHyqj"
				}
			],
			"updated": 1686311159310,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 250,
			"versionNonce": 1759740019,
			"isDeleted": false,
			"id": "XTNcHyqj",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 606.5859724854554,
			"y": 1054.668703073489,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 102,
			"height": 25,
			"seed": 145292834,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159310,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "if l1 != null",
			"rawText": "if l1 != null",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "i_c62OAKmwCyc1MA7ILGX",
			"originalText": "if l1 != null",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 325,
			"versionNonce": 694760509,
			"isDeleted": false,
			"id": "IoHzJiE6iYj3EepXNUw-Z",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 596.695542704362,
			"y": 1095.393142415786,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 127,
			"height": 35,
			"seed": 1847875426,
			"groupIds": [],
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "UJkg4XXO"
				},
				{
					"id": "oHZDYj41TNFK4PrMthRv6",
					"type": "arrow"
				}
			],
			"updated": 1686311159310,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 312,
			"versionNonce": 1679882771,
			"isDeleted": false,
			"id": "UJkg4XXO",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 604.695542704362,
			"y": 1100.393142415786,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 111,
			"height": 25,
			"seed": 906082338,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159310,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "if l2 != null",
			"rawText": "if l2 != null",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "IoHzJiE6iYj3EepXNUw-Z",
			"originalText": "if l2 != null",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 268,
			"versionNonce": 638690461,
			"isDeleted": false,
			"id": "3eceJrTA",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 792.5150781152308,
			"y": 1057.530842656977,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 99,
			"height": 25,
			"seed": 1364997054,
			"groupIds": [],
			"roundness": null,
			"boundElements": [
				{
					"id": "7GEW_8TKSqvJrC8mX6Rpn",
					"type": "arrow"
				}
			],
			"updated": 1686311159310,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "l1 = l1.next",
			"rawText": "l1 = l1.next",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "l1 = l1.next",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 286,
			"versionNonce": 951992243,
			"isDeleted": false,
			"id": "PUoVTY2C",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 784.1728176655074,
			"y": 1098.3158989111728,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 117,
			"height": 25,
			"seed": 648429118,
			"groupIds": [],
			"roundness": null,
			"boundElements": [
				{
					"id": "oHZDYj41TNFK4PrMthRv6",
					"type": "arrow"
				}
			],
			"updated": 1686311159310,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "l2 = l2.next",
			"rawText": "l2 = l2.next",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "l2 = l2.next",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "arrow",
			"version": 483,
			"versionNonce": 1762461949,
			"isDeleted": false,
			"id": "7GEW_8TKSqvJrC8mX6Rpn",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 719.7510739265713,
			"y": 1071.363797321503,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 61.17742526287475,
			"height": 0.00020867805596935796,
			"seed": 789981474,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "WyDR98C8"
				}
			],
			"updated": 1686311159310,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": {
				"elementId": "3eceJrTA",
				"focus": -0.10660156952356736,
				"gap": 11.586578925784806
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					61.17742526287475,
					-0.00020867805596935796
				]
			]
		},
		{
			"type": "text",
			"version": 190,
			"versionNonce": 1088541011,
			"isDeleted": false,
			"id": "WyDR98C8",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 740.4859509025143,
			"y": 1057.5444454894543,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 16,
			"height": 25,
			"seed": 334352062,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159310,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "T",
			"rawText": "T",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "7GEW_8TKSqvJrC8mX6Rpn",
			"originalText": "T",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "arrow",
			"version": 885,
			"versionNonce": 333242717,
			"isDeleted": false,
			"id": "oHZDYj41TNFK4PrMthRv6",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 728.1285512963491,
			"y": 1110.7173418536188,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 52.37159982033154,
			"height": 1.1286090202147534,
			"seed": 1908017442,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "eTMXarA5"
				}
			],
			"updated": 1686311159310,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "IoHzJiE6iYj3EepXNUw-Z",
				"gap": 4.433008591987118,
				"focus": -0.03772666902136126
			},
			"endBinding": {
				"elementId": "PUoVTY2C",
				"gap": 3.6726665488267827,
				"focus": 0.1865452140841219
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					52.37159982033154,
					-1.1286090202147534
				]
			]
		},
		{
			"type": "text",
			"version": 276,
			"versionNonce": 1306668787,
			"isDeleted": false,
			"id": "eTMXarA5",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 746.0826040697539,
			"y": 1098.258337135402,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 16,
			"height": 25,
			"seed": 295736546,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159310,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "T",
			"rawText": "T",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "oHZDYj41TNFK4PrMthRv6",
			"originalText": "T",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 445,
			"versionNonce": 466791869,
			"isDeleted": false,
			"id": "vbG4JsQ7plrfgL5NZRzxl",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 601.7048791824361,
			"y": 1166.6186839705576,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 233,
			"height": 35,
			"seed": 254315810,
			"groupIds": [],
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "RGZeWxgw"
				},
				{
					"id": "EeX-2jgbjK6uHY6Y9BhQz",
					"type": "arrow"
				},
				{
					"id": "_sUU7kmSwFxfD_R_6eJLB",
					"type": "arrow"
				}
			],
			"updated": 1686311159310,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 459,
			"versionNonce": 1111873683,
			"isDeleted": false,
			"id": "RGZeWxgw",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 610.7048791824361,
			"y": 1171.6186839705576,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 215,
			"height": 25,
			"seed": 111057122,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159310,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "if l1 != null || l2 != null",
			"rawText": "if l1 != null || l2 != null",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "vbG4JsQ7plrfgL5NZRzxl",
			"originalText": "if l1 != null || l2 != null",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 351,
			"versionNonce": 1343221277,
			"isDeleted": false,
			"id": "21X7o51b",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 798.0767972396054,
			"y": 1244.3077551585004,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 247,
			"height": 50,
			"seed": 712431486,
			"groupIds": [],
			"roundness": null,
			"boundElements": [
				{
					"id": "EeX-2jgbjK6uHY6Y9BhQz",
					"type": "arrow"
				}
			],
			"updated": 1686311159310,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "solution.next = new LL(0)\nsolution = solution.next",
			"rawText": "solution.next = new LL(0)\nsolution = solution.next",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "solution.next = new LL(0)\nsolution = solution.next",
			"lineHeight": 1.25,
			"baseline": 42
		},
		{
			"type": "arrow",
			"version": 673,
			"versionNonce": 1807961651,
			"isDeleted": false,
			"id": "EeX-2jgbjK6uHY6Y9BhQz",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 719.1413381374236,
			"y": 1208.6207823165616,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 87.51237251878729,
			"height": 27.80806522714215,
			"seed": 698298110,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "Yhg6cteH"
				}
			],
			"updated": 1686311159310,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "vbG4JsQ7plrfgL5NZRzxl",
				"gap": 7.002098346004004,
				"focus": 0.4439632223301765
			},
			"endBinding": {
				"elementId": "21X7o51b",
				"gap": 7.878907614796617,
				"focus": -0.05664736886679968
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					87.51237251878729,
					27.80806522714215
				]
			]
		},
		{
			"type": "text",
			"version": 127,
			"versionNonce": 528884349,
			"isDeleted": false,
			"id": "Yhg6cteH",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 758.0975310683041,
			"y": 1223.2336061334206,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 16,
			"height": 25,
			"seed": 1079468862,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159311,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "T",
			"rawText": "T",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "EeX-2jgbjK6uHY6Y9BhQz",
			"originalText": "T",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 301,
			"versionNonce": 490803155,
			"isDeleted": false,
			"id": "YZk7k4G8AX1fz0zyRGxf-",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 584.9629055130176,
			"y": 1349.5062158639896,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 150,
			"height": 39,
			"seed": 615472062,
			"groupIds": [],
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "aM0MnguH"
				},
				{
					"id": "_sUU7kmSwFxfD_R_6eJLB",
					"type": "arrow"
				},
				{
					"id": "qZOvKlvnOG6T3ceyd4Oef",
					"type": "arrow"
				}
			],
			"updated": 1686311159311,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 391,
			"versionNonce": 519490269,
			"isDeleted": false,
			"id": "aM0MnguH",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 598.9629055130176,
			"y": 1356.5062158639896,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 122,
			"height": 25,
			"seed": 588168802,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159311,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "else if carry",
			"rawText": "else if carry",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "YZk7k4G8AX1fz0zyRGxf-",
			"originalText": "else if carry",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "arrow",
			"version": 611,
			"versionNonce": 148217203,
			"isDeleted": false,
			"id": "_sUU7kmSwFxfD_R_6eJLB",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 674.4070945238054,
			"y": 1208.1572880430397,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 18.909039920301893,
			"height": 129.30705247069068,
			"seed": 427572030,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "VbZv4or5"
				}
			],
			"updated": 1686311159311,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "vbG4JsQ7plrfgL5NZRzxl",
				"gap": 6.5386040724820305,
				"focus": 0.3383406740756484
			},
			"endBinding": {
				"elementId": "YZk7k4G8AX1fz0zyRGxf-",
				"gap": 12.04187535025926,
				"focus": -0.11659797681249234
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					-18.909039920301893,
					129.30705247069068
				]
			]
		},
		{
			"type": "text",
			"version": 124,
			"versionNonce": 1324574525,
			"isDeleted": false,
			"id": "VbZv4or5",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 670.685193469837,
			"y": 1236.442308937587,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 11,
			"height": 25,
			"seed": 1623093310,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159311,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "F",
			"rawText": "F",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "_sUU7kmSwFxfD_R_6eJLB",
			"originalText": "F",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 246,
			"versionNonce": 1506244371,
			"isDeleted": false,
			"id": "zhRP7JL5",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 791.5883724453761,
			"y": 1356.4664742193838,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 238,
			"height": 25,
			"seed": 9443518,
			"groupIds": [],
			"roundness": null,
			"boundElements": [
				{
					"id": "qZOvKlvnOG6T3ceyd4Oef",
					"type": "arrow"
				}
			],
			"updated": 1686311159311,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "solution.next = new LL(1)",
			"rawText": "solution.next = new LL(1)",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "solution.next = new LL(1)",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "arrow",
			"version": 580,
			"versionNonce": 568162205,
			"isDeleted": false,
			"id": "qZOvKlvnOG6T3ceyd4Oef",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 740.9274312797174,
			"y": 1372.4631610610302,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 43.245527824384794,
			"height": 0.4090642460776053,
			"seed": 112005794,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "AqBeoXcy"
				}
			],
			"updated": 1686311159311,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "YZk7k4G8AX1fz0zyRGxf-",
				"gap": 5.964525766699808,
				"focus": 0.1331602287605074
			},
			"endBinding": {
				"elementId": "zhRP7JL5",
				"gap": 7.415413341273961,
				"focus": -0.37440668322994336
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					43.245527824384794,
					0.4090642460776053
				]
			]
		},
		{
			"type": "text",
			"version": 124,
			"versionNonce": 244128947,
			"isDeleted": false,
			"id": "AqBeoXcy",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 717.5444164289365,
			"y": 1345.1251745435404,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 16,
			"height": 25,
			"seed": 250617086,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159311,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "T",
			"rawText": "T",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "qZOvKlvnOG6T3ceyd4Oef",
			"originalText": "T",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "line",
			"version": 272,
			"versionNonce": 1105624061,
			"isDeleted": false,
			"id": "q6-SN0w2sC7Pwcu-lCMQb",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 526.0224545151882,
			"y": 1416.2538409774754,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 546.8898632478588,
			"height": 0,
			"seed": 155173182,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1686311159311,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					546.8898632478588,
					0
				]
			]
		},
		{
			"type": "line",
			"version": 246,
			"versionNonce": 315428435,
			"isDeleted": false,
			"id": "G_xmYU72_KKJ5OYLJK4U4",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1067.2681257044012,
			"y": 620.059075701106,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 0,
			"height": 797.3574167954677,
			"seed": 865075746,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1686311159311,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					0,
					797.3574167954677
				]
			]
		},
		{
			"type": "text",
			"version": 173,
			"versionNonce": 386921565,
			"isDeleted": false,
			"id": "vMLPktr1",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 547.6885547950408,
			"y": 1455.067259588299,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 190,
			"height": 25,
			"seed": 1000960802,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159311,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "return solutionRoot",
			"rawText": "return solutionRoot",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "return solutionRoot",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 205,
			"versionNonce": 425577459,
			"isDeleted": false,
			"id": "VCCU9bsz",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 507.7545176243225,
			"y": 1544.4206528586383,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 165,
			"height": 25,
			"seed": 1711394814,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159311,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "OPTIMIZATION",
			"rawText": "OPTIMIZATION",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "OPTIMIZATION",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 246,
			"versionNonce": 220946621,
			"isDeleted": false,
			"id": "WzD1RNLk",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 547.6592450335961,
			"y": 1591.0916847973256,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 500,
			"height": 50,
			"seed": 1214359522,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159311,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "- Save space by overwriting l1 to place the results\n",
			"rawText": "- Save space by overwriting l1 to place the results\n",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "- Save space by overwriting l1 to place the results\n",
			"lineHeight": 1.25,
			"baseline": 42
		},
		{
			"type": "text",
			"version": 171,
			"versionNonce": 910546323,
			"isDeleted": false,
			"id": "KHAjE5i0",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 797.9921741846903,
			"y": -504.3955349514223,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 189,
			"height": 25,
			"seed": 1105104226,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159311,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "IMPLEMENTATION",
			"rawText": "IMPLEMENTATION",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "IMPLEMENTATION",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 386,
			"versionNonce": 433733917,
			"isDeleted": false,
			"id": "8HEJKyGR",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 776.4118990598255,
			"y": -461.1675143494115,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 375,
			"height": 25,
			"seed": 1665386558,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159311,
			"link": "[[LeetCode/Questions#Solution 2]]",
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "📍[[LeetCode/Questions#Solution 2]]",
			"rawText": "[[LeetCode/Questions#Solution 2]]",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "📍[[LeetCode/Questions#Solution 2]]",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "line",
			"version": 360,
			"versionNonce": 951823155,
			"isDeleted": false,
			"id": "nlNHxucCe0InCk0cy5Q3D",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1370.4378048268636,
			"y": -547.1153953590187,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 0,
			"height": 2059.2000732421875,
			"seed": 2000487970,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1686311159311,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					0,
					2059.2000732421875
				]
			]
		},
		{
			"type": "text",
			"version": 41,
			"versionNonce": 42866045,
			"isDeleted": false,
			"id": "xhM5EUUD",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1443.6280570522028,
			"y": -516.2869258988712,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 549,
			"height": 50,
			"seed": 632834217,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159312,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "## 3. Longest Substring Without Repeating Characters\n",
			"rawText": "## 3. Longest Substring Without Repeating Characters\n",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "## 3. Longest Substring Without Repeating Characters\n",
			"lineHeight": 1.25,
			"baseline": 42
		},
		{
			"type": "text",
			"version": 279,
			"versionNonce": 1160105171,
			"isDeleted": false,
			"id": "roA8ufOK",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2019.2948291432308,
			"y": -467.3475250236642,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 189,
			"height": 25,
			"seed": 499695369,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159312,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "IMPLEMENTATION",
			"rawText": "IMPLEMENTATION",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "IMPLEMENTATION",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 297,
			"versionNonce": 1653104093,
			"isDeleted": false,
			"id": "NNWqlJlc",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1994.9313888319148,
			"y": -417.6505368311932,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 375,
			"height": 25,
			"seed": 99058791,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159312,
			"link": "[[LeetCode/Questions#Solution 3]]",
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "📍[[LeetCode/Questions#Solution 3]]",
			"rawText": "[[LeetCode/Questions#Solution 3]]",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "📍[[LeetCode/Questions#Solution 3]]",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 48,
			"versionNonce": 790280819,
			"isDeleted": false,
			"id": "GMHL0rQL",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1448.2514930681682,
			"y": -427.56872475289015,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 50,
			"height": 25,
			"seed": 163237735,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159312,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "INFO",
			"rawText": "INFO",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "INFO",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 207,
			"versionNonce": 1893374525,
			"isDeleted": false,
			"id": "ZaCZwczy",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1499.9182614600948,
			"y": -371.90196653348755,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 750,
			"height": 100,
			"seed": 1231002953,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159312,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "- String s: some string with size\n- find the length (int) of the longest substring without repeated characters\n\n > int lenghtOfLongestSubstring(String s) <",
			"rawText": "- String s: some string with size\n- find the length (int) of the longest substring without repeated characters\n\n > int lenghtOfLongestSubstring(String s) <",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "- String s: some string with size\n- find the length (int) of the longest substring without repeated characters\n\n > int lenghtOfLongestSubstring(String s) <",
			"lineHeight": 1.25,
			"baseline": 92
		},
		{
			"type": "text",
			"version": 66,
			"versionNonce": 325121043,
			"isDeleted": false,
			"id": "HLDADPi9",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1442.5848874366573,
			"y": -221.56861285510217,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 91,
			"height": 25,
			"seed": 465164585,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159312,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "EXAMPLE",
			"rawText": "EXAMPLE",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "EXAMPLE",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 65,
			"versionNonce": 107367069,
			"isDeleted": false,
			"id": "bHKtblkx",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1518.2516456560575,
			"y": -145.90200722359225,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 538,
			"height": 75,
			"seed": 362736585,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159312,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Input: s = \"abcabcbb\"\nOutput: 3\nExplanation: The answer is \"abc\", with the length of 3.",
			"rawText": "Input: s = \"abcabcbb\"\nOutput: 3\nExplanation: The answer is \"abc\", with the length of 3.",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Input: s = \"abcabcbb\"\nOutput: 3\nExplanation: The answer is \"abc\", with the length of 3.",
			"lineHeight": 1.25,
			"baseline": 67
		},
		{
			"type": "text",
			"version": 184,
			"versionNonce": 837745075,
			"isDeleted": false,
			"id": "Hcpkd9il",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2036.3849464373066,
			"y": -234.50208453479013,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 43,
			"height": 25,
			"seed": 855532359,
			"groupIds": [
				"UphowJeaRVofNSoQ_TxLi"
			],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159312,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "s = ",
			"rawText": "s = ",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "s = ",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 460,
			"versionNonce": 1675423485,
			"isDeleted": false,
			"id": "8ArDQW-85OzqqMEk-9gUh",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2087.2183814959003,
			"y": -251.26547300102706,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 277,
			"height": 54,
			"seed": 1515861159,
			"groupIds": [
				"UphowJeaRVofNSoQ_TxLi"
			],
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "O9WPDf8g"
				}
			],
			"updated": 1686311159312,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 740,
			"versionNonce": 132860755,
			"isDeleted": false,
			"id": "O9WPDf8g",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2108.2183814959003,
			"y": -243.2170968424529,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 235,
			"height": 37.903247682851635,
			"seed": 1399680713,
			"groupIds": [
				"UphowJeaRVofNSoQ_TxLi"
			],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159312,
			"link": null,
			"locked": false,
			"fontSize": 30.322598146281308,
			"fontFamily": 1,
			"text": "a b c a b c b b",
			"rawText": "a b c a b c b b",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "8ArDQW-85OzqqMEk-9gUh",
			"originalText": "a b c a b c b b",
			"lineHeight": 1.25,
			"baseline": 26
		},
		{
			"type": "text",
			"version": 322,
			"versionNonce": 935331677,
			"isDeleted": false,
			"id": "LrTy4VPp",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2034.3849260922548,
			"y": -164.16878171903494,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 111,
			"height": 25,
			"seed": 851197929,
			"groupIds": [
				"UphowJeaRVofNSoQ_TxLi"
			],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159312,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "answer = 3",
			"rawText": "answer = 3",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "answer = 3",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "line",
			"version": 250,
			"versionNonce": 699164915,
			"isDeleted": false,
			"id": "U2HwU-tgx-20HiugvRulg",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2103.0517148292342,
			"y": -186.16875120145687,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 90.66660563151027,
			"height": 1.33331298828125,
			"seed": 1148016745,
			"groupIds": [
				"UphowJeaRVofNSoQ_TxLi"
			],
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1686311159312,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					90.66660563151027,
					-1.33331298828125
				]
			]
		},
		{
			"type": "text",
			"version": 56,
			"versionNonce": 1684083645,
			"isDeleted": false,
			"id": "qsfNyCd1",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1519.5851112322284,
			"y": -4.901997051066246,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 506,
			"height": 75,
			"seed": 1245661737,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159312,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Input: s = \"bbbbb\"\nOutput: 1\nExplanation: The answer is \"b\", with the length of 1.",
			"rawText": "Input: s = \"bbbbb\"\nOutput: 1\nExplanation: The answer is \"b\", with the length of 1.",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Input: s = \"bbbbb\"\nOutput: 1\nExplanation: The answer is \"b\", with the length of 1.",
			"lineHeight": 1.25,
			"baseline": 67
		},
		{
			"type": "text",
			"version": 143,
			"versionNonce": 1555616403,
			"isDeleted": false,
			"id": "Cjhf1DmE",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2068.4516578630883,
			"y": -21.702076396769428,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 43,
			"height": 25,
			"seed": 1910315175,
			"groupIds": [
				"E9gpPbqWmEEqmeOF517Oz"
			],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159312,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "s = ",
			"rawText": "s = ",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "s = ",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 527,
			"versionNonce": 98669597,
			"isDeleted": false,
			"id": "iqw57qDd8RdrhziNfYWIG",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2127.6182838396503,
			"y": -34.33375028483587,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 193,
			"height": 48,
			"seed": 1438376905,
			"groupIds": [
				"E9gpPbqWmEEqmeOF517Oz"
			],
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "8LchyRmr"
				}
			],
			"updated": 1686311159312,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 813,
			"versionNonce": 1908869171,
			"isDeleted": false,
			"id": "8LchyRmr",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2156.6182838396503,
			"y": -29.28537412626169,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 135,
			"height": 37.903247682851635,
			"seed": 637436585,
			"groupIds": [
				"E9gpPbqWmEEqmeOF517Oz"
			],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159312,
			"link": null,
			"locked": false,
			"fontSize": 30.322598146281308,
			"fontFamily": 1,
			"text": "b b b b b",
			"rawText": "b b b b b",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "iqw57qDd8RdrhziNfYWIG",
			"originalText": "b b b b b",
			"lineHeight": 1.25,
			"baseline": 26
		},
		{
			"type": "text",
			"version": 181,
			"versionNonce": 942868605,
			"isDeleted": false,
			"id": "DuNZWEmW",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2060.784930161265,
			"y": 45.29789308565233,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 102,
			"height": 25,
			"seed": 1506537255,
			"groupIds": [
				"E9gpPbqWmEEqmeOF517Oz"
			],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159312,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "answer = 1",
			"rawText": "answer = 1",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "answer = 1",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "line",
			"version": 177,
			"versionNonce": 1589479891,
			"isDeleted": false,
			"id": "2MeP7BBc2lUvSMgrH7lVZ",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2146.7849911964213,
			"y": 20.63124676403794,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 30,
			"height": 2.0000203450520075,
			"seed": 1151938215,
			"groupIds": [
				"E9gpPbqWmEEqmeOF517Oz"
			],
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1686311159313,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					30,
					2.0000203450520075
				]
			]
		},
		{
			"type": "text",
			"version": 76,
			"versionNonce": 488042717,
			"isDeleted": false,
			"id": "d97KNsgQ",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1447.1926836495518,
			"y": 173.78864952881048,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 149,
			"height": 25,
			"seed": 1412649447,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159313,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "WALKTHROUGH",
			"rawText": "WALKTHROUGH",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "WALKTHROUGH",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 184,
			"versionNonce": 414373747,
			"isDeleted": false,
			"id": "awDk0lBX",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1447.6763043505243,
			"y": 585.5122307116377,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 138,
			"height": 25,
			"seed": 2053389117,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159313,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "BRUTEFORCE",
			"rawText": "BRUTEFORCE",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "BRUTEFORCE",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 490,
			"versionNonce": 572443965,
			"isDeleted": false,
			"id": "TJzEns7o",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1522.3787602013088,
			"y": 236.6266272830922,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 345,
			"height": 300,
			"seed": 370523727,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159313,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "- HM map = new HM()\n- maxSize = 0\n- for i=0; i < s.size; i++\n    - char c = s.charAt(i)\n    - if char not in map\n        - add char to map, index\n    - else\n        - if size of map > maxSize\n            - maxSize = map.size\n        - i = map.get(c)\n        - reset map\n- return math.max maxSize, HM.size",
			"rawText": "- HM map = new HM()\n- maxSize = 0\n- for i=0; i < s.size; i++\n    - char c = s.charAt(i)\n    - if char not in map\n        - add char to map, index\n    - else\n        - if size of map > maxSize\n            - maxSize = map.size\n        - i = map.get(c)\n        - reset map\n- return math.max maxSize, HM.size",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "- HM map = new HM()\n- maxSize = 0\n- for i=0; i < s.size; i++\n    - char c = s.charAt(i)\n    - if char not in map\n        - add char to map, index\n    - else\n        - if size of map > maxSize\n            - maxSize = map.size\n        - i = map.get(c)\n        - reset map\n- return math.max maxSize, HM.size",
			"lineHeight": 1.25,
			"baseline": 292
		},
		{
			"type": "freedraw",
			"version": 61,
			"versionNonce": 770535699,
			"isDeleted": false,
			"id": "6PjlyUkXOYhWTzcax-vm0",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2045.5936509438359,
			"y": 976.1904593415402,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 2.2322809473234884,
			"height": 1.6742373215074622,
			"seed": 38241871,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159313,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-2.2322809473234884,
					-1.116129829255783
				],
				[
					-2.2322809473234884,
					-1.6742373215074622
				],
				[
					0,
					0
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.17578125,
				0.1962890625,
				0.0224609375,
				0
			]
		},
		{
			"type": "text",
			"version": 164,
			"versionNonce": 111943069,
			"isDeleted": false,
			"id": "6O8ooDM9",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1539.4574165912754,
			"y": 650.646506205907,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 121,
			"height": 50,
			"seed": 237690383,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159313,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "HashMap hp\nmaxSize = 0",
			"rawText": "HashMap hp\nmaxSize = 0",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "HashMap hp\nmaxSize = 0",
			"lineHeight": 1.25,
			"baseline": 42
		},
		{
			"type": "rectangle",
			"version": 223,
			"versionNonce": 535025331,
			"isDeleted": false,
			"id": "ltCk9EpwxvhMVMHjHQ7UU",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1535.4921515686724,
			"y": 714.5918625543156,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 286,
			"height": 35,
			"seed": 1562113519,
			"groupIds": [],
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "mIdyLAej"
				}
			],
			"updated": 1686311159313,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 272,
			"versionNonce": 569401853,
			"isDeleted": false,
			"id": "mIdyLAej",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1558.9921515686724,
			"y": 719.5918625543156,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 239,
			"height": 25,
			"seed": 1453149601,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159313,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "for i = 0; i < s.size; i++",
			"rawText": "for i = 0; i < s.size; i++",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "ltCk9EpwxvhMVMHjHQ7UU",
			"originalText": "for i = 0; i < s.size; i++",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "line",
			"version": 200,
			"versionNonce": 2101119059,
			"isDeleted": false,
			"id": "6tuly7dzpjyhD2JefzSv5",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1822.7304144940626,
			"y": 730.4637711932047,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 242.0601221918837,
			"height": 3.1300802384739086,
			"seed": 17978479,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1686311159313,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					242.0601221918837,
					3.1300802384739086
				]
			]
		},
		{
			"type": "line",
			"version": 286,
			"versionNonce": 1760369245,
			"isDeleted": false,
			"id": "pBY-QA_cOjAYMRoFxCGDr",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1563.454791288878,
			"y": 750.2876392376259,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 0,
			"height": 448.1243017407526,
			"seed": 847866369,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1686311159313,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					0,
					448.1243017407526
				]
			]
		},
		{
			"type": "text",
			"version": 183,
			"versionNonce": 1003357683,
			"isDeleted": false,
			"id": "t4sY6wXv",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1592.66905925324,
			"y": 772.9807707179739,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 195,
			"height": 25,
			"seed": 274727745,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159313,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "char c = s.charAt(i)",
			"rawText": "char c = s.charAt(i)",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "char c = s.charAt(i)",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 255,
			"versionNonce": 880002749,
			"isDeleted": false,
			"id": "hY79e_5HLUYHIL1OSZ-5U",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1597.3297773109957,
			"y": 811.9931759635472,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 192,
			"height": 35,
			"seed": 2007045793,
			"groupIds": [],
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "5GbI1Dya"
				},
				{
					"id": "egE-OmGR1sB0nKnirXHlO",
					"type": "arrow"
				},
				{
					"id": "pCLKpkOP2WMd0bjim_JxX",
					"type": "arrow"
				}
			],
			"updated": 1686311159313,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 238,
			"versionNonce": 1386139539,
			"isDeleted": false,
			"id": "5GbI1Dya",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1605.3297773109957,
			"y": 816.9931759635472,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 176,
			"height": 25,
			"seed": 1496399969,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159313,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "if char not in map",
			"rawText": "if char not in map",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "hY79e_5HLUYHIL1OSZ-5U",
			"originalText": "if char not in map",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 293,
			"versionNonce": 1193666333,
			"isDeleted": false,
			"id": "MBRee8Me",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1707.6998164759102,
			"y": 915.1389828767213,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 165,
			"height": 25,
			"seed": 575037793,
			"groupIds": [],
			"roundness": null,
			"boundElements": [
				{
					"id": "egE-OmGR1sB0nKnirXHlO",
					"type": "arrow"
				}
			],
			"updated": 1686311159313,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "add char to map",
			"rawText": "add char to map",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "add char to map",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "arrow",
			"version": 620,
			"versionNonce": 333800755,
			"isDeleted": false,
			"id": "egE-OmGR1sB0nKnirXHlO",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1648.9450713240524,
			"y": 855.3531712388233,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 96.22363906243163,
			"height": 48.56961449786786,
			"seed": 1245967745,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "kVdmDfZi"
				}
			],
			"updated": 1686311159313,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "hY79e_5HLUYHIL1OSZ-5U",
				"gap": 8.359995275275992,
				"focus": 0.7317450829861635
			},
			"endBinding": {
				"elementId": "MBRee8Me",
				"gap": 11.216197140030204,
				"focus": 0.018218652638402628
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					96.22363906243163,
					48.56961449786786
				]
			]
		},
		{
			"type": "text",
			"version": 113,
			"versionNonce": 326433661,
			"isDeleted": false,
			"id": "kVdmDfZi",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1806.1227833908015,
			"y": 818.6482709379366,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 16,
			"height": 25,
			"seed": 495251361,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159313,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "T",
			"rawText": "T",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "egE-OmGR1sB0nKnirXHlO",
			"originalText": "T",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 288,
			"versionNonce": 1191724755,
			"isDeleted": false,
			"id": "0JRMCfbRdwRCOt_9U8PRj",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1593.424545848733,
			"y": 947.4582765425113,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 71,
			"height": 35,
			"seed": 1722706831,
			"groupIds": [],
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "r3CyvYMt"
				},
				{
					"id": "pCLKpkOP2WMd0bjim_JxX",
					"type": "arrow"
				}
			],
			"updated": 1686311159313,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 250,
			"versionNonce": 1101169629,
			"isDeleted": false,
			"id": "r3CyvYMt",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1609.924545848733,
			"y": 952.4582765425113,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 38,
			"height": 25,
			"seed": 1847537167,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159314,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "else",
			"rawText": "else",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "0JRMCfbRdwRCOt_9U8PRj",
			"originalText": "else",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 365,
			"versionNonce": 43906163,
			"isDeleted": false,
			"id": "DGijO7MBf0lBlQJdp2uBv",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1630.788936397555,
			"y": 1006.4332220054662,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 239,
			"height": 35,
			"seed": 127961089,
			"groupIds": [],
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "l7Vr1W1T"
				},
				{
					"id": "5c1-Tg4N8zJKbqURuIm_T",
					"type": "arrow"
				}
			],
			"updated": 1686311159314,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 448,
			"versionNonce": 1975517245,
			"isDeleted": false,
			"id": "l7Vr1W1T",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1640.788936397555,
			"y": 1011.4332220054662,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 219,
			"height": 25,
			"seed": 935999119,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159314,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "if map.size >= maxSize",
			"rawText": "if map.size >= maxSize",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "DGijO7MBf0lBlQJdp2uBv",
			"originalText": "if map.size >= maxSize",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 439,
			"versionNonce": 1181543955,
			"isDeleted": false,
			"id": "3ZO2W5dZ",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1820.1220076618129,
			"y": 1106.596068244539,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 185,
			"height": 25,
			"seed": 1663387937,
			"groupIds": [],
			"roundness": null,
			"boundElements": [
				{
					"id": "5c1-Tg4N8zJKbqURuIm_T",
					"type": "arrow"
				}
			],
			"updated": 1686311159314,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "maxSize = map.size",
			"rawText": "maxSize = map.size",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "maxSize = map.size",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "arrow",
			"version": 577,
			"versionNonce": 1437528221,
			"isDeleted": false,
			"id": "pCLKpkOP2WMd0bjim_JxX",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1607.4741416965308,
			"y": 856.710685754776,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 10.485025041976769,
			"height": 76.16551134259976,
			"seed": 1343282145,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "OexmKV6X"
				}
			],
			"updated": 1686311159314,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "hY79e_5HLUYHIL1OSZ-5U",
				"gap": 9.71750979122885,
				"focus": 0.9105098563106434
			},
			"endBinding": {
				"elementId": "0JRMCfbRdwRCOt_9U8PRj",
				"gap": 14.582079445135491,
				"focus": -0.17275354658742992
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					10.485025041976769,
					76.16551134259976
				]
			]
		},
		{
			"type": "text",
			"version": 172,
			"versionNonce": 1433121715,
			"isDeleted": false,
			"id": "OexmKV6X",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1688.8968461087252,
			"y": 854.3834763806634,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 11,
			"height": 25,
			"seed": 2004386383,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159314,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "F",
			"rawText": "F",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "pCLKpkOP2WMd0bjim_JxX",
			"originalText": "F",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "arrow",
			"version": 744,
			"versionNonce": 1327551741,
			"isDeleted": false,
			"id": "5c1-Tg4N8zJKbqURuIm_T",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1688.4199030242644,
			"y": 1052.2814034199548,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 190.8592220100145,
			"height": 43.881117097844935,
			"seed": 1621983343,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "dg3ZClGf"
				}
			],
			"updated": 1686311159314,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "DGijO7MBf0lBlQJdp2uBv",
				"gap": 10.848181414488579,
				"focus": 0.9465931016210912
			},
			"endBinding": {
				"elementId": "3ZO2W5dZ",
				"gap": 10.433547726739334,
				"focus": 0.45214461861260763
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					190.8592220100145,
					43.881117097844935
				]
			]
		},
		{
			"type": "text",
			"version": 113,
			"versionNonce": 1338033491,
			"isDeleted": false,
			"id": "dg3ZClGf",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1914.1107705243644,
			"y": 1014.8005164645947,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 16,
			"height": 25,
			"seed": 1190012239,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159314,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "T",
			"rawText": "T",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "5c1-Tg4N8zJKbqURuIm_T",
			"originalText": "T",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 236,
			"versionNonce": 496446813,
			"isDeleted": false,
			"id": "IFmFOM5C",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1637.0118957992277,
			"y": 1116.507942565055,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 134,
			"height": 50,
			"seed": 1896912129,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159314,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "i = map.get(c)\nreset map",
			"rawText": "i = map.get(c)\nreset map",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "i = map.get(c)\nreset map",
			"lineHeight": 1.25,
			"baseline": 42
		},
		{
			"type": "line",
			"version": 243,
			"versionNonce": 214082291,
			"isDeleted": false,
			"id": "QSDA9Ugiaou9s_vlkdsWx",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2063.747269475758,
			"y": 737.7672983831654,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 4.547473508864641e-13,
			"height": 446.5592616215157,
			"seed": 1366959279,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1686311159314,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					-4.547473508864641e-13,
					446.5592616215157
				]
			]
		},
		{
			"type": "line",
			"version": 180,
			"versionNonce": 274954685,
			"isDeleted": false,
			"id": "9VkeIGSnModdxk9J0kupJ",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1564.498177902456,
			"y": 1186.9349668369312,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 496.64068474105216,
			"height": 0,
			"seed": 1037634799,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1686311159314,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					496.64068474105216,
					0
				]
			]
		},
		{
			"type": "text",
			"version": 165,
			"versionNonce": 888654995,
			"isDeleted": false,
			"id": "acF9zMYQ",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1580.409515300762,
			"y": 1229.1911893602824,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 327,
			"height": 25,
			"seed": 1407156847,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159314,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "return math.max maxSize, HM.size",
			"rawText": "return math.max maxSize, HM.size",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "return math.max maxSize, HM.size",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "line",
			"version": 208,
			"versionNonce": 279394845,
			"isDeleted": false,
			"id": "pIvQ3O9Pad4hEiKHmAwe7",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2415.9666401444006,
			"y": -518.6203507849407,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 0,
			"height": 2009.3332417805989,
			"seed": 1120813291,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1686311159314,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					0,
					2009.3332417805989
				]
			]
		},
		{
			"type": "text",
			"version": 32,
			"versionNonce": 471253555,
			"isDeleted": false,
			"id": "5iylbkuX",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2489.711167382242,
			"y": -486.2072556264469,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 362,
			"height": 50,
			"seed": 594371877,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159314,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "## 4. Median of Two Sorted Arrays\n",
			"rawText": "## 4. Median of Two Sorted Arrays\n",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "## 4. Median of Two Sorted Arrays\n",
			"lineHeight": 1.25,
			"baseline": 42
		},
		{
			"type": "text",
			"version": 75,
			"versionNonce": 1733553789,
			"isDeleted": false,
			"id": "r4cG85MX",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2514.225952464672,
			"y": -429.43139624336715,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 50,
			"height": 25,
			"seed": 2137077741,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159314,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "INFO",
			"rawText": "INFO",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "INFO",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 391,
			"versionNonce": 1527120851,
			"isDeleted": false,
			"id": "a2b23STU",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2550.767292280491,
			"y": -390.04391612603416,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 585,
			"height": 175,
			"seed": 1761281763,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159314,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "- two sorted arrays size <= 1000\n    - nums1: int[] size m\n    - nums2: int[] size n\n- get the median of the two arrays\n- time complexity has to be O (log (n+m))\n\n > double findMedianSortedArrays(int[] nums1, int[] nums2 <",
			"rawText": "- two sorted arrays size <= 1000\n    - nums1: int[] size m\n    - nums2: int[] size n\n- get the median of the two arrays\n- time complexity has to be O (log (n+m))\n\n > double findMedianSortedArrays(int[] nums1, int[] nums2 <",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "- two sorted arrays size <= 1000\n    - nums1: int[] size m\n    - nums2: int[] size n\n- get the median of the two arrays\n- time complexity has to be O (log (n+m))\n\n > double findMedianSortedArrays(int[] nums1, int[] nums2 <",
			"lineHeight": 1.25,
			"baseline": 167
		},
		{
			"type": "text",
			"version": 211,
			"versionNonce": 1126897373,
			"isDeleted": false,
			"id": "zFhOJ4IL",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2499.261141241068,
			"y": -172.55468653772198,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 91,
			"height": 25,
			"seed": 909549667,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159315,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "EXAMPLE",
			"rawText": "EXAMPLE",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "EXAMPLE",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 80,
			"versionNonce": 702288243,
			"isDeleted": false,
			"id": "1DmY6bW3",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2539.2766769529444,
			"y": -122.96936629267458,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 515,
			"height": 75,
			"seed": 1791064227,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159315,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Input: nums1 = [1,3], nums2 = [2]\nOutput: 2.00000\nExplanation: merged array = [1,2,3] and median is 2.",
			"rawText": "Input: nums1 = [1,3], nums2 = [2]\nOutput: 2.00000\nExplanation: merged array = [1,2,3] and median is 2.",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Input: nums1 = [1,3], nums2 = [2]\nOutput: 2.00000\nExplanation: merged array = [1,2,3] and median is 2.",
			"lineHeight": 1.25,
			"baseline": 67
		},
		{
			"type": "text",
			"version": 103,
			"versionNonce": 2126394173,
			"isDeleted": false,
			"id": "WD8Nvqq3",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2696.838910569709,
			"y": -1.929770737788317,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 81,
			"height": 25,
			"seed": 1650177475,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159315,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "nums1 = ",
			"rawText": "nums1 = ",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "nums1 = ",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 105,
			"versionNonce": 2044685075,
			"isDeleted": false,
			"id": "yerdBEBp",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2696.838910569709,
			"y": 53.088230489318846,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 90,
			"height": 25,
			"seed": 1478600653,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159315,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "nums2 = ",
			"rawText": "nums2 = ",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "nums2 = ",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "freedraw",
			"version": 114,
			"versionNonce": 644793245,
			"isDeleted": false,
			"id": "Ol2HaD5j_eGiRocOvsZiC",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2793.7642618253294,
			"y": 1.3479188546710361,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 5.61884541029076,
			"height": 30.43549004052744,
			"seed": 332835341,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159315,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					-0.9364980508803455
				],
				[
					0.9364623271326309,
					-2.3411915415790077
				],
				[
					1.872924654264807,
					-3.745920756025612
				],
				[
					3.2776538687116954,
					-6.0871122976046195
				],
				[
					5.150614246724217,
					-9.364766166316144
				],
				[
					5.61884541029076,
					-10.30126421719649
				],
				[
					5.61884541029076,
					-9.364766166316144
				],
				[
					5.61884541029076,
					-5.150649970472159
				],
				[
					5.150614246724217,
					3.7458850322777266
				],
				[
					4.682383083158129,
					9.364766166316144
				],
				[
					3.7458850322777835,
					13.578882362160073
				],
				[
					2.3411915415790645,
					16.856571954619426
				],
				[
					1.404693490698719,
					19.19776349619849
				],
				[
					0.9364623271326309,
					19.665994659764692
				],
				[
					0.9364623271326309,
					20.13422582333095
				],
				[
					0.9364623271326309,
					19.665994659764692
				],
				[
					0.46823116356608807,
					19.19776349619849
				],
				[
					0.46823116356608807,
					19.19776349619849
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2255859375,
				0.24609375,
				0.341796875,
				0.400390625,
				0.4306640625,
				0.4482421875,
				0.4560546875,
				0.498046875,
				0.498046875,
				0.49609375,
				0.49609375,
				0.49609375,
				0.5029296875,
				0.517578125,
				0.5244140625,
				0.529296875,
				0.296875,
				0.072265625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 103,
			"versionNonce": 1334218931,
			"isDeleted": false,
			"id": "eq37QPSjRSNpU9rMKvInD",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2827.009174571002,
			"y": 11.64914734811964,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 7.960072675617084,
			"height": 9.832997329882346,
			"seed": 1852960205,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159315,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.46823116356608807,
					0
				],
				[
					-1.8729603780125217,
					1.4047292144465473
				],
				[
					-4.682383083158129,
					4.214151919591814
				],
				[
					-6.555343461170651,
					6.555343461170821
				],
				[
					-7.960072675617084,
					8.428303839183627
				],
				[
					-7.960072675617084,
					9.832997329882346
				],
				[
					-7.960072675617084,
					9.832997329882346
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.234375,
				0.2802734375,
				0.4326171875,
				0.4775390625,
				0.490234375,
				0.4931640625,
				0.439453125,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 122,
			"versionNonce": 1047414781,
			"isDeleted": false,
			"id": "_5yyXN1QG0gBr0I3pxfTe",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2839.6515946060294,
			"y": 14.926801216831109,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 14.983611576606563,
			"height": 23.411915415790304,
			"seed": 2105804803,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159315,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					0.46826688731408694
				],
				[
					0.9364980508808003,
					0.46826688731408694
				],
				[
					2.8094227051456073,
					0.9364980508803455
				],
				[
					6.087112297605017,
					0.46826688731408694
				],
				[
					9.364766166316258,
					0
				],
				[
					11.705957707895323,
					-0.9364623271324604
				],
				[
					13.110686922342211,
					-1.8729246542649207
				],
				[
					13.578918085908299,
					-3.277653868711468
				],
				[
					12.642455758775668,
					-4.214116195843928
				],
				[
					11.237726544329234,
					-5.150614246724274
				],
				[
					10.301264217196604,
					-6.087076573856734
				],
				[
					10.301264217196604,
					-7.96003695186954
				],
				[
					11.237726544329234,
					-10.769459657014806
				],
				[
					12.642455758775668,
					-12.17418887146141
				],
				[
					14.047149249474387,
					-13.578882362160073
				],
				[
					14.515380413040475,
					-14.98361157660662
				],
				[
					14.515380413040475,
					-15.92007390373908
				],
				[
					14.047149249474387,
					-16.388340791053224
				],
				[
					12.642455758775668,
					-17.793034281751886
				],
				[
					11.237726544329234,
					-19.19776349619849
				],
				[
					8.428303839184082,
					-20.602456986897153
				],
				[
					3.745920756025953,
					-22.007186201343757
				],
				[
					1.4047292144468884,
					-22.47541736490996
				],
				[
					0.4682311635665428,
					-22.007186201343757
				],
				[
					-0.46823116356608807,
					-21.070723874211296
				],
				[
					-0.46823116356608807,
					-21.070723874211296
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.181640625,
				0.4931640625,
				0.4951171875,
				0.4970703125,
				0.4990234375,
				0.49609375,
				0.49609375,
				0.49609375,
				0.49609375,
				0.49609375,
				0.4990234375,
				0.49609375,
				0.5048828125,
				0.501953125,
				0.5,
				0.498046875,
				0.498046875,
				0.5,
				0.5234375,
				0.5419921875,
				0.5498046875,
				0.5537109375,
				0.55078125,
				0.5234375,
				0.4287109375,
				0.1298828125,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 120,
			"versionNonce": 1551368787,
			"isDeleted": false,
			"id": "PrfNiuMpPA8PSvR2pNykr",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2816.707910353806,
			"y": 68.30597550958254,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 15.920073903739194,
			"height": 24.34841346667065,
			"seed": 1104459459,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159315,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.4682311635665428,
					0.4682311635662586
				],
				[
					-0.9364623271326309,
					0.9364980508803455
				],
				[
					-3.7458850322777835,
					1.4047292144466041
				],
				[
					-5.150614246724217,
					1.4047292144466041
				],
				[
					-6.555307737423391,
					0.4682311635662586
				],
				[
					-7.0235746247371935,
					-1.4046934906986621
				],
				[
					-6.087076573856848,
					-5.150614246724274
				],
				[
					-5.150614246724217,
					-7.02357462473708
				],
				[
					-3.7458850322777835,
					-8.896535002749886
				],
				[
					-2.3411915415790645,
					-9.832997329882346
				],
				[
					-0.9364623271326309,
					-11.237726544328893
				],
				[
					-0.4682311635665428,
					-12.174188871461354
				],
				[
					-0.4682311635665428,
					-12.642420035027556
				],
				[
					-0.9364623271326309,
					-13.578918085907901
				],
				[
					-2.3411915415790645,
					-14.04714924947416
				],
				[
					-4.682383083158129,
					-15.451842740172822
				],
				[
					-6.087076573856848,
					-16.388340791053167
				],
				[
					-8.428268115435912,
					-17.324803118185628
				],
				[
					-12.642420035027953,
					-19.665994659764692
				],
				[
					-14.983611576606563,
					-21.07072387421124
				],
				[
					-15.920073903739194,
					-22.47541736490996
				],
				[
					-15.920073903739194,
					-22.943684252224045
				],
				[
					-15.920073903739194,
					-22.0071862013437
				],
				[
					-15.920073903739194,
					-22.0071862013437
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.1923828125,
				0.357421875,
				0.4072265625,
				0.49609375,
				0.51953125,
				0.5322265625,
				0.53515625,
				0.521484375,
				0.5126953125,
				0.5068359375,
				0.49609375,
				0.4990234375,
				0.4990234375,
				0.4990234375,
				0.5107421875,
				0.5400390625,
				0.5556640625,
				0.56640625,
				0.57421875,
				0.580078125,
				0.58203125,
				0.5693359375,
				0.564453125,
				0.0146484375,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 93,
			"versionNonce": 1220427869,
			"isDeleted": false,
			"id": "sggysTZu1oLbpJHYOS4iP",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2864.468239236268,
			"y": -18.78634269240797,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 43.07791007555534,
			"height": 63.680402786200034,
			"seed": 1138454819,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159315,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					-0.46823116356620176
				],
				[
					0,
					-0.9364623271324604
				],
				[
					0,
					-1.4046934906986621
				],
				[
					0.9364623271326309,
					-2.3411915415790077
				],
				[
					2.3411915415790645,
					-3.7458850322777266
				],
				[
					4.2141161958438715,
					-4.214116195843928
				],
				[
					6.555307737422936,
					-4.214116195843928
				],
				[
					9.364766166316258,
					-3.277653868711468
				],
				[
					15.451842740173106,
					0.4682668873141438
				],
				[
					18.729532332632516,
					3.745920756025612
				],
				[
					21.07072387421158,
					7.02357462473708
				],
				[
					22.007186201343757,
					10.769495380762692
				],
				[
					22.007186201343757,
					24.816644630236908
				],
				[
					20.13422582333078,
					32.30845041854019
				],
				[
					19.665994659764692,
					35.117873123685456
				],
				[
					17.79303428175217,
					40.736754257723874
				],
				[
					15.920073903739194,
					44.95090617731569
				],
				[
					15.451842740173106,
					47.76032888246095
				],
				[
					17.324803118185628,
					50.56975158760622
				],
				[
					19.665994659764692,
					51.97448080205277
				],
				[
					21.53895503777767,
					52.91094312918523
				],
				[
					25.284840070055452,
					55.25213467076429
				],
				[
					27.626031611634517,
					56.65686388521084
				],
				[
					30.435490040527384,
					57.1250950487771
				],
				[
					34.649606236371255,
					56.65686388521084
				],
				[
					38.39552699239721,
					56.18859699789675
				],
				[
					41.20494969754236,
					55.720365834330494
				],
				[
					42.609678911988794,
					56.65686388521084
				],
				[
					43.07791007555534,
					59.466286590356106
				],
				[
					43.07791007555534,
					59.466286590356106
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.1923828125,
				0.28515625,
				0.310546875,
				0.3369140625,
				0.38671875,
				0.3994140625,
				0.3994140625,
				0.3955078125,
				0.3935546875,
				0.3935546875,
				0.3935546875,
				0.3935546875,
				0.3935546875,
				0.3876953125,
				0.396484375,
				0.396484375,
				0.3984375,
				0.41796875,
				0.4365234375,
				0.4541015625,
				0.458984375,
				0.46484375,
				0.470703125,
				0.470703125,
				0.4765625,
				0.478515625,
				0.48046875,
				0.4306640625,
				0.2587890625,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 91,
			"versionNonce": 1502232563,
			"isDeleted": false,
			"id": "MVPWVAA1F3M3J--5iW849",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2855.571704233518,
			"y": 74.86131897075325,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 49.63325353672599,
			"height": 38.86379387971101,
			"seed": 1002654499,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159315,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.9364623271321761,
					0.4682668873141438
				],
				[
					2.8094227051451526,
					1.4047292144465473
				],
				[
					5.150614246724217,
					2.8094584288931514
				],
				[
					7.491805788303282,
					3.277689592459353
				],
				[
					10.769459657014522,
					2.3411915415790077
				],
				[
					14.515380413040475,
					0.4682668873141438
				],
				[
					17.324803118185628,
					-1.4046934906986621
				],
				[
					20.13422582333078,
					-2.8094227051452663
				],
				[
					23.88014657935628,
					-4.682383083158072
				],
				[
					25.284875793803167,
					-6.555307737422993
				],
				[
					25.753106957369255,
					-8.428268115435799
				],
				[
					25.284875793803167,
					-10.301228493448548
				],
				[
					23.88014657935628,
					-12.174188871461354
				],
				[
					22.475417364909845,
					-15.451842740172879
				],
				[
					21.538955037777214,
					-18.261265445318145
				],
				[
					21.538955037777214,
					-20.602456986897153
				],
				[
					22.475417364909845,
					-22.47541736490996
				],
				[
					26.221338120935343,
					-25.284840070055225
				],
				[
					28.09429849894832,
					-27.15780044806803
				],
				[
					30.435490040527384,
					-29.49899198964704
				],
				[
					33.244912745672536,
					-30.903721204093642
				],
				[
					36.05433545081769,
					-32.77668158210639
				],
				[
					40.73671853397582,
					-35.117873123685456
				],
				[
					43.07791007555488,
					-35.117873123685456
				],
				[
					45.887332780700035,
					-35.58610428725166
				],
				[
					48.2285243222791,
					-35.117873123685456
				],
				[
					49.63325353672599,
					-32.77668158210639
				],
				[
					49.63325353672599,
					-32.77668158210639
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.212890625,
				0.3212890625,
				0.3681640625,
				0.390625,
				0.4052734375,
				0.4150390625,
				0.4208984375,
				0.4248046875,
				0.4267578125,
				0.4267578125,
				0.4345703125,
				0.4384765625,
				0.44140625,
				0.4501953125,
				0.455078125,
				0.466796875,
				0.478515625,
				0.4873046875,
				0.4951171875,
				0.4970703125,
				0.4970703125,
				0.4970703125,
				0.4970703125,
				0.4990234375,
				0.4990234375,
				0.44921875,
				0.2177734375,
				0.0126953125,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 74,
			"versionNonce": 187706557,
			"isDeleted": false,
			"id": "EalT4cA3kIy3lBe_oW-6-",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2937.98163935235,
			"y": 49.108212013383934,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 2.8094227051456073,
			"height": 36.522566614384175,
			"seed": 908447107,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159315,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					-2.8094227051452663
				],
				[
					0,
					-7.491805788303338
				],
				[
					0.4682311635665428,
					-10.301228493448605
				],
				[
					1.4047292144468884,
					-15.920073903739137
				],
				[
					2.3411915415790645,
					-21.538955037777498
				],
				[
					2.8094227051456073,
					-29.49899198964704
				],
				[
					2.3411915415790645,
					-34.64960623637137
				],
				[
					1.4047292144468884,
					-36.522566614384175
				],
				[
					0.9364623271326309,
					-34.18137507280511
				],
				[
					1.8729603780129764,
					-26.22133812093557
				],
				[
					1.8729603780129764,
					-26.22133812093557
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.212890625,
				0.3115234375,
				0.431640625,
				0.4794921875,
				0.525390625,
				0.5419921875,
				0.5439453125,
				0.5419921875,
				0.5322265625,
				0.34765625,
				0.0146484375,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 72,
			"versionNonce": 549702035,
			"isDeleted": false,
			"id": "AigP_W4XK9kyTFDtJm3WK",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2956.2429405214166,
			"y": 44.42582893022586,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 8.89653500275017,
			"height": 16.85660767836731,
			"seed": 1501117037,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159315,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.9364623271326309,
					1.4047292144465473
				],
				[
					-2.809458428893322,
					4.214151919591814
				],
				[
					-4.214151919592041,
					5.618881134038418
				],
				[
					-6.087112297605017,
					8.896535002749886
				],
				[
					-8.428303839184082,
					12.642455758775498
				],
				[
					-8.89653500275017,
					15.451878463920764
				],
				[
					-8.428303839184082,
					16.85660767836731
				],
				[
					-7.0235746247371935,
					16.85660767836731
				],
				[
					-7.0235746247371935,
					16.85660767836731
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2392578125,
				0.2861328125,
				0.37890625,
				0.408203125,
				0.4453125,
				0.4541015625,
				0.462890625,
				0.2626953125,
				0.0224609375,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 87,
			"versionNonce": 358976797,
			"isDeleted": false,
			"id": "ltxLhVufCTgvog-gPmOa6",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2993.233738299367,
			"y": 42.084637388646854,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 17.793070005499885,
			"height": 29.030796549828665,
			"seed": 493289731,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159315,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-1.8729246542652618,
					0.46826688731408694
				],
				[
					-2.809386981397438,
					0.46826688731408694
				],
				[
					-4.682383083158129,
					0.9364980508802887
				],
				[
					-6.555307737423391,
					0.46826688731408694
				],
				[
					-7.960036951869824,
					-0.9364623271324604
				],
				[
					-8.428232391688198,
					-2.8094227051452663
				],
				[
					-7.491770064555567,
					-5.150614246724331
				],
				[
					-6.087040850109133,
					-7.023574624737137
				],
				[
					-4.214116195844326,
					-8.896499279002057
				],
				[
					-1.8729246542652618,
					-10.301228493448605
				],
				[
					-0.4681954398183734,
					-11.705957707895152
				],
				[
					0.4682668873138027,
					-13.110651198593871
				],
				[
					0.9365337746280602,
					-14.515380413040418
				],
				[
					0.4682668873138027,
					-15.920073903739137
				],
				[
					-0.9364623271326309,
					-17.324803118185685
				],
				[
					-3.2776538687116954,
					-18.72953233263229
				],
				[
					-6.087040850109133,
					-21.070723874211296
				],
				[
					-11.237690820581065,
					-24.816608906489023
				],
				[
					-14.51534468929276,
					-26.68956928450183
				],
				[
					-16.38834079105345,
					-27.62603161163429
				],
				[
					-16.856536230871825,
					-27.62603161163429
				],
				[
					-15.920073903739194,
					-28.094298498948376
				],
				[
					-11.237690820581065,
					-26.68956928450183
				],
				[
					-11.237690820581065,
					-26.68956928450183
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.234375,
				0.3330078125,
				0.37890625,
				0.4443359375,
				0.48828125,
				0.5087890625,
				0.51171875,
				0.5087890625,
				0.498046875,
				0.47265625,
				0.453125,
				0.4423828125,
				0.4423828125,
				0.4521484375,
				0.4794921875,
				0.50390625,
				0.5224609375,
				0.5361328125,
				0.5478515625,
				0.5498046875,
				0.5498046875,
				0.5498046875,
				0.3212890625,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 73,
			"versionNonce": 123412275,
			"isDeleted": false,
			"id": "ZgJLvEQEMCTsAWrpy_5uj",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3012.899804406627,
			"y": 41.148175061514394,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 8.428303839183627,
			"height": 23.411915415790304,
			"seed": 641428515,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159315,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-1.4047292144464336,
					3.277653868711468
				],
				[
					-2.3411915415790645,
					4.682383083158015
				],
				[
					-3.2777253162071247,
					6.0871122976046195
				],
				[
					-5.150649970471932,
					9.364766166316087
				],
				[
					-7.023574624736739,
					13.1106869223417
				],
				[
					-8.428303839183627,
					17.79307000549977
				],
				[
					-8.428303839183627,
					21.538955037777498
				],
				[
					-7.023574624736739,
					23.411915415790304
				],
				[
					-3.745920756025498,
					22.0071862013437
				],
				[
					-3.745920756025498,
					22.0071862013437
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2412109375,
				0.333984375,
				0.3779296875,
				0.4140625,
				0.4599609375,
				0.474609375,
				0.474609375,
				0.4296875,
				0.2529296875,
				0.0126953125,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 89,
			"versionNonce": 114286973,
			"isDeleted": false,
			"id": "S3A5u3zQJ1Guu6fomETjm",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3028.819878310366,
			"y": 39.27521468350159,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 19.665994659764692,
			"height": 34.18137507280511,
			"seed": 872592867,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159315,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.9364623271326309,
					0.46823116356620176
				],
				[
					2.3411915415790645,
					0
				],
				[
					5.1506499704723865,
					-0.4682311635662586
				],
				[
					7.491841512051451,
					-1.872960378012806
				],
				[
					10.301228493448889,
					-3.7458850322777266
				],
				[
					13.57888236216013,
					-5.150614246724331
				],
				[
					14.983611576606563,
					-6.555343461170878
				],
				[
					14.047149249474387,
					-7.96003695186954
				],
				[
					11.705957707895323,
					-9.364766166316144
				],
				[
					9.833033053630515,
					-10.301228493448605
				],
				[
					8.896499279002,
					-11.23772654432895
				],
				[
					9.833033053630515,
					-14.047149249474217
				],
				[
					12.642420035027953,
					-15.920109627487022
				],
				[
					16.38834079105345,
					-17.793034281751943
				],
				[
					18.72953233263206,
					-20.13422582333095
				],
				[
					19.665994659764692,
					-22.007186201343757
				],
				[
					19.19779921994632,
					-24.348377742922764
				],
				[
					17.793070005499885,
					-25.75310695736937
				],
				[
					14.515416136788645,
					-27.626067335382174
				],
				[
					11.237690820581065,
					-29.49899198964704
				],
				[
					7.960036951869824,
					-31.371952367659844
				],
				[
					5.1506499704723865,
					-33.71314390923891
				],
				[
					4.2141161958438715,
					-33.71314390923891
				],
				[
					3.745920756025498,
					-33.71314390923891
				],
				[
					3.2776538687116954,
					-32.30845041854019
				],
				[
					3.2776538687116954,
					-32.30845041854019
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2255859375,
				0.44921875,
				0.451171875,
				0.45703125,
				0.45703125,
				0.45703125,
				0.45703125,
				0.4521484375,
				0.4599609375,
				0.482421875,
				0.5,
				0.515625,
				0.5234375,
				0.5146484375,
				0.4990234375,
				0.4765625,
				0.470703125,
				0.486328125,
				0.5166015625,
				0.5380859375,
				0.548828125,
				0.548828125,
				0.54296875,
				0.5185546875,
				0.427734375,
				0.1298828125,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 75,
			"versionNonce": 2008465619,
			"isDeleted": false,
			"id": "CzMdXLHDCdRttFfSWed_z",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2972.1630144251553,
			"y": -36.57937697415986,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 3.745920756025953,
			"height": 20.13422582333095,
			"seed": 1914936483,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159315,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					1.404693490698719
				],
				[
					0,
					1.872960378012806
				],
				[
					0.4682668873142575,
					6.087076573856734
				],
				[
					1.4047292144468884,
					8.896535002749886
				],
				[
					1.872996101760691,
					11.23772654432895
				],
				[
					2.3411915415790645,
					13.578918085907958
				],
				[
					2.809458428893322,
					15.920109627486966
				],
				[
					2.809458428893322,
					18.26130116906603
				],
				[
					2.809458428893322,
					19.665994659764692
				],
				[
					3.2777253162075795,
					20.13422582333095
				],
				[
					3.745920756025953,
					20.13422582333095
				],
				[
					3.745920756025953,
					20.13422582333095
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2275390625,
				0.2744140625,
				0.28125,
				0.3642578125,
				0.37890625,
				0.3896484375,
				0.39453125,
				0.40625,
				0.412109375,
				0.4150390625,
				0.361328125,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 84,
			"versionNonce": 347122141,
			"isDeleted": false,
			"id": "rKxRsjnmD9eSWSehNLDZ1",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2968.4171651166257,
			"y": -21.595765397553237,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 19.665994659764692,
			"height": 21.070723874211296,
			"seed": 1597227523,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159315,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					0.4682311635662586
				],
				[
					0,
					1.4047292144466041
				],
				[
					0,
					3.745920756025612
				],
				[
					0.4681954398183734,
					6.087112297604676
				],
				[
					1.4046577669505496,
					10.769495380762692
				],
				[
					2.3411915415790645,
					13.110686922341756
				],
				[
					2.809386981397438,
					14.047149249474217
				],
				[
					3.745849308529614,
					14.983647300354562
				],
				[
					4.682383083158129,
					14.983647300354562
				],
				[
					6.087040850108679,
					14.047149249474217
				],
				[
					7.0235746247371935,
					12.642455758775498
				],
				[
					9.364766166316258,
					10.30126421719649
				],
				[
					12.174153147713696,
					7.023574624737137
				],
				[
					14.983611576606563,
					3.27768959245941
				],
				[
					17.324803118185628,
					-2.8094227051452094
				],
				[
					17.792998558004,
					-4.682383083158015
				],
				[
					17.792998558004,
					-5.618845410290476
				],
				[
					18.261265445317804,
					-6.087076573856734
				],
				[
					18.72953233263206,
					-6.087076573856734
				],
				[
					19.665994659764692,
					-5.618845410290476
				],
				[
					19.665994659764692,
					-5.618845410290476
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2158203125,
				0.248046875,
				0.271484375,
				0.3291015625,
				0.373046875,
				0.3955078125,
				0.3974609375,
				0.3974609375,
				0.3974609375,
				0.4013671875,
				0.4228515625,
				0.4287109375,
				0.4365234375,
				0.4404296875,
				0.44921875,
				0.45703125,
				0.4560546875,
				0.4482421875,
				0.4443359375,
				0.263671875,
				0.013671875,
				0
			]
		},
		{
			"type": "text",
			"version": 95,
			"versionNonce": 1265446515,
			"isDeleted": false,
			"id": "Fq6dwvk2",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2541.617832770775,
			"y": 115.83218881026019,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 702,
			"height": 75,
			"seed": 2060458029,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159316,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Input: nums1 = [1,2], nums2 = [3,4]\nOutput: 2.50000\nExplanation: merged array = [1,2,3,4] and median is (2 + 3) / 2 = 2.5.",
			"rawText": "Input: nums1 = [1,2], nums2 = [3,4]\nOutput: 2.50000\nExplanation: merged array = [1,2,3,4] and median is (2 + 3) / 2 = 2.5.",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Input: nums1 = [1,2], nums2 = [3,4]\nOutput: 2.50000\nExplanation: merged array = [1,2,3,4] and median is (2 + 3) / 2 = 2.5.",
			"lineHeight": 1.25,
			"baseline": 67
		},
		{
			"type": "text",
			"version": 36,
			"versionNonce": 1343841853,
			"isDeleted": false,
			"id": "9dS3OjAn",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2674.5975552009622,
			"y": 254.8989520905554,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 81,
			"height": 25,
			"seed": 2074816643,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159316,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "nums1 = ",
			"rawText": "nums1 = ",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "nums1 = ",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 55,
			"versionNonce": 1699014675,
			"isDeleted": false,
			"id": "gxNuMUtL",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2668.7445763470146,
			"y": 304.0639744637151,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 90,
			"height": 25,
			"seed": 44658957,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159316,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "nums2 = ",
			"rawText": "nums2 = ",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "nums2 = ",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "freedraw",
			"version": 49,
			"versionNonce": 736859805,
			"isDeleted": false,
			"id": "WCYLvUTiKOHS8rCuEUDiJ",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2769.884043798479,
			"y": 255.60131669777874,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 9.364766166316258,
			"height": 32.30845041854016,
			"seed": 1732925603,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159316,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					-0.4682311635662586
				],
				[
					1.4047292144464336,
					-2.8094227051452663
				],
				[
					4.682383083158129,
					-7.491805788303338
				],
				[
					7.0235746247371935,
					-10.769495380762748
				],
				[
					8.428303839183627,
					-12.642420035027612
				],
				[
					8.896535002749715,
					-13.578918085907958
				],
				[
					9.364766166316258,
					-12.17418887146141
				],
				[
					9.364766166316258,
					-8.896535002749943
				],
				[
					8.896535002749715,
					-5.150614246724331
				],
				[
					8.896535002749715,
					-0.4682311635662586
				],
				[
					8.428303839183627,
					3.7459207560255265
				],
				[
					7.960072675617539,
					8.428303839183656
				],
				[
					7.491841512050996,
					10.76949538076272
				],
				[
					7.0235746247371935,
					12.642420035027527
				],
				[
					6.555343461170651,
					14.983611576606592
				],
				[
					6.555343461170651,
					15.451878463920735
				],
				[
					6.555343461170651,
					15.920109627486937
				],
				[
					6.555343461170651,
					17.324803118185656
				],
				[
					6.555343461170651,
					18.729532332632203
				],
				[
					6.555343461170651,
					18.729532332632203
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.212890625,
				0.4814453125,
				0.505859375,
				0.509765625,
				0.5078125,
				0.501953125,
				0.501953125,
				0.50390625,
				0.51171875,
				0.51171875,
				0.51171875,
				0.521484375,
				0.53125,
				0.5400390625,
				0.5458984375,
				0.54296875,
				0.54296875,
				0.54296875,
				0.3662109375,
				0.015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 48,
			"versionNonce": 187985331,
			"isDeleted": false,
			"id": "pFwGIIc70Yek7yP3Nd0ef",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2833.5644823084267,
			"y": 264.0296205369624,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 13.578918085907844,
			"height": 23.411915415790276,
			"seed": 315712643,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159316,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.4682668873138027,
					0
				],
				[
					-2.3411915415786098,
					0.46823116356620176
				],
				[
					-5.150649970471932,
					0.46823116356620176
				],
				[
					-8.896535002749715,
					0
				],
				[
					-11.23772654432878,
					-0.4682668873141438
				],
				[
					-11.705957707894868,
					-1.8729603780128627
				],
				[
					-11.705957707894868,
					-2.8094584288932083
				],
				[
					-10.301264217196149,
					-5.150649970472159
				],
				[
					-7.960072675617084,
					-7.02357462473708
				],
				[
					-4.214151919591586,
					-9.364766166316116
				],
				[
					0.4682311635665428,
					-14.047149249474188
				],
				[
					0.4682311635665428,
					-14.983647300354534
				],
				[
					-0.4682668873138027,
					-16.388340791053253
				],
				[
					-3.2776895924589553,
					-17.324838841933598
				],
				[
					-7.491841512050996,
					-19.197799219946404
				],
				[
					-12.642455758775213,
					-22.475453088657872
				],
				[
					-13.110686922341301,
					-22.943684252224074
				],
				[
					-13.110686922341301,
					-22.007221925091613
				],
				[
					-13.110686922341301,
					-22.007221925091613
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.17578125,
				0.1943359375,
				0.23828125,
				0.3330078125,
				0.4365234375,
				0.5,
				0.513671875,
				0.521484375,
				0.5126953125,
				0.5009765625,
				0.4658203125,
				0.4296875,
				0.44140625,
				0.466796875,
				0.5,
				0.5166015625,
				0.5244140625,
				0.5244140625,
				0.0166015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 38,
			"versionNonce": 1121499901,
			"isDeleted": false,
			"id": "whyl5tPB6m7IUH9f1F7bR",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2805.938414973045,
			"y": 263.56135364964825,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 6.5553434611711054,
			"height": 19.66603038351252,
			"seed": 1156068589,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159316,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					-0.46823116356620176
				],
				[
					-0.46823116356608807,
					0.4682668873141438
				],
				[
					-1.4047292144468884,
					2.8094584288932083
				],
				[
					-3.27768959245941,
					6.555343461170878
				],
				[
					-4.214151919592041,
					8.428303839183627
				],
				[
					-5.150614246724217,
					13.110686922341756
				],
				[
					-6.087112297604563,
					16.388340791053224
				],
				[
					-6.5553434611711054,
					19.19779921994632
				],
				[
					-6.5553434611711054,
					19.19779921994632
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2412109375,
				0.2900390625,
				0.39453125,
				0.46484375,
				0.4921875,
				0.4951171875,
				0.466796875,
				0.2861328125,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 51,
			"versionNonce": 6438739,
			"isDeleted": false,
			"id": "f8qkxeAo962k0ttTqBQOG",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2768.4793503077804,
			"y": 321.62291102555776,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 15.45187846392082,
			"height": 24.348377742922708,
			"seed": 381058691,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159316,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.46823116356608807,
					0
				],
				[
					-0.9364980508803455,
					0
				],
				[
					-0.9364980508803455,
					0.9364623271324035
				],
				[
					0.46823116356608807,
					1.872996101760691
				],
				[
					2.8094227051451526,
					2.3411915415790645
				],
				[
					5.150614246724217,
					1.872996101760691
				],
				[
					8.428268115435912,
					0.9364623271324035
				],
				[
					12.642420035027499,
					-0.9364623271324035
				],
				[
					14.047149249473932,
					-1.8729246542649207
				],
				[
					14.515380413040475,
					-2.8093869813973242
				],
				[
					13.578918085907844,
					-3.745920756025612
				],
				[
					12.17418887146141,
					-5.6188454102905325
				],
				[
					11.23772654432878,
					-7.491770064555453
				],
				[
					11.705957707895323,
					-9.832961606134404
				],
				[
					12.642420035027499,
					-12.642420035027612
				],
				[
					12.642420035027499,
					-14.04714924947416
				],
				[
					10.769459657014977,
					-16.856536230871598
				],
				[
					9.364766166316258,
					-17.79307000549977
				],
				[
					5.150614246724217,
					-22.007186201343643
				],
				[
					5.150614246724217,
					-21.07072387421124
				],
				[
					7.0235746247371935,
					-19.19772777245055
				],
				[
					7.0235746247371935,
					-19.19772777245055
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.232421875,
				0.2529296875,
				0.35546875,
				0.4794921875,
				0.49609375,
				0.51171875,
				0.5146484375,
				0.517578125,
				0.5146484375,
				0.509765625,
				0.5048828125,
				0.498046875,
				0.498046875,
				0.49609375,
				0.5,
				0.4970703125,
				0.4970703125,
				0.5078125,
				0.529296875,
				0.5400390625,
				0.4169921875,
				0.015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 37,
			"versionNonce": 1566724957,
			"isDeleted": false,
			"id": "lDws9-Wq5IKGsjWE0DvEG",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2800.3195338390065,
			"y": 318.3452571568463,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 8.428268115435912,
			"height": 24.348377742922708,
			"seed": 1133916675,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159316,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.9364623271326309,
					2.3411915415790645
				],
				[
					-1.872924654264807,
					3.745920756025612
				],
				[
					-4.682383083158129,
					7.491841512051224
				],
				[
					-7.960036951869824,
					14.04714924947416
				],
				[
					-8.428268115435912,
					16.388340791053224
				],
				[
					-8.428268115435912,
					20.602456986897096
				],
				[
					-7.0235746247371935,
					24.348377742922708
				],
				[
					-7.0235746247371935,
					24.348377742922708
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.353515625,
				0.4052734375,
				0.4375,
				0.4765625,
				0.49609375,
				0.49609375,
				0.4287109375,
				0.015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 39,
			"versionNonce": 1596251379,
			"isDeleted": false,
			"id": "7Ji-HqAGUmuyiOjaD_POR",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2834.969175799126,
			"y": 325.8370986688975,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 4.214151919592041,
			"height": 22.007257648839527,
			"seed": 2034733091,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159316,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.4682311635665428,
					-0.4682668873141438
				],
				[
					-0.4682311635665428,
					-1.404729214446661
				],
				[
					0,
					-3.277725316207352
				],
				[
					0.46823116356608807,
					-6.55537918491882
				],
				[
					0.9364980508798908,
					-10.769495380762692
				],
				[
					1.8729603780125217,
					-15.45187846392082
				],
				[
					2.3411915415786098,
					-18.72953233263229
				],
				[
					3.2776895924589553,
					-21.070723874211353
				],
				[
					3.745920756025498,
					-22.007257648839527
				],
				[
					3.745920756025498,
					-22.007257648839527
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2158203125,
				0.2607421875,
				0.423828125,
				0.486328125,
				0.5087890625,
				0.51171875,
				0.517578125,
				0.4658203125,
				0.244140625,
				0.0556640625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 39,
			"versionNonce": 937025469,
			"isDeleted": false,
			"id": "tum13p4kaxVNj11rUZhx-",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2834.969175799126,
			"y": 313.66287407368816,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 15.451842740173106,
			"height": 16.856571954619426,
			"seed": 1084479971,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159316,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-3.7458850322777835,
					0.9364623271325172
				],
				[
					-7.960036951869824,
					0.4682668873141438
				],
				[
					-10.769459657014977,
					-0.4682668873140301
				],
				[
					-14.047149249474387,
					-4.682383083158015
				],
				[
					-14.983611576607018,
					-7.49184151205111
				],
				[
					-15.451842740173106,
					-11.237690820580951
				],
				[
					-15.451842740173106,
					-14.047149249474046
				],
				[
					-14.983611576607018,
					-15.920109627486909
				],
				[
					-14.983611576607018,
					-14.047149249474046
				],
				[
					-14.983611576607018,
					-14.047149249474046
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.216796875,
				0.265625,
				0.380859375,
				0.4658203125,
				0.53125,
				0.5478515625,
				0.55078125,
				0.541015625,
				0.498046875,
				0.02734375,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 50,
			"versionNonce": 855819923,
			"isDeleted": false,
			"id": "IMn08VNsBb8nlxlu69BEd",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2841.9927504238626,
			"y": 234.0623616600012,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 55.25213467076446,
			"height": 59.934517753922336,
			"seed": 573428643,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159316,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.4682311635665428,
					-0.46823116356620176
				],
				[
					1.4047292144464336,
					-1.4047292144465473
				],
				[
					4.214151919592041,
					-1.872960378012749
				],
				[
					9.832997329882346,
					-3.277689592459353
				],
				[
					17.324838841933797,
					-3.277689592459353
				],
				[
					22.007221925091926,
					-0.9364980508802887
				],
				[
					26.6896050082496,
					2.8094227051452663
				],
				[
					30.435490040527384,
					6.555343461170878
				],
				[
					32.30845041854036,
					10.769459657014806
				],
				[
					33.244912745672536,
					19.66599465976475
				],
				[
					32.30845041854036,
					25.753106957369397
				],
				[
					29.499027713395208,
					31.37195236765993
				],
				[
					23.41191541579019,
					39.80025620684356
				],
				[
					19.66603038351286,
					49.6332535367259
				],
				[
					19.197763496198604,
					52.44267624187117
				],
				[
					23.880146579356733,
					55.720365834330465
				],
				[
					32.77668158210645,
					56.18859699789678
				],
				[
					41.204985421290075,
					56.65682816146298
				],
				[
					43.54617696286914,
					56.65682816146298
				],
				[
					55.25213467076446,
					55.720365834330465
				],
				[
					55.25213467076446,
					55.720365834330465
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2666015625,
				0.3076171875,
				0.3603515625,
				0.3837890625,
				0.392578125,
				0.3994140625,
				0.39453125,
				0.3876953125,
				0.3857421875,
				0.3857421875,
				0.390625,
				0.392578125,
				0.392578125,
				0.396484375,
				0.447265625,
				0.462890625,
				0.4765625,
				0.48046875,
				0.48046875,
				0.48046875,
				0.015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 49,
			"versionNonce": 140566557,
			"isDeleted": false,
			"id": "GXlMRyrVeXKW8uIDOYj0V",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2854.6352061826383,
			"y": 338.9477141437434,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 40.26848737040973,
			"height": 47.76032888246095,
			"seed": 1674063405,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159316,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.46823116356608807,
					0.4682668873141438
				],
				[
					2.3411915415790645,
					0.4682668873141438
				],
				[
					5.150614246724217,
					-1.404657766950777
				],
				[
					8.896499279002,
					-4.2141161958438715
				],
				[
					13.57888236216013,
					-7.49177006455534
				],
				[
					18.72953233263206,
					-11.237690820580951
				],
				[
					20.60245698689687,
					-14.04714924947416
				],
				[
					20.13422582333078,
					-16.388340791053224
				],
				[
					19.197763496198604,
					-18.729532332632175
				],
				[
					17.324803118185628,
					-22.007186201343643
				],
				[
					14.047149249473932,
					-28.09429849894832
				],
				[
					12.642420035027499,
					-30.435490040527384
				],
				[
					13.110651198593587,
					-32.308414694792305
				],
				[
					14.983611576606563,
					-34.181339349057225
				],
				[
					22.943648528475933,
					-39.33198931952927
				],
				[
					26.689569284501886,
					-42.14141202467454
				],
				[
					32.77668158210645,
					-46.355563944266464
				],
				[
					37.45906466526458,
					-47.29206199514681
				],
				[
					40.26848737040973,
					-40.26845164666179
				],
				[
					40.26848737040973,
					-40.26845164666179
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.234375,
				0.2744140625,
				0.2958984375,
				0.3154296875,
				0.3212890625,
				0.33203125,
				0.3623046875,
				0.3779296875,
				0.4013671875,
				0.4365234375,
				0.4736328125,
				0.494140625,
				0.4990234375,
				0.5087890625,
				0.517578125,
				0.51953125,
				0.51953125,
				0.5146484375,
				0.46484375,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 46,
			"versionNonce": 1387428915,
			"isDeleted": false,
			"id": "fuQwbliCtmM-j24sPEenM",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2923.4662232155624,
			"y": 283.6956151967271,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 12.17418887146141,
			"height": 42.609678911988794,
			"seed": 1394410573,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159316,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.4682311635665428,
					-0.46823116356620176
				],
				[
					0.4682311635665428,
					-1.8729603780128627
				],
				[
					1.8729603780129764,
					-5.150614246724331
				],
				[
					5.61884541029076,
					-10.301228493448548
				],
				[
					9.364766166316258,
					-14.983611576606677
				],
				[
					11.705957707895323,
					-18.72953233263229
				],
				[
					12.17418887146141,
					-17.324803118185628
				],
				[
					11.237726544329234,
					-9.364766166316144
				],
				[
					10.301228493448434,
					-2.8094227051452663
				],
				[
					8.89653500275017,
					2.8094227051452663
				],
				[
					6.087112297605017,
					13.110686922341756
				],
				[
					4.682383083158129,
					18.261301169065973
				],
				[
					4.214151919592041,
					21.53895503777744
				],
				[
					4.214151919592041,
					22.47541736490996
				],
				[
					4.214151919592041,
					23.880146579356506
				],
				[
					4.682383083158129,
					22.94368425222399
				],
				[
					4.682383083158129,
					22.94368425222399
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.310546875,
				0.3642578125,
				0.4130859375,
				0.4677734375,
				0.478515625,
				0.4736328125,
				0.4716796875,
				0.453125,
				0.4423828125,
				0.4423828125,
				0.458984375,
				0.49609375,
				0.5107421875,
				0.51953125,
				0.51953125,
				0.4365234375,
				0.0126953125,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 38,
			"versionNonce": 1156109437,
			"isDeleted": false,
			"id": "CXLFVglNNS65NM6-EXvK5",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2959.5205586663806,
			"y": 300.08399171152814,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 12.17418887146141,
			"height": 17.792998558004,
			"seed": 1600096163,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159316,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					0.4681954398183734
				],
				[
					-1.404693490698719,
					2.3411915415790645
				],
				[
					-3.7458850322777835,
					5.150578522976389
				],
				[
					-9.364766166316258,
					10.769423933266921
				],
				[
					-11.705957707895323,
					14.983611576606677
				],
				[
					-12.17418887146141,
					16.856536230871598
				],
				[
					-12.17418887146141,
					17.792998558004
				],
				[
					-7.491805788303282,
					17.324803118185628
				],
				[
					-7.491805788303282,
					17.324803118185628
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.1865234375,
				0.3642578125,
				0.4296875,
				0.44921875,
				0.46875,
				0.4775390625,
				0.4736328125,
				0.3671875,
				0.0146484375,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 48,
			"versionNonce": 2048556499,
			"isDeleted": false,
			"id": "4iMjFMe8Dm1eSXE44Lxza",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2999.7890460367903,
			"y": 299.14745793689997,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 32.308414694792646,
			"height": 32.77668158210645,
			"seed": 1099616237,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159316,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-2.3411915415790645,
					0.4682668873141438
				],
				[
					-6.555307737422936,
					0.4682668873141438
				],
				[
					-10.769423933267262,
					0
				],
				[
					-14.047149249474387,
					-1.404693490698719
				],
				[
					-15.920073903739194,
					-3.7458850322777835
				],
				[
					-15.451807016424937,
					-8.896499279002
				],
				[
					-13.57888236216013,
					-12.17418887146141
				],
				[
					-9.832961606134631,
					-15.92007390373908
				],
				[
					-5.61884541029076,
					-20.134225823331008
				],
				[
					-6.555307737422936,
					-22.47541736490996
				],
				[
					-9.832961606134631,
					-23.880146579356506
				],
				[
					-13.57888236216013,
					-25.753071233621426
				],
				[
					-17.324803118185628,
					-28.09426277520049
				],
				[
					-22.47538164116213,
					-31.3719523676599
				],
				[
					-26.689569284501886,
					-32.308414694792305
				],
				[
					-30.903685480345757,
					-31.840183531226103
				],
				[
					-32.308414694792646,
					-31.840183531226103
				],
				[
					-31.371952367660015,
					-32.308414694792305
				],
				[
					-31.371952367660015,
					-32.308414694792305
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.23046875,
				0.279296875,
				0.388671875,
				0.466796875,
				0.5029296875,
				0.51171875,
				0.513671875,
				0.498046875,
				0.4462890625,
				0.4130859375,
				0.427734375,
				0.4609375,
				0.5,
				0.513671875,
				0.5224609375,
				0.5224609375,
				0.5078125,
				0.033203125,
				0.015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 37,
			"versionNonce": 691223773,
			"isDeleted": false,
			"id": "RzDi0AntOMTaZ1_C6_XyB",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3014.7727290608927,
			"y": 293.99684369017564,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 13.578953809656014,
			"height": 26.22133812093557,
			"seed": 17457571,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159316,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-2.3411915415790645,
					1.8729603780128627
				],
				[
					-4.214187643339756,
					3.27768959245941
				],
				[
					-7.9601083993657085,
					7.491805788303282
				],
				[
					-11.23776226807695,
					12.17418887146141
				],
				[
					-13.110686922341756,
					16.856571954619426
				],
				[
					-13.578953809656014,
					24.34841346667065
				],
				[
					-12.642491482523383,
					26.22133812093557
				],
				[
					-12.642491482523383,
					26.22133812093557
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.296875,
				0.349609375,
				0.3974609375,
				0.4638671875,
				0.4912109375,
				0.49609375,
				0.3271484375,
				0.02734375,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 46,
			"versionNonce": 609307507,
			"isDeleted": false,
			"id": "siz4Ufit8Jnz1_ZiYggrp",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3028.3516114230524,
			"y": 300.08399171152814,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 16.856607678367254,
			"height": 32.77671730585428,
			"seed": 1577712579,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159316,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					5.61884541029076,
					-0.4682668873140301
				],
				[
					7.491841512051451,
					-0.9365337746281739
				],
				[
					10.769495380763146,
					-3.74595647977344
				],
				[
					12.17422459520958,
					-6.555379184918706
				],
				[
					11.705957707895323,
					-8.896570726497771
				],
				[
					10.301228493448889,
					-10.76953110451052
				],
				[
					6.555307737423391,
					-13.110722646089584
				],
				[
					4.214116195844326,
					-14.515416136788303
				],
				[
					3.745920756025953,
					-15.92014535123485
				],
				[
					5.61884541029076,
					-17.7931057292476
				],
				[
					7.491841512051451,
					-20.134297270826664
				],
				[
					8.428303839184082,
					-23.411951139538132
				],
				[
					6.555307737423391,
					-25.753142681117197
				],
				[
					1.8729246542652618,
					-28.562565386262463
				],
				[
					-4.682383083157674,
					-32.308486142288075
				],
				[
					-3.2776538687112406,
					-32.77671730585428
				],
				[
					-3.2776538687112406,
					-32.77671730585428
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2392578125,
				0.361328125,
				0.361328125,
				0.37109375,
				0.3916015625,
				0.396484375,
				0.4091796875,
				0.4462890625,
				0.4736328125,
				0.4794921875,
				0.4736328125,
				0.46875,
				0.4580078125,
				0.4755859375,
				0.5048828125,
				0.525390625,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 38,
			"versionNonce": 2094111037,
			"isDeleted": false,
			"id": "rrKt9ccCfec4UFwdeqoag",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3062.0647553322915,
			"y": 289.78272749433165,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 13.57888236216013,
			"height": 26.22133812093557,
			"seed": 398504781,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159317,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.9364623271321761,
					0.9364623271325172
				],
				[
					-2.809386981397438,
					4.682383083158129
				],
				[
					-4.2141161958438715,
					7.491805788303395
				],
				[
					-8.428303839183627,
					12.17418887146141
				],
				[
					-13.110686922341756,
					18.261301169066087
				],
				[
					-13.57888236216013,
					22.47541736490996
				],
				[
					-12.642420035027499,
					24.816608906489023
				],
				[
					-8.428303839183627,
					26.22133812093557
				],
				[
					-8.428303839183627,
					26.22133812093557
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.357421875,
				0.396484375,
				0.453125,
				0.4814453125,
				0.4990234375,
				0.501953125,
				0.439453125,
				0.205078125,
				0.0126953125,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 39,
			"versionNonce": 631072019,
			"isDeleted": false,
			"id": "e1IsH53b5dCstX1ZwpFXt",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3089.6908583914214,
			"y": 292.5921501994769,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 2.3411915415790645,
			"height": 25.284875793803053,
			"seed": 1865470499,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159317,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					-2.341191541578951
				],
				[
					0,
					-5.618881134038361
				],
				[
					0.4681954398183734,
					-9.36476616631603
				],
				[
					0.4681954398183734,
					-13.110686922341642
				],
				[
					0,
					-18.261301169065973
				],
				[
					0,
					-22.475453088657787
				],
				[
					-0.4682668873142575,
					-24.81664463023685
				],
				[
					0,
					-25.284875793803053
				],
				[
					1.872924654264807,
					-25.284875793803053
				],
				[
					1.872924654264807,
					-25.284875793803053
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.1630859375,
				0.4609375,
				0.5146484375,
				0.53515625,
				0.5390625,
				0.5390625,
				0.5107421875,
				0.447265625,
				0.203125,
				0.01171875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 41,
			"versionNonce": 421882269,
			"isDeleted": false,
			"id": "_CJvOw6i0hGVL4wmY1vJA",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3095.309703801712,
			"y": 275.26731135754346,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 20.13426154707895,
			"height": 21.538955037777555,
			"seed": 1530108899,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159317,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-4.214187643339756,
					1.872960378012749
				],
				[
					-7.960036951869824,
					2.8094584288930946
				],
				[
					-11.705957707895323,
					3.745920756025498
				],
				[
					-14.983611576606563,
					4.682383083158015
				],
				[
					-18.729532332632516,
					3.745920756025498
				],
				[
					-20.13426154707895,
					-0.9364623271325172
				],
				[
					-19.665994659764692,
					-6.55530773742305
				],
				[
					-18.261336892814143,
					-11.705957707895209
				],
				[
					-17.324803118185628,
					-16.388340791053224
				],
				[
					-15.920145351235078,
					-16.85657195461954
				],
				[
					-14.51541613678819,
					-15.920073903739194
				],
				[
					-14.51541613678819,
					-15.920073903739194
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.21875,
				0.259765625,
				0.34375,
				0.4287109375,
				0.490234375,
				0.5224609375,
				0.54296875,
				0.5400390625,
				0.5380859375,
				0.4638671875,
				0.2646484375,
				0.021484375,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 58,
			"versionNonce": 91572915,
			"isDeleted": false,
			"id": "ECZgWQ_KJ46eK-dsei308",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2967.9488982293124,
			"y": 246.70485314252474,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 87.09231820199011,
			"height": 80.53697474081943,
			"seed": 1633118531,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159317,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-5.150614246724217,
					13.578882362160101
				],
				[
					-7.023574624736739,
					22.47541736490993
				],
				[
					-7.960072675617084,
					31.371952367659873
				],
				[
					-6.087112297604108,
					44.48263929000163
				],
				[
					-3.7459207560250434,
					52.44267624187111
				],
				[
					0,
					59.93448203017451
				],
				[
					7.491841512051451,
					67.42628781847779
				],
				[
					14.515416136788645,
					71.6404397380696
				],
				[
					28.562565386262577,
					75.38636049409521
				],
				[
					37.927331552578835,
					75.85459165766142
				],
				[
					48.69675548584564,
					74.91812933052901
				],
				[
					56.65686388521135,
					72.1086709016358
				],
				[
					67.89455470579196,
					65.55336316421287
				],
				[
					73.04520467626435,
					58.99801970304199
				],
				[
					76.32285854497604,
					51.97444507830491
				],
				[
					78.19578319924085,
					44.014372402687485
				],
				[
					79.13224552637303,
					36.5225666143842
				],
				[
					79.13224552637303,
					30.43549004052747
				],
				[
					77.25932087210822,
					20.60245698689718
				],
				[
					73.98166700339698,
					14.983611576606648
				],
				[
					66.95809237865979,
					9.832997329882318
				],
				[
					56.65686388521135,
					1.404693490698719
				],
				[
					44.01437240268751,
					-3.745920756025555
				],
				[
					40.2685230941579,
					-4.214151919591814
				],
				[
					33.71314390923908,
					-4.682383083158015
				],
				[
					26.689569284501886,
					-3.745920756025555
				],
				[
					22.943648528476388,
					-2.3411915415790077
				],
				[
					21.07072387421158,
					3.7458850322777266
				],
				[
					21.07072387421158,
					3.7458850322777266
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.216796875,
				0.2822265625,
				0.3427734375,
				0.375,
				0.3896484375,
				0.392578125,
				0.39453125,
				0.39453125,
				0.3876953125,
				0.3857421875,
				0.3857421875,
				0.3857421875,
				0.4013671875,
				0.4189453125,
				0.4267578125,
				0.439453125,
				0.4609375,
				0.4873046875,
				0.5068359375,
				0.5244140625,
				0.5380859375,
				0.546875,
				0.548828125,
				0.548828125,
				0.548828125,
				0.548828125,
				0.5224609375,
				0.3369140625,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 52,
			"versionNonce": 794832381,
			"isDeleted": false,
			"id": "TBUkmSqzcFcy3AY0mrj29",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3019.4551121440513,
			"y": 321.62298247305375,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 140.93975938205585,
			"height": 55.25209894701641,
			"seed": 1682935821,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159317,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.4682668873142575,
					2.8094227051452663
				],
				[
					0.9364623271326309,
					7.02357462473708
				],
				[
					1.4047292144464336,
					8.896499279002
				],
				[
					3.745920756025498,
					13.110651198593814
				],
				[
					6.555307737422936,
					17.79303428175183
				],
				[
					9.83303305363006,
					22.47541736490996
				],
				[
					18.26126544531826,
					30.903721204093586
				],
				[
					23.41191541579019,
					35.5861042872516
				],
				[
					29.03076082608095,
					39.80025620684353
				],
				[
					37.92733155257838,
					42.609678911988794
				],
				[
					51.50621391473851,
					44.0143724026874
				],
				[
					62.2757092955012,
					42.609678911988794
				],
				[
					72.10867090163583,
					40.26848737040973
				],
				[
					82.40997084258015,
					36.52256661438412
				],
				[
					105.82188625837034,
					22.47541736490996
				],
				[
					113.31365632292591,
					16.388340791053224
				],
				[
					121.27369327479528,
					9.832997329882346
				],
				[
					132.9796509826906,
					-4.214151919591814
				],
				[
					136.25737629889773,
					-7.491841512051224
				],
				[
					138.5985678404768,
					-9.833033053630288
				],
				[
					140.4714924947416,
					-11.237726544329007
				],
				[
					140.0032256074278,
					-11.237726544329007
				],
				[
					140.0032256074278,
					-11.237726544329007
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2509765625,
				0.30859375,
				0.3447265625,
				0.361328125,
				0.369140625,
				0.3876953125,
				0.3955078125,
				0.3994140625,
				0.4013671875,
				0.408203125,
				0.41015625,
				0.41015625,
				0.412109375,
				0.4208984375,
				0.42578125,
				0.4326171875,
				0.44140625,
				0.458984375,
				0.4931640625,
				0.4990234375,
				0.50390625,
				0.3330078125,
				0.0146484375,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 44,
			"versionNonce": 411008083,
			"isDeleted": false,
			"id": "YRTK0Q584imcdUP5K9tZS",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3137.919418437449,
			"y": 301.4887209259749,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 28.562493938767147,
			"height": 40.26848737040973,
			"seed": 860985027,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159317,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					2.809386981397438,
					-1.4047292144465473
				],
				[
					4.682383083158129,
					-2.8094227051452663
				],
				[
					13.57888236216013,
					-10.769495380762692
				],
				[
					15.920073903739194,
					-12.642420035027612
				],
				[
					20.13426154707895,
					-14.515380413040361
				],
				[
					24.34837774292282,
					-13.110686922341756
				],
				[
					25.284840070055452,
					-10.769495380762692
				],
				[
					26.221302397188083,
					-5.6188454102905325
				],
				[
					26.689569284501886,
					-0.9364623271325172
				],
				[
					27.157836171816143,
					3.745920756025612
				],
				[
					28.094298498948774,
					11.237726544328893
				],
				[
					28.094298498948774,
					15.920109627487022
				],
				[
					28.094298498948774,
					20.602492710645038
				],
				[
					28.562493938767147,
					25.75310695736937
				],
				[
					28.562493938767147,
					25.75310695736937
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.29296875,
				0.3583984375,
				0.3662109375,
				0.3876953125,
				0.3857421875,
				0.40625,
				0.4599609375,
				0.4716796875,
				0.4892578125,
				0.5078125,
				0.513671875,
				0.5244140625,
				0.5244140625,
				0.443359375,
				0.015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 47,
			"versionNonce": 1317234269,
			"isDeleted": false,
			"id": "G5LUVebZyHxcU8v6GHEVl",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3209.091627011953,
			"y": 296.8063378428169,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 27.626031611634517,
			"height": 35.11787312368551,
			"seed": 573500909,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159317,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-3.745920756025498,
					0
				],
				[
					-7.960036951869824,
					-1.404729214446661
				],
				[
					-9.364766166316258,
					-3.745920756025612
				],
				[
					-9.364766166316258,
					-6.555343461170878
				],
				[
					-7.960036951869824,
					-10.301228493448662
				],
				[
					-5.61884541029076,
					-13.110686922341756
				],
				[
					-3.745920756025498,
					-15.920109627487022
				],
				[
					-1.4047292144464336,
					-19.19776349619849
				],
				[
					-1.4047292144464336,
					-22.4754530886579
				],
				[
					-3.745920756025498,
					-25.284875793803167
				],
				[
					-8.428303839183627,
					-28.094298498948433
				],
				[
					-16.856607678367254,
					-31.840219254974045
				],
				[
					-21.070723874211126,
					-33.24491274567265
				],
				[
					-24.34837774292282,
					-34.181410796552996
				],
				[
					-27.626031611634517,
					-35.11787312368551
				],
				[
					-26.689569284501886,
					-35.11787312368551
				],
				[
					-21.070723874211126,
					-35.11787312368551
				],
				[
					-21.070723874211126,
					-35.11787312368551
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.138671875,
				0.271484375,
				0.4169921875,
				0.48046875,
				0.5078125,
				0.51171875,
				0.5048828125,
				0.5,
				0.498046875,
				0.486328125,
				0.5009765625,
				0.529296875,
				0.5712890625,
				0.583984375,
				0.58984375,
				0.576171875,
				0.515625,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 39,
			"versionNonce": 1519548915,
			"isDeleted": false,
			"id": "B7N-XEAAq9zdx9Hy6DySO",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3222.670509374113,
			"y": 279.013267837317,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 17.324874565681057,
			"height": 4.214151919591814,
			"seed": 2084624813,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159317,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					0.4682668873141438
				],
				[
					2.3411915415790645,
					0.4682668873141438
				],
				[
					5.150649970471932,
					0
				],
				[
					7.960108399365254,
					-0.9364623271324035
				],
				[
					11.237762268076494,
					-1.4046934906986053
				],
				[
					13.578953809655559,
					-1.872924654264807
				],
				[
					16.388340791052997,
					-2.8094227051451526
				],
				[
					17.324874565681057,
					-3.277653868711468
				],
				[
					16.388340791052997,
					-3.74588503227767
				],
				[
					16.388340791052997,
					-3.74588503227767
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2490234375,
				0.31640625,
				0.4609375,
				0.4765625,
				0.478515625,
				0.478515625,
				0.4716796875,
				0.4091796875,
				0.2421875,
				0.0126953125,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 38,
			"versionNonce": 694194877,
			"isDeleted": false,
			"id": "sWBdbfuvhEGF6WZiVYyu1",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3229.225888559032,
			"y": 265.434385475157,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 5.618916857786189,
			"height": 27.157800448067974,
			"seed": 1646195693,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159317,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-1.4047292144468884,
					5.6188454102905325
				],
				[
					-1.4047292144468884,
					7.960036951869597
				],
				[
					-1.872996101760691,
					11.705957707895209
				],
				[
					-1.872996101760691,
					17.324803118185628
				],
				[
					-0.4682668873142575,
					20.134225823330894
				],
				[
					1.4047292144464336,
					22.94364852847616
				],
				[
					3.2776538687112406,
					25.284840070055225
				],
				[
					3.745920756025498,
					27.157800448067974
				],
				[
					3.745920756025498,
					27.157800448067974
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.30859375,
				0.3818359375,
				0.4091796875,
				0.4609375,
				0.5068359375,
				0.51171875,
				0.5009765625,
				0.38671875,
				0.11328125,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 49,
			"versionNonce": 146064275,
			"isDeleted": false,
			"id": "elOx_hh3KrgVckaOp828d",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3247.018958564531,
			"y": 286.97334051293456,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 21.538990761525383,
			"height": 27.157836171815916,
			"seed": 167808899,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159317,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.9365337746280602,
					0
				],
				[
					-0.4682668873138027,
					0
				],
				[
					1.8729246542652618,
					0
				],
				[
					4.214116195844326,
					-0.9364980508803455
				],
				[
					7.960036951869824,
					-2.3411915415790645
				],
				[
					11.237690820581065,
					-3.745920756025612
				],
				[
					13.110615474845872,
					-5.150614246724331
				],
				[
					11.237690820581065,
					-7.491805788303395
				],
				[
					8.428232391687743,
					-8.896535002749943
				],
				[
					6.087040850109133,
					-9.832997329882346
				],
				[
					5.61884541029076,
					-10.769495380762692
				],
				[
					6.555307737422936,
					-12.17418887146141
				],
				[
					10.769423933266808,
					-15.45187846392082
				],
				[
					14.047149249474387,
					-20.134261547078836
				],
				[
					9.832961606134631,
					-22.4754530886579
				],
				[
					2.3411915415790645,
					-25.75310695736937
				],
				[
					-2.3411915415790645,
					-26.689605008249714
				],
				[
					-7.491841512050996,
					-27.157836171815916
				],
				[
					-1.4047292144464336,
					-26.22133812093557
				],
				[
					-1.4047292144464336,
					-26.22133812093557
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.234375,
				0.306640625,
				0.490234375,
				0.4931640625,
				0.4951171875,
				0.4951171875,
				0.4951171875,
				0.4970703125,
				0.5107421875,
				0.5166015625,
				0.5400390625,
				0.55078125,
				0.552734375,
				0.54296875,
				0.501953125,
				0.5078125,
				0.5673828125,
				0.5888671875,
				0.587890625,
				0.0283203125,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 45,
			"versionNonce": 479802141,
			"isDeleted": false,
			"id": "L6cxi7adnjqOjue8b6YCT",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3192.7032862208994,
			"y": 324.432405178199,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 119.40076862053093,
			"height": 46.82383083158061,
			"seed": 1995679587,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159317,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1.872924654264807,
					-0.46823116356631544
				],
				[
					6.555307737422936,
					-1.404729214446661
				],
				[
					9.833033053630515,
					-2.8094227051452663
				],
				[
					16.38834079105345,
					-5.618881134038475
				],
				[
					25.284840070055452,
					-8.896535002749943
				],
				[
					36.054335450818144,
					-14.515380413040475
				],
				[
					55.25213467076446,
					-23.411915415790304
				],
				[
					69.76747936005677,
					-29.03079654982878
				],
				[
					82.4099708425806,
					-34.64964196011931
				],
				[
					93.64766166316122,
					-39.332025043277326
				],
				[
					102.0759655023453,
					-42.14144774842259
				],
				[
					112.84546088310753,
					-44.48263929000166
				],
				[
					115.1866524246866,
					-45.419137340882
				],
				[
					119.40076862053093,
					-46.82383083158061
				],
				[
					119.40076862053093,
					-45.887368504448204
				],
				[
					119.40076862053093,
					-45.887368504448204
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2109375,
				0.25,
				0.283203125,
				0.3017578125,
				0.3251953125,
				0.349609375,
				0.369140625,
				0.384765625,
				0.3935546875,
				0.41015625,
				0.423828125,
				0.435546875,
				0.443359375,
				0.443359375,
				0.314453125,
				0.0146484375,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 46,
			"versionNonce": 2065488179,
			"isDeleted": false,
			"id": "yod0JyVfstf8EeCJRowhN",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3253.574266301954,
			"y": 339.8842479183719,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 25.753106957369255,
			"height": 16.856607678367254,
			"seed": 1393119235,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159317,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-5.618845410290305,
					0.4682668873140301
				],
				[
					-9.364766166315803,
					0.4682668873140301
				],
				[
					-13.110686922341756,
					0
				],
				[
					-14.983611576606563,
					-0.46823116356631544
				],
				[
					-12.642420035027499,
					-2.3411915415790645
				],
				[
					-9.364766166315803,
					-4.214116195843985
				],
				[
					-5.618845410290305,
					-6.55530773742305
				],
				[
					-2.3411915415786098,
					-10.301228493448662
				],
				[
					-2.3411915415786098,
					-12.17418887146141
				],
				[
					-4.2141161958438715,
					-13.57888236216013
				],
				[
					-7.96003695186937,
					-14.515380413040475
				],
				[
					-14.51541613678819,
					-15.451842740172879
				],
				[
					-22.007186201343302,
					-16.388340791053224
				],
				[
					-25.753106957369255,
					-16.388340791053224
				],
				[
					-25.753106957369255,
					-15.920073903739194
				],
				[
					-22.007186201343302,
					-14.983611576606677
				],
				[
					-22.007186201343302,
					-14.983611576606677
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2900390625,
				0.4052734375,
				0.48828125,
				0.5283203125,
				0.5400390625,
				0.5400390625,
				0.5283203125,
				0.5263671875,
				0.5068359375,
				0.501953125,
				0.5166015625,
				0.5458984375,
				0.5751953125,
				0.5927734375,
				0.5927734375,
				0.5380859375,
				0.0146484375,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 39,
			"versionNonce": 1956562813,
			"isDeleted": false,
			"id": "jeqOg6R3XSKcaFXkNvCNT",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3295.715714050377,
			"y": 314.5994078483167,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 29.967223153213126,
			"height": 5.618881134038475,
			"seed": 1927547661,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159318,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.9364623271326309,
					0
				],
				[
					6.087112297604563,
					0
				],
				[
					10.769495380762692,
					0
				],
				[
					15.45187846392082,
					-0.4682668873141438
				],
				[
					20.13426154707895,
					-1.404729214446661
				],
				[
					25.284840070054997,
					-2.3411915415790645
				],
				[
					28.562565386262577,
					-3.27768959245941
				],
				[
					29.967223153213126,
					-4.214151919591927
				],
				[
					28.562565386262577,
					-5.618881134038475
				],
				[
					28.562565386262577,
					-5.618881134038475
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.333984375,
				0.4619140625,
				0.5,
				0.5107421875,
				0.5107421875,
				0.517578125,
				0.513671875,
				0.4306640625,
				0.2109375,
				0.0126953125,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 39,
			"versionNonce": 1060190931,
			"isDeleted": false,
			"id": "uLohsc_lim7qI9DwRGKPv",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3305.548747104007,
			"y": 299.14752938439585,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 24.34837774292282,
			"height": 1.4047292144465473,
			"seed": 2059771213,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159318,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.4681954398183734,
					0
				],
				[
					3.2776538687116954,
					0
				],
				[
					7.491770064555567,
					0
				],
				[
					13.110615474845872,
					0
				],
				[
					18.729532332632516,
					-0.46823116356620176
				],
				[
					20.602456986897323,
					-0.46823116356620176
				],
				[
					22.943648528476388,
					-0.9364623271324035
				],
				[
					23.88011085560902,
					-0.9364623271324035
				],
				[
					24.34837774292282,
					-1.4047292144465473
				],
				[
					24.34837774292282,
					-1.4047292144465473
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.3203125,
				0.4365234375,
				0.482421875,
				0.49609375,
				0.505859375,
				0.5224609375,
				0.5166015625,
				0.484375,
				0.3046875,
				0.244140625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 44,
			"versionNonce": 1941098461,
			"isDeleted": false,
			"id": "LqgptDgPIXeeu5kJMh9Mp",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3364.546731083301,
			"y": 309.91702476515854,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 16.388340791052997,
			"height": 26.2213738446834,
			"seed": 1868857229,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159318,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-10.301228493448434,
					-1.4047292144465473
				],
				[
					-11.23769082058061,
					-2.341191541578951
				],
				[
					-12.642420035027499,
					-4.682383083158015
				],
				[
					-12.174153147713241,
					-7.491841512051224
				],
				[
					-10.769495380762237,
					-10.30126421719649
				],
				[
					-7.96003695186937,
					-12.64245575877544
				],
				[
					-3.2776538687112406,
					-15.451878463920707
				],
				[
					-1.872924654264807,
					-17.32483884193357
				],
				[
					-3.745920756025498,
					-19.19779921994632
				],
				[
					-7.491770064555112,
					-21.07072387421124
				],
				[
					-13.110686922341301,
					-23.880182303104334
				],
				[
					-15.451878463920366,
					-25.284875793803053
				],
				[
					-16.388340791052997,
					-26.2213738446834
				],
				[
					-14.047149249473932,
					-26.2213738446834
				],
				[
					-14.047149249473932,
					-26.2213738446834
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2822265625,
				0.3974609375,
				0.4423828125,
				0.4990234375,
				0.517578125,
				0.513671875,
				0.5029296875,
				0.4912109375,
				0.4833984375,
				0.48828125,
				0.51171875,
				0.544921875,
				0.552734375,
				0.5478515625,
				0.0166015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 34,
			"versionNonce": 1904765043,
			"isDeleted": false,
			"id": "pWF1h4ln3xwhp8x_vLtSN",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3377.6574180056427,
			"y": 303.829912467554,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 1.4047292144464336,
			"height": 0.9364623271325172,
			"seed": 692361411,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159318,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.4682668873138027,
					0.46823116356620176
				],
				[
					-0.9364623271321761,
					0.46823116356620176
				],
				[
					-1.4047292144464336,
					-0.46823116356631544
				],
				[
					0,
					0
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.34375,
				0.39453125,
				0.4560546875,
				0.10546875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 49,
			"versionNonce": 401001533,
			"isDeleted": false,
			"id": "pzdud8ndOvDRadhTGDBAO",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3390.7681049279845,
			"y": 307.10756633626545,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 21.538990761525383,
			"height": 29.49902771339498,
			"seed": 317338637,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159318,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.4681954398183734,
					0.4682668873141438
				],
				[
					0.9364623271326309,
					0.4682668873141438
				],
				[
					4.214116195844326,
					-0.9364623271325172
				],
				[
					7.0235746247371935,
					-2.3411915415790645
				],
				[
					8.896499279002,
					-3.7458850322777835
				],
				[
					9.364766166316258,
					-5.6188454102905325
				],
				[
					8.428303839183627,
					-7.02357462473708
				],
				[
					6.087112297605017,
					-7.960036951869597
				],
				[
					2.809386981397438,
					-10.301228493448548
				],
				[
					0.9364623271326309,
					-11.705957707895209
				],
				[
					-0.4682668873138027,
					-14.04714924947416
				],
				[
					-2.8094584288928672,
					-19.19776349619849
				],
				[
					-3.745920756025498,
					-22.47541736490996
				],
				[
					-3.745920756025498,
					-23.880146579356506
				],
				[
					-1.4047292144464336,
					-26.689569284501772
				],
				[
					3.2776538687116954,
					-28.094298498948433
				],
				[
					9.832961606134631,
					-29.030760826080837
				],
				[
					14.047149249474387,
					-29.030760826080837
				],
				[
					17.793070005499885,
					-28.562529662514635
				],
				[
					17.793070005499885,
					-28.562529662514635
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.30859375,
				0.3994140625,
				0.4267578125,
				0.455078125,
				0.4580078125,
				0.4580078125,
				0.466796875,
				0.4765625,
				0.4814453125,
				0.4990234375,
				0.5146484375,
				0.5244140625,
				0.529296875,
				0.5380859375,
				0.5556640625,
				0.56640625,
				0.5712890625,
				0.5283203125,
				0.4248046875,
				0.015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 42,
			"versionNonce": 1474880019,
			"isDeleted": false,
			"id": "DYVuL08_mzqmrWTSEyS3w",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3373.443301809799,
			"y": 211.1187131315252,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 2.3411915415790645,
			"height": 45.887368504448176,
			"seed": 176846381,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159318,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					2.3411915415790077
				],
				[
					0,
					5.618881134038418
				],
				[
					0.4681954398183734,
					9.833033053630231
				],
				[
					0.9364623271326309,
					14.983647300354505
				],
				[
					1.8729246542652618,
					24.34841346667065
				],
				[
					1.8729246542652618,
					29.499027713394923
				],
				[
					1.8729246542652618,
					34.181410796552996
				],
				[
					1.4046577669510043,
					39.33202504327727
				],
				[
					1.4046577669510043,
					43.07794579930288
				],
				[
					1.4046577669510043,
					44.95090617731566
				],
				[
					1.8729246542652618,
					45.41913734088186
				],
				[
					2.3411915415790645,
					45.887368504448176
				],
				[
					2.3411915415790645,
					45.887368504448176
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.353515625,
				0.400390625,
				0.4404296875,
				0.4814453125,
				0.4970703125,
				0.515625,
				0.5205078125,
				0.5234375,
				0.5322265625,
				0.53515625,
				0.537109375,
				0.5078125,
				0.37890625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 44,
			"versionNonce": 555498653,
			"isDeleted": false,
			"id": "HqH2FyXjXhFTXF9Z_VkQa",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3366.88792262488,
			"y": 253.72842776726188,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 22.475453088658014,
			"height": 15.451842740172793,
			"seed": 1791165571,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159318,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.4682668873142575,
					0.9364623271324604
				],
				[
					0.9364623271326309,
					3.2776538687114964
				],
				[
					1.4047292144468884,
					6.5553077374229645
				],
				[
					2.3411915415790645,
					11.23769082058098
				],
				[
					3.745920756025953,
					13.578882362160044
				],
				[
					5.1506499704723865,
					15.451842740172793
				],
				[
					7.491841512051451,
					14.983611576606592
				],
				[
					10.769495380762692,
					13.110651198593843
				],
				[
					16.38834079105345,
					8.896499279002029
				],
				[
					19.19779921994632,
					6.5553077374229645
				],
				[
					20.602528434393207,
					3.745885032277698
				],
				[
					21.07072387421158,
					2.3411915415789792
				],
				[
					21.538990761525383,
					1.4046934906986621
				],
				[
					22.475453088658014,
					1.8729246542648639
				],
				[
					22.475453088658014,
					1.8729246542648639
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2646484375,
				0.41015625,
				0.47265625,
				0.5,
				0.51953125,
				0.521484375,
				0.525390625,
				0.5341796875,
				0.5390625,
				0.541015625,
				0.541015625,
				0.5458984375,
				0.5390625,
				0.517578125,
				0.0341796875,
				0
			]
		},
		{
			"type": "text",
			"version": 100,
			"versionNonce": 994650035,
			"isDeleted": false,
			"id": "2W2MNvNT",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2522.509548932696,
			"y": 484.2427486289856,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 149,
			"height": 25,
			"seed": 427412675,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159318,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "WALKTHROUGH",
			"rawText": "WALKTHROUGH",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "WALKTHROUGH",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 201,
			"versionNonce": 1459921149,
			"isDeleted": false,
			"id": "39LNsojw",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3055.350642747153,
			"y": 463.3019897470274,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 138,
			"height": 25,
			"seed": 745422701,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159318,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "BRUTEFORCE",
			"rawText": "BRUTEFORCE",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "BRUTEFORCE",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 1381,
			"versionNonce": 30390611,
			"isDeleted": false,
			"id": "Q1wWuBcj",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2579.4487745605816,
			"y": 545.9853394387584,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 475,
			"height": 450,
			"seed": 999575875,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159318,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "- index1 = 0\n- index2 = 0\n- isValidn1 = false\n- isValidn2 = false\n- eleStack\n- isEven = false\n- totalLenght = 0\n- add lenghts to total if exist\n- middle = totalLen / 2\n- if totalLen is even\n    - isEven = true \n- traverse middle number of times\n    -  push lowest number to the stack if exist\n       // if statements checking valid entries\n- if isEven\n    - return eleQu.pop +eleQ.pop / 2\n- else // its odd\n    - return eleQ.pop",
			"rawText": "- index1 = 0\n- index2 = 0\n- isValidn1 = false\n- isValidn2 = false\n- eleStack\n- isEven = false\n- totalLenght = 0\n- add lenghts to total if exist\n- middle = totalLen / 2\n- if totalLen is even\n    - isEven = true \n- traverse middle number of times\n    -  push lowest number to the stack if exist\n       // if statements checking valid entries\n- if isEven\n    - return eleQu.pop +eleQ.pop / 2\n- else // its odd\n    - return eleQ.pop",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "- index1 = 0\n- index2 = 0\n- isValidn1 = false\n- isValidn2 = false\n- eleStack\n- isEven = false\n- totalLenght = 0\n- add lenghts to total if exist\n- middle = totalLen / 2\n- if totalLen is even\n    - isEven = true \n- traverse middle number of times\n    -  push lowest number to the stack if exist\n       // if statements checking valid entries\n- if isEven\n    - return eleQu.pop +eleQ.pop / 2\n- else // its odd\n    - return eleQ.pop",
			"lineHeight": 1.25,
			"baseline": 442
		},
		{
			"type": "text",
			"version": 96,
			"versionNonce": 253851997,
			"isDeleted": false,
			"id": "KhqMIAub",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3123.0583351259334,
			"y": 532.1008483095289,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 229,
			"height": 175,
			"seed": 711524557,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159318,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "int index1 = 0\nint index2 = 0\nbool isValidn1 = false\nbool isValidn2 = false\nStack eleStack\nbool isEven = false\ndouble totalLenght = 0",
			"rawText": "int index1 = 0\nint index2 = 0\nbool isValidn1 = false\nbool isValidn2 = false\nStack eleStack\nbool isEven = false\ndouble totalLenght = 0",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "int index1 = 0\nint index2 = 0\nbool isValidn1 = false\nbool isValidn2 = false\nStack eleStack\nbool isEven = false\ndouble totalLenght = 0",
			"lineHeight": 1.25,
			"baseline": 167
		},
		{
			"type": "text",
			"version": 99,
			"versionNonce": 148051699,
			"isDeleted": false,
			"id": "VhgxddiH",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3124.62128852995,
			"y": 719.6974654231709,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 115,
			"height": 25,
			"seed": 142769443,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159318,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "totalLen = ",
			"rawText": "totalLen = ",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "totalLen = ",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 142,
			"versionNonce": 1925465533,
			"isDeleted": false,
			"id": "3v2udqof",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3118.50369891598,
			"y": 768.6385772682995,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 118,
			"height": 25,
			"seed": 1984457517,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159318,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "totalLen +=",
			"rawText": "totalLen +=",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "totalLen +=",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 185,
			"versionNonce": 1054458003,
			"isDeleted": false,
			"id": "Y7R7t4K_NDXScB2_W4H5-",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3238.6507433782954,
			"y": 718.3740329495957,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 168,
			"height": 35,
			"seed": 290482179,
			"groupIds": [],
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "xX0dtknE"
				},
				{
					"id": "uHXV45CkmQeKyr4dCHwgj",
					"type": "arrow"
				}
			],
			"updated": 1686311159318,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 162,
			"versionNonce": 84837917,
			"isDeleted": false,
			"id": "xX0dtknE",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3252.1507433782954,
			"y": 723.3740329495957,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 141,
			"height": 25,
			"seed": 2118849837,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159318,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "if nums1 != null",
			"rawText": "if nums1 != null",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "Y7R7t4K_NDXScB2_W4H5-",
			"originalText": "if nums1 != null",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "arrow",
			"version": 360,
			"versionNonce": 2107258419,
			"isDeleted": false,
			"id": "uHXV45CkmQeKyr4dCHwgj",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3407.6507433782954,
			"y": 735.9075986360366,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 54.85287655101138,
			"height": 2.530089055124222,
			"seed": 1821142669,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "yggfoPQl"
				}
			],
			"updated": 1686311159318,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "Y7R7t4K_NDXScB2_W4H5-",
				"gap": 1,
				"focus": 0.18499571188691438
			},
			"endBinding": {
				"elementId": "eAUcrbGd",
				"gap": 14.82350068933738,
				"focus": -0.00821552131643394
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					54.85287655101138,
					-2.530089055124222
				]
			]
		},
		{
			"type": "text",
			"version": 57,
			"versionNonce": 1760672381,
			"isDeleted": false,
			"id": "yggfoPQl",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3430.5771816538013,
			"y": 722.1056775917547,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 9,
			"height": 25,
			"seed": 696211533,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159318,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "?",
			"rawText": "?",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "uHXV45CkmQeKyr4dCHwgj",
			"originalText": "?",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 125,
			"versionNonce": 603650003,
			"isDeleted": false,
			"id": "eAUcrbGd",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3477.327120618644,
			"y": 717.5798686285939,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 108,
			"height": 25,
			"seed": 1683356301,
			"groupIds": [],
			"roundness": null,
			"boundElements": [
				{
					"id": "uHXV45CkmQeKyr4dCHwgj",
					"type": "arrow"
				}
			],
			"updated": 1686311159318,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "nums1.len; 0",
			"rawText": "nums1.len; 0",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "nums1.len; 0",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 229,
			"versionNonce": 1731158749,
			"isDeleted": false,
			"id": "uXjhqB4cnnBERY-X1kgag",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3247.283107090382,
			"y": 760.7122951709882,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 168,
			"height": 35,
			"seed": 476108867,
			"groupIds": [],
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "26z4DY0E"
				},
				{
					"id": "_I86mI03T-VSwYRFz2gJy",
					"type": "arrow"
				}
			],
			"updated": 1686311159319,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 208,
			"versionNonce": 1880262003,
			"isDeleted": false,
			"id": "26z4DY0E",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3256.283107090382,
			"y": 765.7122951709882,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 150,
			"height": 25,
			"seed": 1673713635,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159319,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "if nums2 != null",
			"rawText": "if nums2 != null",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "uXjhqB4cnnBERY-X1kgag",
			"originalText": "if nums2 != null",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "arrow",
			"version": 496,
			"versionNonce": 878247741,
			"isDeleted": false,
			"id": "_I86mI03T-VSwYRFz2gJy",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3416.283107090382,
			"y": 778.2714490899725,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 54.85287655101138,
			"height": 2.4517773367891778,
			"seed": 1510204291,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "5AAk21cK"
				}
			],
			"updated": 1686311159319,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "uXjhqB4cnnBERY-X1kgag",
				"gap": 1,
				"focus": 0.18153395718508342
			},
			"endBinding": {
				"elementId": "lAzkYAHh",
				"gap": 14.823500689336925,
				"focus": -0.008215521316436505
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					54.85287655101138,
					-2.4517773367891778
				]
			]
		},
		{
			"type": "text",
			"version": 102,
			"versionNonce": 422010643,
			"isDeleted": false,
			"id": "5AAk21cK",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3439.209545365888,
			"y": 764.4652735124815,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 9,
			"height": 25,
			"seed": 1734507299,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159319,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "?",
			"rawText": "?",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "_I86mI03T-VSwYRFz2gJy",
			"originalText": "?",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 171,
			"versionNonce": 1993346973,
			"isDeleted": false,
			"id": "lAzkYAHh",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3485.9594843307304,
			"y": 759.9181308499865,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 117,
			"height": 25,
			"seed": 1749884611,
			"groupIds": [],
			"roundness": null,
			"boundElements": [
				{
					"id": "_I86mI03T-VSwYRFz2gJy",
					"type": "arrow"
				}
			],
			"updated": 1686311159319,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "nums2.len; 0",
			"rawText": "nums2.len; 0",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "nums2.len; 0",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 124,
			"versionNonce": 699401395,
			"isDeleted": false,
			"id": "FEp81Olq",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3124.1507074752626,
			"y": 810.5210450991821,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 283,
			"height": 25,
			"seed": 1036724355,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159319,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "double middle = totalLen / 2",
			"rawText": "double middle = totalLen / 2",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "double middle = totalLen / 2",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 250,
			"versionNonce": 214307837,
			"isDeleted": false,
			"id": "71_l-bV3izePbmSBZnlet",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3118.8860123638206,
			"y": 852.5798901704139,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 188,
			"height": 35,
			"seed": 721232941,
			"groupIds": [],
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "iXFgkvIs"
				}
			],
			"updated": 1686311159319,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 202,
			"versionNonce": 424867411,
			"isDeleted": false,
			"id": "iXFgkvIs",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3132.8860123638206,
			"y": 857.5798901704139,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 160,
			"height": 25,
			"seed": 1922345603,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159319,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "if totalLen % 2",
			"rawText": "if totalLen % 2",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "71_l-bV3izePbmSBZnlet",
			"originalText": "if totalLen % 2",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "arrow",
			"version": 216,
			"versionNonce": 305957981,
			"isDeleted": false,
			"id": "nlhugoyndnCaXeSkcVopI",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3305.3271780634986,
			"y": 870.0504640444948,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 78.58822093290473,
			"height": 0.4706169577206083,
			"seed": 1594377869,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "8lVrTGXP"
				}
			],
			"updated": 1686311159319,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": {
				"elementId": "HgAyVWZA",
				"focus": -0.06857706490538838,
				"gap": 7.999985638786711
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					78.58822093290473,
					0.4706169577206083
				]
			]
		},
		{
			"type": "text",
			"version": 101,
			"versionNonce": 652653555,
			"isDeleted": false,
			"id": "8lVrTGXP",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3336.621288529951,
			"y": 857.7857725233551,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 16,
			"height": 25,
			"seed": 2093519981,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159319,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "T",
			"rawText": "T",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "nlhugoyndnCaXeSkcVopI",
			"originalText": "T",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 134,
			"versionNonce": 654637245,
			"isDeleted": false,
			"id": "HgAyVWZA",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3391.91538463519,
			"y": 857.5799045316272,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 132,
			"height": 25,
			"seed": 1540616077,
			"groupIds": [],
			"roundness": null,
			"boundElements": [
				{
					"id": "nlhugoyndnCaXeSkcVopI",
					"type": "arrow"
				}
			],
			"updated": 1686311159319,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "isEven = true",
			"rawText": "isEven = true",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "isEven = true",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 228,
			"versionNonce": 1920056723,
			"isDeleted": false,
			"id": "xTixuyEcSAargtJtIW6CW",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3119.386048266854,
			"y": 913.2563571683465,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 270,
			"height": 35,
			"seed": 184228493,
			"groupIds": [],
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "yHM1IhuC"
				}
			],
			"updated": 1686311159319,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 272,
			"versionNonce": 1958795549,
			"isDeleted": false,
			"id": "yHM1IhuC",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3127.886048266854,
			"y": 918.2563571683465,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 253,
			"height": 25,
			"seed": 126205827,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159319,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "for i = 0; i <= middle; i++",
			"rawText": "for i = 0; i <= middle; i++",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "xTixuyEcSAargtJtIW6CW",
			"originalText": "for i = 0; i <= middle; i++",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "line",
			"version": 159,
			"versionNonce": 1462407987,
			"isDeleted": false,
			"id": "wsduKTmRR1LBPnKM5-Ve1",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3390.9742225258146,
			"y": 928.4034124015723,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 317.31243366293256,
			"height": 0,
			"seed": 539690573,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1686311159319,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					317.31243366293256,
					0
				]
			]
		},
		{
			"type": "line",
			"version": 233,
			"versionNonce": 1960947069,
			"isDeleted": false,
			"id": "UtTrMncynEyy3TalrHt9z",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3134.974215345208,
			"y": 952.8739862756532,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 0,
			"height": 791.2596589518646,
			"seed": 1193660931,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1686311159319,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					0,
					791.2596589518646
				]
			]
		},
		{
			"type": "rectangle",
			"version": 357,
			"versionNonce": 91731155,
			"isDeleted": false,
			"id": "CCSITZZYlVmjFdBFCDC8d",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3167.8238211299063,
			"y": 962.2334482407779,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 380,
			"height": 35,
			"seed": 1300657421,
			"groupIds": [],
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "ryXRNAEw"
				},
				{
					"id": "UuczJCM2clis2L879WAZO",
					"type": "arrow"
				}
			],
			"updated": 1686311159319,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 451,
			"versionNonce": 1990784477,
			"isDeleted": false,
			"id": "ryXRNAEw",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3182.3238211299063,
			"y": 967.2334482407779,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 351,
			"height": 25,
			"seed": 515715053,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159319,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "if nums1 != null && index1 < nums1.len",
			"rawText": "if nums1 != null && index1 < nums1.len",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "CCSITZZYlVmjFdBFCDC8d",
			"originalText": "if nums1 != null && index1 < nums1.len",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 547,
			"versionNonce": 1559208563,
			"isDeleted": false,
			"id": "XT_5FeURnHvc-k85RWddz",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3166.5528102760204,
			"y": 1039.5047120115855,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 399,
			"height": 35,
			"seed": 821950349,
			"groupIds": [],
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "CO8SUKbN"
				},
				{
					"id": "tMgY2QAXpOSSOEhIC7m13",
					"type": "arrow"
				}
			],
			"updated": 1686311159319,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 685,
			"versionNonce": 1697133117,
			"isDeleted": false,
			"id": "CO8SUKbN",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3177.0528102760204,
			"y": 1044.5047120115855,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 378,
			"height": 25,
			"seed": 1792114157,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159319,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "if nums2 != null && index2 < nums2.len",
			"rawText": "if nums2 != null && index2 < nums2.len",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "XT_5FeURnHvc-k85RWddz",
			"originalText": "if nums2 != null && index2 < nums2.len",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "arrow",
			"version": 942,
			"versionNonce": 106486803,
			"isDeleted": false,
			"id": "UuczJCM2clis2L879WAZO",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3192.1670556987724,
			"y": 1003.2268949399327,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 191.45745324495692,
			"height": 16.258090168213357,
			"seed": 1943004045,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "RkcFzKen"
				}
			],
			"updated": 1686311159320,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "CCSITZZYlVmjFdBFCDC8d",
				"gap": 5.993446699154788,
				"focus": 1.1167343069995213
			},
			"endBinding": {
				"elementId": "ufQY7RpN",
				"gap": 14.147147073712404,
				"focus": -0.33388804264198824
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					191.45745324495692,
					16.258090168213357
				]
			]
		},
		{
			"type": "text",
			"version": 94,
			"versionNonce": 1296097949,
			"isDeleted": false,
			"id": "RkcFzKen",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3586.7650442744375,
			"y": 965.0276017908699,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 16,
			"height": 25,
			"seed": 1925040195,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159320,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "T",
			"rawText": "T",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "UuczJCM2clis2L879WAZO",
			"originalText": "T",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 410,
			"versionNonce": 1302978995,
			"isDeleted": false,
			"id": "ufQY7RpN",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3397.7716560174417,
			"y": 1008.1419385900427,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 146,
			"height": 25,
			"seed": 170285613,
			"groupIds": [],
			"roundness": null,
			"boundElements": [
				{
					"id": "UuczJCM2clis2L879WAZO",
					"type": "arrow"
				}
			],
			"updated": 1686311159320,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "isValidn1 = true",
			"rawText": "isValidn1 = true",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "isValidn1 = true",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "arrow",
			"version": 1271,
			"versionNonce": 597985021,
			"isDeleted": false,
			"id": "tMgY2QAXpOSSOEhIC7m13",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3185.6453847327857,
			"y": 1082.657412174452,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 202.81903595407266,
			"height": 18.81721018461849,
			"seed": 79375715,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "7o0IcGUM"
				}
			],
			"updated": 1686311159320,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "XT_5FeURnHvc-k85RWddz",
				"gap": 8.152700162866495,
				"focus": 1.1772133152734268
			},
			"endBinding": {
				"elementId": "F5Gj3LdF",
				"gap": 12.979623520028781,
				"focus": -0.5211447126117842
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					202.81903595407266,
					18.81721018461849
				]
			]
		},
		{
			"type": "text",
			"version": 222,
			"versionNonce": 1007235923,
			"isDeleted": false,
			"id": "7o0IcGUM",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3591.6923671363193,
			"y": 1043.8749565632456,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 16,
			"height": 25,
			"seed": 878020867,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159320,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "T",
			"rawText": "T",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "tMgY2QAXpOSSOEhIC7m13",
			"originalText": "T",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 468,
			"versionNonce": 1255448413,
			"isDeleted": false,
			"id": "F5Gj3LdF",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3401.444044206887,
			"y": 1087.1076639589664,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 155,
			"height": 25,
			"seed": 593719459,
			"groupIds": [],
			"roundness": null,
			"boundElements": [
				{
					"id": "tMgY2QAXpOSSOEhIC7m13",
					"type": "arrow"
				}
			],
			"updated": 1686311159320,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "isValidn2 = true",
			"rawText": "isValidn2 = true",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "isValidn2 = true",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 253,
			"versionNonce": 1909281011,
			"isDeleted": false,
			"id": "F4nWbgvGJaBh17kYL8K45",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3167.5984765405733,
			"y": 1122.9295462193581,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 214,
			"height": 35,
			"seed": 1753375171,
			"groupIds": [],
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "RBLxe1zd"
				},
				{
					"id": "tCUQ5UZZYYSdl9rrsEiYa",
					"type": "arrow"
				}
			],
			"updated": 1686311159320,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 240,
			"versionNonce": 1495444413,
			"isDeleted": false,
			"id": "RBLxe1zd",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3193.5984765405733,
			"y": 1127.9295462193581,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 162,
			"height": 25,
			"seed": 2016540707,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159320,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "if both are valid",
			"rawText": "if both are valid",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "F4nWbgvGJaBh17kYL8K45",
			"originalText": "if both are valid",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 463,
			"versionNonce": 1081916051,
			"isDeleted": false,
			"id": "fGZJVeZ2RMZSsjNLOaONk",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3169.912295777578,
			"y": 1390.8805657059283,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 256,
			"height": 35,
			"seed": 624978595,
			"groupIds": [],
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "6xdptmqX"
				}
			],
			"updated": 1686311159320,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 453,
			"versionNonce": 514862109,
			"isDeleted": false,
			"id": "6xdptmqX",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3181.412295777578,
			"y": 1395.8805657059283,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 233,
			"height": 25,
			"seed": 1096026851,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159320,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "elseif nums1 is valid only",
			"rawText": "elseif nums1 is valid only",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "fGZJVeZ2RMZSsjNLOaONk",
			"originalText": "elseif nums1 is valid only",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 502,
			"versionNonce": 80605235,
			"isDeleted": false,
			"id": "2oExhjpWJ0TEAGn-5B6u5",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3168.8011205396606,
			"y": 1488.2171418809949,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 255,
			"height": 35,
			"seed": 1620364483,
			"groupIds": [],
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "P8WmMKNf"
				}
			],
			"updated": 1686311159320,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 516,
			"versionNonce": 1802412157,
			"isDeleted": false,
			"id": "P8WmMKNf",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3175.3011205396606,
			"y": 1493.2171418809949,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 242,
			"height": 25,
			"seed": 2094676333,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159320,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "elseif nums2 is valid only",
			"rawText": "elseif nums2 is valid only",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "2oExhjpWJ0TEAGn-5B6u5",
			"originalText": "elseif nums2 is valid only",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 437,
			"versionNonce": 1084715475,
			"isDeleted": false,
			"id": "0CSwFNPUiCrRW9YSkSg-O",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3168.6409366144053,
			"y": 1588.3184393966644,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 216,
			"height": 36,
			"seed": 1674799811,
			"groupIds": [],
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "jOCb8bFq"
				}
			],
			"updated": 1686311159320,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 473,
			"versionNonce": 354388189,
			"isDeleted": false,
			"id": "jOCb8bFq",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3177.6409366144053,
			"y": 1593.8184393966644,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 198,
			"height": 25,
			"seed": 1743479555,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159320,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "elseif none are valid",
			"rawText": "elseif none are valid",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "0CSwFNPUiCrRW9YSkSg-O",
			"originalText": "elseif none are valid",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "arrow",
			"version": 1761,
			"versionNonce": 1965014899,
			"isDeleted": false,
			"id": "tCUQ5UZZYYSdl9rrsEiYa",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3198.4389204097993,
			"y": 1160.742016836488,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 74.89575730779643,
			"height": 16.658081316209064,
			"seed": 1926303331,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "riqi57Pn"
				}
			],
			"updated": 1686311159320,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "F4nWbgvGJaBh17kYL8K45",
				"gap": 2.8124706171297476,
				"focus": 0.9020072288344891
			},
			"endBinding": {
				"elementId": "ooh6jp6Ly6WS40SMvEPYw",
				"gap": 1,
				"focus": -0.2824137943528526
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					74.89575730779643,
					16.658081316209064
				]
			]
		},
		{
			"type": "text",
			"version": 232,
			"versionNonce": 1028941117,
			"isDeleted": false,
			"id": "riqi57Pn",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3309.203428898447,
			"y": 1243.9322816071458,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 16,
			"height": 25,
			"seed": 117918211,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159320,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "T",
			"rawText": "T",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "tCUQ5UZZYYSdl9rrsEiYa",
			"originalText": "T",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 244,
			"versionNonce": 1014847763,
			"isDeleted": false,
			"id": "FfAoqAbR",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3323.836889036106,
			"y": 1225.8674216055151,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 265,
			"height": 50,
			"seed": 874753965,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159320,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "eleStack.push(nums1[index1])\nindex1++",
			"rawText": "eleStack.push(nums1[index1])\nindex1++",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "eleStack.push(nums1[index1])\nindex1++",
			"lineHeight": 1.25,
			"baseline": 42
		},
		{
			"type": "text",
			"version": 150,
			"versionNonce": 1466873245,
			"isDeleted": false,
			"id": "xAtyoG4x",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3324.539481474448,
			"y": 1335.8477846410292,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 283,
			"height": 50,
			"seed": 1267877827,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159320,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "eleStack.push(nums2[index2])\nindex2++",
			"rawText": "eleStack.push(nums2[index2])\nindex2++",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "eleStack.push(nums2[index2])\nindex2++",
			"lineHeight": 1.25,
			"baseline": 42
		},
		{
			"type": "rectangle",
			"version": 459,
			"versionNonce": 607567539,
			"isDeleted": false,
			"id": "ooh6jp6Ly6WS40SMvEPYw",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3265.712608293535,
			"y": 1178.400098152697,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 315,
			"height": 35,
			"seed": 2008385165,
			"groupIds": [],
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "XtkzbQgg"
				},
				{
					"id": "tCUQ5UZZYYSdl9rrsEiYa",
					"type": "arrow"
				}
			],
			"updated": 1686311159320,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 461,
			"versionNonce": 1855977981,
			"isDeleted": false,
			"id": "XtkzbQgg",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3275.712608293535,
			"y": 1183.400098152697,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 295,
			"height": 25,
			"seed": 961118627,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159321,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "if nums1[index] < nums2[index]",
			"rawText": "if nums1[index] < nums2[index]",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "ooh6jp6Ly6WS40SMvEPYw",
			"originalText": "if nums1[index] < nums2[index]",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 185,
			"versionNonce": 1190293587,
			"isDeleted": false,
			"id": "_7BUXEGFi2P67k22K--OT",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3262.0230853570824,
			"y": 1287.566687029458,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 81,
			"height": 35,
			"seed": 19780771,
			"groupIds": [],
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "ywBQiAMy"
				}
			],
			"updated": 1686311159321,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 163,
			"versionNonce": 736735837,
			"isDeleted": false,
			"id": "ywBQiAMy",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3283.5230853570824,
			"y": 1292.566687029458,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 38,
			"height": 25,
			"seed": 2116974061,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159321,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "else",
			"rawText": "else",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "_7BUXEGFi2P67k22K--OT",
			"originalText": "else",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 193,
			"versionNonce": 646376947,
			"isDeleted": false,
			"id": "j7MZjHWE",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3265.7845285014378,
			"y": 1436.3277932694386,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 265,
			"height": 50,
			"seed": 1609439299,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159321,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "eleStack.push(nums1[index1])\nindex1++",
			"rawText": "eleStack.push(nums1[index1])\nindex1++",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "eleStack.push(nums1[index1])\nindex1++",
			"lineHeight": 1.25,
			"baseline": 42
		},
		{
			"type": "text",
			"version": 219,
			"versionNonce": 471686845,
			"isDeleted": false,
			"id": "wkFv7olp",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3261.59002726039,
			"y": 1535.8556312346623,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 283,
			"height": 50,
			"seed": 832550467,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159321,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "eleStack.push(nums2[index2])\nindex2++",
			"rawText": "eleStack.push(nums2[index2])\nindex2++",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "eleStack.push(nums2[index2])\nindex2++",
			"lineHeight": 1.25,
			"baseline": 42
		},
		{
			"type": "text",
			"version": 147,
			"versionNonce": 1174058899,
			"isDeleted": false,
			"id": "r1sCVGVw",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3251.201144305474,
			"y": 1632.4111418615612,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 198,
			"height": 25,
			"seed": 713712269,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159321,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "shouldn't reach here",
			"rawText": "shouldn't reach here",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "shouldn't reach here",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 195,
			"versionNonce": 903642909,
			"isDeleted": false,
			"id": "WjtWYwuI",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3172.1019907565224,
			"y": 1670.1719080923663,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 170,
			"height": 50,
			"seed": 945273133,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159321,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "isValudn1 = false\nisvaludn2 = false",
			"rawText": "isValudn1 = false\nisvaludn2 = false",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "isValudn1 = false\nisvaludn2 = false",
			"lineHeight": 1.25,
			"baseline": 42
		},
		{
			"type": "rectangle",
			"version": 300,
			"versionNonce": 59002163,
			"isDeleted": false,
			"id": "24UqiNGq9eeFBj3aB3qAk",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3134.467059464669,
			"y": 1763.3305675278207,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 148,
			"height": 41,
			"seed": 854405155,
			"groupIds": [],
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "LQuSoN04"
				},
				{
					"id": "osa6nrY0KSmvJYt2rwk94",
					"type": "arrow"
				}
			],
			"updated": 1686311159321,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 283,
			"versionNonce": 530092925,
			"isDeleted": false,
			"id": "LQuSoN04",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3167.467059464669,
			"y": 1771.3305675278207,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 82,
			"height": 25,
			"seed": 1000015683,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159321,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "if isEven",
			"rawText": "if isEven",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "24UqiNGq9eeFBj3aB3qAk",
			"originalText": "if isEven",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 341,
			"versionNonce": 847916755,
			"isDeleted": false,
			"id": "42KrUdP5Q62fr28MiumSp",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3136.0622597762394,
			"y": 1882.949629679049,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 93,
			"height": 35,
			"seed": 1010338371,
			"groupIds": [],
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "tjyHz7s2"
				}
			],
			"updated": 1686311159321,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 319,
			"versionNonce": 898833373,
			"isDeleted": false,
			"id": "tjyHz7s2",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3163.5622597762394,
			"y": 1887.949629679049,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 38,
			"height": 25,
			"seed": 1291861123,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159321,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "else",
			"rawText": "else",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "42KrUdP5Q62fr28MiumSp",
			"originalText": "else",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 388,
			"versionNonce": 1973607539,
			"isDeleted": false,
			"id": "Gm1AkSqTnSSEvgKfZJj6E",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3238.300418229317,
			"y": 1828.1638601710497,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 345,
			"height": 35,
			"seed": 1058840003,
			"groupIds": [
				"r1V5L-BUxLmvY9BWxChLg"
			],
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "ykpUG89g"
				},
				{
					"id": "osa6nrY0KSmvJYt2rwk94",
					"type": "arrow"
				}
			],
			"updated": 1686311159321,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 290,
			"versionNonce": 1339922493,
			"isDeleted": false,
			"id": "ykpUG89g",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3246.300418229317,
			"y": 1833.1638601710497,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 329,
			"height": 25,
			"seed": 1213441389,
			"groupIds": [
				"r1V5L-BUxLmvY9BWxChLg"
			],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159321,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "return stack.pop + stack.pop / 2",
			"rawText": "return stack.pop + stack.pop / 2",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "Gm1AkSqTnSSEvgKfZJj6E",
			"originalText": "return stack.pop + stack.pop / 2",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 254,
			"versionNonce": 1486149139,
			"isDeleted": false,
			"id": "aFbGw03W-6f5MjoXC1DGg",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3230.1337159588097,
			"y": 1817.6638906886278,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 362.0000712076826,
			"height": 55.33335367838572,
			"seed": 25024621,
			"groupIds": [
				"r1V5L-BUxLmvY9BWxChLg"
			],
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1686311159321,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 304,
			"versionNonce": 1213827229,
			"isDeleted": false,
			"id": "TcT_-nY5FHnmdLQaXGkdi",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3239.0622445174504,
			"y": 1943.949558471366,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 177,
			"height": 35,
			"seed": 2016599555,
			"groupIds": [
				"86EIrOeeLIRUSNrxTocmH"
			],
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "78kTVTN0"
				}
			],
			"updated": 1686311159321,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 298,
			"versionNonce": 710319027,
			"isDeleted": false,
			"id": "78kTVTN0",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3247.0622445174504,
			"y": 1948.949558471366,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 161,
			"height": 25,
			"seed": 681344099,
			"groupIds": [
				"86EIrOeeLIRUSNrxTocmH"
			],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159321,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "return stack.pop",
			"rawText": "return stack.pop",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "TcT_-nY5FHnmdLQaXGkdi",
			"originalText": "return stack.pop",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 358,
			"versionNonce": 1085828349,
			"isDeleted": false,
			"id": "aXyPKy6cVCZ6zr-Pav_gH",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3227.5621377059274,
			"y": 1934.6162963457145,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 198.66668701171878,
			"height": 52.000020345052235,
			"seed": 667830083,
			"groupIds": [
				"86EIrOeeLIRUSNrxTocmH"
			],
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1686311159321,
			"link": null,
			"locked": false
		},
		{
			"type": "line",
			"version": 167,
			"versionNonce": 386837843,
			"isDeleted": false,
			"id": "uIMjJQ-ZKVhZYVY4sCQaW",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3125.3241529123993,
			"y": 1746.092533324881,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 597.7144077845987,
			"height": 0,
			"seed": 1981030381,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1686311159321,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					597.7144077845987,
					0
				]
			]
		},
		{
			"type": "line",
			"version": 187,
			"versionNonce": 679200093,
			"isDeleted": false,
			"id": "T7oKNkEsLSgfx0eeNfCQ6",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3711.6099892684283,
			"y": 1743.562138182317,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 0,
			"height": 814.0410857447125,
			"seed": 316893283,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1686311159321,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					0,
					-814.0410857447125
				]
			]
		},
		{
			"type": "arrow",
			"version": 588,
			"versionNonce": 34835187,
			"isDeleted": false,
			"id": "osa6nrY0KSmvJYt2rwk94",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3176.8582591463382,
			"y": 1813.8478699066477,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 58.857116699218295,
			"height": 35.99997384207586,
			"seed": 2006323949,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "WAyHZxe1"
				}
			],
			"updated": 1686311159322,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "24UqiNGq9eeFBj3aB3qAk",
				"gap": 9.517302378827026,
				"focus": 0.7504446726771345
			},
			"endBinding": {
				"elementId": "Gm1AkSqTnSSEvgKfZJj6E",
				"gap": 2.5850423837605376,
				"focus": -0.9046020236919887
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					58.857116699218295,
					35.99997384207586
				]
			]
		},
		{
			"type": "text",
			"version": 181,
			"versionNonce": 49615293,
			"isDeleted": false,
			"id": "WAyHZxe1",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3198.286817495947,
			"y": 1819.3478568276855,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 16,
			"height": 25,
			"seed": 1878170605,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159322,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "T",
			"rawText": "T",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "osa6nrY0KSmvJYt2rwk94",
			"originalText": "T",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 366,
			"versionNonce": 535540883,
			"isDeleted": false,
			"id": "PhwtVNwT",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3042.7030564964734,
			"y": -446.31762126586193,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 189,
			"height": 25,
			"seed": 950480387,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159322,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "IMPLEMENTATION",
			"rawText": "IMPLEMENTATION",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "IMPLEMENTATION",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 388,
			"versionNonce": 1833292317,
			"isDeleted": false,
			"id": "Dy4mZlvk",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3018.339616185158,
			"y": -396.6206330733909,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 374,
			"height": 25,
			"seed": 1480095139,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159322,
			"link": "[[LeetCode/Questions#Solution 4]]",
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "📍[[LeetCode/Questions#Solution 4]]",
			"rawText": "[[LeetCode/Questions#Solution 4]]",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "📍[[LeetCode/Questions#Solution 4]]",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "line",
			"version": 125,
			"versionNonce": 1347267123,
			"isDeleted": false,
			"id": "AzID4SCf40YPXqgSQu0YC",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3791.916817832794,
			"y": -473.3280757060353,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 0,
			"height": 1992.0000203450518,
			"seed": 2049888973,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1686311159322,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					0,
					1992.0000203450518
				]
			]
		},
		{
			"type": "text",
			"version": 26,
			"versionNonce": 1683981949,
			"isDeleted": false,
			"id": "g10tFFxD",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3893.788241707351,
			"y": -457.97165018998015,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 352,
			"height": 50,
			"seed": 264676635,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159322,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "## 5. Longest Palindromic substring\n",
			"rawText": "## 5. Longest Palindromic substring\n",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "## 5. Longest Palindromic substring\n",
			"lineHeight": 1.25,
			"baseline": 42
		},
		{
			"type": "text",
			"version": 406,
			"versionNonce": 941616083,
			"isDeleted": false,
			"id": "0nS4OByO",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4376.929541176652,
			"y": -475.764548040556,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 189,
			"height": 25,
			"seed": 902503861,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159322,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "IMPLEMENTATION",
			"rawText": "IMPLEMENTATION",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "IMPLEMENTATION",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 466,
			"versionNonce": 1258532573,
			"isDeleted": false,
			"id": "Q4qt0CVq",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4401.559523429674,
			"y": -435.06096246629363,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 373,
			"height": 25,
			"seed": 442998549,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159322,
			"link": "[[LeetCode/Questions#Solution 5]]",
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "📍[[LeetCode/Questions#Solution 5]]",
			"rawText": "[[LeetCode/Questions#Solution 5]]",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "📍[[LeetCode/Questions#Solution 5]]",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 53,
			"versionNonce": 460913011,
			"isDeleted": false,
			"id": "XL6MFY2i",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3889.3437972629054,
			"y": -379.3049292698412,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 50,
			"height": 25,
			"seed": 987794267,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159322,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "INFO",
			"rawText": "INFO",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "INFO",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 205,
			"versionNonce": 801360701,
			"isDeleted": false,
			"id": "iPySBb4F",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3931.9936945203954,
			"y": -330.1438456245501,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 516,
			"height": 150,
			"seed": 4017941,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159322,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "- Get the longest palindrome out of the given string\n- s: String\n    - between 1 and 1000 chars\n    - only digits and English letters\n\n> String longestPalindrome(String s) <",
			"rawText": "- Get the longest palindrome out of the given string\n- s: String\n    - between 1 and 1000 chars\n    - only digits and English letters\n\n> String longestPalindrome(String s) <",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "- Get the longest palindrome out of the given string\n- s: String\n    - between 1 and 1000 chars\n    - only digits and English letters\n\n> String longestPalindrome(String s) <",
			"lineHeight": 1.25,
			"baseline": 142
		},
		{
			"type": "text",
			"version": 32,
			"versionNonce": 2006930195,
			"isDeleted": false,
			"id": "6OXOtOz9",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3904.7436716322118,
			"y": -119.89384943924739,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 91,
			"height": 25,
			"seed": 1316717973,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159322,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "EXAMPLE",
			"rawText": "EXAMPLE",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "EXAMPLE",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 92,
			"versionNonce": 1392597917,
			"isDeleted": false,
			"id": "uTeXJ0gs",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3949.927189437896,
			"y": -65.98319460806835,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 405,
			"height": 75,
			"seed": 803489115,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159322,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Input: s = \"babad\"\nOutput: \"bab\"\nExplanation: \"aba\" is also a valid answer.",
			"rawText": "Input: s = \"babad\"\nOutput: \"bab\"\nExplanation: \"aba\" is also a valid answer.",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Input: s = \"babad\"\nOutput: \"bab\"\nExplanation: \"aba\" is also a valid answer.",
			"lineHeight": 1.25,
			"baseline": 67
		},
		{
			"type": "text",
			"version": 27,
			"versionNonce": 1560901811,
			"isDeleted": false,
			"id": "ME505CXW",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4422.868401811517,
			"y": -96.80677428407927,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 33,
			"height": 25,
			"seed": 69783323,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159322,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "s =",
			"rawText": "s =",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "s =",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "freedraw",
			"version": 101,
			"versionNonce": 1827528701,
			"isDeleted": false,
			"id": "PkGFW9EoKVvo-ENh4njzI",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4485.362437736431,
			"y": -104.7126621079584,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 11.199979313015458,
			"height": 30.635277448383096,
			"seed": 1122452181,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159322,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					-2.635278901600551
				],
				[
					-0.32938158906320225,
					-2.635278901600551
				],
				[
					-1.3176268847393398,
					-0.6588134423696699
				],
				[
					-1.9764403271090096,
					2.3058973125375477
				],
				[
					-2.6353040337225817,
					6.588234952184105
				],
				[
					-3.6234990651554537,
					11.200004445137369
				],
				[
					-3.9529309184619215,
					15.152960495720961
				],
				[
					-3.9529309184619215,
					18.77648469299789
				],
				[
					-3.6234990651554537,
					21.741195447905106
				],
				[
					-3.6234990651554537,
					24.047067628320782
				],
				[
					-3.6234990651554537,
					25.03531292399716
				],
				[
					-3.6234990651554537,
					25.69412636636683
				],
				[
					-3.6234990651554537,
					26.352939808736497
				],
				[
					-3.2941174760922514,
					27.01177838322804
				],
				[
					-2.9646856227857836,
					27.67059182559771
				],
				[
					-1.9764403271090096,
					27.999998546782546
				],
				[
					-0.32938158906320225,
					27.999998546782546
				],
				[
					2.964735887029049,
					27.67059182559771
				],
				[
					4.941176214138059,
					27.01177838322804
				],
				[
					6.2588533631213,
					26.023533087551662
				],
				[
					6.9176668054909705,
					25.03531292399716
				],
				[
					7.247048394553536,
					22.400008890274776
				],
				[
					6.9176668054909705,
					19.764704856552353
				],
				[
					6.2588533631213,
					17.78823939732151
				],
				[
					4.6117946250748565,
					16.4705873804603
				],
				[
					2.6353040337225817,
					16.141180659275467
				],
				[
					-0.6588134423696699,
					15.811773938090631
				],
				[
					-2.305872180416114,
					15.482367216905796
				],
				[
					-2.6353040337225817,
					15.482367216905796
				],
				[
					-2.9646856227857836,
					15.482367216905796
				],
				[
					-1.647058738046444,
					15.811773938090631
				],
				[
					0.3294318533064676,
					15.811773938090631
				],
				[
					0.3294318533064676,
					15.811773938090631
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2255859375,
				0.3798828125,
				0.453125,
				0.5126953125,
				0.515625,
				0.5234375,
				0.52734375,
				0.52734375,
				0.529296875,
				0.529296875,
				0.53125,
				0.537109375,
				0.5390625,
				0.5390625,
				0.5390625,
				0.5390625,
				0.5390625,
				0.5458984375,
				0.5380859375,
				0.5361328125,
				0.5302734375,
				0.5283203125,
				0.53515625,
				0.5390625,
				0.541015625,
				0.54296875,
				0.5458984375,
				0.5556640625,
				0.5615234375,
				0.5615234375,
				0.5615234375,
				0.38671875,
				0.0146484375,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 95,
			"versionNonce": 157149779,
			"isDeleted": false,
			"id": "Ts7nFVu4n2Bt4ButMGevD",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4535.433013320182,
			"y": -91.53619220359015,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 16.141155527153515,
			"height": 15.15293536359913,
			"seed": 2072171419,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159322,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.3293815890625656,
					-0.9882201635545048
				],
				[
					-1.6470587380458073,
					-1.3176268847393398
				],
				[
					-3.623499065154817,
					-0.6588134423696699
				],
				[
					-7.905861836923206,
					1.3176520168612111
				],
				[
					-9.882352428276118,
					3.2941174760920524
				],
				[
					-11.858792755385128,
					5.929421509814475
				],
				[
					-13.17646990436837,
					8.894132264721692
				],
				[
					-13.505851493430935,
					11.200004445137369
				],
				[
					-13.17646990436837,
					12.847063183183415
				],
				[
					-11.199979313015458,
					13.176469904368249
				],
				[
					-9.223488721662546,
					12.51765646199858
				],
				[
					-7.247048394553536,
					10.870597723952534
				],
				[
					-5.270557803200624,
					8.564725543536857
				],
				[
					-3.9529309184612846,
					4.941176214138099
				],
				[
					-3.623499065154817,
					3.6235493293987586
				],
				[
					-3.623499065154817,
					2.9647107549072174
				],
				[
					-4.2823125075244866,
					5.60001478862964
				],
				[
					-3.9529309184612846,
					8.23529369023015
				],
				[
					-3.2941174760916145,
					9.882352428276198
				],
				[
					-2.305872180415477,
					11.529411166322204
				],
				[
					-0.9881950314322354,
					12.51765646199858
				],
				[
					-0.9881950314322354,
					12.847063183183415
				],
				[
					0,
					13.176469904368249
				],
				[
					0.6588637066135719,
					13.505901757674955
				],
				[
					1.9764905913529116,
					13.83530847885979
				],
				[
					2.6353040337225817,
					13.505901757674955
				],
				[
					2.6353040337225817,
					13.505901757674955
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.1142578125,
				0.28515625,
				0.3994140625,
				0.4423828125,
				0.4794921875,
				0.4912109375,
				0.5078125,
				0.51171875,
				0.51953125,
				0.521484375,
				0.521484375,
				0.5185546875,
				0.515625,
				0.513671875,
				0.5166015625,
				0.521484375,
				0.5263671875,
				0.5537109375,
				0.5576171875,
				0.5673828125,
				0.5673828125,
				0.5693359375,
				0.5673828125,
				0.5341796875,
				0.462890625,
				0.19921875,
				0.0556640625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 95,
			"versionNonce": 864737373,
			"isDeleted": false,
			"id": "I58v-9pNybIwHEprqzAQO",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4581.221276396408,
			"y": -112.28911722369705,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 12.517606197754796,
			"height": 31.952954597366098,
			"seed": 1931849429,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159322,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					-0.6588385744915015
				],
				[
					-0.3294318533071043,
					0.6588134423696699
				],
				[
					-0.3294318533071043,
					4.941176214138099
				],
				[
					-0.6588134423696699,
					10.211759149461033
				],
				[
					-0.6588134423696699,
					16.141180659275506
				],
				[
					-0.6588134423696699,
					20.7529250201069
				],
				[
					-0.3294318533071043,
					24.04704249619895
				],
				[
					0.3293815890625656,
					27.01175325110621
				],
				[
					1.3176268847393398,
					29.64705728482859
				],
				[
					1.9764403271090096,
					30.635277448383096
				],
				[
					2.9646856227851472,
					31.294116022874597
				],
				[
					4.282362771768389,
					31.294116022874597
				],
				[
					7.247048394553536,
					30.30587072719826
				],
				[
					9.223538985906448,
					28.98821871033705
				],
				[
					10.870597723952255,
					27.01175325110621
				],
				[
					11.529411166321925,
					25.694101234244997
				],
				[
					11.858792755385128,
					24.376474349505656
				],
				[
					11.199979313015458,
					22.07057703696811
				],
				[
					10.541165870645788,
					20.7529250201069
				],
				[
					8.894107132599343,
					19.764704856552395
				],
				[
					4.941176214138059,
					19.764704856552395
				],
				[
					2.9646856227851472,
					20.7529250201069
				],
				[
					1.6470587380458073,
					21.741170315783275
				],
				[
					1.3176268847393398,
					22.399983758152946
				],
				[
					1.6470587380458073,
					23.058822332644446
				],
				[
					3.2941174760916145,
					23.38822905382928
				],
				[
					3.2941174760916145,
					23.38822905382928
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2568359375,
				0.412109375,
				0.4462890625,
				0.478515625,
				0.490234375,
				0.4951171875,
				0.4970703125,
				0.4970703125,
				0.4970703125,
				0.5009765625,
				0.5068359375,
				0.5126953125,
				0.5126953125,
				0.5166015625,
				0.513671875,
				0.513671875,
				0.513671875,
				0.51953125,
				0.5234375,
				0.525390625,
				0.525390625,
				0.52734375,
				0.537109375,
				0.5400390625,
				0.5400390625,
				0.330078125,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 87,
			"versionNonce": 1098065907,
			"isDeleted": false,
			"id": "jEbSSac8rG0k5X9UIMjrv",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4634.256537602943,
			"y": -97.13618186009792,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 23.388254185950952,
			"height": 19.764704856552395,
			"seed": 1000681915,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159322,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-7.5764299836161015,
					5.270582935322934
				],
				[
					-9.552920574969013,
					9.882352428276198
				],
				[
					-9.552920574969013,
					12.847063183183415
				],
				[
					-8.894107132599343,
					15.15293536359913
				],
				[
					-6.917616541246431,
					15.811773938090631
				],
				[
					-3.9529309184612846,
					15.482342084783966
				],
				[
					0.3294318533071043,
					12.188224608691874
				],
				[
					1.647058738046444,
					9.882352428276198
				],
				[
					2.3059224446600157,
					7.576480247860481
				],
				[
					2.6353040337225817,
					4.941176214138099
				],
				[
					3.2941174760922514,
					2.9647107549072174
				],
				[
					3.6235493293993555,
					4.611769492953264
				],
				[
					3.6235493293993555,
					7.576480247860481
				],
				[
					3.6235493293993555,
					10.211759149461033
				],
				[
					4.941176214138696,
					14.49412192122946
				],
				[
					6.2588533631213,
					16.799994101645137
				],
				[
					7.905912101167744,
					18.44705283969118
				],
				[
					13.835333610981941,
					19.764704856552395
				],
				[
					13.835333610981941,
					19.764704856552395
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2255859375,
				0.3681640625,
				0.4580078125,
				0.4775390625,
				0.4814453125,
				0.484375,
				0.484375,
				0.4794921875,
				0.4814453125,
				0.4912109375,
				0.505859375,
				0.517578125,
				0.55078125,
				0.548828125,
				0.5537109375,
				0.5595703125,
				0.5537109375,
				0.5107421875,
				0.0146484375,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 97,
			"versionNonce": 547996861,
			"isDeleted": false,
			"id": "MmNZD-a0xfiHDAfsBpE7S",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4674.444811022662,
			"y": -112.28911722369705,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 15.811773938090314,
			"height": 36.56469895819753,
			"seed": 599538997,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159322,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.3294318533071043,
					-0.9882452956763365
				],
				[
					0.6588134423696699,
					1.6470587380460462
				],
				[
					2.6352537694786795,
					5.929396377692603
				],
				[
					4.2823125075244866,
					11.529411166322243
				],
				[
					5.599989656507729,
					17.12940082283001
				],
				[
					6.588234952183866,
					21.082356873413605
				],
				[
					6.917616541247068,
					24.04704249619895
				],
				[
					7.247048394553536,
					27.01175325110621
				],
				[
					7.247048394553536,
					29.317650563643756
				],
				[
					7.247048394553536,
					31.294116022874597
				],
				[
					6.917616541247068,
					33.27058148210548
				],
				[
					6.258803098877398,
					33.599988203290316
				],
				[
					4.611744360830954,
					35.24704694133636
				],
				[
					2.9646856227851472,
					35.576453662521196
				],
				[
					0.6588134423696699,
					35.24704694133636
				],
				[
					-3.2941174760922514,
					33.92939492447515
				],
				[
					-5.270608067445163,
					32.941174760920646
				],
				[
					-6.9176668054909705,
					30.964709301689762
				],
				[
					-7.905912101167108,
					29.317650563643756
				],
				[
					-8.564725543536778,
					27.67059182559771
				],
				[
					-7.905912101167108,
					25.694101234244997
				],
				[
					-6.2588533631213,
					24.04704249619895
				],
				[
					-4.611794625075493,
					23.38822905382928
				],
				[
					-2.3059224446593793,
					23.058822332644446
				],
				[
					1.9764403271090096,
					22.72941561145961
				],
				[
					3.9529309184612846,
					22.72941561145961
				],
				[
					5.599989656507729,
					22.72941561145961
				],
				[
					6.588234952183866,
					23.058822332644446
				],
				[
					6.588234952183866,
					23.058822332644446
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.3671875,
				0.4072265625,
				0.5107421875,
				0.50390625,
				0.5,
				0.498046875,
				0.49609375,
				0.498046875,
				0.498046875,
				0.498046875,
				0.49609375,
				0.5029296875,
				0.5078125,
				0.5126953125,
				0.5146484375,
				0.51953125,
				0.5361328125,
				0.5498046875,
				0.5546875,
				0.5595703125,
				0.5615234375,
				0.5615234375,
				0.556640625,
				0.5546875,
				0.5546875,
				0.55078125,
				0.51171875,
				0.40625,
				0.015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 97,
			"versionNonce": 1800384915,
			"isDeleted": false,
			"id": "EtG5PL2LTBQEp2dAAxBFp",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4474.491789748234,
			"y": -57.60677214699305,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 111.01177402357568,
			"height": 12.188249740813745,
			"seed": 2095742459,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159323,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.32940672118483494,
					0
				],
				[
					1.9764905913529116,
					-0.6588385744915413
				],
				[
					4.941176214138696,
					-0.9882452956763762
				],
				[
					9.552970839213552,
					-1.6470587380460462
				],
				[
					14.164715200045142,
					-2.9647107549072174
				],
				[
					19.76470485655287,
					-3.6235241972768875
				],
				[
					25.364694513060602,
					-3.9529560505835937
				],
				[
					29.976489138135456,
					-4.282362771768429
				],
				[
					35.24704694133672,
					-4.611769492953264
				],
				[
					40.84708686208835,
					-5.270582935322934
				],
				[
					46.11764466528897,
					-5.60001478862964
				],
				[
					55.34118365119542,
					-6.91764167336898
				],
				[
					59.95292801202701,
					-7.905886969045316
				],
				[
					65.8823495218412,
					-8.564700411414986
				],
				[
					70.4941441469167,
					-8.894132264721692
				],
				[
					76.42351539248763,
					-9.552945707091363
				],
				[
					81.3646916066257,
					-9.552945707091363
				],
				[
					85.31767278933087,
					-9.882352428276198
				],
				[
					88.28235841211666,
					-10.211759149461033
				],
				[
					91.90590774151474,
					-10.541191002767698
				],
				[
					97.17646554471601,
					-10.870597723952534
				],
				[
					100.14120143174506,
					-11.529411166322204
				],
				[
					102.77645520122373,
					-11.858817887507039
				],
				[
					105.08237764588311,
					-11.858817887507039
				],
				[
					109.36469015340823,
					-11.858817887507039
				],
				[
					110.68236730239084,
					-11.858817887507039
				],
				[
					110.35293544908437,
					-12.188249740813745
				],
				[
					108.70587671103857,
					-11.858817887507039
				],
				[
					108.70587671103857,
					-11.858817887507039
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.322265625,
				0.4609375,
				0.482421875,
				0.4912109375,
				0.4931640625,
				0.4951171875,
				0.4970703125,
				0.5078125,
				0.5107421875,
				0.5107421875,
				0.5185546875,
				0.521484375,
				0.525390625,
				0.525390625,
				0.529296875,
				0.53515625,
				0.5400390625,
				0.5400390625,
				0.5400390625,
				0.5400390625,
				0.546875,
				0.5517578125,
				0.5556640625,
				0.5595703125,
				0.556640625,
				0.5673828125,
				0.5703125,
				0.4794921875,
				0.0166015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 108,
			"versionNonce": 2011964701,
			"isDeleted": false,
			"id": "whh8a2rJwVxX7peActiTN",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4529.5035415461225,
			"y": -50.0303170312544,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 115.29411166322244,
			"height": 12.847038051061583,
			"seed": 753626069,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159323,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					-0.6588134423696699
				],
				[
					0,
					-0.9882201635545048
				],
				[
					1.3176771489832417,
					-0.9882201635545048
				],
				[
					3.952981182705823,
					-1.3176268847393398
				],
				[
					5.60003992075163,
					-1.976465459230881
				],
				[
					8.564725543536778,
					-2.305872180415716
				],
				[
					12.188274872935496,
					-2.9646856227853857
				],
				[
					13.835333610981941,
					-3.2941174760920924
				],
				[
					16.47058738046062,
					-3.952930918461762
				],
				[
					19.435323267489668,
					-4.611744360831432
				],
				[
					24.705881070690292,
					-5.270582935322934
				],
				[
					30.305920991441923,
					-6.588234952184145
				],
				[
					34.58823349896705,
					-7.247048394553815
				],
				[
					40.188273419718044,
					-7.905861836923484
				],
				[
					44.80001778054963,
					-8.564700411415025
				],
				[
					52.04706617510317,
					-8.89410713259986
				],
				[
					57.317674242548335,
					-9.223513853784695
				],
				[
					61.60003701431672,
					-9.882352428276198
				],
				[
					66.87059481751734,
					-10.211759149461033
				],
				[
					71.48238944259283,
					-10.870572591830703
				],
				[
					77.74119254147024,
					-11.199979313015536
				],
				[
					83.01180060891477,
					-11.529411166322243
				],
				[
					86.96473152737668,
					-11.858817887507078
				],
				[
					92.23528933057794,
					-12.517631329876748
				],
				[
					95.52940680666956,
					-12.517631329876748
				],
				[
					98.82352428276181,
					-12.847038051061583
				],
				[
					101.1294467274212,
					-12.847038051061583
				],
				[
					102.77650546546764,
					-12.847038051061583
				],
				[
					104.75294579257664,
					-12.847038051061583
				],
				[
					107.71768167960569,
					-12.847038051061583
				],
				[
					109.69412200671471,
					-12.847038051061583
				],
				[
					111.3411807447605,
					-12.847038051061583
				],
				[
					112.98823948280632,
					-12.517631329876748
				],
				[
					113.64705292517598,
					-12.188224608691913
				],
				[
					114.30591663178956,
					-11.858817887507078
				],
				[
					114.63529822085276,
					-11.858817887507078
				],
				[
					114.96473007415923,
					-11.858817887507078
				],
				[
					115.29411166322244,
					-12.188224608691913
				],
				[
					115.29411166322244,
					-12.847038051061583
				],
				[
					115.29411166322244,
					-12.847038051061583
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.171875,
				0.2783203125,
				0.443359375,
				0.482421875,
				0.484375,
				0.490234375,
				0.4873046875,
				0.4931640625,
				0.4931640625,
				0.4951171875,
				0.4970703125,
				0.4970703125,
				0.4970703125,
				0.4970703125,
				0.494140625,
				0.494140625,
				0.4921875,
				0.4921875,
				0.4921875,
				0.4921875,
				0.4921875,
				0.4921875,
				0.494140625,
				0.49609375,
				0.49609375,
				0.498046875,
				0.5,
				0.5,
				0.5068359375,
				0.5087890625,
				0.5126953125,
				0.5126953125,
				0.5126953125,
				0.5166015625,
				0.515625,
				0.5107421875,
				0.498046875,
				0.4384765625,
				0.2060546875,
				0.017578125,
				0
			]
		},
		{
			"type": "text",
			"version": 53,
			"versionNonce": 1747584819,
			"isDeleted": false,
			"id": "iwtpZdPp",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3952.2800767598155,
			"y": 76.36967476233627,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 165,
			"height": 50,
			"seed": 575396283,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159323,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Input: s = \"cbbd\"\nOutput: \"bb\"",
			"rawText": "Input: s = \"cbbd\"\nOutput: \"bb\"",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Input: s = \"cbbd\"\nOutput: \"bb\"",
			"lineHeight": 1.25,
			"baseline": 42
		},
		{
			"type": "text",
			"version": 27,
			"versionNonce": 214137213,
			"isDeleted": false,
			"id": "mXhtfKSp",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4266.633014345983,
			"y": 102.72260875820024,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 33,
			"height": 25,
			"seed": 2097559963,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159323,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "s =",
			"rawText": "s =",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "s =",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "freedraw",
			"version": 100,
			"versionNonce": 778610899,
			"isDeleted": false,
			"id": "IW_AWpFdcBHS41gQH6EX4",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4356.283215737425,
			"y": 99.79114855114504,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 14.61207080550585,
			"height": 18.888792361875954,
			"seed": 904152629,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159323,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-5.702268217933944,
					1.781960517514321
				],
				[
					-7.840615400839677,
					2.851147704246807
				],
				[
					-9.266189252962844,
					4.98949488715211
				],
				[
					-10.691763105086011,
					7.12784207005737
				],
				[
					-11.760950291818926,
					9.266216443522342
				],
				[
					-12.473723622600804,
					11.76095029181854
				],
				[
					-12.473723622600804,
					13.899297474723843
				],
				[
					-12.117336957209865,
					15.681257992238164
				],
				[
					-11.404536435867888,
					16.75044517897065
				],
				[
					-9.622575918353782,
					18.176019031094075
				],
				[
					-8.197029256790028,
					18.532405696485014
				],
				[
					-6.415068739275921,
					18.888792361875954
				],
				[
					-3.9203077004198383,
					18.888792361875954
				],
				[
					-1.0691871867329166,
					18.532405696485014
				],
				[
					0,
					18.532405696485014
				],
				[
					0.7127733307818775,
					18.888792361875954
				],
				[
					2.1383471829050444,
					18.532405696485014
				],
				[
					2.1383471829050444,
					18.532405696485014
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2587890625,
				0.4521484375,
				0.4873046875,
				0.505859375,
				0.5185546875,
				0.52734375,
				0.537109375,
				0.54296875,
				0.548828125,
				0.5517578125,
				0.5615234375,
				0.5634765625,
				0.5654296875,
				0.5673828125,
				0.5634765625,
				0.552734375,
				0.5244140625,
				0.3359375,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 115,
			"versionNonce": 1215381981,
			"isDeleted": false,
			"id": "ZL5dtsa48sLXBe9GxNBMO",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4471.754262710467,
			"y": 76.26927515806754,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 15.681285182797488,
			"height": 39.5595180507066,
			"seed": 1264907835,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159323,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.3564138559503502,
					0.7128005213415474
				],
				[
					0.7127733307818777,
					4.276721556370233
				],
				[
					1.7819605175141056,
					11.760950291818583
				],
				[
					2.1383743734644556,
					19.601565692657832
				],
				[
					2.1383743734644556,
					24.234673914419
				],
				[
					2.1383743734644556,
					28.15498161483867
				],
				[
					2.1383743734644556,
					31.006129319085478
				],
				[
					2.4947338482959833,
					33.85724983277266
				],
				[
					2.4947338482959833,
					35.63921035028698
				],
				[
					2.4947338482959833,
					36.35201087162853
				],
				[
					2.4947338482959833,
					36.708397537019465
				],
				[
					2.1383743734644556,
					37.0647842024104
				],
				[
					1.7819605175141056,
					37.421170867801344
				],
				[
					0,
					38.13397138914284
				],
				[
					-2.1383743734651444,
					39.203131385315665
				],
				[
					-4.276694365810777,
					39.5595180507066
				],
				[
					-6.058654883324882,
					39.5595180507066
				],
				[
					-7.48425592600815,
					39.203131385315665
				],
				[
					-8.909802587571905,
					38.13397138914284
				],
				[
					-9.978989774304132,
					36.35201087162853
				],
				[
					-9.978989774304132,
					34.21363649816355
				],
				[
					-9.266216443522255,
					32.43167598064923
				],
				[
					-7.840615400839677,
					31.006129319085478
				],
				[
					-6.415068739275922,
					29.580555466962053
				],
				[
					-4.989467696592655,
					28.511368280229604
				],
				[
					-3.5639210350289,
					27.442208284056793
				],
				[
					-1.4255466615637553,
					27.085794428106183
				],
				[
					0,
					27.085794428106183
				],
				[
					0.7127733307818777,
					27.442208284056793
				],
				[
					2.4947338482959833,
					27.442208284056793
				],
				[
					4.276694365810089,
					27.442208284056793
				],
				[
					5.702295408493355,
					27.442208284056793
				],
				[
					5.702295408493355,
					27.442208284056793
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2802734375,
				0.4619140625,
				0.4912109375,
				0.5029296875,
				0.515625,
				0.513671875,
				0.513671875,
				0.5205078125,
				0.5322265625,
				0.537109375,
				0.548828125,
				0.5517578125,
				0.5654296875,
				0.560546875,
				0.544921875,
				0.5380859375,
				0.5361328125,
				0.5380859375,
				0.5380859375,
				0.5380859375,
				0.5380859375,
				0.5380859375,
				0.5380859375,
				0.5380859375,
				0.5302734375,
				0.5283203125,
				0.5263671875,
				0.5263671875,
				0.5263671875,
				0.5263671875,
				0.4921875,
				0.2763671875,
				0.0126953125,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 97,
			"versionNonce": 597825139,
			"isDeleted": false,
			"id": "LyHcuNdh-qvIx9usD0z8V",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4385.8637712043865,
			"y": 136.49954608816446,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 60.586684786047265,
			"height": 3.920307700419624,
			"seed": 1524985429,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159323,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-2.1383743734651444,
					0
				],
				[
					-1.7819605175147946,
					0.35638666539093883
				],
				[
					2.1383471829050444,
					0.7127733307818777
				],
				[
					8.197002066229928,
					0
				],
				[
					14.255656949554812,
					-0.35638666539093883
				],
				[
					17.463218509752185,
					-0.35638666539093883
				],
				[
					23.165459537126715,
					-1.0691871867324862
				],
				[
					41.34147856822088,
					-2.138347182905303
				],
				[
					49.5385078250109,
					-2.851147704246807
				],
				[
					54.88438937755391,
					-3.2075343696377456
				],
				[
					58.091896556631774,
					-2.851147704246807
				],
				[
					58.448310412582124,
					-2.851147704246807
				],
				[
					57.02270936989955,
					-2.4947338482962413
				],
				[
					54.88438937755391,
					-2.4947338482962413
				],
				[
					54.88438937755391,
					-2.4947338482962413
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2109375,
				0.3984375,
				0.5185546875,
				0.5126953125,
				0.5126953125,
				0.5126953125,
				0.5126953125,
				0.5126953125,
				0.51953125,
				0.5234375,
				0.525390625,
				0.52734375,
				0.52734375,
				0.3466796875,
				0.0146484375,
				0
			]
		},
		{
			"type": "text",
			"version": 50,
			"versionNonce": 1879506493,
			"isDeleted": false,
			"id": "C5VKkpwl",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3837.4565581189604,
			"y": 219.89912243007515,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 149,
			"height": 25,
			"seed": 699070709,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159323,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "WALKTHROUGH",
			"rawText": "WALKTHROUGH",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "WALKTHROUGH",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 75,
			"versionNonce": 916246547,
			"isDeleted": false,
			"id": "w5bjdWB9",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4279.103673589498,
			"y": 198.46122590102075,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 138,
			"height": 25,
			"seed": 1870630549,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159323,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "BRUTEFORCE",
			"rawText": "BRUTEFORCE",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "BRUTEFORCE",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 497,
			"versionNonce": 711339677,
			"isDeleted": false,
			"id": "Rgp0ljmA",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3840.99781765444,
			"y": 278.4088653164872,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 394,
			"height": 250,
			"seed": 1142195771,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159323,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "- curLongest = \" \"\n- if s.len < 2, return s\n- iterate string \n    - iterate string (from i to end)\n        - if len i to j is shorter than \n          curLong, skip\n        - curSub = all chars from i tp j\n        - if curSub isPalindrome\n            - curLongest = curSub\n            - j = curLongest.len - 1 ",
			"rawText": "- curLongest = \" \"\n- if s.len < 2, return s\n- iterate string \n    - iterate string (from i to end)\n        - if len i to j is shorter than \n          curLong, skip\n        - curSub = all chars from i tp j\n        - if curSub isPalindrome\n            - curLongest = curSub\n            - j = curLongest.len - 1 ",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "- curLongest = \" \"\n- if s.len < 2, return s\n- iterate string \n    - iterate string (from i to end)\n        - if len i to j is shorter than \n          curLong, skip\n        - curSub = all chars from i tp j\n        - if curSub isPalindrome\n            - curLongest = curSub\n            - j = curLongest.len - 1 ",
			"lineHeight": 1.25,
			"baseline": 242
		},
		{
			"type": "freedraw",
			"version": 48,
			"versionNonce": 961500595,
			"isDeleted": false,
			"id": "rK1EPsVDaQHSG7FsfX7KH",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4391.809199505104,
			"y": 79.66386780576426,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 14.117647058823422,
			"height": 38.11767578125,
			"seed": 1608055221,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159323,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.9411980124077672,
					4.235301298253717
				],
				[
					-1.8823601217827672,
					11.764705882352928
				],
				[
					-2.8235222311577672,
					18.823529411764696
				],
				[
					-3.2941391888780345,
					24.470609777113964
				],
				[
					-3.2941391888780345,
					32.94117647058823
				],
				[
					-3.2941391888780345,
					34.35295553768384
				],
				[
					-3.2941391888780345,
					35.29411764705884
				],
				[
					-3.2941391888780345,
					35.76473460477939
				],
				[
					-3.2941391888780345,
					36.70589671415439
				],
				[
					-2.3529411764702672,
					37.64705882352939
				],
				[
					-0.9411980124077672,
					38.11767578125
				],
				[
					2.3529411764711767,
					38.11767578125
				],
				[
					4.235301298253944,
					37.64705882352939
				],
				[
					7.058823529411711,
					36.23531565946689
				],
				[
					9.411764705882888,
					34.82353659237134
				],
				[
					10.823507869945388,
					32.47059541590073
				],
				[
					9.882345760570388,
					30.58823529411768
				],
				[
					7.529404584099211,
					29.17649213005518
				],
				[
					3.2941032858461767,
					27.764713062959572
				],
				[
					-0.4705810546875,
					29.17649213005518
				],
				[
					-2.3529411764702672,
					30.58823529411768
				],
				[
					-2.8235222311577672,
					32.00001436121323
				],
				[
					-1.4117790670952672,
					33.41179342830884
				],
				[
					-1.4117790670952672,
					33.41179342830884
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.318359375,
				0.49609375,
				0.51171875,
				0.5234375,
				0.525390625,
				0.5458984375,
				0.5517578125,
				0.5556640625,
				0.5595703125,
				0.5673828125,
				0.5595703125,
				0.5576171875,
				0.5556640625,
				0.5537109375,
				0.5498046875,
				0.544921875,
				0.5322265625,
				0.5302734375,
				0.53515625,
				0.5419921875,
				0.552734375,
				0.552734375,
				0.486328125,
				0.0185546875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 53,
			"versionNonce": 1178620669,
			"isDeleted": false,
			"id": "WkrfdA1CZ2lmOJQgAD73P",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4414.397413257401,
			"y": 77.3109266292937,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 15.058809168199332,
			"height": 38.58825683593744,
			"seed": 453747605,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159323,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.4705810546875,
					3.7647202435661598
				],
				[
					-0.4705810546875,
					8.47060259650732
				],
				[
					-0.941162109375,
					16.470588235294088
				],
				[
					-1.4117431640625,
					22.588249655330856
				],
				[
					-1.4117431640625,
					26.352969898897015
				],
				[
					-1.4117431640625,
					29.647073184742624
				],
				[
					-0.941162109375,
					33.41179342830878
				],
				[
					-0.941162109375,
					35.29411764705878
				],
				[
					-0.941162109375,
					36.23531565946689
				],
				[
					-0.941162109375,
					37.64705882352939
				],
				[
					-0.4705810546875,
					38.11767578124994
				],
				[
					-0.4705810546875,
					38.58825683593744
				],
				[
					0,
					38.58825683593744
				],
				[
					1.8823601217836767,
					38.58825683593744
				],
				[
					3.764720243566444,
					38.11767578124994
				],
				[
					7.058823529411711,
					37.17647776884189
				],
				[
					9.411764705882888,
					35.76473460477939
				],
				[
					11.764705882353155,
					34.35295553768378
				],
				[
					13.647066004136832,
					31.529433306525732
				],
				[
					13.647066004136832,
					29.176492130055124
				],
				[
					13.647066004136832,
					26.823550953584515
				],
				[
					12.705903894761832,
					25.411771886488964
				],
				[
					10.823543772978155,
					24.000028722426464
				],
				[
					9.411764705882888,
					23.529411764705856
				],
				[
					7.529440487132888,
					24.000028722426464
				],
				[
					6.117661420036711,
					24.941190831801464
				],
				[
					3.764720243566444,
					28.235294117647015
				],
				[
					2.3529411764711767,
					30.588235294117624
				],
				[
					2.3529411764711767,
					30.588235294117624
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2578125,
				0.4423828125,
				0.490234375,
				0.5146484375,
				0.5234375,
				0.5322265625,
				0.54296875,
				0.5517578125,
				0.55859375,
				0.564453125,
				0.5791015625,
				0.58203125,
				0.583984375,
				0.583984375,
				0.583984375,
				0.5810546875,
				0.5810546875,
				0.576171875,
				0.5654296875,
				0.5546875,
				0.5546875,
				0.5546875,
				0.5625,
				0.564453125,
				0.564453125,
				0.55859375,
				0.5361328125,
				0.357421875,
				0.013671875,
				0
			]
		},
		{
			"type": "text",
			"version": 172,
			"versionNonce": 2061510483,
			"isDeleted": false,
			"id": "ySQtmyjD",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4318.838016077306,
			"y": 256.13856080107627,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 232,
			"height": 25,
			"seed": 1118194229,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159323,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "String curLongest = null",
			"rawText": "String curLongest = null",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "String curLongest = null",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 181,
			"versionNonce": 1075243869,
			"isDeleted": false,
			"id": "KngdRPh8G5JZCUeQvSjPr",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4311.890037915186,
			"y": 301.9666302894635,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 132,
			"height": 35,
			"seed": 985276667,
			"groupIds": [],
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "gDEJ3UsG"
				},
				{
					"id": "71WtiTWoNCnxtuuw3QVP5",
					"type": "arrow"
				}
			],
			"updated": 1686311159323,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 174,
			"versionNonce": 564511987,
			"isDeleted": false,
			"id": "gDEJ3UsG",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4322.390037915186,
			"y": 306.9666302894635,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 111,
			"height": 25,
			"seed": 945756373,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159323,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "if s.len < 2",
			"rawText": "if s.len < 2",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "KngdRPh8G5JZCUeQvSjPr",
			"originalText": "if s.len < 2",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "arrow",
			"version": 422,
			"versionNonce": 138115005,
			"isDeleted": false,
			"id": "71WtiTWoNCnxtuuw3QVP5",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4447.037125461143,
			"y": 317.07719985804795,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 50.35292681525698,
			"height": 0.5629735168207617,
			"seed": 41677013,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "WPxyK0Ph"
				}
			],
			"updated": 1686311159323,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "KngdRPh8G5JZCUeQvSjPr",
				"gap": 3.1470875459563104,
				"focus": -0.0886245876370955
			},
			"endBinding": {
				"elementId": "0mtFPYfaBxkCIXYfOViQc",
				"gap": 7.529368681066444,
				"focus": 0.00001232561552759341
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					50.35292681525698,
					-0.5629735168207617
				]
			]
		},
		{
			"type": "text",
			"version": 103,
			"versionNonce": 1160162963,
			"isDeleted": false,
			"id": "WPxyK0Ph",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4479.74301499469,
			"y": 303.1137178354194,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 16,
			"height": 25,
			"seed": 1828820315,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159323,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "T",
			"rawText": "T",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "71WtiTWoNCnxtuuw3QVP5",
			"originalText": "T",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 185,
			"versionNonce": 147814429,
			"isDeleted": false,
			"id": "URlCykkV0cAU9jkXwFEkJ",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4510.03702493265,
			"y": 298.0548476320646,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 92,
			"height": 35,
			"seed": 1751676885,
			"groupIds": [
				"RaOr8kvRg4XSSq1c0ywWg"
			],
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "taMMKozs"
				},
				{
					"id": "71WtiTWoNCnxtuuw3QVP5",
					"type": "arrow"
				}
			],
			"updated": 1686311159323,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 178,
			"versionNonce": 1209623603,
			"isDeleted": false,
			"id": "taMMKozs",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4515.53702493265,
			"y": 303.0548476320646,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 81,
			"height": 25,
			"seed": 1976874075,
			"groupIds": [
				"RaOr8kvRg4XSSq1c0ywWg"
			],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159324,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "return s",
			"rawText": "return s",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "URlCykkV0cAU9jkXwFEkJ",
			"originalText": "return s",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 175,
			"versionNonce": 1808034941,
			"isDeleted": false,
			"id": "0mtFPYfaBxkCIXYfOViQc",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4504.919420957466,
			"y": 290.67250905210136,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 104.00002872242658,
			"height": 50.352926815257376,
			"seed": 1634305813,
			"groupIds": [
				"RaOr8kvRg4XSSq1c0ywWg"
			],
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"id": "71WtiTWoNCnxtuuw3QVP5",
					"type": "arrow"
				}
			],
			"updated": 1686311159324,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 307,
			"versionNonce": 1919182291,
			"isDeleted": false,
			"id": "TmORRHkmL0eSrCbuvTN1F",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4308.566637754341,
			"y": 355.23133258151313,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 240,
			"height": 35,
			"seed": 237697877,
			"groupIds": [],
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "yncwLfvN"
				}
			],
			"updated": 1686311159324,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 394,
			"versionNonce": 551277789,
			"isDeleted": false,
			"id": "yncwLfvN",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4315.066637754341,
			"y": 360.23133258151313,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 227,
			"height": 25,
			"seed": 84359931,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159324,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "for i = 0; i < s.len; i++",
			"rawText": "for i = 0; i < s.len; i++",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "TmORRHkmL0eSrCbuvTN1F",
			"originalText": "for i = 0; i < s.len; i++",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "line",
			"version": 300,
			"versionNonce": 1260270451,
			"isDeleted": false,
			"id": "mOTiqCkH-ciWvHyLh_leS",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4553.390167166105,
			"y": 371.1431260098219,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 312.47052360983344,
			"height": 0,
			"seed": 1658836155,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1686311159324,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					312.47052360983344,
					0
				]
			]
		},
		{
			"type": "line",
			"version": 246,
			"versionNonce": 598159677,
			"isDeleted": false,
			"id": "1-xfO7mfUBFie433ry8nJ",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4332.21369657787,
			"y": 390.9078534339948,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 0,
			"height": 358.5883645450368,
			"seed": 1603321301,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1686311159324,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					0,
					358.5883645450368
				]
			]
		},
		{
			"type": "rectangle",
			"version": 253,
			"versionNonce": 848121107,
			"isDeleted": false,
			"id": "LiHOPPf2EmE0NdGPs0oSE",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4357.065140402878,
			"y": 412.42146304178596,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 240,
			"height": 35,
			"seed": 438977147,
			"groupIds": [],
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "VVdoI2YW"
				}
			],
			"updated": 1686311159324,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 400,
			"versionNonce": 25690525,
			"isDeleted": false,
			"id": "VVdoI2YW",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4364.065140402878,
			"y": 417.42146304178596,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 226,
			"height": 25,
			"seed": 1515338523,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159324,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "for j = i; j < s.len; j++",
			"rawText": "for j = i; j < s.len; j++",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "LiHOPPf2EmE0NdGPs0oSE",
			"originalText": "for j = i; j < s.len; j++",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "line",
			"version": 258,
			"versionNonce": 1009267379,
			"isDeleted": false,
			"id": "lzZeUerC2sJ6Ar7Nk9pYF",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4604.241610991111,
			"y": 431.62735975594046,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 226.32496213776903,
			"height": 0,
			"seed": 271720379,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1686311159324,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					226.32496213776903,
					0
				]
			]
		},
		{
			"type": "line",
			"version": 283,
			"versionNonce": 531613181,
			"isDeleted": false,
			"id": "ZRosHIDhnQNDjoqk0x-fk",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4381.182816184128,
			"y": 447.1567858818595,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 0,
			"height": 267.98651246252143,
			"seed": 367816795,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1686311159324,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					0,
					267.98651246252143
				]
			]
		},
		{
			"type": "rectangle",
			"version": 218,
			"versionNonce": 1217750099,
			"isDeleted": false,
			"id": "yFC6odGtN6X6cHrerx1UQ",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4418.478352195977,
			"y": 511.40798627521724,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 249,
			"height": 35,
			"seed": 926048795,
			"groupIds": [],
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "yezUe9A6"
				},
				{
					"id": "9RrUQYEz2X7DaqwCES4h5",
					"type": "arrow"
				}
			],
			"updated": 1686311159324,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 266,
			"versionNonce": 1092615773,
			"isDeleted": false,
			"id": "yezUe9A6",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4434.978352195977,
			"y": 516.4079862752172,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 216,
			"height": 25,
			"seed": 895384597,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159324,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "if isPalindrome(curSub)",
			"rawText": "if isPalindrome(curSub)",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "yFC6odGtN6X6cHrerx1UQ",
			"originalText": "if isPalindrome(curSub)",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "arrow",
			"version": 406,
			"versionNonce": 1605067251,
			"isDeleted": false,
			"id": "9RrUQYEz2X7DaqwCES4h5",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4449.860719498366,
			"y": 552.790285361844,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 61.17647058823695,
			"height": 36.70589671415439,
			"seed": 1411773685,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "xyh2wMIt"
				}
			],
			"updated": 1686311159324,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "yFC6odGtN6X6cHrerx1UQ",
				"gap": 6.382299086626745,
				"focus": 0.864998647329439
			},
			"endBinding": {
				"elementId": "D11DQ9zVggHvIoJ0qM6gE",
				"gap": 8.323486328125114,
				"focus": -0.5029118911926618
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					61.17647058823695,
					36.70589671415439
				]
			]
		},
		{
			"type": "text",
			"version": 147,
			"versionNonce": 1286220477,
			"isDeleted": false,
			"id": "xyh2wMIt",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4469.390124082466,
			"y": 564.9961677147852,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 16,
			"height": 25,
			"seed": 1425306389,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159324,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "T",
			"rawText": "T",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "9RrUQYEz2X7DaqwCES4h5",
			"originalText": "T",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 293,
			"versionNonce": 1248897939,
			"isDeleted": false,
			"id": "D11DQ9zVggHvIoJ0qM6gE",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4493.684270451952,
			"y": 597.8196684041235,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 302,
			"height": 35,
			"seed": 1094434965,
			"groupIds": [],
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "z41nsNAC"
				},
				{
					"id": "9RrUQYEz2X7DaqwCES4h5",
					"type": "arrow"
				},
				{
					"id": "BgzvpcdgEH-seTvOcmFo4",
					"type": "arrow"
				}
			],
			"updated": 1686311159324,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 304,
			"versionNonce": 1391446813,
			"isDeleted": false,
			"id": "z41nsNAC",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4503.684270451952,
			"y": 602.8196684041235,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 282,
			"height": 25,
			"seed": 1791843765,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159324,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "if curSub.len > curLongest.len",
			"rawText": "if curSub.len > curLongest.len",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "D11DQ9zVggHvIoJ0qM6gE",
			"originalText": "if curSub.len > curLongest.len",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "arrow",
			"version": 424,
			"versionNonce": 1830535475,
			"isDeleted": false,
			"id": "BgzvpcdgEH-seTvOcmFo4",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4549.242617431907,
			"y": 638.3578833410587,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 42.533278847286056,
			"height": 36.70589671415439,
			"seed": 56893435,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "F5JbdS1y"
				}
			],
			"updated": 1686311159324,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "D11DQ9zVggHvIoJ0qM6gE",
				"gap": 5.538214936935219,
				"focus": 0.7130932623646694
			},
			"endBinding": {
				"elementId": "PK7kNpnW",
				"gap": 5.726526848450817,
				"focus": -0.5345697417461527
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					42.533278847286056,
					36.70589671415439
				]
			]
		},
		{
			"type": "text",
			"version": 182,
			"versionNonce": 1415733117,
			"isDeleted": false,
			"id": "F5JbdS1y",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4540.536377300273,
			"y": 644.2108316981358,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 16,
			"height": 25,
			"seed": 192178331,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159325,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "T",
			"rawText": "T",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "BgzvpcdgEH-seTvOcmFo4",
			"originalText": "T",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 143,
			"versionNonce": 1628644051,
			"isDeleted": false,
			"id": "PK7kNpnW",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4574.095984893587,
			"y": 680.7903069036639,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 200,
			"height": 25,
			"seed": 63530709,
			"groupIds": [],
			"roundness": null,
			"boundElements": [
				{
					"id": "BgzvpcdgEH-seTvOcmFo4",
					"type": "arrow"
				}
			],
			"updated": 1686311159325,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "curLongest = curSub",
			"rawText": "curLongest = curSub",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "curLongest = curSub",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "line",
			"version": 139,
			"versionNonce": 1195599837,
			"isDeleted": false,
			"id": "IDQ3HSGOPasX9BN6cFn0b",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4380.684191465277,
			"y": 718.4374375332594,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 455.0588091681984,
			"height": 0,
			"seed": 602288821,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1686311159325,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					455.0588091681984,
					0
				]
			]
		},
		{
			"type": "line",
			"version": 140,
			"versionNonce": 1324175475,
			"isDeleted": false,
			"id": "DJHsXopdJXjkqhd9P6pCk",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4330.801798754587,
			"y": 746.8536180360345,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 537.8823313993562,
			"height": 0,
			"seed": 1141291221,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1686311159325,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					537.8823313993562,
					0
				]
			]
		},
		{
			"type": "line",
			"version": 146,
			"versionNonce": 1571054653,
			"isDeleted": false,
			"id": "vsKtOIwWzs5B0QkiDnD3S",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4864.448911708843,
			"y": 749.0256728273772,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 0,
			"height": 378.35298426011013,
			"seed": 1318294651,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1686311159325,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					0,
					-378.35298426011013
				]
			]
		},
		{
			"type": "rectangle",
			"version": 116,
			"versionNonce": 141609491,
			"isDeleted": false,
			"id": "KZ-vVTGvUrKuweGgAjKqx",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4333.9082183826085,
			"y": 774.7948873021545,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 191,
			"height": 42,
			"seed": 1595765269,
			"groupIds": [
				"CuAoCkzJB6HMRXVuXUfnY"
			],
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "0zl7uVyB"
				}
			],
			"updated": 1686311159325,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 100,
			"versionNonce": 191288477,
			"isDeleted": false,
			"id": "0zl7uVyB",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4341.9082183826085,
			"y": 783.2948873021545,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 175,
			"height": 25,
			"seed": 745136757,
			"groupIds": [
				"CuAoCkzJB6HMRXVuXUfnY"
			],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159325,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "return curLongest",
			"rawText": "return curLongest",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "KZ-vVTGvUrKuweGgAjKqx",
			"originalText": "return curLongest",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 106,
			"versionNonce": 1653870515,
			"isDeleted": false,
			"id": "zeh5xLqjqYkIDegpNYqD5",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4326.639006393426,
			"y": 765.6410317582844,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 204.92304875300397,
			"height": 59.69228891225964,
			"seed": 1782434331,
			"groupIds": [
				"CuAoCkzJB6HMRXVuXUfnY"
			],
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1686311159325,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 358,
			"versionNonce": 1279015165,
			"isDeleted": false,
			"id": "VZYUFZyh",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3878.4337054241273,
			"y": 811.6822189506844,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 442,
			"height": 225,
			"seed": 1121620539,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159325,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "// isPalindrome s: String\n- Dequeue = new dequeu()\n- if str < 2 return s\n- iterate s\n    - add all chars to the deque\n- loop s.len times / 2\n    - if start of dequeue != end of dequeue\n        - return false\n- return true",
			"rawText": "// isPalindrome s: String\n- Dequeue = new dequeu()\n- if str < 2 return s\n- iterate s\n    - add all chars to the deque\n- loop s.len times / 2\n    - if start of dequeue != end of dequeue\n        - return false\n- return true",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "// isPalindrome s: String\n- Dequeue = new dequeu()\n- if str < 2 return s\n- iterate s\n    - add all chars to the deque\n- loop s.len times / 2\n    - if start of dequeue != end of dequeue\n        - return false\n- return true",
			"lineHeight": 1.25,
			"baseline": 217
		},
		{
			"type": "text",
			"version": 711,
			"versionNonce": 1333633363,
			"isDeleted": false,
			"id": "Q58zagls",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3854.6023551462426,
			"y": 1134.2392049516845,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 527,
			"height": 225,
			"seed": 607674295,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159325,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "- iterate s\n    - iterate sIndex = i - 1; eIndex = i + 1; \n      not stIndex >= 0 && not enIndex <= s.len - 1\n        - check substring (i - 1, i)\n        - curSub = s.substring (startIndex, endIndex)\n        - if curSub > curLongest\n            - if isPal(curSub)\n                - curLongest = curSub\n    - reset start and end index",
			"rawText": "- iterate s\n    - iterate sIndex = i - 1; eIndex = i + 1; \n      not stIndex >= 0 && not enIndex <= s.len - 1\n        - check substring (i - 1, i)\n        - curSub = s.substring (startIndex, endIndex)\n        - if curSub > curLongest\n            - if isPal(curSub)\n                - curLongest = curSub\n    - reset start and end index",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "- iterate s\n    - iterate sIndex = i - 1; eIndex = i + 1; \n      not stIndex >= 0 && not enIndex <= s.len - 1\n        - check substring (i - 1, i)\n        - curSub = s.substring (startIndex, endIndex)\n        - if curSub > curLongest\n            - if isPal(curSub)\n                - curLongest = curSub\n    - reset start and end index",
			"lineHeight": 1.25,
			"baseline": 217
		},
		{
			"type": "text",
			"version": 55,
			"versionNonce": 698749277,
			"isDeleted": false,
			"id": "gR6wU2vO",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3816.058863692117,
			"y": 1087.9083470634382,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 147,
			"height": 25,
			"seed": 770205841,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159325,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "SecondSolution?",
			"rawText": "SecondSolution?",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "SecondSolution?",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "line",
			"version": 153,
			"versionNonce": 948174579,
			"isDeleted": false,
			"id": "RtfManWINHFWENCGTkC7b",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4908.624323338264,
			"y": -404.95406821767835,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 0,
			"height": 2065.5999145507812,
			"seed": 1411389425,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1686311159325,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					0,
					2065.5999145507812
				]
			]
		},
		{
			"type": "text",
			"version": 15,
			"versionNonce": 16113085,
			"isDeleted": false,
			"id": "Rur1RGNw",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4977.8686809771525,
			"y": -408.4206548604737,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 305,
			"height": 50,
			"seed": 63776959,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159325,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "## 8. String to Integer (atoi)\n",
			"rawText": "## 8. String to Integer (atoi)\n",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "## 8. String to Integer (atoi)\n",
			"lineHeight": 1.25,
			"baseline": 42
		},
		{
			"type": "text",
			"version": 502,
			"versionNonce": 405645459,
			"isDeleted": false,
			"id": "txKTVQEb",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 6425.73049945055,
			"y": -384.8178789195532,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 189,
			"height": 25,
			"seed": 1835354865,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159325,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "IMPLEMENTATION",
			"rawText": "IMPLEMENTATION",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "IMPLEMENTATION",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 573,
			"versionNonce": 156048925,
			"isDeleted": false,
			"id": "qFvkk2O0",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 6450.360481703572,
			"y": -344.1142933452908,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 380,
			"height": 25,
			"seed": 625001681,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159325,
			"link": "[[LeetCode/Questions#Solution 10]]",
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "📍[[LeetCode/Questions#Solution 10]]",
			"rawText": "[[LeetCode/Questions#Solution 10]]",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "📍[[LeetCode/Questions#Solution 10]]",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 15,
			"versionNonce": 1412505139,
			"isDeleted": false,
			"id": "1XLVD5Xb",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4948.999974996452,
			"y": -326.23878982338414,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 50,
			"height": 25,
			"seed": 214654239,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159325,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "INFO",
			"rawText": "INFO",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "INFO",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 377,
			"versionNonce": 429740669,
			"isDeleted": false,
			"id": "hbY9mC6m",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4983.66675541045,
			"y": -280.89228931105987,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 388,
			"height": 250,
			"seed": 1919122929,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159325,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Implement a function which converts a \nstring to a 32-bit signed integer\n- ignore whitespaces\n- check for + and -\n- null answer is 0\n- max is 2^31 min is -2^31 - 1\n    - if bigger than that make it max\n    - if smaller than that make it min\n- ignore anything before and after the \n  number string",
			"rawText": "Implement a function which converts a \nstring to a 32-bit signed integer\n- ignore whitespaces\n- check for + and -\n- null answer is 0\n- max is 2^31 min is -2^31 - 1\n    - if bigger than that make it max\n    - if smaller than that make it min\n- ignore anything before and after the \n  number string",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Implement a function which converts a \nstring to a 32-bit signed integer\n- ignore whitespaces\n- check for + and -\n- null answer is 0\n- max is 2^31 min is -2^31 - 1\n    - if bigger than that make it max\n    - if smaller than that make it min\n- ignore anything before and after the \n  number string",
			"lineHeight": 1.25,
			"baseline": 242
		},
		{
			"type": "text",
			"version": 60,
			"versionNonce": 1467277267,
			"isDeleted": false,
			"id": "TPHEztcL",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 5006.41030524644,
			"y": 68.2358978195993,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 654,
			"height": 125,
			"seed": 801553567,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159325,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Input: s = \"4193 with words\"\nOutput: 4193\nExplanation:\nThe parsed integer is 4193.\nSince 4193 is in the range [-231, 231 - 1], the final result is 4193.",
			"rawText": "Input: s = \"4193 with words\"\nOutput: 4193\nExplanation:\nThe parsed integer is 4193.\nSince 4193 is in the range [-231, 231 - 1], the final result is 4193.",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Input: s = \"4193 with words\"\nOutput: 4193\nExplanation:\nThe parsed integer is 4193.\nSince 4193 is in the range [-231, 231 - 1], the final result is 4193.",
			"lineHeight": 1.25,
			"baseline": 117
		},
		{
			"type": "text",
			"version": 18,
			"versionNonce": 782760669,
			"isDeleted": false,
			"id": "gvcG0D3u",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4959.948794954973,
			"y": 16.851338775128,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 91,
			"height": 25,
			"seed": 727494737,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159326,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "EXAMPLE",
			"rawText": "EXAMPLE",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "EXAMPLE",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 38,
			"versionNonce": 1812950387,
			"isDeleted": false,
			"id": "C94UUQqM",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4957.179653390986,
			"y": 271.00506285866174,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 149,
			"height": 25,
			"seed": 728316977,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159326,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "WALKTHROUGH",
			"rawText": "WALKTHROUGH",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "WALKTHROUGH",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 63,
			"versionNonce": 821991229,
			"isDeleted": false,
			"id": "fTXnsmfZ",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 5527.641196547536,
			"y": 273.4666576603445,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 138,
			"height": 25,
			"seed": 524356945,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159326,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "BRUTEFORCE",
			"rawText": "BRUTEFORCE",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "BRUTEFORCE",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 941,
			"versionNonce": 1430734611,
			"isDeleted": false,
			"id": "bC6w54eJ",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 5007.33334460944,
			"y": 334.0820798358252,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 350,
			"height": 400,
			"seed": 617715857,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159326,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "- long result\n- isValid = notLetter AND \n           notWhitespace AND ...\n- iterate the string\n    - if NOT isValid (str[i]), skip\n    - if +, positive = true\n    - if -, negative = true\n    - if isNumers(str[i]) \n        - Stack.push (str[i])\n- iterate stack i = 0\n    - result += stack.pop * (10 * i)\n    - if result < -2^31\n        - return -2^31\n    - if result > 2^31 - 1\n        - return 2^31 - 1\n- return result",
			"rawText": "- long result\n- isValid = notLetter AND \n           notWhitespace AND ...\n- iterate the string\n    - if NOT isValid (str[i]), skip\n    - if +, positive = true\n    - if -, negative = true\n    - if isNumers(str[i]) \n        - Stack.push (str[i])\n- iterate stack i = 0\n    - result += stack.pop * (10 * i)\n    - if result < -2^31\n        - return -2^31\n    - if result > 2^31 - 1\n        - return 2^31 - 1\n- return result",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "- long result\n- isValid = notLetter AND \n           notWhitespace AND ...\n- iterate the string\n    - if NOT isValid (str[i]), skip\n    - if +, positive = true\n    - if -, negative = true\n    - if isNumers(str[i]) \n        - Stack.push (str[i])\n- iterate stack i = 0\n    - result += stack.pop * (10 * i)\n    - if result < -2^31\n        - return -2^31\n    - if result > 2^31 - 1\n        - return 2^31 - 1\n- return result",
			"lineHeight": 1.25,
			"baseline": 392
		},
		{
			"type": "line",
			"version": 244,
			"versionNonce": 2063771549,
			"isDeleted": false,
			"id": "hhZnwOSQtTqhUSlXC3vdk",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 5916.533028406996,
			"y": -440.4135375780909,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 0,
			"height": 2065.5999145507812,
			"seed": 1783089111,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1686311159326,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					0,
					2065.5999145507812
				]
			]
		},
		{
			"type": "text",
			"version": 12,
			"versionNonce": 697494707,
			"isDeleted": false,
			"id": "FC6Kc4U1",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 6000.936312006013,
			"y": -388.14518331172434,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 351,
			"height": 50,
			"seed": 1040924217,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159326,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "## 10. Regular Expression Matching\n",
			"rawText": "## 10. Regular Expression Matching\n",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "## 10. Regular Expression Matching\n",
			"lineHeight": 1.25,
			"baseline": 42
		},
		{
			"type": "text",
			"version": 47,
			"versionNonce": 518368253,
			"isDeleted": false,
			"id": "EaF72K9B",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 5945.18603734781,
			"y": -281.88974222130724,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 50,
			"height": 25,
			"seed": 1457119321,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159326,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "INFO",
			"rawText": "INFO",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "INFO",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 355,
			"versionNonce": 1821957715,
			"isDeleted": false,
			"id": "QS6xixLZ",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 6008.436064050691,
			"y": -240.13973077721545,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 424,
			"height": 250,
			"seed": 749339543,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159326,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Implement a regular expression matching \nwith support for . and *\n    - s :String 1 <= s.length <= 20 \n    - p :String pattern 1 <= p.length <= 20\n    - . Matches any single character\n    - * Matches zero or more of the \n        preceding element \n\n> boolean isMatch(String  s, String p) <\n",
			"rawText": "Implement a regular expression matching \nwith support for . and *\n    - s :String 1 <= s.length <= 20 \n    - p :String pattern 1 <= p.length <= 20\n    - . Matches any single character\n    - * Matches zero or more of the \n        preceding element \n\n> boolean isMatch(String  s, String p) <\n",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Implement a regular expression matching \nwith support for . and *\n    - s :String 1 <= s.length <= 20 \n    - p :String pattern 1 <= p.length <= 20\n    - . Matches any single character\n    - * Matches zero or more of the \n        preceding element \n\n> boolean isMatch(String  s, String p) <\n",
			"lineHeight": 1.25,
			"baseline": 242
		},
		{
			"type": "text",
			"version": 35,
			"versionNonce": 1823024221,
			"isDeleted": false,
			"id": "iC30sz9z",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 5942.686018274324,
			"y": 34.86021200232554,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 91,
			"height": 25,
			"seed": 259953625,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159326,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "EXAMPLE",
			"rawText": "EXAMPLE",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "EXAMPLE",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 90,
			"versionNonce": 1764727795,
			"isDeleted": false,
			"id": "bv4ytyYR",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 6000.436033533113,
			"y": 96.36024633460096,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 539,
			"height": 75,
			"seed": 465097559,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159326,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Input: s = \"aa\", p = \"a\"\nOutput: false\nExplanation: \"a\" does not match the entire string \"aa\".",
			"rawText": "Input: s = \"aa\", p = \"a\"\nOutput: false\nExplanation: \"a\" does not match the entire string \"aa\".",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Input: s = \"aa\", p = \"a\"\nOutput: false\nExplanation: \"a\" does not match the entire string \"aa\".",
			"lineHeight": 1.25,
			"baseline": 67
		},
		{
			"type": "text",
			"version": 11,
			"versionNonce": 941527229,
			"isDeleted": false,
			"id": "VuknZj0n",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 5999.186033533113,
			"y": 231.36024633460096,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 611,
			"height": 100,
			"seed": 12733655,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159326,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Input: s = \"aa\", p = \"a*\"\nOutput: true\nExplanation: '*' means zero or more of the preceding element, \n'a'. Therefore, by repeating 'a' once, it becomes \"aa\".",
			"rawText": "Input: s = \"aa\", p = \"a*\"\nOutput: true\nExplanation: '*' means zero or more of the preceding element, \n'a'. Therefore, by repeating 'a' once, it becomes \"aa\".",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Input: s = \"aa\", p = \"a*\"\nOutput: true\nExplanation: '*' means zero or more of the preceding element, \n'a'. Therefore, by repeating 'a' once, it becomes \"aa\".",
			"lineHeight": 1.25,
			"baseline": 92
		},
		{
			"type": "text",
			"version": 35,
			"versionNonce": 1264428435,
			"isDeleted": false,
			"id": "3ErbVFPg",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 6004.4380161865765,
			"y": 366.72799244491154,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 618,
			"height": 75,
			"seed": 769943159,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159326,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Input: s = \"ab\", p = \".*\"\nOutput: true\nExplanation: \".*\" means \"zero or more (*) of any character (.)\".",
			"rawText": "Input: s = \"ab\", p = \".*\"\nOutput: true\nExplanation: \".*\" means \"zero or more (*) of any character (.)\".",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Input: s = \"ab\", p = \".*\"\nOutput: true\nExplanation: \".*\" means \"zero or more (*) of any character (.)\".",
			"lineHeight": 1.25,
			"baseline": 67
		},
		{
			"type": "text",
			"version": 20,
			"versionNonce": 1592226077,
			"isDeleted": false,
			"id": "DQp9SlhM",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 5956.438020881584,
			"y": 502.1125139292862,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 149,
			"height": 25,
			"seed": 34518777,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159326,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "WALKTHROUGH",
			"rawText": "WALKTHROUGH",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "WALKTHROUGH",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 20,
			"versionNonce": 2052684595,
			"isDeleted": false,
			"id": "OKLnofNr",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 6462.5918670354295,
			"y": 519.0355908523632,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 151,
			"height": 25,
			"seed": 1034549529,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159326,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "BRUTEFORECE",
			"rawText": "BRUTEFORECE",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "BRUTEFORECE",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "line",
			"version": 355,
			"versionNonce": 242566525,
			"isDeleted": false,
			"id": "gPEmd2mqkbrFzy3jB7CWK",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 6894.731491331663,
			"y": -401.5612678482628,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 0,
			"height": 2065.5999145507812,
			"seed": 1664362724,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1686311159326,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					0,
					2065.5999145507812
				]
			]
		},
		{
			"type": "text",
			"version": 10,
			"versionNonce": 847879379,
			"isDeleted": false,
			"id": "7E6maRv2",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 6974.129494242654,
			"y": -342.47836660029964,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 334,
			"height": 50,
			"seed": 1479951332,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159326,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "## 11. Container With Most Water\n",
			"rawText": "## 11. Container With Most Water\n",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "## 11. Container With Most Water\n",
			"lineHeight": 1.25,
			"baseline": 42
		},
		{
			"type": "text",
			"version": 554,
			"versionNonce": 1242140125,
			"isDeleted": false,
			"id": "TsBS2I7U",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 7440.3145641513,
			"y": -338.83018227561445,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 189,
			"height": 25,
			"seed": 1993477476,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159326,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "IMPLEMENTATION",
			"rawText": "IMPLEMENTATION",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "IMPLEMENTATION",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 631,
			"versionNonce": 1602521715,
			"isDeleted": false,
			"id": "xcIGUIFU",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 7464.94454640432,
			"y": -298.126596701352,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 371,
			"height": 25,
			"seed": 192069860,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159327,
			"link": "[[LeetCode/Questions#Solution 11]]",
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "📍[[LeetCode/Questions#Solution 11]]",
			"rawText": "[[LeetCode/Questions#Solution 11]]",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "📍[[LeetCode/Questions#Solution 11]]",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 84,
			"versionNonce": 817220157,
			"isDeleted": false,
			"id": "1wV7KCko",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 6941.229391354819,
			"y": -240.52838055119244,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 50,
			"height": 25,
			"seed": 1524031460,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159327,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "INFO",
			"rawText": "INFO",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "INFO",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 274,
			"versionNonce": 907068435,
			"isDeleted": false,
			"id": "BC6F8C7t",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 6999.699726256734,
			"y": -173.3810903109151,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 458,
			"height": 200,
			"seed": 1176142564,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159327,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Find two lines that together with \nthe x-axis form a container, this \ncontainer must contain the most water.\n- height: int[]      (\n- n:      int length ( n== heght.len )\n- return the max water a container can store\n\n>  int maxArea (int[] height) <",
			"rawText": "Find two lines that together with \nthe x-axis form a container, this \ncontainer must contain the most water.\n- height: int[]      (\n- n:      int length ( n== heght.len )\n- return the max water a container can store\n\n>  int maxArea (int[] height) <",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Find two lines that together with \nthe x-axis form a container, this \ncontainer must contain the most water.\n- height: int[]      (\n- n:      int length ( n== heght.len )\n- return the max water a container can store\n\n>  int maxArea (int[] height) <",
			"lineHeight": 1.25,
			"baseline": 192
		},
		{
			"type": "text",
			"version": 25,
			"versionNonce": 56326813,
			"isDeleted": false,
			"id": "lMxKPcvf",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 6941.985427463486,
			"y": 75.47602638830364,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 91,
			"height": 25,
			"seed": 626437340,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159327,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "EXAMPLE",
			"rawText": "EXAMPLE",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "EXAMPLE",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 68,
			"versionNonce": 237291955,
			"isDeleted": false,
			"id": "zEW3vNBp",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 7007.414003251714,
			"y": 146.04748983696453,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 560,
			"height": 125,
			"seed": 239320028,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159327,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Input: height = [1,8,6,2,5,4,8,3,7]\nOutput: 49\nExplanation: The above vertical lines are represented \nby array [1,8,6,2,5,4,8,3,7]. In this case, the max area \nof water (blue section) the container can contain is 49.",
			"rawText": "Input: height = [1,8,6,2,5,4,8,3,7]\nOutput: 49\nExplanation: The above vertical lines are represented \nby array [1,8,6,2,5,4,8,3,7]. In this case, the max area \nof water (blue section) the container can contain is 49.",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Input: height = [1,8,6,2,5,4,8,3,7]\nOutput: 49\nExplanation: The above vertical lines are represented \nby array [1,8,6,2,5,4,8,3,7]. In this case, the max area \nof water (blue section) the container can contain is 49.",
			"lineHeight": 1.25,
			"baseline": 117
		},
		{
			"type": "freedraw",
			"version": 306,
			"versionNonce": 1789665021,
			"isDeleted": false,
			"id": "1DkcQeCD0tfr1SnhtFrUq",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 7024.53011883667,
			"y": 333.16908663546474,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 12.004568800389206,
			"height": 22.917828302845244,
			"seed": 28253668,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159327,
			"link": null,
			"locked": true,
			"points": [
				[
					0,
					0
				],
				[
					0,
					-0.5456546489666136
				],
				[
					2.1826394112571075,
					-2.1826602266474904
				],
				[
					3.8196241735472762,
					-4.365278822513728
				],
				[
					5.4566297512276645,
					-7.639289977875483
				],
				[
					5.4566297512276645,
					-9.821908573741775
				],
				[
					4.365299637904434,
					-12.55022344935577
				],
				[
					-0.5456754643571585,
					-12.55022344935577
				],
				[
					-1.6370055776812562,
					-10.913259502456093
				],
				[
					-1.6370055776812562,
					-8.184944626842094
				],
				[
					-0.5456754643571585,
					-6.002284400194605
				],
				[
					2.1826394112571075,
					-2.7283148756140503
				],
				[
					3.8196241735472762,
					-1.091309297933173
				],
				[
					5.4566297512276645,
					1.0913509287143173
				],
				[
					6.547939049161542,
					3.8196658043283134
				],
				[
					5.4566297512276645,
					5.456629751227991
				],
				[
					3.2739695245803366,
					7.093635328908921
				],
				[
					-1.6370055776812562,
					8.7305992758086
				],
				[
					-4.9109751022615935,
					8.184944626842041
				],
				[
					-5.4566297512276645,
					7.639289977875483
				],
				[
					-5.4566297512276645,
					8.184944626842041
				],
				[
					-4.365320453294654,
					8.7305992758086
				],
				[
					-2.182660226647327,
					10.367604853489476
				],
				[
					0,
					0
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.1611328125,
				0.294921875,
				0.3369140625,
				0.369140625,
				0.3818359375,
				0.3916015625,
				0.4052734375,
				0.4541015625,
				0.4658203125,
				0.474609375,
				0.4736328125,
				0.4736328125,
				0.4736328125,
				0.4736328125,
				0.470703125,
				0.4755859375,
				0.5,
				0.5166015625,
				0.5263671875,
				0.5283203125,
				0.4931640625,
				0.310546875,
				0.025390625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 304,
			"versionNonce": 2095520595,
			"isDeleted": false,
			"id": "qL2qOP6t0VfdSKCKyjm4w",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 7023.438788723346,
			"y": 365.3632104938664,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 9.8219293891321,
			"height": 17.461198551617255,
			"seed": 1893419876,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159327,
			"link": null,
			"locked": true,
			"points": [
				[
					0,
					0
				],
				[
					-1.0913301133232296,
					0
				],
				[
					-1.0913301133232296,
					-1.637005577680931
				],
				[
					0,
					-4.365320453294926
				],
				[
					0.5456546489669394,
					-5.456629751228045
				],
				[
					1.6369847622910374,
					-8.184944626842093
				],
				[
					2.7283148756142674,
					-10.36760485348953
				],
				[
					3.819644988938365,
					-12.550265080136967
				],
				[
					4.365299637904436,
					-13.095919729103525
				],
				[
					4.910954286871375,
					-14.187229027036699
				],
				[
					4.910954286871375,
					-14.732883676003254
				],
				[
					4.910954286871375,
					-15.278579955751015
				],
				[
					4.910954286871375,
					-15.824234604717574
				],
				[
					2.7283148756142674,
					-15.824234604717574
				],
				[
					0.5456546489669394,
					-15.824234604717574
				],
				[
					-1.636984762290169,
					-16.369889253684136
				],
				[
					-2.7283148756133984,
					-16.369889253684136
				],
				[
					-3.819644988937496,
					-16.915543902650693
				],
				[
					-4.365299637903568,
					-16.915543902650693
				],
				[
					-4.910975102260727,
					-17.461198551617255
				],
				[
					-4.910975102260727,
					-16.915543902650693
				],
				[
					-3.2739903399705566,
					-15.278579955751015
				],
				[
					-3.2739903399705566,
					-15.278579955751015
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2158203125,
				0.3525390625,
				0.455078125,
				0.4677734375,
				0.4677734375,
				0.4677734375,
				0.4677734375,
				0.4677734375,
				0.4677734375,
				0.470703125,
				0.4765625,
				0.484375,
				0.4931640625,
				0.5068359375,
				0.521484375,
				0.5361328125,
				0.5439453125,
				0.5458984375,
				0.5458984375,
				0.5224609375,
				0.32421875,
				0.02734375,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 303,
			"versionNonce": 2099853149,
			"isDeleted": false,
			"id": "g4WcCiIUGq5bAEEczV7LD",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 7021.256128496699,
			"y": 369.7285309471613,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 7.639289977874991,
			"height": 22.917828302845297,
			"seed": 295556452,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159327,
			"link": null,
			"locked": true,
			"points": [
				[
					0,
					0
				],
				[
					-1.6369847622901683,
					1.6369639468997321
				],
				[
					-2.7283148756133975,
					5.456629751228045
				],
				[
					-4.910954286870505,
					10.91325950245609
				],
				[
					-5.4566297512276645,
					15.824192973936377
				],
				[
					-5.4566297512276645,
					19.64385877826469
				],
				[
					-4.910954286870505,
					21.82651900491218
				],
				[
					-2.7283148756133975,
					22.917828302845297
				],
				[
					0,
					21.28082272516442
				],
				[
					1.0913301133240978,
					19.09820412929813
				],
				[
					2.182660226647327,
					16.915543902650693
				],
				[
					2.182660226647327,
					14.732883676003254
				],
				[
					1.6369847622901683,
					13.095878098322324
				],
				[
					0.5456754643571585,
					11.458914151422649
				],
				[
					-0.5456546489660707,
					10.91325950245609
				],
				[
					-1.6369847622901683,
					12.004568800389206
				],
				[
					-2.182639411256239,
					13.095878098322324
				],
				[
					-2.7283148756133975,
					14.732883676003254
				],
				[
					-2.7283148756133975,
					15.278538324969816
				],
				[
					-2.182639411256239,
					16.369889253684136
				],
				[
					0.5456754643571585,
					19.09820412929813
				],
				[
					0.5456754643571585,
					19.09820412929813
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.216796875,
				0.3779296875,
				0.4375,
				0.4775390625,
				0.4931640625,
				0.498046875,
				0.498046875,
				0.498046875,
				0.49609375,
				0.49609375,
				0.49609375,
				0.49609375,
				0.498046875,
				0.5,
				0.51171875,
				0.51953125,
				0.521484375,
				0.509765625,
				0.5029296875,
				0.4208984375,
				0.015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 295,
			"versionNonce": 783169779,
			"isDeleted": false,
			"id": "ZVUtzZzCOES0vhOyr3CM4",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 7019.619143734408,
			"y": 416.6555384815661,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 3.8196241735464076,
			"height": 8.184944626842093,
			"seed": 1657709660,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159327,
			"link": null,
			"locked": true,
			"points": [
				[
					0,
					0
				],
				[
					0,
					0.5456546489666135
				],
				[
					-0.5456546489660707,
					0
				],
				[
					-0.5456546489660707,
					-0.5456546489665592
				],
				[
					0.5456546489669392,
					-2.7283148756139948
				],
				[
					1.6369847622901683,
					-4.91097510226143
				],
				[
					2.182660226647327,
					-6.547980679942305
				],
				[
					2.728314875614266,
					-7.63928997787548
				],
				[
					2.728314875614266,
					-7.093635328908866
				],
				[
					2.728314875614266,
					-6.547980679942305
				],
				[
					2.728314875614266,
					-6.002284400194602
				],
				[
					3.2739695245803366,
					-5.4566297512279895
				],
				[
					3.2739695245803366,
					-3.819665804328312
				],
				[
					0,
					0
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2060546875,
				0.2421875,
				0.35546875,
				0.4208984375,
				0.453125,
				0.4580078125,
				0.4580078125,
				0.4580078125,
				0.4580078125,
				0.4560546875,
				0.4560546875,
				0.3984375,
				0.0263671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 311,
			"versionNonce": 86262717,
			"isDeleted": false,
			"id": "wWaNjF2LOj3D5Dgci2ixG",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 7016.8908288587945,
			"y": 422.6578228817607,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 10.9132595024562,
			"height": 22.372173653878683,
			"seed": 81758300,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159327,
			"link": null,
			"locked": true,
			"points": [
				[
					0,
					0
				],
				[
					0.5456546489669393,
					0
				],
				[
					1.6369847622910372,
					0
				],
				[
					2.728314875614267,
					-0.5456546489665592
				],
				[
					4.910975102261594,
					-1.6370055776808765
				],
				[
					6.547959864551762,
					-3.2739695245805542
				],
				[
					8.1849446268428,
					-4.910975102261431
				],
				[
					8.73059927580887,
					-6.547939049161162
				],
				[
					9.276274740166029,
					-7.639289977875481
				],
				[
					8.73059927580887,
					-8.730599275808599
				],
				[
					7.63928997787586,
					-10.367604853489475
				],
				[
					6.547959864551762,
					-10.913259502456036
				],
				[
					5.456629751228534,
					-11.458914151422594
				],
				[
					4.365299637904435,
					-10.913259502456036
				],
				[
					3.8196449889383643,
					-10.913259502456036
				],
				[
					2.728314875614267,
					-11.458914151422594
				],
				[
					2.1826602266481956,
					-13.095919729103471
				],
				[
					1.0913301133240978,
					-14.732883676003203
				],
				[
					0,
					-16.36988925368408
				],
				[
					-1.0913301133232294,
					-19.098204129298075
				],
				[
					-1.6369847622901685,
					-19.64385877826469
				],
				[
					-1.6369847622901685,
					-20.189513427231248
				],
				[
					-1.6369847622901685,
					-20.735209706979006
				],
				[
					-0.5456546489660709,
					-21.280864355945564
				],
				[
					0.5456546489669393,
					-21.82651900491212
				],
				[
					2.1826602266481956,
					-21.82651900491212
				],
				[
					4.910975102261594,
					-21.82651900491212
				],
				[
					6.547959864551762,
					-22.372173653878683
				],
				[
					7.63928997787586,
					-22.372173653878683
				],
				[
					8.1849446268428,
					-22.372173653878683
				],
				[
					8.1849446268428,
					-22.372173653878683
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.181640625,
				0.3642578125,
				0.380859375,
				0.392578125,
				0.41796875,
				0.439453125,
				0.453125,
				0.4580078125,
				0.46484375,
				0.47265625,
				0.4853515625,
				0.490234375,
				0.49609375,
				0.49609375,
				0.49609375,
				0.5078125,
				0.5126953125,
				0.51953125,
				0.5166015625,
				0.533203125,
				0.54296875,
				0.5458984375,
				0.5517578125,
				0.5537109375,
				0.5595703125,
				0.5615234375,
				0.5615234375,
				0.5439453125,
				0.5,
				0.4873046875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 305,
			"versionNonce": 16818835,
			"isDeleted": false,
			"id": "Yae8gClQPsRhtgApektVf",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 7020.164798383375,
			"y": 446.66700211332034,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 11.458934966813358,
			"height": 17.4612401823984,
			"seed": 244666460,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159327,
			"link": null,
			"locked": true,
			"points": [
				[
					0,
					0
				],
				[
					0.5456754643571586,
					-0.5456546489665592
				],
				[
					1.0913301133232296,
					-2.728314875613995
				],
				[
					2.1826602266473274,
					-5.456629751228045
				],
				[
					2.7283148756133984,
					-8.730599275808599
				],
				[
					3.2739903399705574,
					-10.91325950245609
				],
				[
					3.2739903399705574,
					-11.458914151422649
				],
				[
					3.8196449889374966,
					-11.458914151422649
				],
				[
					4.365320453294655,
					-10.367604853489475
				],
				[
					3.8196449889374966,
					-9.821950204522917
				],
				[
					2.7283148756133984,
					-8.730599275808599
				],
				[
					1.0913301133232296,
					-7.0936353289089205
				],
				[
					0,
					-6.547980679942362
				],
				[
					-1.0913092979330103,
					-6.547980679942362
				],
				[
					-2.7283148756142674,
					-7.0936353289089205
				],
				[
					-3.8196241735472776,
					-8.18494462684204
				],
				[
					-5.456629751228535,
					-9.276295555556356
				],
				[
					-7.093614513518703,
					-12.004610431170406
				],
				[
					-7.093614513518703,
					-13.641574378070084
				],
				[
					-6.547939049161545,
					-14.732925306784402
				],
				[
					-4.910954286871375,
					-16.36988925368408
				],
				[
					-3.273969524581206,
					-17.4612401823984
				],
				[
					-2.7283148756142674,
					-17.4612401823984
				],
				[
					-1.0913092979330103,
					-17.4612401823984
				],
				[
					-1.0913092979330103,
					-17.4612401823984
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2255859375,
				0.4296875,
				0.4755859375,
				0.4931640625,
				0.49609375,
				0.49609375,
				0.44921875,
				0.3076171875,
				0.2001953125,
				0.224609375,
				0.2666015625,
				0.3408203125,
				0.41015625,
				0.4609375,
				0.5,
				0.509765625,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.5087890625,
				0.4990234375,
				0.49609375,
				0.015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 305,
			"versionNonce": 113165341,
			"isDeleted": false,
			"id": "WDJwtPxOUlzKjpvNKZ6uq",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 7013.616859334214,
			"y": 471.2218359938465,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 8.73062009119909,
			"height": 18.552549480331514,
			"seed": 1862400732,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159327,
			"link": null,
			"locked": true,
			"points": [
				[
					0,
					0
				],
				[
					-1.0913301133232294,
					0.5456546489666135
				],
				[
					-1.637005577680388,
					1.0913092979331185
				],
				[
					-1.0913301133232294,
					1.636963946899732
				],
				[
					-0.5456754643571586,
					2.728314875614049
				],
				[
					1.09130929793301,
					3.273969524580554
				],
				[
					3.273969524580337,
					3.273969524580554
				],
				[
					4.365299637904435,
					2.1826602266474353
				],
				[
					5.456629751228534,
					1.0913092979331185
				],
				[
					5.456629751228534,
					-0.5456546489666135
				],
				[
					4.910954286871374,
					-1.0913509287143168
				],
				[
					3.273969524580337,
					-2.1826602266474353
				],
				[
					2.182639411257108,
					-2.1826602266474353
				],
				[
					2.182639411257108,
					-3.273969524580554
				],
				[
					4.365299637904435,
					-4.365320453294871
				],
				[
					6.002284400194603,
					-6.002284400194602
				],
				[
					7.093614513518702,
					-8.730599275808652
				],
				[
					5.456629751228534,
					-10.913259502456087
				],
				[
					3.8196241735472767,
					-12.550265080136908
				],
				[
					2.182639411257108,
					-14.187229027036642
				],
				[
					1.09130929793301,
					-15.27857995575096
				],
				[
					1.6369847622901685,
					-14.187229027036642
				],
				[
					2.728314875614267,
					-9.821950204522969
				],
				[
					0,
					0
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.1943359375,
				0.2529296875,
				0.384765625,
				0.412109375,
				0.4521484375,
				0.478515625,
				0.490234375,
				0.4951171875,
				0.4970703125,
				0.4970703125,
				0.4970703125,
				0.5009765625,
				0.5087890625,
				0.5166015625,
				0.509765625,
				0.4912109375,
				0.4658203125,
				0.501953125,
				0.5205078125,
				0.5224609375,
				0.5205078125,
				0.259765625,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 303,
			"versionNonce": 1553258547,
			"isDeleted": false,
			"id": "VQCMsrfTiiPoDrpnMNAVD",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 7021.256128496699,
			"y": 496.3223245233392,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 10.9132595024562,
			"height": 13.095919729103525,
			"seed": 571577692,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159327,
			"link": null,
			"locked": true,
			"points": [
				[
					0,
					0
				],
				[
					-1.6369847622901685,
					0.5456546489666136
				],
				[
					-2.728314875613398,
					0.5456546489666136
				],
				[
					-4.365299637904435,
					0.5456546489666136
				],
				[
					-5.456629751227665,
					0
				],
				[
					-6.002284400194603,
					-0.5456546489666136
				],
				[
					-5.456629751227665,
					-2.182660226647436
				],
				[
					-2.728314875613398,
					-4.365320453294872
				],
				[
					-1.6369847622901685,
					-6.002284400194605
				],
				[
					-1.6369847622901685,
					-7.639289977875536
				],
				[
					-1.6369847622901685,
					-8.730599275808656
				],
				[
					-2.728314875613398,
					-10.913259502456093
				],
				[
					-4.910954286870506,
					-12.00456880038921
				],
				[
					-8.184944626841931,
					-12.550265080136912
				],
				[
					-9.8219293891321,
					-12.00456880038921
				],
				[
					-10.367584038099038,
					-12.00456880038921
				],
				[
					-10.9132595024562,
					-12.00456880038921
				],
				[
					-10.9132595024562,
					-11.458914151422595
				],
				[
					-10.367584038099038,
					-9.27625392477516
				],
				[
					-8.184944626841931,
					-7.093635328908921
				],
				[
					0,
					0
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.189453125,
				0.3291015625,
				0.4111328125,
				0.498046875,
				0.5244140625,
				0.5361328125,
				0.5361328125,
				0.5224609375,
				0.5029296875,
				0.4970703125,
				0.4970703125,
				0.4990234375,
				0.509765625,
				0.5341796875,
				0.5390625,
				0.5390625,
				0.5390625,
				0.4345703125,
				0.2119140625,
				0.0126953125,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 289,
			"versionNonce": 99235965,
			"isDeleted": false,
			"id": "elFx3phLJBMhzuUL1I1ZD",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 7015.799498745471,
			"y": 527.4250974530266,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 1.6369847622901685,
			"height": 18.006853200583866,
			"seed": 478299364,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159327,
			"link": null,
			"locked": true,
			"points": [
				[
					0,
					0
				],
				[
					0.5456754643571586,
					-6.547939049161271
				],
				[
					1.6369847622901685,
					-11.458914151422649
				],
				[
					1.6369847622901685,
					-15.278538324969816
				],
				[
					0.5456754643571586,
					-17.461198551617255
				],
				[
					0.5456754643571586,
					-18.006853200583866
				],
				[
					0.5456754643571586,
					-17.461198551617255
				],
				[
					1.0913301133232294,
					-15.278538324969816
				],
				[
					1.0913301133232294,
					-15.278538324969816
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2109375,
				0.4482421875,
				0.49609375,
				0.498046875,
				0.498046875,
				0.484375,
				0.271484375,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 299,
			"versionNonce": 1330731475,
			"isDeleted": false,
			"id": "CXubDOUDlLikJEqih4rfl",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 7009.251538880919,
			"y": 554.1625915602003,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 10.36760485348926,
			"height": 17.4612401823984,
			"seed": 277263972,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159327,
			"link": null,
			"locked": true,
			"points": [
				[
					0,
					0
				],
				[
					1.637005577680388,
					4.3653204532948715
				],
				[
					4.910975102261594,
					3.8196241735470595
				],
				[
					7.639289977874991,
					2.1827018574286345
				],
				[
					9.276274740166029,
					0.5456962797478121
				],
				[
					10.36760485348926,
					-1.091309297933227
				],
				[
					10.36760485348926,
					-3.8196241735470595
				],
				[
					10.36760485348926,
					-8.184944626842148
				],
				[
					9.821950204523189,
					-10.367604853489475
				],
				[
					9.276274740166029,
					-11.458914151422704
				],
				[
					8.73062009119909,
					-12.004568800389206
				],
				[
					7.0936353289089205,
					-12.550223449355714
				],
				[
					4.365320453294655,
					-13.095919729103525
				],
				[
					2.728314875614267,
					-12.550223449355714
				],
				[
					1.637005577680388,
					-12.004568800389206
				],
				[
					1.0913301133232294,
					-8.730599275808654
				],
				[
					2.1826602266473274,
					-4.910975102261377
				],
				[
					0,
					0
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2021484375,
				0.248046875,
				0.2744140625,
				0.28125,
				0.310546875,
				0.353515625,
				0.404296875,
				0.45703125,
				0.4814453125,
				0.490234375,
				0.501953125,
				0.509765625,
				0.51171875,
				0.51171875,
				0.50390625,
				0.3203125,
				0.0146484375,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 343,
			"versionNonce": 208150749,
			"isDeleted": false,
			"id": "O_yNuEUA1LQVpXBMRneme",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 7003.7949091296905,
			"y": 562.8932324667901,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 548.3913108138083,
			"height": 25.10053016027382,
			"seed": 1199622500,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159327,
			"link": null,
			"locked": true,
			"points": [
				[
					0,
					0
				],
				[
					0.5456754643571586,
					0
				],
				[
					2.1826602266481956,
					0
				],
				[
					4.910975102261594,
					-0.545696279747595
				],
				[
					7.0936353289089205,
					-0.545696279747595
				],
				[
					12.004589615780297,
					-1.09130929793301
				],
				[
					15.27857995575172,
					-1.09130929793301
				],
				[
					18.552549480332058,
					-1.6370055776808223
				],
				[
					21.8265190049124,
					-2.1827018574286345
				],
				[
					27.28314875614093,
					-2.72831487561405
				],
				[
					36.55942349630609,
					-3.2740111553616447
				],
				[
					42.56172871189178,
					-3.8196241735470595
				],
				[
					48.56401311208639,
					-4.3653204532948715
				],
				[
					61.114257376832754,
					-4.9110167330426835
				],
				[
					68.75354735470775,
					-5.456629751227882
				],
				[
					77.4841466305166,
					-5.456629751227882
				],
				[
					87.30607601964871,
					-6.002326030975693
				],
				[
					95.49102064649064,
					-6.002326030975693
				],
				[
					105.85862549998076,
					-6.002326030975693
				],
				[
					120.04585452701731,
					-6.5479390491611085
				],
				[
					131.50478949383066,
					-6.5479390491611085
				],
				[
					141.32673969835298,
					-7.0936353289089205
				],
				[
					158.24228360100378,
					-8.184944626841931
				],
				[
					168.6098884544939,
					-8.184944626841931
				],
				[
					180.61445725488312,
					-8.730640906589743
				],
				[
					190.98206210837236,
					-9.27629555555625
				],
				[
					204.0779818374759,
					-9.82195020452297
				],
				[
					214.44554506018386,
					-10.913301133237288
				],
				[
					232.99809454051592,
					-12.004610431170299
				],
				[
					245.00270497168555,
					-12.550265080136803
				],
				[
					257.00727377207477,
					-13.641616008851122
				],
				[
					275.5598232524068,
					-15.278579955750851
				],
				[
					285.92742810589607,
					-15.824234604717574
				],
				[
					298.4776515552522,
					-16.915585533431894
				],
				[
					309.3909110577084,
					-17.4612401823984
				],
				[
					321.941176137845,
					-18.006894831364903
				],
				[
					332.85443564030123,
					-19.09824576007922
				],
				[
					351.4069851206324,
					-20.18955505801244
				],
				[
					363.41155392102166,
					-20.73520970697895
				],
				[
					375.9618190011591,
					-21.280864355945457
				],
				[
					387.9663878015483,
					-21.826560635693266
				],
				[
					404.3362770552322,
					-22.372215284659774
				],
				[
					416.3408458556213,
					-22.9178699336265
				],
				[
					426.1627960601445,
					-23.463524582593
				],
				[
					437.0760555626007,
					-24.009179231559507
				],
				[
					446.3523094873757,
					-24.554875511307323
				],
				[
					460.5395801451935,
					-24.554875511307323
				],
				[
					473.0898035945488,
					-25.10053016027382
				],
				[
					480.18343892345774,
					-25.10053016027382
				],
				[
					488.91407983004785,
					-25.10053016027382
				],
				[
					494.9163225994611,
					-25.10053016027382
				],
				[
					500.9186486304371,
					-25.10053016027382
				],
				[
					508.5578969775317,
					-24.554875511307323
				],
				[
					527.6561011068299,
					-24.554875511307323
				],
				[
					533.6584271378057,
					-24.554875511307323
				],
				[
					540.2063661869663,
					-24.009179231559507
				],
				[
					542.9346810625806,
					-24.009179231559507
				],
				[
					545.6629959381949,
					-23.463524582593
				],
				[
					546.754305236128,
					-22.9178699336265
				],
				[
					547.8456145340609,
					-22.9178699336265
				],
				[
					548.3913108138083,
					-22.372215284659774
				],
				[
					546.754305236128,
					-22.9178699336265
				],
				[
					546.754305236128,
					-22.9178699336265
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2158203125,
				0.4462890625,
				0.474609375,
				0.482421875,
				0.484375,
				0.4912109375,
				0.4931640625,
				0.4931640625,
				0.4931640625,
				0.4931640625,
				0.4931640625,
				0.4951171875,
				0.4970703125,
				0.4970703125,
				0.4970703125,
				0.4970703125,
				0.4970703125,
				0.4970703125,
				0.4970703125,
				0.4970703125,
				0.4970703125,
				0.4970703125,
				0.4970703125,
				0.4970703125,
				0.4970703125,
				0.4990234375,
				0.4990234375,
				0.5009765625,
				0.5009765625,
				0.5068359375,
				0.5068359375,
				0.5087890625,
				0.5087890625,
				0.5107421875,
				0.5126953125,
				0.5126953125,
				0.5126953125,
				0.5146484375,
				0.517578125,
				0.517578125,
				0.5146484375,
				0.517578125,
				0.517578125,
				0.51953125,
				0.515625,
				0.5185546875,
				0.521484375,
				0.515625,
				0.513671875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.494140625,
				0.46875,
				0.0126953125,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 336,
			"versionNonce": 1716299635,
			"isDeleted": false,
			"id": "3xQbE4d5ogHNdjrh8xAxy",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 7053.4502523551,
			"y": 542.7036774087777,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 6.547939049161543,
			"height": 37.65075360962959,
			"seed": 1009662308,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159327,
			"link": null,
			"locked": true,
			"points": [
				[
					0,
					0
				],
				[
					0.5456546489669393,
					-2.72831487561405
				],
				[
					1.0913301133240978,
					-4.910975102261377
				],
				[
					1.6369847622901685,
					-8.184944626841931
				],
				[
					2.182639411257108,
					-11.458914151422485
				],
				[
					1.6369847622901685,
					-17.46119855161709
				],
				[
					1.6369847622901685,
					-20.18951342723119
				],
				[
					1.6369847622901685,
					-21.280864355945507
				],
				[
					1.0913301133240978,
					-19.64385877826458
				],
				[
					0.5456546489669393,
					-13.095919729103525
				],
				[
					-0.5456754643571586,
					-7.0936353289089205
				],
				[
					-1.0913301133232294,
					-3.2739695245805542
				],
				[
					-1.6369847622901685,
					-0.545654648966505
				],
				[
					-2.1826602266473274,
					1.091309297933227
				],
				[
					-2.728314875613398,
					2.182660226647544
				],
				[
					-2.728314875613398,
					1.6370055776810395
				],
				[
					-2.1826602266473274,
					-1.09130929793301
				],
				[
					-0.5456754643571586,
					-6.002284400194603
				],
				[
					0.5456546489669393,
					-12.004568800389206
				],
				[
					1.6369847622901685,
					-18.006894831364903
				],
				[
					2.182639411257108,
					-22.37217365387863
				],
				[
					2.182639411257108,
					-24.554833880526065
				],
				[
					2.182639411257108,
					-21.280864355945507
				],
				[
					1.0913301133240978,
					-13.095919729103525
				],
				[
					0.5456546489669393,
					-8.184944626841931
				],
				[
					-0.5456754643571586,
					-3.2739695245805542
				],
				[
					-2.1826602266473274,
					4.3653204532948715
				],
				[
					-2.728314875613398,
					7.639289977875643
				],
				[
					-3.273990339970556,
					6.547939049161326
				],
				[
					-2.728314875613398,
					1.091309297933227
				],
				[
					-2.1826602266473274,
					-3.2739695245805542
				],
				[
					-1.6369847622901685,
					-8.730599275808654
				],
				[
					-1.0913301133232294,
					-16.915543902650583
				],
				[
					-1.0913301133232294,
					-20.735209706978896
				],
				[
					-1.0913301133232294,
					-21.280864355945507
				],
				[
					-1.0913301133232294,
					-20.18951342723119
				],
				[
					-1.6369847622901685,
					-14.187229027036535
				],
				[
					-2.1826602266473274,
					-3.8196241735470595
				],
				[
					-3.273990339970556,
					3.8196241735472767
				],
				[
					-3.8196449889374957,
					9.276253924775158
				],
				[
					-4.365299637904435,
					12.550223449355931
				],
				[
					-4.365299637904435,
					13.095919729103525
				],
				[
					-4.365299637904435,
					12.550223449355931
				],
				[
					-4.365299637904435,
					6.547939049161326
				],
				[
					-3.8196449889374957,
					-0.545654648966505
				],
				[
					-2.728314875613398,
					-6.5479390491611085
				],
				[
					-2.1826602266473274,
					-15.278579955750851
				],
				[
					-2.1826602266473274,
					-16.915543902650583
				],
				[
					-2.1826602266473274,
					-13.64157437807003
				],
				[
					-2.728314875613398,
					-9.276253924775158
				],
				[
					-2.728314875613398,
					-3.2739695245805542
				],
				[
					-2.728314875613398,
					-1.6370055776808223
				],
				[
					-2.728314875613398,
					1.6370055776810395
				],
				[
					-2.728314875613398,
					2.182660226647544
				],
				[
					0,
					0
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.1943359375,
				0.333984375,
				0.39453125,
				0.4443359375,
				0.4716796875,
				0.4931640625,
				0.49609375,
				0.498046875,
				0.509765625,
				0.5,
				0.498046875,
				0.49609375,
				0.498046875,
				0.498046875,
				0.5,
				0.5078125,
				0.509765625,
				0.509765625,
				0.505859375,
				0.5,
				0.498046875,
				0.498046875,
				0.50390625,
				0.5,
				0.50390625,
				0.5126953125,
				0.5126953125,
				0.5126953125,
				0.5244140625,
				0.529296875,
				0.5263671875,
				0.5244140625,
				0.5244140625,
				0.5185546875,
				0.515625,
				0.5087890625,
				0.501953125,
				0.5,
				0.5048828125,
				0.5087890625,
				0.5107421875,
				0.5107421875,
				0.529296875,
				0.5400390625,
				0.5341796875,
				0.5283203125,
				0.5263671875,
				0.5244140625,
				0.5244140625,
				0.5244140625,
				0.5224609375,
				0.5166015625,
				0.4423828125,
				0.33203125,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 329,
			"versionNonce": 1875508541,
			"isDeleted": false,
			"id": "-fVB2RQtKx73ZwQaKfMfj",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 7099.285929776181,
			"y": 323.34717806172296,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 6.002305215584823,
			"height": 235.1807755825534,
			"seed": 1059871964,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159327,
			"link": null,
			"locked": true,
			"points": [
				[
					0,
					0
				],
				[
					0.5456754643571585,
					-1.0913509287143173
				],
				[
					0.5456754643571585,
					-0.5456962797477578
				],
				[
					0,
					5.456629751228045
				],
				[
					0,
					9.276253924775158
				],
				[
					0,
					15.278538324969762
				],
				[
					0,
					19.09820412929813
				],
				[
					0,
					26.191797827425855
				],
				[
					-0.5456546489660707,
					33.285433156334776
				],
				[
					-1.09130929793301,
					45.290001956723984
				],
				[
					-1.09130929793301,
					52.92929193459946
				],
				[
					-1.09130929793301,
					61.65989121040812
				],
				[
					-1.09130929793301,
					75.3014655884782
				],
				[
					-1.09130929793301,
					85.66907044196766
				],
				[
					-1.09130929793301,
					96.58232994442376
				],
				[
					-1.6369847622901683,
					111.86090990017472
				],
				[
					-1.6369847622901683,
					121.13716382494994
				],
				[
					-1.6369847622901683,
					130.41341774972514
				],
				[
					-2.182639411256239,
					140.23536795424803
				],
				[
					-2.182639411256239,
					148.42031258109017
				],
				[
					-2.182639411256239,
					158.78791743457964
				],
				[
					-2.182639411256239,
					167.5185167103883
				],
				[
					-2.7283148756133975,
					180.06878179052518
				],
				[
					-2.7283148756133975,
					186.6167208396864
				],
				[
					-2.7283148756133975,
					191.5276959419478
				],
				[
					-2.7283148756133975,
					198.62128964007562
				],
				[
					-3.2739695245803366,
					210.08024542227938
				],
				[
					-3.819624173546407,
					215.53687517350747
				],
				[
					-3.819624173546407,
					217.71949376937368
				],
				[
					-4.365299637903566,
					220.99350492473553
				],
				[
					-4.365299637903566,
					223.1761235206018
				],
				[
					-4.365299637903566,
					224.81312909828264
				],
				[
					-4.365299637903566,
					226.99578932493014
				],
				[
					-4.365299637903566,
					228.63275327182967
				],
				[
					-4.365299637903566,
					229.724104200544
				],
				[
					-4.365299637903566,
					231.36110977822503
				],
				[
					-4.365299637903566,
					231.90672279641043
				],
				[
					-4.365299637903566,
					232.45241907615804
				],
				[
					-4.365299637903566,
					233.54372837409127
				],
				[
					-4.365299637903566,
					234.08942465383907
				],
				[
					-4.910954286870505,
					233.54372837409127
				],
				[
					-4.910954286870505,
					232.99811535590587
				],
				[
					-4.910954286870505,
					231.90672279641043
				],
				[
					-4.910954286870505,
					230.2697588495107
				],
				[
					-4.910954286870505,
					226.99578932493014
				],
				[
					-5.4566297512276645,
					221.53915957370208
				],
				[
					-5.4566297512276645,
					220.44780864498776
				],
				[
					-5.4566297512276645,
					220.44780864498776
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.177734375,
				0.25,
				0.365234375,
				0.392578125,
				0.39453125,
				0.39453125,
				0.3994140625,
				0.408203125,
				0.416015625,
				0.443359375,
				0.4609375,
				0.474609375,
				0.4833984375,
				0.4892578125,
				0.486328125,
				0.490234375,
				0.4921875,
				0.494140625,
				0.494140625,
				0.4990234375,
				0.5087890625,
				0.51171875,
				0.517578125,
				0.517578125,
				0.513671875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.560546875,
				0.5185546875,
				0.5126953125,
				0.5146484375,
				0.51953125,
				0.51953125,
				0.51953125,
				0.51953125,
				0.51953125,
				0.51953125,
				0.517578125,
				0.51953125,
				0.501953125,
				0.498046875,
				0.458984375,
				0.4140625,
				0.2646484375,
				0.05078125,
				0.0126953125,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 330,
			"versionNonce": 1204633875,
			"isDeleted": false,
			"id": "k4Nk0VBIMYB2CEYgHDHEY",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 7096.557614900568,
			"y": 332.0777773375316,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 2.1826602266473274,
			"height": 217.17388075118834,
			"seed": 1624048356,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159327,
			"link": null,
			"locked": true,
			"points": [
				[
					0,
					0
				],
				[
					-0.5456546489669393,
					-1.0913509287143168
				],
				[
					-0.5456546489669393,
					-0.5456546489665592
				],
				[
					-0.5456546489669393,
					2.728314875614049
				],
				[
					-0.5456546489669393,
					8.184944626842093
				],
				[
					-0.5456546489669393,
					13.095919729103523
				],
				[
					-0.5456546489669393,
					20.73516807619786
				],
				[
					-0.5456546489669393,
					25.646143178459287
				],
				[
					0,
					32.73977850736821
				],
				[
					0,
					39.28771755652942
				],
				[
					0,
					45.83569823647173
				],
				[
					0,
					53.47494658356606
				],
				[
					0.5456754643571585,
					60.56858191247498
				],
				[
					0.5456754643571585,
					69.84483583725014
				],
				[
					0.5456754643571585,
					76.93847116615906
				],
				[
					1.0913301133232294,
					83.48641021532022
				],
				[
					1.0913301133232294,
					89.48873624629603
				],
				[
					1.0913301133232294,
					98.76499017107125
				],
				[
					1.0913301133232294,
					105.31292922023239
				],
				[
					1.0913301133232294,
					110.76955897146046
				],
				[
					1.0913301133232294,
					116.77188500243618
				],
				[
					1.637005577680388,
					123.86547870056397
				],
				[
					1.637005577680388,
					132.5960779763726
				],
				[
					1.637005577680388,
					138.05270772760062
				],
				[
					1.637005577680388,
					144.0550337585764
				],
				[
					1.637005577680388,
					150.057318158771
				],
				[
					1.0913301133232294,
					157.15091185689874
				],
				[
					1.0913301133232294,
					162.60754160812672
				],
				[
					1.0913301133232294,
					167.51851671038818
				],
				[
					1.0913301133232294,
					172.4294918126497
				],
				[
					0.5456754643571585,
					177.34046691491116
				],
				[
					0.5456754643571585,
					182.25144201717265
				],
				[
					0,
					185.52541154175321
				],
				[
					0,
					188.79938106633378
				],
				[
					0,
					192.07335059091443
				],
				[
					0,
					196.9843256931759
				],
				[
					0,
					199.71264056878988
				],
				[
					0,
					201.89530079543724
				],
				[
					0,
					204.0779610220848
				],
				[
					0,
					205.71492496898452
				],
				[
					0,
					207.89758519563182
				],
				[
					0,
					209.53459077331286
				],
				[
					0,
					211.1715547202126
				],
				[
					0,
					212.2629056489269
				],
				[
					0,
					212.80856029789345
				],
				[
					0.5456754643571585,
					213.35421494685994
				],
				[
					0.5456754643571585,
					214.44552424479318
				],
				[
					0.5456754643571585,
					216.08252982247402
				],
				[
					0.5456754643571585,
					216.08252982247402
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.17578125,
				0.263671875,
				0.365234375,
				0.365234375,
				0.38671875,
				0.396484375,
				0.41015625,
				0.4140625,
				0.4140625,
				0.423828125,
				0.4287109375,
				0.4345703125,
				0.4345703125,
				0.439453125,
				0.4453125,
				0.4580078125,
				0.4736328125,
				0.4833984375,
				0.4921875,
				0.4951171875,
				0.4970703125,
				0.4970703125,
				0.5009765625,
				0.5068359375,
				0.5107421875,
				0.5107421875,
				0.5146484375,
				0.51953125,
				0.51953125,
				0.51953125,
				0.51953125,
				0.521484375,
				0.521484375,
				0.521484375,
				0.521484375,
				0.521484375,
				0.521484375,
				0.515625,
				0.513671875,
				0.513671875,
				0.513671875,
				0.517578125,
				0.517578125,
				0.517578125,
				0.5107421875,
				0.48046875,
				0.41015625,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 321,
			"versionNonce": 1467043229,
			"isDeleted": false,
			"id": "wCPURhtYGwsNY_g_061Qa",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 7143.484643250364,
			"y": 376.82212464528897,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 2.1826602266473274,
			"height": 160.4249230122606,
			"seed": 1488460388,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159328,
			"link": null,
			"locked": true,
			"points": [
				[
					0,
					0
				],
				[
					0.5456546489660709,
					0.5456546489666135
				],
				[
					0.5456546489660709,
					1.0913509287143173
				],
				[
					0.5456546489660709,
					3.273969524580609
				],
				[
					0.5456546489660709,
					5.456629751228045
				],
				[
					0.5456546489660709,
					9.82195020452297
				],
				[
					0.5456546489660709,
					14.732925306784455
				],
				[
					0.5456546489660709,
					18.55254948033157
				],
				[
					0.5456546489660709,
					24.554833880526175
				],
				[
					0.5456546489660709,
					29.46580898278766
				],
				[
					1.09130929793301,
					35.46809338298227
				],
				[
					1.09130929793301,
					41.470377783176865
				],
				[
					1.09130929793301,
					46.381352885438346
				],
				[
					1.09130929793301,
					55.6576484409947
				],
				[
					1.637005577680388,
					62.20558749015587
				],
				[
					1.637005577680388,
					67.66221724138391
				],
				[
					1.637005577680388,
					73.66450164157851
				],
				[
					1.637005577680388,
					81.303791619454
				],
				[
					1.637005577680388,
					87.85173066861522
				],
				[
					1.637005577680388,
					97.12802622417158
				],
				[
					1.637005577680388,
					103.6759652733327
				],
				[
					1.637005577680388,
					109.67824967352729
				],
				[
					1.637005577680388,
					115.13487942475537
				],
				[
					1.637005577680388,
					121.1372054557312
				],
				[
					1.637005577680388,
					128.23079915385892
				],
				[
					1.637005577680388,
					132.59611960715378
				],
				[
					1.637005577680388,
					135.87008913173435
				],
				[
					1.637005577680388,
					139.144058656315
				],
				[
					1.637005577680388,
					141.87237353192893
				],
				[
					1.637005577680388,
					144.600688407543
				],
				[
					1.09130929793301,
					147.32900328315702
				],
				[
					1.09130929793301,
					151.14866908748525
				],
				[
					1.09130929793301,
					152.78563303438497
				],
				[
					1.09130929793301,
					153.8769839630993
				],
				[
					1.09130929793301,
					154.9682932610325
				],
				[
					1.637005577680388,
					157.69660813664657
				],
				[
					1.637005577680388,
					159.3336137143274
				],
				[
					1.637005577680388,
					159.8792683632939
				],
				[
					1.637005577680388,
					160.4249230122606
				],
				[
					2.1826602266473274,
					160.4249230122606
				],
				[
					2.1826602266473274,
					160.4249230122606
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2109375,
				0.3046875,
				0.3271484375,
				0.38671875,
				0.41015625,
				0.4296875,
				0.4462890625,
				0.4560546875,
				0.470703125,
				0.478515625,
				0.48046875,
				0.48046875,
				0.486328125,
				0.494140625,
				0.4970703125,
				0.4970703125,
				0.4970703125,
				0.4990234375,
				0.5048828125,
				0.5107421875,
				0.513671875,
				0.51953125,
				0.5126953125,
				0.51953125,
				0.521484375,
				0.521484375,
				0.521484375,
				0.521484375,
				0.5234375,
				0.5234375,
				0.5234375,
				0.5234375,
				0.525390625,
				0.525390625,
				0.568359375,
				0.5263671875,
				0.5263671875,
				0.5263671875,
				0.5166015625,
				0.3388671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 321,
			"versionNonce": 222930611,
			"isDeleted": false,
			"id": "TzBskays86CLJsdsA1oIM",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 7142.938988601396,
			"y": 390.46369902335914,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 2.728314875614267,
			"height": 165.8815111327074,
			"seed": 390124516,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159328,
			"link": null,
			"locked": true,
			"points": [
				[
					0,
					0
				],
				[
					-1.0913509287143173,
					-5.456629751228045
				],
				[
					-1.0913509287143173,
					-6.547939049161218
				],
				[
					-1.0913509287143173,
					-8.184944626842093
				],
				[
					-1.0913509287143173,
					-9.821908573741773
				],
				[
					-1.0913509287143173,
					-9.276253924775212
				],
				[
					-1.0913509287143173,
					-3.8196241735471683
				],
				[
					-0.545654648966071,
					3.2739695245805542
				],
				[
					0,
					11.458914151422594
				],
				[
					0,
					18.006894831364956
				],
				[
					0.5456546489669394,
					25.10048852949268
				],
				[
					0.5456546489669394,
					31.64846920943504
				],
				[
					0.5456546489669394,
					38.74206290756282
				],
				[
					0.5456546489669394,
					46.3813528854383
				],
				[
					0.5456546489669394,
					56.20330308996122
				],
				[
					0.5456546489669394,
					62.20558749015587
				],
				[
					0.5456546489669394,
					65.47955701473643
				],
				[
					0.5456546489669394,
					72.02753769467873
				],
				[
					0.5456546489669394,
					77.48416744590683
				],
				[
					0.5456546489669394,
					82.94079719713481
				],
				[
					0.5456546489669394,
					92.7627057708766
				],
				[
					0.5456546489669394,
					98.76499017107119
				],
				[
					0.5456546489669394,
					103.6759652733327
				],
				[
					0,
					109.13259502456067
				],
				[
					0,
					115.13487942475527
				],
				[
					0.5456546489669394,
					122.77416940263082
				],
				[
					0.5456546489669394,
					127.13948985592567
				],
				[
					0.5456546489669394,
					128.77645380282542
				],
				[
					0.5456546489669394,
					137.50709470941513
				],
				[
					0.5456546489669394,
					141.32671888296238
				],
				[
					1.0913092979330103,
					144.05503375857643
				],
				[
					1.0913092979330103,
					146.78334863419047
				],
				[
					1.0913092979330103,
					149.51166350980432
				],
				[
					1.0913092979330103,
					151.69432373645185
				],
				[
					1.0913092979330103,
					153.33128768335158
				],
				[
					1.6369639468999495,
					154.42263861206592
				],
				[
					1.6369639468999495,
					154.9682932610324
				],
				[
					1.6369639468999495,
					155.5139479099989
				],
				[
					1.6369639468999495,
					156.05960255896565
				],
				[
					1.6369639468999495,
					155.5139479099989
				],
				[
					1.6369639468999495,
					155.5139479099989
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.0859375,
				0.1875,
				0.205078125,
				0.2421875,
				0.2861328125,
				0.4091796875,
				0.443359375,
				0.4638671875,
				0.4794921875,
				0.484375,
				0.4931640625,
				0.4970703125,
				0.4970703125,
				0.4970703125,
				0.5078125,
				0.5107421875,
				0.513671875,
				0.51953125,
				0.5126953125,
				0.51953125,
				0.5234375,
				0.525390625,
				0.52734375,
				0.5322265625,
				0.53515625,
				0.537109375,
				0.5498046875,
				0.580078125,
				0.541015625,
				0.541015625,
				0.541015625,
				0.541015625,
				0.541015625,
				0.541015625,
				0.541015625,
				0.541015625,
				0.541015625,
				0.5439453125,
				0.541015625,
				0.0146484375,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 309,
			"versionNonce": 42963453,
			"isDeleted": false,
			"id": "K4bMImxqNMlPtvNQAP58f",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 7191.503001713483,
			"y": 485.40906502088313,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 3.2740111553625133,
			"height": 75.84716186822595,
			"seed": 1914871140,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159328,
			"link": null,
			"locked": true,
			"points": [
				[
					0,
					0
				],
				[
					0,
					1.6370055776809305
				],
				[
					0,
					4.365320453294871
				],
				[
					0,
					6.547939049161217
				],
				[
					0,
					7.639289977875533
				],
				[
					-0.5456962797482464,
					12.004568800389205
				],
				[
					-0.5456962797482464,
					16.369889253684075
				],
				[
					-1.0913509287143173,
					21.28086435594556
				],
				[
					-1.6370055776812567,
					26.191839458207046
				],
				[
					-1.6370055776812567,
					30.55711828072082
				],
				[
					-2.1826602266481956,
					36.55940268091543
				],
				[
					-2.1826602266481956,
					42.56172871189107
				],
				[
					-2.1826602266481956,
					46.38135288543834
				],
				[
					-2.728314875614267,
					49.6553224100189
				],
				[
					-2.728314875614267,
					50.74667333873321
				],
				[
					-2.728314875614267,
					53.47498821434726
				],
				[
					-2.728314875614267,
					56.748957738927814
				],
				[
					-2.728314875614267,
					59.47727261454187
				],
				[
					-2.728314875614267,
					62.205587490155914
				],
				[
					-3.2740111553625133,
					64.38824771680324
				],
				[
					-3.2740111553625133,
					66.57086631266948
				],
				[
					-3.2740111553625133,
					69.84483583725024
				],
				[
					-3.2740111553625133,
					72.02753769467888
				],
				[
					-3.2740111553625133,
					74.21015629054511
				],
				[
					-3.2740111553625133,
					75.30146558847814
				],
				[
					-3.2740111553625133,
					75.84716186822595
				],
				[
					-2.728314875614267,
					75.30146558847814
				],
				[
					-1.6370055776812567,
					73.66454327235971
				],
				[
					-1.6370055776812567,
					73.66454327235971
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2001953125,
				0.3017578125,
				0.36328125,
				0.3896484375,
				0.4013671875,
				0.4345703125,
				0.44921875,
				0.45703125,
				0.4677734375,
				0.4775390625,
				0.486328125,
				0.4951171875,
				0.4970703125,
				0.4970703125,
				0.4970703125,
				0.4990234375,
				0.50390625,
				0.5087890625,
				0.5107421875,
				0.5126953125,
				0.517578125,
				0.513671875,
				0.513671875,
				0.513671875,
				0.51953125,
				0.51953125,
				0.30859375,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 300,
			"versionNonce": 1567119443,
			"isDeleted": false,
			"id": "gc_0qmj9kvewxcrxC4ZH5",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 7190.957305433734,
			"y": 491.9570040700443,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 3.273969524580337,
			"height": 60.02292726350837,
			"seed": 406925796,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159329,
			"link": null,
			"locked": true,
			"points": [
				[
					0,
					0
				],
				[
					-0.5456546489660709,
					-0.5456546489666134
				],
				[
					-0.5456546489660709,
					0.5456962797477034
				],
				[
					-0.5456546489660709,
					4.910975102261484
				],
				[
					-0.5456546489660709,
					12.550265080136908
				],
				[
					0,
					18.006894831365006
				],
				[
					-0.5456546489660709,
					25.64618480924043
				],
				[
					-1.09130929793301,
					31.10281456046853
				],
				[
					-1.6369639468999493,
					38.19640825859631
				],
				[
					-2.18261859586602,
					42.01607406292446
				],
				[
					-2.728314875614267,
					44.7443889385385
				],
				[
					-3.273969524580337,
					47.47270381415255
				],
				[
					-3.273969524580337,
					48.56401311208578
				],
				[
					-3.273969524580337,
					50.2010186897666
				],
				[
					-3.273969524580337,
					51.83798263666633
				],
				[
					-2.728314875614267,
					53.47498821434716
				],
				[
					-2.728314875614267,
					55.111993792027974
				],
				[
					-2.18261859586602,
					59.47727261454176
				],
				[
					-2.18261859586602,
					59.47727261454176
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.1630859375,
				0.23828125,
				0.3837890625,
				0.4296875,
				0.470703125,
				0.4892578125,
				0.5,
				0.51171875,
				0.5205078125,
				0.533203125,
				0.5458984375,
				0.548828125,
				0.5517578125,
				0.5517578125,
				0.546875,
				0.5107421875,
				0.439453125,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 315,
			"versionNonce": 1311132253,
			"isDeleted": false,
			"id": "5vHTD-HlibR5uidfXoSMT",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 7244.977948297048,
			"y": 406.8335882770432,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 4.365278822514216,
			"height": 134.23308355405345,
			"seed": 410969316,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159329,
			"link": null,
			"locked": true,
			"points": [
				[
					0,
					0
				],
				[
					0,
					0.5456546489665592
				],
				[
					0,
					1.6370055776808765
				],
				[
					0,
					4.365320453294926
				],
				[
					0,
					8.730599275808599
				],
				[
					-0.5456546489669393,
					11.458914151422649
				],
				[
					-0.5456546489669393,
					15.278579955750962
				],
				[
					-0.5456546489669393,
					19.64385877826469
				],
				[
					-0.5456546489669393,
					22.37217365387874
				],
				[
					-0.5456546489669393,
					30.01146363175422
				],
				[
					-1.09130929793301,
					33.83112943608253
				],
				[
					-1.09130929793301,
					38.19640825859626
				],
				[
					-1.09130929793301,
					42.561728711891185
				],
				[
					-1.6369639468999493,
					47.47270381415261
				],
				[
					-1.6369639468999493,
					53.47498821434722
				],
				[
					-2.1826602266473274,
					60.56858191247494
				],
				[
					-2.728314875614267,
					64.3882477168033
				],
				[
					-2.728314875614267,
					69.29922281906478
				],
				[
					-2.728314875614267,
					74.75585257029279
				],
				[
					-2.728314875614267,
					79.66678604177307
				],
				[
					-3.2739695245812057,
					85.66911207274887
				],
				[
					-3.8196241735472767,
					89.48873624629604
				],
				[
					-3.8196241735472767,
					96.03667529545724
				],
				[
					-3.8196241735472767,
					100.40199574875213
				],
				[
					-3.8196241735472767,
					103.6759652733327
				],
				[
					-3.8196241735472767,
					106.94993479791324
				],
				[
					-3.8196241735472767,
					111.31525525120823
				],
				[
					-3.8196241735472767,
					114.04357012682216
				],
				[
					-4.365278822514216,
					123.31982405159746
				],
				[
					-4.365278822514216,
					130.4134593805064
				],
				[
					-4.365278822514216,
					130.95911402947291
				],
				[
					-4.365278822514216,
					132.05046495818723
				],
				[
					-3.8196241735472767,
					133.14177425612021
				],
				[
					-3.8196241735472767,
					134.23308355405345
				],
				[
					-3.8196241735472767,
					134.23308355405345
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.1943359375,
				0.3203125,
				0.40234375,
				0.4716796875,
				0.4921875,
				0.4951171875,
				0.4970703125,
				0.4990234375,
				0.4990234375,
				0.5107421875,
				0.515625,
				0.521484375,
				0.5126953125,
				0.5146484375,
				0.51953125,
				0.521484375,
				0.521484375,
				0.5234375,
				0.5234375,
				0.5322265625,
				0.5400390625,
				0.5400390625,
				0.5400390625,
				0.54296875,
				0.5458984375,
				0.5478515625,
				0.5537109375,
				0.5556640625,
				0.5556640625,
				0.5556640625,
				0.5556640625,
				0.5556640625,
				0.4345703125,
				0.2734375,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 323,
			"versionNonce": 1174394355,
			"isDeleted": false,
			"id": "f-hRZXoeWABoY9ziH6kyJ",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 7242.249633421434,
			"y": 412.83587267723783,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 4.365278822514216,
			"height": 143.50937910960988,
			"seed": 541570020,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159329,
			"link": null,
			"locked": true,
			"points": [
				[
					0,
					0
				],
				[
					0.5456546489669393,
					-1.636963946899678
				],
				[
					0.5456546489669393,
					-1.0913092979331185
				],
				[
					0.5456546489669393,
					-0.5456546489665592
				],
				[
					0,
					4.365320453294926
				],
				[
					0,
					7.639289977875481
				],
				[
					0,
					12.004610431170406
				],
				[
					0,
					20.735209706979006
				],
				[
					-0.5456546489669393,
					27.283148756140168
				],
				[
					-1.6369639468999493,
					36.01378966272997
				],
				[
					-2.182660226647327,
					42.56172871189113
				],
				[
					-2.7283148756142666,
					48.01835846311923
				],
				[
					-2.7283148756142666,
					55.11199379202815
				],
				[
					-2.7283148756142666,
					58.93161796557532
				],
				[
					-2.7283148756142666,
					64.93390236576992
				],
				[
					-3.2739695245803375,
					69.29922281906478
				],
				[
					-3.2739695245803375,
					73.11884699261196
				],
				[
					-3.2739695245803375,
					78.57547674383994
				],
				[
					-3.2739695245803375,
					81.84944626842052
				],
				[
					-3.2739695245803375,
					86.760421370682
				],
				[
					-3.2739695245803375,
					91.12574182397698
				],
				[
					-3.819624173547277,
					94.94536599752402
				],
				[
					-3.819624173547277,
					98.2193355221047
				],
				[
					-3.819624173547277,
					100.94765039771865
				],
				[
					-3.819624173547277,
					103.6759652733327
				],
				[
					-3.2739695245803375,
					106.40428014894674
				],
				[
					-3.2739695245803375,
					110.7696006022416
				],
				[
					-3.2739695245803375,
					115.68057570450314
				],
				[
					-3.2739695245803375,
					118.4088905801172
				],
				[
					-3.2739695245803375,
					120.59155080676453
				],
				[
					-3.2739695245803375,
					123.86552033134508
				],
				[
					-3.2739695245803375,
					126.04818055799261
				],
				[
					-3.2739695245803375,
					128.23079915385884
				],
				[
					-3.2739695245803375,
					129.86780473153968
				],
				[
					-3.2739695245803375,
					131.50481030922072
				],
				[
					-3.2739695245803375,
					133.14177425612021
				],
				[
					-3.2739695245803375,
					134.23312518483453
				],
				[
					-2.7283148756142666,
					136.9614400604486
				],
				[
					-2.7283148756142666,
					139.14405865631483
				],
				[
					-2.7283148756142666,
					140.23540958502915
				],
				[
					-2.7283148756142666,
					141.87241516271018
				],
				[
					-2.7283148756142666,
					141.87241516271018
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.1123046875,
				0.216796875,
				0.3779296875,
				0.3857421875,
				0.421875,
				0.439453125,
				0.4541015625,
				0.4775390625,
				0.4853515625,
				0.494140625,
				0.5078125,
				0.51171875,
				0.521484375,
				0.525390625,
				0.525390625,
				0.525390625,
				0.525390625,
				0.52734375,
				0.529296875,
				0.5322265625,
				0.53515625,
				0.53515625,
				0.53515625,
				0.53515625,
				0.5390625,
				0.5390625,
				0.5390625,
				0.5390625,
				0.5390625,
				0.5439453125,
				0.5458984375,
				0.548828125,
				0.55078125,
				0.55078125,
				0.552734375,
				0.552734375,
				0.552734375,
				0.5126953125,
				0.4912109375,
				0.4453125,
				0.349609375,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 313,
			"versionNonce": 2064053949,
			"isDeleted": false,
			"id": "D1s0VFjEnicBEfYFdginh",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 7289.722337235587,
			"y": 428.1144526329888,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 4.365278822514216,
			"height": 120.04585452701681,
			"seed": 1871608540,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159329,
			"link": null,
			"locked": true,
			"points": [
				[
					0,
					0
				],
				[
					0.5456546489669393,
					0.5456546489665592
				],
				[
					1.09130929793301,
					7.639289977875481
				],
				[
					1.6369639468999493,
					12.550265080136967
				],
				[
					1.6369639468999493,
					17.461198551617255
				],
				[
					1.6369639468999493,
					21.82651900491218
				],
				[
					1.6369639468999493,
					26.73749410717366
				],
				[
					1.09130929793301,
					32.19412385840165
				],
				[
					1.09130929793301,
					36.55940268091544
				],
				[
					0.5456546489669393,
					42.016032432143426
				],
				[
					0,
					46.3813528854383
				],
				[
					0,
					51.837982636666396
				],
				[
					0,
					56.20330308996127
				],
				[
					0,
					61.65993284118925
				],
				[
					0,
					66.57086631266955
				],
				[
					0,
					70.93618676596454
				],
				[
					0,
					75.84716186822601
				],
				[
					0,
					80.21244069073968
				],
				[
					0,
					85.12341579300117
				],
				[
					-0.5456962797473779,
					89.48873624629604
				],
				[
					-0.5456962797473779,
					92.7627057708766
				],
				[
					-1.0913509287143173,
					97.1280262241716
				],
				[
					-1.0913509287143173,
					101.4933050466852
				],
				[
					-1.637005577680388,
					108.0412857266276
				],
				[
					-1.637005577680388,
					109.13259502456083
				],
				[
					-1.637005577680388,
					110.76960060224165
				],
				[
					-2.1826602266473274,
					111.86090990017466
				],
				[
					-2.1826602266473274,
					114.58922477578872
				],
				[
					-2.1826602266473274,
					116.22623035346976
				],
				[
					-2.728314875614267,
					117.86319430036926
				],
				[
					-2.728314875614267,
					120.04585452701681
				],
				[
					-2.1826602266473274,
					115.13487942475544
				],
				[
					-2.1826602266473274,
					115.13487942475544
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.173828125,
				0.4462890625,
				0.4921875,
				0.4970703125,
				0.4970703125,
				0.5009765625,
				0.5068359375,
				0.513671875,
				0.51953125,
				0.5205078125,
				0.5234375,
				0.525390625,
				0.533203125,
				0.53515625,
				0.537109375,
				0.5390625,
				0.5390625,
				0.541015625,
				0.5458984375,
				0.5478515625,
				0.5498046875,
				0.5546875,
				0.5546875,
				0.5615234375,
				0.5615234375,
				0.5615234375,
				0.5615234375,
				0.5556640625,
				0.5537109375,
				0.5439453125,
				0.509765625,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 310,
			"versionNonce": 1444323219,
			"isDeleted": false,
			"id": "aXRL8wJmNfn05Qds5Wu_W",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 7286.994022359972,
			"y": 437.390706557764,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 5.456629751227665,
			"height": 112.95221919810795,
			"seed": 1729791836,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159329,
			"link": null,
			"locked": true,
			"points": [
				[
					0,
					0
				],
				[
					1.6369639468999493,
					-3.273969524580609
				],
				[
					1.6369639468999493,
					-3.8196241735471683
				],
				[
					2.1826185958668884,
					-3.273969524580609
				],
				[
					2.728314875614267,
					1.6370055776808765
				],
				[
					3.2739695245812057,
					9.276295555556356
				],
				[
					3.8196241735472767,
					16.915585533431837
				],
				[
					3.8196241735472767,
					22.91786993362644
				],
				[
					3.2739695245812057,
					31.648469209435095
				],
				[
					2.728314875614267,
					38.1964082585962
				],
				[
					2.1826185958668884,
					45.290043587505124
				],
				[
					1.6369639468999493,
					50.74667333873322
				],
				[
					1.6369639468999493,
					55.6576484409947
				],
				[
					1.6369639468999493,
					63.29693841887013
				],
				[
					1.0913092979338785,
					69.29922281906474
				],
				[
					1.0913092979338785,
					73.66450164157851
				],
				[
					0.5456546489669393,
					79.12113139280652
				],
				[
					0.5456546489669393,
					82.39514254816827
				],
				[
					0,
					86.21476672171543
				],
				[
					0,
					90.03439089526265
				],
				[
					-0.5456962797473779,
					94.94536599752402
				],
				[
					-1.0913509287143173,
					97.6736808731381
				],
				[
					-1.0913509287143173,
					100.94765039771865
				],
				[
					-1.0913509287143173,
					102.58465597539947
				],
				[
					-1.637005577680388,
					106.40428014894674
				],
				[
					-1.637005577680388,
					107.49563107766106
				],
				[
					-1.637005577680388,
					108.04128572662755
				],
				[
					-1.637005577680388,
					108.58694037559405
				],
				[
					-1.637005577680388,
					109.13259502456079
				],
				[
					-1.637005577680388,
					109.13259502456079
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.189453125,
				0.259765625,
				0.275390625,
				0.33203125,
				0.3994140625,
				0.46484375,
				0.4853515625,
				0.49609375,
				0.5087890625,
				0.51171875,
				0.5185546875,
				0.5234375,
				0.52734375,
				0.537109375,
				0.5390625,
				0.5478515625,
				0.5498046875,
				0.5517578125,
				0.5537109375,
				0.5556640625,
				0.5556640625,
				0.5556640625,
				0.5615234375,
				0.5615234375,
				0.5615234375,
				0.5634765625,
				0.5634765625,
				0.5634765625,
				0.4833984375,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 329,
			"versionNonce": 869472029,
			"isDeleted": false,
			"id": "kDUI3J6KIW4rszWt3aN1u",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 7335.012339192311,
			"y": 323.89283271068956,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 4.910975102261594,
			"height": 217.71949376937368,
			"seed": 620071260,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159329,
			"link": null,
			"locked": true,
			"points": [
				[
					0,
					0
				],
				[
					0.5456546489669393,
					-0.5456546489665592
				],
				[
					0.5456546489669393,
					0.5456546489665592
				],
				[
					0.5456546489669393,
					4.910975102261484
				],
				[
					1.0913509287143173,
					8.730599275808597
				],
				[
					1.6370055776812567,
					14.7328836760032
				],
				[
					2.1826602266473274,
					22.372173653878733
				],
				[
					2.1826602266473274,
					30.011463631754214
				],
				[
					2.1826602266473274,
					32.73977850736821
				],
				[
					2.728314875614267,
					39.287717556529365
				],
				[
					2.728314875614267,
					45.83569823647173
				],
				[
					3.2739695245812057,
					51.837982636666325
				],
				[
					3.2739695245812057,
					59.4772726145418
				],
				[
					3.2739695245812057,
					67.11652096163614
				],
				[
					3.8196658043285843,
					78.02978046409218
				],
				[
					3.8196658043285843,
					85.66907044196772
				],
				[
					3.8196658043285843,
					92.76270577087658
				],
				[
					4.3653204532955225,
					102.58461434461836
				],
				[
					4.3653204532955225,
					110.22390432249384
				],
				[
					4.3653204532955225,
					120.0458545270168
				],
				[
					4.910975102261594,
					126.59379357617797
				],
				[
					4.910975102261594,
					133.68742890508682
				],
				[
					4.910975102261594,
					139.68971330528143
				],
				[
					4.910975102261594,
					145.14634305650952
				],
				[
					4.3653204532955225,
					151.14862745670413
				],
				[
					4.3653204532955225,
					159.87922673251276
				],
				[
					4.3653204532955225,
					164.79020183477417
				],
				[
					4.3653204532955225,
					168.60986763910253
				],
				[
					3.8196658043285843,
					175.15780668826372
				],
				[
					3.8196658043285843,
					179.5231271415586
				],
				[
					3.8196658043285843,
					183.3427513151058
				],
				[
					3.8196658043285843,
					188.79938106633378
				],
				[
					3.2739695245812057,
					191.52769594194783
				],
				[
					3.2739695245812057,
					193.7103561685952
				],
				[
					3.2739695245812057,
					196.98432569317578
				],
				[
					3.2739695245812057,
					200.25829521775646
				],
				[
					3.2739695245812057,
					204.6236156710514
				],
				[
					3.2739695245812057,
					206.8062758976987
				],
				[
					3.2739695245812057,
					207.89758519563196
				],
				[
					3.8196658043285843,
					209.53459077331277
				],
				[
					3.8196658043285843,
					210.625900071246
				],
				[
					3.8196658043285843,
					211.717209369179
				],
				[
					3.8196658043285843,
					212.26290564892685
				],
				[
					4.3653204532955225,
					212.8085602978933
				],
				[
					4.3653204532955225,
					214.44552424479303
				],
				[
					4.910975102261594,
					215.53687517350738
				],
				[
					4.910975102261594,
					216.6281844714406
				],
				[
					4.910975102261594,
					217.1738391204071
				],
				[
					4.910975102261594,
					217.1738391204071
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.173828125,
				0.21875,
				0.3681640625,
				0.4052734375,
				0.4287109375,
				0.44921875,
				0.470703125,
				0.48828125,
				0.4912109375,
				0.4951171875,
				0.5009765625,
				0.5087890625,
				0.5146484375,
				0.51953125,
				0.513671875,
				0.5185546875,
				0.521484375,
				0.521484375,
				0.521484375,
				0.5234375,
				0.525390625,
				0.525390625,
				0.525390625,
				0.525390625,
				0.525390625,
				0.525390625,
				0.52734375,
				0.529296875,
				0.53515625,
				0.53515625,
				0.53515625,
				0.537109375,
				0.5390625,
				0.541015625,
				0.541015625,
				0.541015625,
				0.541015625,
				0.541015625,
				0.541015625,
				0.541015625,
				0.5390625,
				0.5244140625,
				0.5078125,
				0.5029296875,
				0.4150390625,
				0.365234375,
				0.28125,
				0.1904296875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 311,
			"versionNonce": 2011378995,
			"isDeleted": false,
			"id": "SVtIHXZSlj8YpPIJjwMzR",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 7385.759012531044,
			"y": 443.9386872377063,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 2.18261859586602,
			"height": 91.12570019319571,
			"seed": 1321609692,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159329,
			"link": null,
			"locked": true,
			"points": [
				[
					0,
					0
				],
				[
					0,
					1.636963946899678
				],
				[
					0.5456546489660707,
					5.456629751228045
				],
				[
					1.09130929793301,
					9.821908573741773
				],
				[
					1.09130929793301,
					12.004568800389206
				],
				[
					1.09130929793301,
					16.36988925368408
				],
				[
					1.09130929793301,
					20.73516807619786
				],
				[
					1.09130929793301,
					26.737494107173557
				],
				[
					1.09130929793301,
					31.102772929687333
				],
				[
					1.09130929793301,
					36.559402680915326
				],
				[
					1.09130929793301,
					43.107383360857746
				],
				[
					1.09130929793301,
					46.92700753440491
				],
				[
					1.6369639468990806,
					51.83798263666628
				],
				[
					1.6369639468990806,
					56.20326145918007
				],
				[
					1.09130929793301,
					60.56858191247494
				],
				[
					1.09130929793301,
					66.02521166370305
				],
				[
					1.09130929793301,
					68.75352653931698
				],
				[
					1.09130929793301,
					71.48184141493103
				],
				[
					1.09130929793301,
					73.66450164157845
				],
				[
					0.5456546489660707,
					76.39281651719251
				],
				[
					0.5456546489660707,
					79.66678604177307
				],
				[
					0.5456546489660707,
					82.39510091738707
				],
				[
					0,
					82.94075556635357
				],
				[
					0.5456546489660707,
					84.57776114403461
				],
				[
					0,
					86.21472509093434
				],
				[
					0,
					88.39738531758167
				],
				[
					0,
					89.488736246296
				],
				[
					-0.5456546489669392,
					90.03439089526249
				],
				[
					-0.5456546489669392,
					90.58004554422922
				],
				[
					-0.5456546489669392,
					91.12570019319571
				],
				[
					-0.5456546489669392,
					91.12570019319571
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.216796875,
				0.3828125,
				0.408203125,
				0.4345703125,
				0.4443359375,
				0.4560546875,
				0.4677734375,
				0.48046875,
				0.48828125,
				0.4970703125,
				0.509765625,
				0.5126953125,
				0.51953125,
				0.513671875,
				0.513671875,
				0.521484375,
				0.525390625,
				0.5341796875,
				0.537109375,
				0.5390625,
				0.541015625,
				0.541015625,
				0.541015625,
				0.541015625,
				0.541015625,
				0.541015625,
				0.541015625,
				0.541015625,
				0.541015625,
				0.5107421875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 300,
			"versionNonce": 1392257917,
			"isDeleted": false,
			"id": "HZQ5J_px-ee0KOkn09uSm",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 7383.030697655429,
			"y": 447.2126567622869,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 3.273969524580337,
			"height": 84.57776114403461,
			"seed": 642314716,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159330,
			"link": null,
			"locked": true,
			"points": [
				[
					0,
					0
				],
				[
					0,
					2.72831487561405
				],
				[
					1.6369639468999493,
					12.004568800389206
				],
				[
					2.1826602266473274,
					19.64385877826474
				],
				[
					2.728314875614267,
					25.646143178459347
				],
				[
					3.273969524580337,
					33.285433156334776
				],
				[
					3.273969524580337,
					42.56172871189113
				],
				[
					2.1826602266473274,
					51.292327987699785
				],
				[
					2.1826602266473274,
					57.84026703686099
				],
				[
					2.1826602266473274,
					62.20558749015587
				],
				[
					2.1826602266473274,
					66.02521166370305
				],
				[
					2.728314875614267,
					70.93618676596454
				],
				[
					2.728314875614267,
					74.21015629054509
				],
				[
					2.728314875614267,
					76.39281651719251
				],
				[
					2.728314875614267,
					79.12113139280652
				],
				[
					2.728314875614267,
					80.21244069073974
				],
				[
					2.728314875614267,
					81.30379161945405
				],
				[
					3.273969524580337,
					82.39510091738707
				],
				[
					3.273969524580337,
					84.57776114403461
				],
				[
					3.273969524580337,
					84.57776114403461
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.123046875,
				0.328125,
				0.40234375,
				0.431640625,
				0.44921875,
				0.462890625,
				0.482421875,
				0.4990234375,
				0.513671875,
				0.5146484375,
				0.5185546875,
				0.5234375,
				0.525390625,
				0.525390625,
				0.525390625,
				0.525390625,
				0.486328125,
				0.34765625,
				0.0146484375,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 284,
			"versionNonce": 181147347,
			"isDeleted": false,
			"id": "kh7_xJ9LXzMyUgGgoVKI0",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 7426.138081016288,
			"y": 346.26500636456825,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 0.5456546489660709,
			"height": 0.5456546489666135,
			"seed": 1059347684,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159330,
			"link": null,
			"locked": true,
			"points": [
				[
					0,
					0
				],
				[
					0.5456546489660709,
					-0.5456546489666135
				],
				[
					0,
					0
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.1015625,
				0.0185546875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 318,
			"versionNonce": 1757656029,
			"isDeleted": false,
			"id": "RcZmvPikcr5pMrtBRTG22",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 7427.775044963188,
			"y": 344.08234613792075,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 1.09130929793301,
			"height": 199.16698591982342,
			"seed": 1138175068,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159330,
			"link": null,
			"locked": true,
			"points": [
				[
					0,
					0
				],
				[
					-0.5456546489669392,
					0.5456546489665592
				],
				[
					0,
					1.6370055776808765
				],
				[
					0,
					3.819665804328367
				],
				[
					0,
					7.0936353289089205
				],
				[
					0,
					13.641574378070084
				],
				[
					0,
					22.9178699336265
				],
				[
					0,
					28.37449968485454
				],
				[
					0,
					37.10509896066314
				],
				[
					-0.5456546489669392,
					44.198692658790854
				],
				[
					-0.5456546489669392,
					53.47498821434727
				],
				[
					0,
					58.93161796557526
				],
				[
					0,
					65.47955701473649
				],
				[
					0.5456546489660707,
					74.75585257029283
				],
				[
					0.5456546489660707,
					83.48645184610143
				],
				[
					0.5456546489660707,
					90.58004554422916
				],
				[
					0.5456546489660707,
					97.1280262241715
				],
				[
					0.5456546489660707,
					103.13031062436612
				],
				[
					0.5456546489660707,
					113.4979154778556
				],
				[
					0.5456546489660707,
					120.04585452701681
				],
				[
					0.5456546489660707,
					127.68514450489235
				],
				[
					0.5456546489660707,
					133.68742890508696
				],
				[
					0,
					148.96600886083792
				],
				[
					0,
					160.97057766122714
				],
				[
					0,
					162.60758323890798
				],
				[
					0,
					169.15552228806916
				],
				[
					0,
					173.52084274136402
				],
				[
					0,
					177.88612156387782
				],
				[
					-0.5456546489669392,
					182.79709666613917
				],
				[
					-0.5456546489669392,
					188.79938106633375
				],
				[
					-0.5456546489669392,
					191.5276959419478
				],
				[
					-0.5456546489669392,
					192.61904687066212
				],
				[
					-0.5456546489669392,
					194.25601081756184
				],
				[
					-0.5456546489669392,
					194.80170709730965
				],
				[
					-0.5456546489669392,
					198.07567662189018
				],
				[
					-0.5456546489669392,
					199.16698591982342
				],
				[
					-0.5456546489669392,
					196.98432569317592
				],
				[
					-0.5456546489669392,
					196.98432569317592
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2041015625,
				0.22265625,
				0.31640625,
				0.333984375,
				0.3564453125,
				0.38671875,
				0.396484375,
				0.396484375,
				0.4033203125,
				0.4228515625,
				0.4443359375,
				0.451171875,
				0.4609375,
				0.46875,
				0.4775390625,
				0.482421875,
				0.490234375,
				0.4931640625,
				0.4970703125,
				0.5009765625,
				0.5087890625,
				0.5107421875,
				0.517578125,
				0.525390625,
				0.525390625,
				0.525390625,
				0.525390625,
				0.525390625,
				0.525390625,
				0.525390625,
				0.525390625,
				0.525390625,
				0.5029296875,
				0.4951171875,
				0.4150390625,
				0.3330078125,
				0.0126953125,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 292,
			"versionNonce": 1030210675,
			"isDeleted": false,
			"id": "LTH65pp7sdcRyFINgzkRZ",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 7081.824731224564,
			"y": 325.5298382883704,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 21.280843540555235,
			"height": 2.728314875613995,
			"seed": 1659378148,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159330,
			"link": null,
			"locked": true,
			"points": [
				[
					0,
					0
				],
				[
					5.456629751227665,
					-1.6370055776808765
				],
				[
					7.093614513517833,
					-1.091350928714317
				],
				[
					10.367584038099038,
					-0.5456546489665594
				],
				[
					12.550244264746366,
					0
				],
				[
					17.46119855161687,
					0
				],
				[
					20.189513427231137,
					0
				],
				[
					21.280843540555235,
					-0.5456546489665594
				],
				[
					19.09820412929813,
					0
				],
				[
					14.187229027036535,
					1.0913092979331187
				],
				[
					14.187229027036535,
					1.0913092979331187
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.142578125,
				0.234375,
				0.2734375,
				0.3173828125,
				0.33984375,
				0.3564453125,
				0.3564453125,
				0.353515625,
				0.1875,
				0.0126953125,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 289,
			"versionNonce": 20656189,
			"isDeleted": false,
			"id": "447YGBr1oqM-DYH0nz6Rt",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 7081.2790557602075,
			"y": 326.6211475863035,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 24.55483388052579,
			"height": 3.2739695245805542,
			"seed": 1642880740,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159330,
			"link": null,
			"locked": true,
			"points": [
				[
					0,
					0
				],
				[
					5.4566297512276645,
					-1.0913092979331185
				],
				[
					7.093614513517832,
					-1.0913092979331185
				],
				[
					12.004589615779425,
					-1.636963946899678
				],
				[
					16.36988925368386,
					-2.728314875613995
				],
				[
					20.735188891588294,
					-2.728314875613995
				],
				[
					22.917849118235623,
					-3.2739695245805542
				],
				[
					24.55483388052579,
					-2.1826602266474358
				],
				[
					24.55483388052579,
					-2.1826602266474358
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.130859375,
				0.23828125,
				0.25390625,
				0.2841796875,
				0.302734375,
				0.30859375,
				0.2783203125,
				0.0126953125,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 288,
			"versionNonce": 662486547,
			"isDeleted": false,
			"id": "MAiRkdh2CAQL5-xr12Twv",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 7322.462115742955,
			"y": 324.4384873596561,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 19.6438587782642,
			"height": 2.1826185958662916,
			"seed": 1851822180,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159330,
			"link": null,
			"locked": true,
			"points": [
				[
					0,
					0
				],
				[
					3.8196241735472767,
					-0.5456546489665592
				],
				[
					8.730599275808002,
					-1.0913092979331185
				],
				[
					16.369889253683862,
					-1.6369639468997321
				],
				[
					19.09820412929813,
					-2.1826185958662916
				],
				[
					19.6438587782642,
					-2.1826185958662916
				],
				[
					17.46119855161687,
					-2.1826185958662916
				],
				[
					17.46119855161687,
					-2.1826185958662916
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.185546875,
				0.2470703125,
				0.2666015625,
				0.2626953125,
				0.259765625,
				0.259765625,
				0.0126953125,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 290,
			"versionNonce": 709107869,
			"isDeleted": false,
			"id": "bKuTonufW3GuYNcM_aCrk",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 7321.916419463207,
			"y": 323.89283271068956,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 18.006894831365116,
			"height": 1.6369639468997321,
			"seed": 493963740,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311159330,
			"link": null,
			"locked": true,
			"points": [
				[
					0,
					0
				],
				[
					0.5456962797482464,
					-0.5456546489665592
				],
				[
					1.6370055776812567,
					-0.5456546489665592
				],
				[
					3.8196658043285843,
					-1.0913092979331729
				],
				[
					6.5479806799428495,
					-1.0913092979331729
				],
				[
					13.095919729103525,
					-1.6369639468997321
				],
				[
					16.36988925368473,
					-1.6369639468997321
				],
				[
					18.006894831365116,
					-1.6369639468997321
				],
				[
					14.732925306784782,
					0
				],
				[
					14.732925306784782,
					0
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.189453125,
				0.2412109375,
				0.26953125,
				0.30078125,
				0.318359375,
				0.328125,
				0.33203125,
				0.33203125,
				0.0126953125,
				0
			]
		},
		{
			"type": "text",
			"version": 52,
			"versionNonce": 180194771,
			"isDeleted": false,
			"id": "JFj5GE8o",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 6950.302368497711,
			"y": 650.3254003419872,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 149,
			"height": 25,
			"seed": 756031332,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311196571,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "WALKTHROUGH",
			"rawText": "WALKTHROUGH",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "WALKTHROUGH",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 142,
			"versionNonce": 1038794771,
			"isDeleted": false,
			"id": "DNPxkTHc",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 6970.302499287334,
			"y": 1013.5636350890109,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 151,
			"height": 25,
			"seed": 2075437412,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1686311217044,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "BRUTEFORECE",
			"rawText": "BRUTEFORECE",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "BRUTEFORECE",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"id": "M0prJgM1",
			"type": "text",
			"x": 6980.478072355648,
			"y": 755.8754083682217,
			"width": 502,
			"height": 200,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"roundness": null,
			"seed": 11511709,
			"version": 298,
			"versionNonce": 1309825907,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686311196571,
			"link": null,
			"locked": false,
			"text": "// iterate heights (start at the ends)\n- maxArea = 0\n- while startIndex < endIndex \n    - currArea = endIndex - startIndex \n      * min(heights[startIndex], heights[endIndex])\n    - if currArea > currMaxArea\n        - maxAea = currArea\n- return MaxArea",
			"rawText": "// iterate heights (start at the ends)\n- maxArea = 0\n- while startIndex < endIndex \n    - currArea = endIndex - startIndex \n      * min(heights[startIndex], heights[endIndex])\n    - if currArea > currMaxArea\n        - maxAea = currArea\n- return MaxArea",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "left",
			"verticalAlign": "top",
			"baseline": 192,
			"containerId": null,
			"originalText": "// iterate heights (start at the ends)\n- maxArea = 0\n- while startIndex < endIndex \n    - currArea = endIndex - startIndex \n      * min(heights[startIndex], heights[endIndex])\n    - if currArea > currMaxArea\n        - maxAea = currArea\n- return MaxArea",
			"lineHeight": 1.25
		},
		{
			"id": "FvKJ5cc8",
			"type": "text",
			"x": 7057.588871509304,
			"y": 1085.4311402475614,
			"width": 235,
			"height": 75,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"roundness": null,
			"seed": 1009336083,
			"version": 187,
			"versionNonce": 2066693789,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686311217044,
			"link": null,
			"locked": false,
			"text": "maxArea = 0\nstartIndex = 0\nendIndex = height.len - 1",
			"rawText": "maxArea = 0\nstartIndex = 0\nendIndex = height.len - 1",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "left",
			"verticalAlign": "top",
			"baseline": 67,
			"containerId": null,
			"originalText": "maxArea = 0\nstartIndex = 0\nendIndex = height.len - 1",
			"lineHeight": 1.25
		},
		{
			"id": "SNcSW2i5ZSYGKZwrOqK0q",
			"type": "rectangle",
			"x": 7049.53330239038,
			"y": 1177.6533421247314,
			"width": 306,
			"height": 35,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"roundness": {
				"type": 3
			},
			"seed": 1313911677,
			"version": 403,
			"versionNonce": 23020979,
			"isDeleted": false,
			"boundElements": [
				{
					"type": "text",
					"id": "ri3wmAZC"
				}
			],
			"updated": 1686311217044,
			"link": null,
			"locked": false
		},
		{
			"id": "ri3wmAZC",
			"type": "text",
			"x": 7059.53330239038,
			"y": 1182.6533421247314,
			"width": 286,
			"height": 25,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"roundness": null,
			"seed": 997919581,
			"version": 374,
			"versionNonce": 996631293,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686311217044,
			"link": null,
			"locked": false,
			"text": "while startIndex < endIndex ",
			"rawText": "while startIndex < endIndex ",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "center",
			"verticalAlign": "middle",
			"baseline": 17,
			"containerId": "SNcSW2i5ZSYGKZwrOqK0q",
			"originalText": "while startIndex < endIndex ",
			"lineHeight": 1.25
		},
		{
			"id": "DsyZAFioMJYqauwhsYhSf",
			"type": "line",
			"x": 7075.144498272536,
			"y": 1214.32002913645,
			"width": 0,
			"height": 221.99996948242267,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"seed": 23788339,
			"version": 206,
			"versionNonce": 460461907,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686311217044,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					221.99996948242267
				]
			],
			"lastCommittedPoint": null,
			"startBinding": null,
			"endBinding": null,
			"startArrowhead": null,
			"endArrowhead": null
		},
		{
			"id": "1m6wc7V3HziW_P5l-2bk2",
			"type": "line",
			"x": 7356.477811260817,
			"y": 1190.891459161097,
			"width": 253.14307803199245,
			"height": 0,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"seed": 397046685,
			"version": 255,
			"versionNonce": 500955997,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686311217044,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					253.14307803199245,
					0
				]
			],
			"lastCommittedPoint": null,
			"startBinding": null,
			"endBinding": null,
			"startArrowhead": null,
			"endArrowhead": null
		},
		{
			"id": "knDqSQjd",
			"type": "text",
			"x": 7140.477851950923,
			"y": 1248.3200189639247,
			"width": 430,
			"height": 50,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"roundness": null,
			"seed": 691864787,
			"version": 221,
			"versionNonce": 981054707,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686311217044,
			"link": null,
			"locked": false,
			"text": "curArea = (endIndex - startIndex) \n* min (height[startIndex], height[endIndex])",
			"rawText": "curArea = (endIndex - startIndex) \n* min (height[startIndex], height[endIndex])",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "left",
			"verticalAlign": "top",
			"baseline": 42,
			"containerId": null,
			"originalText": "curArea = (endIndex - startIndex) \n* min (height[startIndex], height[endIndex])",
			"lineHeight": 1.25
		},
		{
			"id": "BmBBitO2LhhlJJMoPcNyt",
			"type": "rectangle",
			"x": 7148.811236146887,
			"y": 1324.8200240501876,
			"width": 260,
			"height": 35,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"roundness": {
				"type": 3
			},
			"seed": 1577029053,
			"version": 199,
			"versionNonce": 182355901,
			"isDeleted": false,
			"boundElements": [
				{
					"type": "text",
					"id": "lnfT11Nh"
				}
			],
			"updated": 1686311217044,
			"link": null,
			"locked": false
		},
		{
			"id": "lnfT11Nh",
			"type": "text",
			"x": 7172.311236146887,
			"y": 1329.8200240501876,
			"width": 213,
			"height": 25,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"roundness": null,
			"seed": 28472349,
			"version": 216,
			"versionNonce": 2113707667,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686311217044,
			"link": null,
			"locked": false,
			"text": "if curArea > maxArea",
			"rawText": "if curArea > maxArea",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "center",
			"verticalAlign": "middle",
			"baseline": 17,
			"containerId": "BmBBitO2LhhlJJMoPcNyt",
			"originalText": "if curArea > maxArea",
			"lineHeight": 1.25
		},
		{
			"id": "ICvtQYaCdaGax5EUXcANu",
			"type": "arrow",
			"x": 7177.775868377967,
			"y": 1359.7723948300425,
			"width": 90.81473782986723,
			"height": 36.52220574021226,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"seed": 1449810269,
			"version": 603,
			"versionNonce": 21504691,
			"isDeleted": false,
			"boundElements": [
				{
					"type": "text",
					"id": "Qpaygbid"
				}
			],
			"updated": 1686311217322,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					90.81473782986723,
					36.52220574021226
				]
			],
			"lastCommittedPoint": null,
			"startBinding": null,
			"endBinding": {
				"elementId": "eTlcueKy",
				"focus": -0.8351715477706242,
				"gap": 10.648973212398232
			},
			"startArrowhead": null,
			"endArrowhead": "arrow"
		},
		{
			"id": "Qpaygbid",
			"type": "text",
			"x": 7335.18319369636,
			"y": 1364.100604621229,
			"width": 16,
			"height": 25,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"roundness": null,
			"seed": 165862803,
			"version": 152,
			"versionNonce": 1353798707,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686311217044,
			"link": null,
			"locked": false,
			"text": "T",
			"rawText": "T",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "center",
			"verticalAlign": "middle",
			"baseline": 17,
			"containerId": "ICvtQYaCdaGax5EUXcANu",
			"originalText": "T",
			"lineHeight": 1.25
		},
		{
			"id": "eTlcueKy",
			"type": "text",
			"x": 7279.239579420232,
			"y": 1384.0343264764806,
			"width": 193,
			"height": 25,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"roundness": null,
			"seed": 80307965,
			"version": 376,
			"versionNonce": 1289976957,
			"isDeleted": false,
			"boundElements": [
				{
					"id": "ICvtQYaCdaGax5EUXcANu",
					"type": "arrow"
				}
			],
			"updated": 1686311217044,
			"link": null,
			"locked": false,
			"text": "maxArea = cueArea",
			"rawText": "maxArea = cueArea",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "left",
			"verticalAlign": "top",
			"baseline": 17,
			"containerId": null,
			"originalText": "maxArea = cueArea",
			"lineHeight": 1.25
		},
		{
			"id": "8Sz-pHCDh7qYxIwlJFu4q",
			"type": "line",
			"x": 7077.144671205479,
			"y": 1434.3199782738209,
			"width": 530.7619149344282,
			"height": 0,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"seed": 1098097149,
			"version": 284,
			"versionNonce": 731440349,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686311217044,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					530.7619149344282,
					0
				]
			],
			"lastCommittedPoint": null,
			"startBinding": null,
			"endBinding": null,
			"startArrowhead": null,
			"endArrowhead": null
		},
		{
			"id": "1Khb0gkam4sW4OO4PCXSK",
			"type": "line",
			"x": 7612.192329489984,
			"y": 1436.129510802653,
			"width": 0,
			"height": 248.66666158040368,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"seed": 907181459,
			"version": 241,
			"versionNonce": 578429811,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686311217044,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					-248.66666158040368
				]
			],
			"lastCommittedPoint": null,
			"startBinding": null,
			"endBinding": null,
			"startArrowhead": null,
			"endArrowhead": null
		},
		{
			"id": "ReYgHt40JfzsQymkbVMRg",
			"type": "rectangle",
			"x": 7090.64456948022,
			"y": 1477.986680544329,
			"width": 182,
			"height": 35,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [
				"egYVYmNrpBaM5TJqKh5By"
			],
			"roundness": {
				"type": 3
			},
			"seed": 1082216797,
			"version": 260,
			"versionNonce": 1950499133,
			"isDeleted": false,
			"boundElements": [
				{
					"type": "text",
					"id": "IGDlEbPR"
				}
			],
			"updated": 1686311217044,
			"link": null,
			"locked": false
		},
		{
			"id": "IGDlEbPR",
			"type": "text",
			"x": 7105.14456948022,
			"y": 1482.986680544329,
			"width": 153,
			"height": 25,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [
				"egYVYmNrpBaM5TJqKh5By"
			],
			"roundness": null,
			"seed": 1709325107,
			"version": 270,
			"versionNonce": 418069779,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686311217044,
			"link": null,
			"locked": false,
			"text": "return maxArea",
			"rawText": "return maxArea",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "center",
			"verticalAlign": "middle",
			"baseline": 17,
			"containerId": "ReYgHt40JfzsQymkbVMRg",
			"originalText": "return maxArea",
			"lineHeight": 1.25
		},
		{
			"id": "EX_0b3-orrBJf_XqSHloh",
			"type": "rectangle",
			"x": 7084.477943503657,
			"y": 1469.6533319522064,
			"width": 195.33340454101562,
			"height": 53.33333333333326,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [
				"egYVYmNrpBaM5TJqKh5By"
			],
			"roundness": {
				"type": 3
			},
			"seed": 140661043,
			"version": 208,
			"versionNonce": 742461853,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686311217044,
			"link": null,
			"locked": false
		},
		{
			"type": "line",
			"version": 387,
			"versionNonce": 1026788339,
			"isDeleted": false,
			"id": "rRa7yQsNrz1bDOyxh2m5z",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 7902.184066824527,
			"y": -424.8684630805924,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 0,
			"height": 2065.5999145507812,
			"seed": 1905218035,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1686311224019,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					0,
					2065.5999145507812
				]
			]
		}
	],
	"appState": {
		"theme": "dark",
		"viewBackgroundColor": "#ffffff",
		"currentItemStrokeColor": "#1e1e1e",
		"currentItemBackgroundColor": "transparent",
		"currentItemFillStyle": "hachure",
		"currentItemStrokeWidth": 0.5,
		"currentItemStrokeStyle": "solid",
		"currentItemRoughness": 1,
		"currentItemOpacity": 100,
		"currentItemFontFamily": 1,
		"currentItemFontSize": 20,
		"currentItemTextAlign": "left",
		"currentItemStartArrowhead": null,
		"currentItemEndArrowhead": "arrow",
		"scrollX": -6308.549470167298,
		"scrollY": 581.2954440507079,
		"zoom": {
			"value": 0.3
		},
		"currentItemRoundness": "round",
		"gridSize": null,
		"currentStrokeOptions": null,
		"previousGridSize": null
	},
	"files": {}
}
```
%%