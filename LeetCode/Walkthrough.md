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

- currMaxArea = 0
- iterate height i = 0
    - iterate height j = i + 1
        -  currArear = 
           Min of  (len[i], len[j]) x (j - i) 
        - if currArea > currMaxArea
            - currMaxAea = currArea
- return currMaxArea  ^EEkgMBz4

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
			"version": 345,
			"versionNonce": 1656788444,
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
			"updated": 1686230174152,
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
			"version": 341,
			"versionNonce": 396445156,
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
			"updated": 1686230174152,
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
			"version": 333,
			"versionNonce": 577337948,
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
			"updated": 1686230174152,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 309,
			"versionNonce": 784787812,
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
			"updated": 1686230174152,
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
			"version": 385,
			"versionNonce": 880922332,
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
			"updated": 1686230174152,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 353,
			"versionNonce": 678173924,
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
			"updated": 1686230174152,
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
			"version": 427,
			"versionNonce": 2040238940,
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
			"updated": 1686230174152,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 400,
			"versionNonce": 773775460,
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
			"updated": 1686230174153,
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
			"version": 437,
			"versionNonce": 1879623644,
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
			"updated": 1686230174153,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 538,
			"versionNonce": 128791524,
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
			"updated": 1686230174153,
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
			"version": 342,
			"versionNonce": 2077977692,
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
			"updated": 1686230174153,
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
			"version": 404,
			"versionNonce": 1394939748,
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
			"updated": 1686230174153,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 369,
			"versionNonce": 786792668,
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
			"updated": 1686230174153,
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
			"version": 1002,
			"versionNonce": 1020562148,
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
			"updated": 1686230174153,
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
			"version": 1035,
			"versionNonce": 280560988,
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
			"updated": 1686230174153,
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
			"version": 99,
			"versionNonce": 927567460,
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
			"updated": 1686230174153,
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
			"version": 204,
			"versionNonce": 1722284508,
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
			"updated": 1686230174153,
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
			"version": 148,
			"versionNonce": 861020644,
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
			"updated": 1686230174153,
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
			"version": 203,
			"versionNonce": 2076466780,
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
			"updated": 1686230174153,
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
			"version": 1068,
			"versionNonce": 1476150628,
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
			"updated": 1686230174153,
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
			"version": 829,
			"versionNonce": 1759523548,
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
			"updated": 1686230174153,
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
			"version": 1096,
			"versionNonce": 982907108,
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
			"updated": 1686230174153,
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
			"version": 994,
			"versionNonce": 1552775004,
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
			"updated": 1686230174154,
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
			"version": 908,
			"versionNonce": 380451940,
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
			"updated": 1686230174154,
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
			"version": 660,
			"versionNonce": 1662921692,
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
			"updated": 1686230174154,
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
			"version": 852,
			"versionNonce": 101715940,
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
			"updated": 1686230174154,
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
			"version": 761,
			"versionNonce": 782520412,
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
			"updated": 1686230174154,
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
			"version": 1414,
			"versionNonce": 952922980,
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
			"updated": 1686230174154,
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
			"version": 533,
			"versionNonce": 1592911068,
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
			"updated": 1686230174154,
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
			"version": 1586,
			"versionNonce": 758146788,
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
			"updated": 1686230174154,
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
			"version": 436,
			"versionNonce": 1234757980,
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
			"updated": 1686230174154,
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
			"version": 371,
			"versionNonce": 1741285988,
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
			"updated": 1686230174154,
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
			"version": 410,
			"versionNonce": 1105944028,
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
			"updated": 1686230174154,
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
			"version": 429,
			"versionNonce": 728169956,
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
			"updated": 1686230174154,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 415,
			"versionNonce": 1627079260,
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
			"updated": 1686230174154,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 375,
			"versionNonce": 823501156,
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
			"updated": 1686230174154,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 391,
			"versionNonce": 1301976796,
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
			"updated": 1686230174154,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 441,
			"versionNonce": 1612960996,
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
			"updated": 1686230174154,
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
			"version": 516,
			"versionNonce": 73096028,
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
			"updated": 1686230174154,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 403,
			"versionNonce": 102733924,
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
			"updated": 1686230174154,
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
			"version": 442,
			"versionNonce": 529502172,
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
			"updated": 1686230174154,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 464,
			"versionNonce": 248966116,
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
			"updated": 1686230174155,
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
			"version": 379,
			"versionNonce": 524891228,
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
			"updated": 1686230174155,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 232,
			"versionNonce": 1012387684,
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
			"updated": 1686230174155,
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
			"version": 241,
			"versionNonce": 828000476,
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
			"updated": 1686230174155,
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
			"version": 144,
			"versionNonce": 1592804068,
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
			"updated": 1686230174155,
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
			"version": 110,
			"versionNonce": 2035600732,
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
			"updated": 1686230174155,
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
			"version": 106,
			"versionNonce": 221136484,
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
			"updated": 1686230174155,
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
			"version": 143,
			"versionNonce": 1485488604,
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
			"updated": 1686230174155,
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
			"version": 226,
			"versionNonce": 1541396964,
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
			"updated": 1686230174155,
			"link": null,
			"locked": false
		},
		{
			"type": "line",
			"version": 238,
			"versionNonce": 906896988,
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
			"updated": 1686230174155,
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
			"version": 254,
			"versionNonce": 370343268,
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
			"updated": 1686230174155,
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
			"version": 202,
			"versionNonce": 1186003676,
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
			"updated": 1686230174155,
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
			"version": 258,
			"versionNonce": 1964355812,
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
			"updated": 1686230174155,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 431,
			"versionNonce": 1426407260,
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
			"updated": 1686230174155,
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
			"version": 236,
			"versionNonce": 1484125284,
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
			"updated": 1686230174155,
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
			"version": 87,
			"versionNonce": 157086684,
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
			"updated": 1686230174155,
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
			"version": 151,
			"versionNonce": 2114045924,
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
			"updated": 1686230174155,
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
			"version": 143,
			"versionNonce": 835328092,
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
			"updated": 1686230174155,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 174,
			"versionNonce": 969354084,
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
			"updated": 1686230174155,
			"link": null,
			"locked": false
		},
		{
			"type": "arrow",
			"version": 614,
			"versionNonce": 169782492,
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
			"updated": 1686230174156,
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
			"version": 85,
			"versionNonce": 773070564,
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
			"updated": 1686230174156,
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
			"version": 320,
			"versionNonce": 65843548,
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
			"updated": 1686230174156,
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
			"version": 272,
			"versionNonce": 58106468,
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
			"updated": 1686230174156,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 167,
			"versionNonce": 243672540,
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
			"updated": 1686230174156,
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
			"version": 264,
			"versionNonce": 549238244,
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
			"updated": 1686230174156,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 286,
			"versionNonce": 1593641564,
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
			"updated": 1686230174156,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 314,
			"versionNonce": 1660180836,
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
			"updated": 1686230174156,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 384,
			"versionNonce": 941842140,
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
			"updated": 1686230174156,
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
			"version": 376,
			"versionNonce": 1433111780,
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
			"updated": 1686230174156,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 352,
			"versionNonce": 847979356,
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
			"updated": 1686230174156,
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
			"version": 431,
			"versionNonce": 1773162596,
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
			"updated": 1686230174156,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 396,
			"versionNonce": 75913180,
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
			"updated": 1686230174156,
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
			"version": 470,
			"versionNonce": 798008292,
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
			"updated": 1686230174156,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 443,
			"versionNonce": 1244068956,
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
			"updated": 1686230174156,
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
			"version": 480,
			"versionNonce": 219842404,
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
			"updated": 1686230174156,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 581,
			"versionNonce": 1295978716,
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
			"updated": 1686230174156,
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
			"version": 385,
			"versionNonce": 1989933796,
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
			"updated": 1686230174156,
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
			"version": 450,
			"versionNonce": 1298175324,
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
			"updated": 1686230174156,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 412,
			"versionNonce": 648216164,
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
			"updated": 1686230174157,
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
			"version": 283,
			"versionNonce": 1205701084,
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
			"updated": 1686230174157,
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
			"version": 291,
			"versionNonce": 1442681316,
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
			"updated": 1686230174157,
			"link": null,
			"locked": false
		},
		{
			"type": "arrow",
			"version": 911,
			"versionNonce": 1070067292,
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
			"updated": 1686230174157,
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
			"version": 146,
			"versionNonce": 1941550436,
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
			"updated": 1686230174157,
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
			"version": 460,
			"versionNonce": 99730140,
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
			"updated": 1686230174157,
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
			"version": 467,
			"versionNonce": 1562732772,
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
			"updated": 1686230174157,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 509,
			"versionNonce": 15533916,
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
			"updated": 1686230174157,
			"link": null,
			"locked": false
		},
		{
			"type": "arrow",
			"version": 462,
			"versionNonce": 365866084,
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
			"updated": 1686230174157,
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
			"version": 157,
			"versionNonce": 1963703260,
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
			"updated": 1686230174157,
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
			"version": 845,
			"versionNonce": 2139324388,
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
			"updated": 1686230174157,
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
			"version": 314,
			"versionNonce": 1281351772,
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
			"updated": 1686230174157,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 238,
			"versionNonce": 307356516,
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
			"updated": 1686230174157,
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
			"version": 196,
			"versionNonce": 1589343452,
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
			"updated": 1686230174157,
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
			"version": 150,
			"versionNonce": 344446692,
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
			"updated": 1686230174157,
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
			"version": 218,
			"versionNonce": 967866716,
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
			"updated": 1686230174157,
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
			"version": 243,
			"versionNonce": 1387485796,
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
			"updated": 1686230174157,
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
			"version": 141,
			"versionNonce": 1754328540,
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
			"updated": 1686230174157,
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
			"version": 195,
			"versionNonce": 1470262756,
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
			"updated": 1686230174157,
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
			"version": 257,
			"versionNonce": 1013895772,
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
			"updated": 1686230174158,
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
			"version": 239,
			"versionNonce": 610472292,
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
			"updated": 1686230174158,
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
			"version": 120,
			"versionNonce": 337389276,
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
			"updated": 1686230174158,
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
			"version": 81,
			"versionNonce": 1749239012,
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
			"updated": 1686230174158,
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
			"version": 244,
			"versionNonce": 606792540,
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
			"updated": 1686230174158,
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
			"version": 87,
			"versionNonce": 953223268,
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
			"updated": 1686230174158,
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
			"version": 74,
			"versionNonce": 1055727580,
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
			"updated": 1686230174158,
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
			"version": 131,
			"versionNonce": 1239047140,
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
			"updated": 1686230174158,
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
			"version": 1439,
			"versionNonce": 477414492,
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
			"updated": 1686230174158,
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
			"version": 610,
			"versionNonce": 627916644,
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
			"updated": 1686230174158,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 452,
			"versionNonce": 580114652,
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
			"updated": 1686230174158,
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
			"version": 548,
			"versionNonce": 1675080420,
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
			"updated": 1686230174158,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 438,
			"versionNonce": 752639324,
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
			"updated": 1686230174158,
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
			"version": 500,
			"versionNonce": 1671935588,
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
			"updated": 1686230174158,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 412,
			"versionNonce": 1419792860,
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
			"updated": 1686230174158,
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
			"version": 1311,
			"versionNonce": 28002788,
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
			"updated": 1686230174158,
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
			"version": 790,
			"versionNonce": 955364956,
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
			"updated": 1686230174158,
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
			"version": 725,
			"versionNonce": 1357933924,
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
			"updated": 1686230174158,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 670,
			"versionNonce": 1185057500,
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
			"updated": 1686230174159,
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
			"version": 657,
			"versionNonce": 1388650724,
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
			"updated": 1686230174159,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 630,
			"versionNonce": 4509532,
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
			"updated": 1686230174159,
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
			"version": 727,
			"versionNonce": 783770724,
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
			"updated": 1686230174159,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 681,
			"versionNonce": 1177191388,
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
			"updated": 1686230174159,
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
			"version": 611,
			"versionNonce": 1788164068,
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
			"updated": 1686230174159,
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
			"version": 1244,
			"versionNonce": 509978716,
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
			"updated": 1686230174159,
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
			"version": 596,
			"versionNonce": 577543012,
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
			"updated": 1686230174159,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 554,
			"versionNonce": 2093497564,
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
			"updated": 1686230174159,
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
			"version": 613,
			"versionNonce": 1082887908,
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
			"updated": 1686230174159,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 591,
			"versionNonce": 182731100,
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
			"updated": 1686230174159,
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
			"version": 600,
			"versionNonce": 897585764,
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
			"updated": 1686230174159,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 579,
			"versionNonce": 1879815644,
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
			"updated": 1686230174159,
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
			"version": 1084,
			"versionNonce": 806888932,
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
			"updated": 1686230174159,
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
			"version": 550,
			"versionNonce": 424712796,
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
			"updated": 1686230174159,
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
			"version": 305,
			"versionNonce": 1432471908,
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
			"updated": 1686230174159,
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
			"version": 303,
			"versionNonce": 25489116,
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
			"updated": 1686230174159,
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
			"version": 305,
			"versionNonce": 2024471780,
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
			"updated": 1686230174159,
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
			"version": 305,
			"versionNonce": 2033890140,
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
			"updated": 1686230174159,
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
			"version": 298,
			"versionNonce": 1401012324,
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
			"updated": 1686230174159,
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
			"version": 302,
			"versionNonce": 1858332636,
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
			"updated": 1686230174160,
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
			"version": 382,
			"versionNonce": 1035211748,
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
			"updated": 1686230174160,
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
			"version": 394,
			"versionNonce": 909282396,
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
			"updated": 1686230174160,
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
			"version": 380,
			"versionNonce": 1699739492,
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
			"updated": 1686230174160,
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
			"version": 378,
			"versionNonce": 1364762844,
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
			"updated": 1686230174160,
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
			"version": 367,
			"versionNonce": 111373028,
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
			"updated": 1686230174160,
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
			"version": 366,
			"versionNonce": 935863644,
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
			"updated": 1686230174160,
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
			"version": 173,
			"versionNonce": 607940196,
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
			"updated": 1686230174160,
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
			"version": 336,
			"versionNonce": 517151196,
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
			"updated": 1686230174160,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 344,
			"versionNonce": 1055457764,
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
			"updated": 1686230174160,
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
			"version": 350,
			"versionNonce": 1099660892,
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
			"updated": 1686230174160,
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
			"version": 573,
			"versionNonce": 230106468,
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
			"updated": 1686230174160,
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
			"version": 181,
			"versionNonce": 683889372,
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
			"updated": 1686230174160,
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
			"version": 216,
			"versionNonce": 905238756,
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
			"updated": 1686230174160,
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
			"version": 344,
			"versionNonce": 1930205020,
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
			"updated": 1686230174160,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 316,
			"versionNonce": 53484644,
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
			"updated": 1686230174160,
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
			"version": 428,
			"versionNonce": 481905628,
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
			"updated": 1686230174160,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 403,
			"versionNonce": 523694052,
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
			"updated": 1686230174160,
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
			"version": 1095,
			"versionNonce": 1205563484,
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
			"updated": 1686230174160,
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
			"version": 278,
			"versionNonce": 1243042660,
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
			"updated": 1686230174161,
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
			"version": 1047,
			"versionNonce": 71632092,
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
			"updated": 1686230174161,
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
			"version": 336,
			"versionNonce": 304039652,
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
			"updated": 1686230174161,
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
			"version": 398,
			"versionNonce": 394791260,
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
			"updated": 1686230174161,
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
			"version": 319,
			"versionNonce": 199019108,
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
			"updated": 1686230174161,
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
			"version": 238,
			"versionNonce": 1157004764,
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
			"updated": 1686230174161,
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
			"version": 400,
			"versionNonce": 169729508,
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
			"updated": 1686230174161,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 386,
			"versionNonce": 362963548,
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
			"updated": 1686230174161,
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
			"version": 1332,
			"versionNonce": 1441825124,
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
			"updated": 1686230174161,
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
			"version": 229,
			"versionNonce": 543012572,
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
			"updated": 1686230174161,
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
			"version": 526,
			"versionNonce": 1721939172,
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
			"updated": 1686230174161,
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
			"version": 440,
			"versionNonce": 1371175772,
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
			"updated": 1686230174161,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 388,
			"versionNonce": 432175204,
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
			"updated": 1686230174161,
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
			"version": 1510,
			"versionNonce": 873115612,
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
			"updated": 1686230174161,
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
			"version": 281,
			"versionNonce": 1797114852,
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
			"updated": 1686230174161,
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
			"version": 480,
			"versionNonce": 929059932,
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
			"updated": 1686230174161,
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
			"version": 136,
			"versionNonce": 750956388,
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
			"updated": 1686230174161,
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
			"version": 128,
			"versionNonce": 2039310556,
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
			"updated": 1686230174161,
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
			"version": 136,
			"versionNonce": 1056908004,
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
			"updated": 1686230174162,
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
			"version": 129,
			"versionNonce": 237235548,
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
			"updated": 1686230174162,
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
			"version": 256,
			"versionNonce": 1214326372,
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
			"updated": 1686230174162,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 244,
			"versionNonce": 1182130652,
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
			"updated": 1686230174162,
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
			"version": 319,
			"versionNonce": 1840691684,
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
			"updated": 1686230174162,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 306,
			"versionNonce": 2039826012,
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
			"updated": 1686230174162,
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
			"version": 262,
			"versionNonce": 168680804,
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
			"updated": 1686230174162,
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
			"version": 280,
			"versionNonce": 1280580316,
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
			"updated": 1686230174162,
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
			"version": 477,
			"versionNonce": 1723109604,
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
			"updated": 1686230174162,
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
			"version": 184,
			"versionNonce": 2034523996,
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
			"updated": 1686230174162,
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
			"version": 877,
			"versionNonce": 1933104228,
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
			"updated": 1686230174162,
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
			"version": 270,
			"versionNonce": 414716892,
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
			"updated": 1686230174162,
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
			"version": 439,
			"versionNonce": 2104010724,
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
			"updated": 1686230174162,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 453,
			"versionNonce": 1757493340,
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
			"updated": 1686230174162,
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
			"version": 345,
			"versionNonce": 1766984548,
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
			"updated": 1686230174162,
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
			"version": 665,
			"versionNonce": 355585244,
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
			"updated": 1686230174162,
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
			"version": 121,
			"versionNonce": 1765998308,
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
			"updated": 1686230174163,
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
			"version": 295,
			"versionNonce": 2140918108,
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
			"updated": 1686230174163,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 385,
			"versionNonce": 902398564,
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
			"updated": 1686230174163,
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
			"version": 601,
			"versionNonce": 122766812,
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
			"updated": 1686230174163,
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
			"version": 118,
			"versionNonce": 1169397220,
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
			"updated": 1686230174163,
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
			"version": 240,
			"versionNonce": 1365518940,
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
			"updated": 1686230174163,
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
			"version": 572,
			"versionNonce": 101661028,
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
			"updated": 1686230174163,
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
			"version": 118,
			"versionNonce": 279346908,
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
			"updated": 1686230174163,
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
			"version": 266,
			"versionNonce": 304770276,
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
			"updated": 1686230174163,
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
			"version": 240,
			"versionNonce": 1303003996,
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
			"updated": 1686230174163,
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
			"version": 167,
			"versionNonce": 1804808292,
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
			"updated": 1686230174163,
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
			"version": 199,
			"versionNonce": 784431068,
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
			"updated": 1686230174163,
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
			"version": 240,
			"versionNonce": 840401892,
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
			"updated": 1686230174163,
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
			"version": 165,
			"versionNonce": 1073618012,
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
			"updated": 1686230174163,
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
			"version": 380,
			"versionNonce": 1539663716,
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
			"updated": 1686230174163,
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
			"version": 354,
			"versionNonce": 993145052,
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
			"updated": 1686230174163,
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
			"version": 35,
			"versionNonce": 1827330788,
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
			"updated": 1686230174163,
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
			"version": 273,
			"versionNonce": 1341109596,
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
			"updated": 1686230174163,
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
			"version": 291,
			"versionNonce": 806739556,
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
			"updated": 1686230174163,
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
			"version": 42,
			"versionNonce": 1804118492,
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
			"updated": 1686230174164,
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
			"version": 201,
			"versionNonce": 1846833636,
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
			"updated": 1686230174164,
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
			"version": 60,
			"versionNonce": 17763932,
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
			"updated": 1686230174164,
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
			"version": 59,
			"versionNonce": 636786020,
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
			"updated": 1686230174164,
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
			"version": 178,
			"versionNonce": 1364517596,
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
			"updated": 1686230174164,
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
			"version": 454,
			"versionNonce": 1157908708,
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
			"updated": 1686230174164,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 734,
			"versionNonce": 854337372,
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
			"updated": 1686230174164,
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
			"version": 316,
			"versionNonce": 1590791268,
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
			"updated": 1686230174164,
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
			"version": 244,
			"versionNonce": 1512496092,
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
			"updated": 1686230174164,
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
			"version": 50,
			"versionNonce": 1697275876,
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
			"updated": 1686230174164,
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
			"version": 137,
			"versionNonce": 555155548,
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
			"updated": 1686230174164,
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
			"version": 521,
			"versionNonce": 1612497764,
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
			"updated": 1686230174164,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 807,
			"versionNonce": 1334744284,
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
			"updated": 1686230174164,
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
			"version": 175,
			"versionNonce": 636925668,
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
			"updated": 1686230174164,
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
			"version": 171,
			"versionNonce": 1663015260,
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
			"updated": 1686230174164,
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
			"version": 70,
			"versionNonce": 323369572,
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
			"updated": 1686230174164,
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
			"version": 178,
			"versionNonce": 1461456348,
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
			"updated": 1686230174164,
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
			"version": 484,
			"versionNonce": 1121537508,
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
			"updated": 1686230174164,
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
			"version": 55,
			"versionNonce": 1821766236,
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
			"updated": 1686230174164,
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
			"version": 158,
			"versionNonce": 1170076004,
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
			"updated": 1686230174164,
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
			"version": 217,
			"versionNonce": 1918846684,
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
			"updated": 1686230174165,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 266,
			"versionNonce": 1531061476,
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
			"updated": 1686230174165,
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
			"version": 194,
			"versionNonce": 218762076,
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
			"updated": 1686230174165,
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
			"version": 280,
			"versionNonce": 687073380,
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
			"updated": 1686230174165,
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
			"version": 177,
			"versionNonce": 2129149916,
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
			"updated": 1686230174165,
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
			"version": 249,
			"versionNonce": 1923169252,
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
			"updated": 1686230174165,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 232,
			"versionNonce": 1879827548,
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
			"updated": 1686230174165,
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
			"version": 287,
			"versionNonce": 1381506916,
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
			"updated": 1686230174165,
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
			"version": 612,
			"versionNonce": 910620892,
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
			"updated": 1686230174165,
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
			"version": 107,
			"versionNonce": 1885770468,
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
			"updated": 1686230174165,
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
			"version": 282,
			"versionNonce": 489389404,
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
			"updated": 1686230174165,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 244,
			"versionNonce": 995792484,
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
			"updated": 1686230174165,
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
			"version": 359,
			"versionNonce": 772501980,
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
			"updated": 1686230174165,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 442,
			"versionNonce": 537012708,
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
			"updated": 1686230174165,
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
			"version": 433,
			"versionNonce": 2012796508,
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
			"updated": 1686230174165,
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
			"version": 567,
			"versionNonce": 1097551204,
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
			"updated": 1686230174165,
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
			"version": 166,
			"versionNonce": 1472572124,
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
			"updated": 1686230174165,
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
			"version": 736,
			"versionNonce": 820248804,
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
			"updated": 1686230174165,
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
			"version": 107,
			"versionNonce": 1073999708,
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
			"updated": 1686230174165,
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
			"version": 230,
			"versionNonce": 637158500,
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
			"updated": 1686230174165,
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
			"version": 237,
			"versionNonce": 17146844,
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
			"updated": 1686230174166,
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
			"version": 174,
			"versionNonce": 914102244,
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
			"updated": 1686230174166,
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
			"version": 159,
			"versionNonce": 282904668,
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
			"updated": 1686230174166,
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
			"version": 202,
			"versionNonce": 242711396,
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
			"updated": 1686230174166,
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
			"version": 26,
			"versionNonce": 1398496476,
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
			"updated": 1686230174166,
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
			"version": 69,
			"versionNonce": 674918116,
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
			"updated": 1686230174166,
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
			"version": 385,
			"versionNonce": 1645437276,
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
			"updated": 1686230174166,
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
			"version": 205,
			"versionNonce": 72544868,
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
			"updated": 1686230174166,
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
			"version": 74,
			"versionNonce": 1414976988,
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
			"updated": 1686230174166,
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
			"version": 97,
			"versionNonce": 1636763108,
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
			"updated": 1686230174166,
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
			"version": 99,
			"versionNonce": 121092700,
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
			"updated": 1686230174166,
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
			"version": 108,
			"versionNonce": 1962715492,
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
			"updated": 1686230174166,
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
			"version": 97,
			"versionNonce": 1703415516,
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
			"updated": 1686230174166,
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
			"version": 116,
			"versionNonce": 568974564,
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
			"updated": 1686230174166,
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
			"version": 114,
			"versionNonce": 802804572,
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
			"updated": 1686230174166,
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
			"version": 87,
			"versionNonce": 837066852,
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
			"updated": 1686230174166,
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
			"version": 85,
			"versionNonce": 1149175772,
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
			"updated": 1686230174166,
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
			"version": 68,
			"versionNonce": 213578724,
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
			"updated": 1686230174166,
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
			"version": 66,
			"versionNonce": 1737075804,
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
			"updated": 1686230174166,
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
			"version": 81,
			"versionNonce": 1887098724,
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
			"updated": 1686230174166,
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
			"version": 67,
			"versionNonce": 181125340,
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
			"updated": 1686230174167,
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
			"version": 83,
			"versionNonce": 695356132,
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
			"updated": 1686230174167,
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
			"version": 69,
			"versionNonce": 366429532,
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
			"updated": 1686230174167,
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
			"version": 78,
			"versionNonce": 1244614244,
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
			"updated": 1686230174167,
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
			"version": 89,
			"versionNonce": 771635676,
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
			"updated": 1686230174167,
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
			"version": 30,
			"versionNonce": 1669325284,
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
			"updated": 1686230174167,
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
			"version": 49,
			"versionNonce": 2119343708,
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
			"updated": 1686230174167,
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
			"version": 43,
			"versionNonce": 1014105444,
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
			"updated": 1686230174167,
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
			"version": 42,
			"versionNonce": 2141614812,
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
			"updated": 1686230174167,
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
			"version": 32,
			"versionNonce": 173258980,
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
			"updated": 1686230174167,
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
			"version": 45,
			"versionNonce": 1082898268,
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
			"updated": 1686230174167,
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
			"version": 31,
			"versionNonce": 682818660,
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
			"updated": 1686230174167,
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
			"version": 33,
			"versionNonce": 760507356,
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
			"updated": 1686230174167,
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
			"version": 33,
			"versionNonce": 1365102564,
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
			"updated": 1686230174167,
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
			"version": 44,
			"versionNonce": 1477611612,
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
			"updated": 1686230174167,
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
			"version": 43,
			"versionNonce": 1415721828,
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
			"updated": 1686230174167,
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
			"version": 40,
			"versionNonce": 1083712732,
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
			"updated": 1686230174167,
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
			"version": 32,
			"versionNonce": 1343104740,
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
			"updated": 1686230174167,
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
			"version": 42,
			"versionNonce": 477571420,
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
			"updated": 1686230174167,
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
			"version": 31,
			"versionNonce": 1760537188,
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
			"updated": 1686230174167,
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
			"version": 40,
			"versionNonce": 520199644,
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
			"updated": 1686230174167,
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
			"version": 32,
			"versionNonce": 30719460,
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
			"updated": 1686230174167,
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
			"version": 33,
			"versionNonce": 1095336540,
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
			"updated": 1686230174168,
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
			"version": 35,
			"versionNonce": 1942708580,
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
			"updated": 1686230174168,
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
			"version": 52,
			"versionNonce": 169924316,
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
			"updated": 1686230174168,
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
			"version": 46,
			"versionNonce": 1176605924,
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
			"updated": 1686230174168,
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
			"version": 38,
			"versionNonce": 1444518748,
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
			"updated": 1686230174168,
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
			"version": 41,
			"versionNonce": 1717917796,
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
			"updated": 1686230174168,
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
			"version": 33,
			"versionNonce": 528863196,
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
			"updated": 1686230174168,
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
			"version": 32,
			"versionNonce": 1617210340,
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
			"updated": 1686230174168,
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
			"version": 43,
			"versionNonce": 1182233692,
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
			"updated": 1686230174168,
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
			"version": 39,
			"versionNonce": 372084580,
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
			"updated": 1686230174168,
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
			"version": 40,
			"versionNonce": 1489012956,
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
			"updated": 1686230174168,
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
			"version": 33,
			"versionNonce": 2014184164,
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
			"updated": 1686230174168,
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
			"version": 33,
			"versionNonce": 1509100892,
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
			"updated": 1686230174168,
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
			"version": 38,
			"versionNonce": 1016333924,
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
			"updated": 1686230174168,
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
			"version": 28,
			"versionNonce": 190906844,
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
			"updated": 1686230174168,
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
			"version": 43,
			"versionNonce": 411933156,
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
			"updated": 1686230174168,
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
			"version": 36,
			"versionNonce": 874276444,
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
			"updated": 1686230174168,
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
			"version": 38,
			"versionNonce": 1997061476,
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
			"updated": 1686230174168,
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
			"version": 94,
			"versionNonce": 1761032924,
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
			"updated": 1686230174168,
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
			"version": 195,
			"versionNonce": 827551972,
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
			"updated": 1686230174168,
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
			"version": 1375,
			"versionNonce": 1417903964,
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
			"updated": 1686230174168,
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
			"version": 90,
			"versionNonce": 1190900836,
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
			"updated": 1686230174169,
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
			"version": 93,
			"versionNonce": 2131964892,
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
			"updated": 1686230174169,
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
			"version": 136,
			"versionNonce": 365922276,
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
			"updated": 1686230174169,
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
			"version": 179,
			"versionNonce": 381179996,
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
			"updated": 1686230174169,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 156,
			"versionNonce": 299690852,
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
			"updated": 1686230174169,
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
			"version": 352,
			"versionNonce": 927263964,
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
			"updated": 1686230174169,
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
			"version": 51,
			"versionNonce": 2104614628,
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
			"updated": 1686230174169,
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
			"version": 119,
			"versionNonce": 843772252,
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
			"updated": 1686230174169,
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
			"version": 223,
			"versionNonce": 555508324,
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
			"updated": 1686230174169,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 202,
			"versionNonce": 1461478876,
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
			"updated": 1686230174169,
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
			"version": 488,
			"versionNonce": 61502948,
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
			"updated": 1686230174169,
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
			"version": 96,
			"versionNonce": 986401372,
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
			"updated": 1686230174169,
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
			"version": 165,
			"versionNonce": 573184356,
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
			"updated": 1686230174169,
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
			"version": 118,
			"versionNonce": 2727644,
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
			"updated": 1686230174169,
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
			"version": 244,
			"versionNonce": 669600996,
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
			"updated": 1686230174169,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 196,
			"versionNonce": 533291868,
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
			"updated": 1686230174169,
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
			"version": 210,
			"versionNonce": 645271652,
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
			"updated": 1686230174169,
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
			"version": 95,
			"versionNonce": 805083100,
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
			"updated": 1686230174169,
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
			"version": 128,
			"versionNonce": 1302225892,
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
			"updated": 1686230174169,
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
			"version": 222,
			"versionNonce": 752172124,
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
			"updated": 1686230174169,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 266,
			"versionNonce": 594560868,
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
			"updated": 1686230174170,
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
			"version": 153,
			"versionNonce": 1076187356,
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
			"updated": 1686230174170,
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
			"version": 227,
			"versionNonce": 1010416356,
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
			"updated": 1686230174170,
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
			"version": 351,
			"versionNonce": 159307100,
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
			"updated": 1686230174170,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 445,
			"versionNonce": 1921564260,
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
			"updated": 1686230174170,
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
			"version": 541,
			"versionNonce": 1714670044,
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
			"updated": 1686230174170,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 679,
			"versionNonce": 522932708,
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
			"updated": 1686230174170,
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
			"version": 934,
			"versionNonce": 961949276,
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
			"updated": 1686230174170,
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
			"version": 88,
			"versionNonce": 1362064740,
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
			"updated": 1686230174170,
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
			"version": 404,
			"versionNonce": 867697372,
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
			"updated": 1686230174170,
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
			"version": 1263,
			"versionNonce": 98773220,
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
			"updated": 1686230174170,
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
			"version": 216,
			"versionNonce": 468404060,
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
			"updated": 1686230174170,
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
			"version": 462,
			"versionNonce": 1624534116,
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
			"updated": 1686230174170,
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
			"version": 247,
			"versionNonce": 373423068,
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
			"updated": 1686230174170,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 234,
			"versionNonce": 1674657764,
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
			"updated": 1686230174170,
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
			"version": 457,
			"versionNonce": 1825448028,
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
			"updated": 1686230174170,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 447,
			"versionNonce": 652714852,
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
			"updated": 1686230174170,
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
			"version": 496,
			"versionNonce": 1466021084,
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
			"updated": 1686230174170,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 510,
			"versionNonce": 275093220,
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
			"updated": 1686230174170,
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
			"version": 431,
			"versionNonce": 1133427036,
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
			"updated": 1686230174170,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 467,
			"versionNonce": 215554660,
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
			"updated": 1686230174170,
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
			"version": 1751,
			"versionNonce": 480718300,
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
			"updated": 1686230174171,
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
			"version": 226,
			"versionNonce": 1192242660,
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
			"updated": 1686230174171,
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
			"version": 238,
			"versionNonce": 331158108,
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
			"updated": 1686230174171,
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
			"version": 144,
			"versionNonce": 1612239204,
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
			"updated": 1686230174171,
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
			"version": 453,
			"versionNonce": 1738696412,
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
			"updated": 1686230174171,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 455,
			"versionNonce": 658572516,
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
			"updated": 1686230174171,
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
			"version": 179,
			"versionNonce": 753478492,
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
			"updated": 1686230174171,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 157,
			"versionNonce": 1377224804,
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
			"updated": 1686230174171,
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
			"version": 187,
			"versionNonce": 367222748,
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
			"updated": 1686230174171,
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
			"version": 213,
			"versionNonce": 879238116,
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
			"updated": 1686230174171,
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
			"version": 141,
			"versionNonce": 983762012,
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
			"updated": 1686230174171,
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
			"version": 189,
			"versionNonce": 2017656676,
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
			"updated": 1686230174171,
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
			"version": 294,
			"versionNonce": 1627003100,
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
			"updated": 1686230174171,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 277,
			"versionNonce": 1442149092,
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
			"updated": 1686230174171,
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
			"version": 335,
			"versionNonce": 1148886364,
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
			"updated": 1686230174171,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 313,
			"versionNonce": 1275950692,
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
			"updated": 1686230174171,
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
			"version": 382,
			"versionNonce": 1584828892,
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
			"updated": 1686230174171,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 284,
			"versionNonce": 1465453028,
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
			"updated": 1686230174171,
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
			"version": 248,
			"versionNonce": 771749468,
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
			"updated": 1686230174171,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 298,
			"versionNonce": 719727972,
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
			"updated": 1686230174171,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 292,
			"versionNonce": 2145962716,
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
			"updated": 1686230174172,
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
			"version": 352,
			"versionNonce": 1745019108,
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
			"updated": 1686230174172,
			"link": null,
			"locked": false
		},
		{
			"type": "line",
			"version": 161,
			"versionNonce": 918753116,
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
			"updated": 1686230174172,
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
			"version": 181,
			"versionNonce": 1446847588,
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
			"updated": 1686230174172,
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
			"version": 578,
			"versionNonce": 316720092,
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
			"updated": 1686230174172,
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
			"version": 175,
			"versionNonce": 459470820,
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
			"updated": 1686230174172,
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
			"version": 360,
			"versionNonce": 2052319324,
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
			"updated": 1686230174172,
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
			"version": 382,
			"versionNonce": 1937922916,
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
			"updated": 1686230174172,
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
			"version": 119,
			"versionNonce": 1089371356,
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
			"updated": 1686230174172,
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
			"version": 20,
			"versionNonce": 1760120548,
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
			"updated": 1686230174172,
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
			"version": 400,
			"versionNonce": 1883406684,
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
			"updated": 1686230174172,
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
			"version": 460,
			"versionNonce": 203805284,
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
			"updated": 1686230174172,
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
			"version": 47,
			"versionNonce": 262272476,
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
			"updated": 1686230174172,
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
			"version": 199,
			"versionNonce": 738584036,
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
			"updated": 1686230174172,
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
			"version": 26,
			"versionNonce": 1813961308,
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
			"updated": 1686230174172,
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
			"version": 86,
			"versionNonce": 228034916,
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
			"updated": 1686230174172,
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
			"version": 21,
			"versionNonce": 1619734236,
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
			"updated": 1686230174172,
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
			"version": 95,
			"versionNonce": 606649572,
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
			"updated": 1686230174172,
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
			"version": 89,
			"versionNonce": 494465884,
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
			"updated": 1686230174172,
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
			"version": 89,
			"versionNonce": 1229422692,
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
			"updated": 1686230174172,
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
			"version": 81,
			"versionNonce": 1899636700,
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
			"updated": 1686230174173,
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
			"version": 91,
			"versionNonce": 1958859748,
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
			"updated": 1686230174173,
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
			"version": 91,
			"versionNonce": 266390620,
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
			"updated": 1686230174173,
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
			"version": 102,
			"versionNonce": 1957017444,
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
			"updated": 1686230174173,
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
			"version": 47,
			"versionNonce": 1530847452,
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
			"updated": 1686230174173,
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
			"version": 21,
			"versionNonce": 625027812,
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
			"updated": 1686230174173,
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
			"version": 94,
			"versionNonce": 719742300,
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
			"updated": 1686230174173,
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
			"version": 109,
			"versionNonce": 690105956,
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
			"updated": 1686230174173,
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
			"version": 91,
			"versionNonce": 338254300,
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
			"updated": 1686230174173,
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
			"version": 44,
			"versionNonce": 555139556,
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
			"updated": 1686230174173,
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
			"version": 69,
			"versionNonce": 840547932,
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
			"updated": 1686230174173,
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
			"version": 491,
			"versionNonce": 1680663908,
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
			"updated": 1686230174173,
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
			"version": 42,
			"versionNonce": 1837732572,
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
			"updated": 1686230174173,
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
			"version": 47,
			"versionNonce": 934451428,
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
			"updated": 1686230174173,
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
			"version": 166,
			"versionNonce": 1158338396,
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
			"updated": 1686230174173,
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
			"version": 175,
			"versionNonce": 120970340,
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
			"updated": 1686230174173,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 168,
			"versionNonce": 351243228,
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
			"updated": 1686230174173,
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
			"version": 414,
			"versionNonce": 478457828,
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
			"updated": 1686230174173,
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
			"version": 97,
			"versionNonce": 1598664796,
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
			"updated": 1686230174173,
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
			"version": 179,
			"versionNonce": 1470960484,
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
			"updated": 1686230174173,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 172,
			"versionNonce": 334185692,
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
			"updated": 1686230174173,
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
			"version": 169,
			"versionNonce": 1727858404,
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
			"updated": 1686230174174,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 301,
			"versionNonce": 1483098460,
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
			"updated": 1686230174174,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 388,
			"versionNonce": 2130872932,
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
			"updated": 1686230174174,
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
			"version": 294,
			"versionNonce": 1343012316,
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
			"updated": 1686230174174,
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
			"version": 240,
			"versionNonce": 311139812,
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
			"updated": 1686230174174,
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
			"version": 247,
			"versionNonce": 1676714588,
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
			"updated": 1686230174174,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 394,
			"versionNonce": 178667876,
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
			"updated": 1686230174174,
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
			"version": 252,
			"versionNonce": 182712028,
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
			"updated": 1686230174174,
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
			"version": 277,
			"versionNonce": 2124444900,
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
			"updated": 1686230174174,
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
			"version": 212,
			"versionNonce": 293124956,
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
			"updated": 1686230174174,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 260,
			"versionNonce": 1812478052,
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
			"updated": 1686230174174,
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
			"version": 396,
			"versionNonce": 1644228572,
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
			"updated": 1686230174174,
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
			"version": 141,
			"versionNonce": 1856736228,
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
			"updated": 1686230174174,
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
			"version": 287,
			"versionNonce": 1284412508,
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
			"updated": 1686230174174,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 298,
			"versionNonce": 2023255908,
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
			"updated": 1686230174174,
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
			"version": 416,
			"versionNonce": 1324591324,
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
			"updated": 1686230174174,
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
			"version": 176,
			"versionNonce": 169665252,
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
			"updated": 1686230174174,
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
			"version": 137,
			"versionNonce": 1556229468,
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
			"updated": 1686230174174,
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
			"version": 133,
			"versionNonce": 1774642788,
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
			"updated": 1686230174174,
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
			"version": 134,
			"versionNonce": 659300828,
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
			"updated": 1686230174174,
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
			"version": 140,
			"versionNonce": 1550088676,
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
			"updated": 1686230174174,
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
			"version": 110,
			"versionNonce": 1705215580,
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
			"updated": 1686230174175,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 94,
			"versionNonce": 1560517988,
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
			"updated": 1686230174175,
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
			"version": 100,
			"versionNonce": 479877852,
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
			"updated": 1686230174175,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 352,
			"versionNonce": 1425166564,
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
			"updated": 1686230174175,
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
			"version": 705,
			"versionNonce": 1724030812,
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
			"updated": 1686230174175,
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
			"version": 49,
			"versionNonce": 1404998756,
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
			"updated": 1686230174175,
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
			"version": 147,
			"versionNonce": 1013863388,
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
			"updated": 1686230174175,
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
			"version": 9,
			"versionNonce": 1194747876,
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
			"updated": 1686230174175,
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
			"version": 496,
			"versionNonce": 1001355356,
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
			"updated": 1686230174175,
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
			"version": 567,
			"versionNonce": 862440292,
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
			"updated": 1686230174175,
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
			"version": 9,
			"versionNonce": 1884818652,
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
			"updated": 1686230174175,
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
			"version": 371,
			"versionNonce": 1788919524,
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
			"updated": 1686230174175,
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
			"version": 54,
			"versionNonce": 469373276,
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
			"updated": 1686230174175,
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
			"version": 12,
			"versionNonce": 1164919396,
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
			"updated": 1686230174175,
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
			"version": 32,
			"versionNonce": 2112325084,
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
			"updated": 1686230174175,
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
			"version": 57,
			"versionNonce": 1520522724,
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
			"updated": 1686230174175,
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
			"version": 935,
			"versionNonce": 456288860,
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
			"updated": 1686230174175,
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
			"version": 238,
			"versionNonce": 927267172,
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
			"updated": 1686230174175,
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
			"version": 6,
			"versionNonce": 111984348,
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
			"updated": 1686230174175,
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
			"version": 41,
			"versionNonce": 380120292,
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
			"updated": 1686230174176,
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
			"version": 349,
			"versionNonce": 686326620,
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
			"updated": 1686230174176,
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
			"version": 29,
			"versionNonce": 442036324,
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
			"updated": 1686230174176,
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
			"version": 84,
			"versionNonce": 137869276,
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
			"updated": 1686230174176,
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
			"version": 5,
			"versionNonce": 35996644,
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
			"updated": 1686230174176,
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
			"version": 29,
			"versionNonce": 279731292,
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
			"updated": 1686230174176,
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
			"version": 14,
			"versionNonce": 1679501156,
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
			"updated": 1686230174176,
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
			"version": 14,
			"versionNonce": 1545105628,
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
			"updated": 1686230174176,
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
			"version": 349,
			"versionNonce": 1686674148,
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
			"updated": 1686230174176,
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
			"id": "7E6maRv2",
			"type": "text",
			"x": 6974.129494242654,
			"y": -342.47836660029964,
			"width": 334,
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
			"seed": 1479951332,
			"version": 4,
			"versionNonce": 2047735132,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230174176,
			"link": null,
			"locked": false,
			"text": "## 11. Container With Most Water\n",
			"rawText": "## 11. Container With Most Water\n",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "left",
			"verticalAlign": "top",
			"baseline": 42,
			"containerId": null,
			"originalText": "## 11. Container With Most Water\n",
			"lineHeight": 1.25
		},
		{
			"type": "text",
			"version": 548,
			"versionNonce": 1845206628,
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
			"updated": 1686230174176,
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
			"version": 625,
			"versionNonce": 937355740,
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
			"updated": 1686230174176,
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
			"id": "1wV7KCko",
			"type": "text",
			"x": 6941.229391354819,
			"y": -240.52838055119244,
			"width": 50,
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
			"seed": 1524031460,
			"version": 78,
			"versionNonce": 1765945828,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230174176,
			"link": null,
			"locked": false,
			"text": "INFO",
			"rawText": "INFO",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "left",
			"verticalAlign": "top",
			"baseline": 17,
			"containerId": null,
			"originalText": "INFO",
			"lineHeight": 1.25
		},
		{
			"id": "BC6F8C7t",
			"type": "text",
			"x": 6999.699726256734,
			"y": -173.3810903109151,
			"width": 458,
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
			"seed": 1176142564,
			"version": 268,
			"versionNonce": 1755139676,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230174176,
			"link": null,
			"locked": false,
			"text": "Find two lines that together with \nthe x-axis form a container, this \ncontainer must contain the most water.\n- height: int[]      (\n- n:      int length ( n== heght.len )\n- return the max water a container can store\n\n>  int maxArea (int[] height) <",
			"rawText": "Find two lines that together with \nthe x-axis form a container, this \ncontainer must contain the most water.\n- height: int[]      (\n- n:      int length ( n== heght.len )\n- return the max water a container can store\n\n>  int maxArea (int[] height) <",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "left",
			"verticalAlign": "top",
			"baseline": 192,
			"containerId": null,
			"originalText": "Find two lines that together with \nthe x-axis form a container, this \ncontainer must contain the most water.\n- height: int[]      (\n- n:      int length ( n== heght.len )\n- return the max water a container can store\n\n>  int maxArea (int[] height) <",
			"lineHeight": 1.25
		},
		{
			"id": "lMxKPcvf",
			"type": "text",
			"x": 6941.985427463486,
			"y": 75.47602638830364,
			"width": 91,
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
			"seed": 626437340,
			"version": 19,
			"versionNonce": 1969902948,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230174176,
			"link": null,
			"locked": false,
			"text": "EXAMPLE",
			"rawText": "EXAMPLE",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "left",
			"verticalAlign": "top",
			"baseline": 17,
			"containerId": null,
			"originalText": "EXAMPLE",
			"lineHeight": 1.25
		},
		{
			"id": "zEW3vNBp",
			"type": "text",
			"x": 7007.414003251714,
			"y": 146.04748983696453,
			"width": 560,
			"height": 125,
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
			"seed": 239320028,
			"version": 62,
			"versionNonce": 756753116,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230174176,
			"link": null,
			"locked": false,
			"text": "Input: height = [1,8,6,2,5,4,8,3,7]\nOutput: 49\nExplanation: The above vertical lines are represented \nby array [1,8,6,2,5,4,8,3,7]. In this case, the max area \nof water (blue section) the container can contain is 49.",
			"rawText": "Input: height = [1,8,6,2,5,4,8,3,7]\nOutput: 49\nExplanation: The above vertical lines are represented \nby array [1,8,6,2,5,4,8,3,7]. In this case, the max area \nof water (blue section) the container can contain is 49.",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "left",
			"verticalAlign": "top",
			"baseline": 117,
			"containerId": null,
			"originalText": "Input: height = [1,8,6,2,5,4,8,3,7]\nOutput: 49\nExplanation: The above vertical lines are represented \nby array [1,8,6,2,5,4,8,3,7]. In this case, the max area \nof water (blue section) the container can contain is 49.",
			"lineHeight": 1.25
		},
		{
			"id": "1DkcQeCD0tfr1SnhtFrUq",
			"type": "freedraw",
			"x": 7006.137309716637,
			"y": 347.540297623183,
			"width": 15.91246258853434,
			"height": 30.378357735569384,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"roundness": null,
			"seed": 28253668,
			"version": 215,
			"versionNonce": 1494798948,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230204622,
			"link": null,
			"locked": true,
			"points": [
				[
					0,
					0
				],
				[
					0,
					-0.723283720749684
				],
				[
					2.893162474504149,
					-2.8931900660092027
				],
				[
					5.063041228258183,
					-5.786324949007651
				],
				[
					7.2329475735170545,
					-10.12613763952669
				],
				[
					7.2329475735170545,
					-13.019272522525208
				],
				[
					5.786352540513136,
					-16.635746309283952
				],
				[
					-0.7233113122549534,
					-16.635746309283952
				],
				[
					-2.1699063452600225,
					-14.465895147035116
				],
				[
					-2.1699063452600225,
					-10.849421360276372
				],
				[
					-0.7233113122549534,
					-7.95623129426717
				],
				[
					2.893162474504149,
					-3.616473786758815
				],
				[
					5.063041228258183,
					-1.446567441499296
				],
				[
					7.2329475735170545,
					1.4466226245099068
				],
				[
					8.679515015017286,
					5.06309641126865
				],
				[
					7.2329475735170545,
					7.232947573517486
				],
				[
					4.339757507508067,
					9.402853918777076
				],
				[
					-2.1699063452600225,
					11.572705081025912
				],
				[
					-6.50966385276809,
					10.8494213602763
				],
				[
					-7.2329475735170545,
					10.12613763952669
				],
				[
					-7.2329475735170545,
					10.8494213602763
				],
				[
					-5.786380132017974,
					11.572705081025912
				],
				[
					-2.893190066008987,
					13.742611426285432
				],
				[
					0,
					0
				]
			],
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
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				-2.2857230050221915,
				10.85715157645086
			]
		},
		{
			"id": "qL2qOP6t0VfdSKCKyjm4w",
			"type": "freedraw",
			"x": 7004.690714683632,
			"y": 390.21469934353865,
			"width": 13.019300114030191,
			"height": 23.1454101620519,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"roundness": null,
			"seed": 1893419876,
			"version": 213,
			"versionNonce": 2136929756,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230204622,
			"link": null,
			"locked": true,
			"points": [
				[
					0,
					0
				],
				[
					-1.446595033003918,
					0
				],
				[
					-1.446595033003918,
					-2.169906345259591
				],
				[
					0,
					-5.7863801320183335
				],
				[
					0.7232837207501157,
					-7.232947573517558
				],
				[
					2.1698787537551847,
					-10.849421360276372
				],
				[
					3.616473786759103,
					-13.742611426285503
				],
				[
					5.063068819764172,
					-16.635801492294636
				],
				[
					5.786352540513136,
					-17.359085213044246
				],
				[
					6.5096362612632515,
					-18.805652654543543
				],
				[
					6.5096362612632515,
					-19.528936375293153
				],
				[
					6.5096362612632515,
					-20.25227527905345
				],
				[
					6.5096362612632515,
					-20.975558999803063
				],
				[
					3.616473786759103,
					-20.975558999803063
				],
				[
					0.7232837207501157,
					-20.975558999803063
				],
				[
					-2.1698787537540336,
					-21.698842720552673
				],
				[
					-3.6164737867579513,
					-21.698842720552673
				],
				[
					-5.0630688197630205,
					-22.422126441302286
				],
				[
					-5.786352540511985,
					-22.422126441302286
				],
				[
					-6.509663852766939,
					-23.1454101620519
				],
				[
					-6.509663852766939,
					-22.422126441302286
				],
				[
					-4.3397850990129045,
					-20.25227527905345
				],
				[
					-4.3397850990129045,
					-20.25227527905345
				]
			],
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
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				-3.4285845075328325,
				-16.000017438616112
			]
		},
		{
			"id": "g4WcCiIUGq5bAEEczV7LD",
			"type": "freedraw",
			"x": 7001.797524617623,
			"y": 396.00107947555693,
			"width": 10.126137639526041,
			"height": 30.378357735569455,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"roundness": null,
			"seed": 295556452,
			"version": 212,
			"versionNonce": 1654187492,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230204622,
			"link": null,
			"locked": true,
			"points": [
				[
					0,
					0
				],
				[
					-2.1698787537540336,
					2.169851162248908
				],
				[
					-3.6164737867579513,
					7.232947573517558
				],
				[
					-6.5096362612621,
					14.465895147035116
				],
				[
					-7.2329475735170545,
					20.97550381679238
				],
				[
					-7.2329475735170545,
					26.03860022806103
				],
				[
					-6.5096362612621,
					28.931790294070233
				],
				[
					-3.6164737867579513,
					30.378357735569455
				],
				[
					0,
					28.208451390309936
				],
				[
					1.4465950330050692,
					25.315316507311415
				],
				[
					2.893190066008987,
					22.422126441302286
				],
				[
					2.893190066008987,
					19.528936375293153
				],
				[
					2.1698787537540336,
					17.359030030033562
				],
				[
					0.7233113122549534,
					15.189178867784728
				],
				[
					-0.7232837207489645,
					14.465895147035116
				],
				[
					-2.1698787537540336,
					15.91246258853434
				],
				[
					-2.893162474502998,
					17.359030030033562
				],
				[
					-3.6164737867579513,
					19.528936375293153
				],
				[
					-3.6164737867579513,
					20.252220096042766
				],
				[
					-2.893162474502998,
					21.698842720552673
				],
				[
					0.7233113122549534,
					25.315316507311415
				],
				[
					0.7233113122549534,
					25.315316507311415
				]
			],
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
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				0.571441650390625,
				20
			]
		},
		{
			"id": "ZVUtzZzCOES0vhOyr3CM4",
			"type": "freedraw",
			"x": 6999.627645863869,
			"y": 458.2044175712057,
			"width": 5.063041228257031,
			"height": 10.849421360276372,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"roundness": null,
			"seed": 1657709660,
			"version": 205,
			"versionNonce": 1547426396,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230204622,
			"link": null,
			"locked": true,
			"points": [
				[
					0,
					0
				],
				[
					0,
					0.723283720749684
				],
				[
					-0.7232837207489645,
					0
				],
				[
					-0.7232837207489645,
					-0.723283720749612
				],
				[
					0.7232837207501157,
					-3.616473786758743
				],
				[
					2.1698787537540336,
					-6.509663852767874
				],
				[
					2.893190066008987,
					-8.679570198027392
				],
				[
					3.616473786759103,
					-10.12613763952669
				],
				[
					3.616473786759103,
					-9.402853918777005
				],
				[
					3.616473786759103,
					-8.679570198027392
				],
				[
					3.616473786759103,
					-7.95623129426717
				],
				[
					4.339757507508067,
					-7.232947573517486
				],
				[
					4.339757507508067,
					-5.06309641126865
				],
				[
					0,
					0
				]
			],
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
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				3.428562709263133,
				-4.000026157924083
			]
		},
		{
			"id": "wWaNjF2LOj3D5Dgci2ixG",
			"type": "freedraw",
			"x": 6996.01117207711,
			"y": 466.1606488654728,
			"width": 14.46589514703526,
			"height": 29.65507401481977,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"roundness": null,
			"seed": 81758300,
			"version": 221,
			"versionNonce": 2043316580,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230204622,
			"link": null,
			"locked": true,
			"points": [
				[
					0,
					0
				],
				[
					0.7232837207501157,
					0
				],
				[
					2.1698787537551847,
					0
				],
				[
					3.616473786759103,
					-0.723283720749612
				],
				[
					6.50966385276809,
					-2.169906345259519
				],
				[
					8.679542606522123,
					-4.339757507508355
				],
				[
					10.849421360277308,
					-6.509663852767874
				],
				[
					11.572705081026273,
					-8.679515015016781
				],
				[
					12.296016393281226,
					-10.12613763952669
				],
				[
					11.572705081026273,
					-11.572705081025912
				],
				[
					10.126137639527192,
					-13.742611426285432
				],
				[
					8.679542606522123,
					-14.465895147035043
				],
				[
					7.232947573518206,
					-15.189178867784655
				],
				[
					5.786352540513136,
					-14.465895147035043
				],
				[
					5.063068819764172,
					-14.465895147035043
				],
				[
					3.616473786759103,
					-15.189178867784655
				],
				[
					2.8931900660101384,
					-17.359085213044175
				],
				[
					1.4465950330050692,
					-19.528936375293082
				],
				[
					0,
					-21.6988427205526
				],
				[
					-1.446595033003918,
					-25.315316507311344
				],
				[
					-2.1698787537540336,
					-26.03860022806103
				],
				[
					-2.1698787537540336,
					-26.76188394881064
				],
				[
					-2.1698787537540336,
					-27.485222852570935
				],
				[
					-0.7232837207489645,
					-28.20850657332055
				],
				[
					0.7232837207501157,
					-28.931790294070158
				],
				[
					2.8931900660101384,
					-28.931790294070158
				],
				[
					6.50966385276809,
					-28.931790294070158
				],
				[
					8.679542606522123,
					-29.65507401481977
				],
				[
					10.126137639527192,
					-29.65507401481977
				],
				[
					10.849421360277308,
					-29.65507401481977
				],
				[
					10.849421360277308,
					-29.65507401481977
				]
			],
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
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				8.571428571429351,
				-23.42856270926336
			]
		},
		{
			"id": "Yae8gClQPsRhtgApektVf",
			"type": "freedraw",
			"x": 7000.350929584619,
			"y": 497.9856292255522,
			"width": 15.189206459290213,
			"height": 23.145465345062508,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"roundness": null,
			"seed": 244666460,
			"version": 215,
			"versionNonce": 1158164188,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230204622,
			"link": null,
			"locked": true,
			"points": [
				[
					0,
					0
				],
				[
					0.7233113122549534,
					-0.723283720749612
				],
				[
					1.446595033003918,
					-3.616473786758743
				],
				[
					2.893190066008987,
					-7.232947573517558
				],
				[
					3.6164737867579513,
					-11.572705081025912
				],
				[
					4.3397850990129045,
					-14.465895147035116
				],
				[
					4.3397850990129045,
					-15.189178867784728
				],
				[
					5.0630688197630205,
					-15.189178867784728
				],
				[
					5.786380132017974,
					-13.742611426285432
				],
				[
					5.0630688197630205,
					-13.019327705535819
				],
				[
					3.6164737867579513,
					-11.572705081025912
				],
				[
					1.446595033003918,
					-9.402853918777076
				],
				[
					0,
					-8.679570198027465
				],
				[
					-1.4465674414990801,
					-8.679570198027465
				],
				[
					-3.616473786759103,
					-9.402853918777076
				],
				[
					-5.063041228258183,
					-10.8494213602763
				],
				[
					-7.232947573518206,
					-12.296043984786207
				],
				[
					-9.402826327272239,
					-15.912517771545023
				],
				[
					-9.402826327272239,
					-18.08236893379386
				],
				[
					-8.679515015017286,
					-19.528991558303765
				],
				[
					-6.5096362612632515,
					-21.6988427205526
				],
				[
					-4.339757507509218,
					-23.145465345062508
				],
				[
					-3.616473786759103,
					-23.145465345062508
				],
				[
					-1.4465674414990801,
					-23.145465345062508
				],
				[
					-1.4465674414990801,
					-23.145465345062508
				]
			],
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
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				-1.1428397042409415,
				-18.28574044363836
			]
		},
		{
			"id": "WDJwtPxOUlzKjpvNKZ6uq",
			"type": "freedraw",
			"x": 6991.671414569601,
			"y": 530.5338933063812,
			"width": 11.57273267253111,
			"height": 24.59203278656173,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"roundness": null,
			"seed": 1862400732,
			"version": 215,
			"versionNonce": 301710564,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230204622,
			"link": null,
			"locked": true,
			"points": [
				[
					0,
					0
				],
				[
					-1.446595033003918,
					0.723283720749684
				],
				[
					-2.1699063452588714,
					1.446567441499224
				],
				[
					-1.446595033003918,
					2.169851162248908
				],
				[
					-0.7233113122549534,
					3.616473786758815
				],
				[
					1.4465674414990801,
					4.339757507508355
				],
				[
					4.339757507508067,
					4.339757507508355
				],
				[
					5.786352540513136,
					2.8931900660091308
				],
				[
					7.232947573518206,
					1.446567441499224
				],
				[
					7.232947573518206,
					-0.723283720749684
				],
				[
					6.5096362612632515,
					-1.4466226245099068
				],
				[
					4.339757507508067,
					-2.8931900660091308
				],
				[
					2.893162474504149,
					-2.8931900660091308
				],
				[
					2.893162474504149,
					-4.339757507508355
				],
				[
					5.786352540513136,
					-5.7863801320182615
				],
				[
					7.95623129426717,
					-7.95623129426717
				],
				[
					9.402826327272239,
					-11.572705081025985
				],
				[
					7.232947573518206,
					-14.465895147035116
				],
				[
					5.063041228258183,
					-16.63580149229456
				],
				[
					2.893162474504149,
					-18.805652654543472
				],
				[
					1.4465674414990801,
					-20.25227527905338
				],
				[
					2.1698787537540336,
					-18.805652654543472
				],
				[
					3.616473786759103,
					-13.019327705535892
				],
				[
					0,
					0
				]
			],
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
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				2.857142857143117,
				-10.28573172433039
			]
		},
		{
			"id": "VQCMsrfTiiPoDrpnMNAVD",
			"type": "freedraw",
			"x": 7001.797524617623,
			"y": 563.8054411079597,
			"width": 14.46589514703526,
			"height": 17.359085213044246,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"roundness": null,
			"seed": 571577692,
			"version": 212,
			"versionNonce": 1784017756,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230204622,
			"link": null,
			"locked": true,
			"points": [
				[
					0,
					0
				],
				[
					-2.1698787537540336,
					0.723283720749684
				],
				[
					-3.6164737867579513,
					0.723283720749684
				],
				[
					-5.786352540513136,
					0.723283720749684
				],
				[
					-7.2329475735170545,
					0
				],
				[
					-7.95623129426717,
					-0.723283720749684
				],
				[
					-7.2329475735170545,
					-2.8931900660091308
				],
				[
					-3.6164737867579513,
					-5.7863801320182615
				],
				[
					-2.1698787537540336,
					-7.95623129426717
				],
				[
					-2.1698787537540336,
					-10.12613763952676
				],
				[
					-2.1698787537540336,
					-11.572705081025985
				],
				[
					-3.6164737867579513,
					-14.465895147035116
				],
				[
					-6.5096362612621,
					-15.91246258853434
				],
				[
					-10.849421360276157,
					-16.63580149229456
				],
				[
					-13.019300114030191,
					-15.91246258853434
				],
				[
					-13.742583834780305,
					-15.91246258853434
				],
				[
					-14.46589514703526,
					-15.91246258853434
				],
				[
					-14.46589514703526,
					-15.189178867784655
				],
				[
					-13.742583834780305,
					-12.295988801775525
				],
				[
					-10.849421360276157,
					-9.402853918777076
				],
				[
					0,
					0
				]
			],
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
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				-8.571428571428442,
				-7.4285888671875
			]
		},
		{
			"id": "elFx3phLJBMhzuUL1I1ZD",
			"type": "freedraw",
			"x": 6994.564577044106,
			"y": 605.0332202038056,
			"width": 2.1698787537540336,
			"height": 23.86869388280158,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"roundness": null,
			"seed": 478299364,
			"version": 199,
			"versionNonce": 79331428,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230204622,
			"link": null,
			"locked": true,
			"points": [
				[
					0,
					0
				],
				[
					0.7233113122549534,
					-8.679515015016925
				],
				[
					2.1698787537540336,
					-15.189178867784728
				],
				[
					2.1698787537540336,
					-20.252220096042766
				],
				[
					0.7233113122549534,
					-23.1454101620519
				],
				[
					0.7233113122549534,
					-23.86869388280158
				],
				[
					0.7233113122549534,
					-23.1454101620519
				],
				[
					1.446595033003918,
					-20.252220096042766
				],
				[
					1.446595033003918,
					-20.252220096042766
				]
			],
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
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				1.142861502510641,
				-15.999973842075917
			]
		},
		{
			"id": "CXubDOUDlLikJEqih4rfl",
			"type": "freedraw",
			"x": 6985.885034437583,
			"y": 640.4746743506438,
			"width": 13.742611426285144,
			"height": 23.145465345062508,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"roundness": null,
			"seed": 277263972,
			"version": 209,
			"versionNonce": 444016604,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230204622,
			"link": null,
			"locked": true,
			"points": [
				[
					0,
					0
				],
				[
					2.1699063452588714,
					5.7863801320182615
				],
				[
					6.50966385276809,
					5.063041228257895
				],
				[
					10.126137639526041,
					2.8932452490198135
				],
				[
					12.296016393281226,
					0.7233389037603667
				],
				[
					13.742611426285144,
					-1.446567441499368
				],
				[
					13.742611426285144,
					-5.063041228257895
				],
				[
					13.742611426285144,
					-10.849421360276445
				],
				[
					13.01932770553618,
					-13.742611426285432
				],
				[
					12.296016393281226,
					-15.189178867784799
				],
				[
					11.57273267253111,
					-15.91246258853434
				],
				[
					9.402853918777076,
					-16.63574630928388
				],
				[
					5.786380132017974,
					-17.359085213044246
				],
				[
					3.616473786759103,
					-16.63574630928388
				],
				[
					2.1699063452588714,
					-15.91246258853434
				],
				[
					1.446595033003918,
					-11.572705081025985
				],
				[
					2.893190066008987,
					-6.509663852767802
				],
				[
					0,
					0
				]
			],
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
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				2.2857230050221915,
				-5.142865862165081
			]
		},
		{
			"id": "O_yNuEUA1LQVpXBMRneme",
			"type": "freedraw",
			"x": 6978.6520868640655,
			"y": 652.0474346146804,
			"width": 726.9112587300189,
			"height": 33.27160298458912,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"roundness": null,
			"seed": 1199622500,
			"version": 253,
			"versionNonce": 1238684644,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230204622,
			"link": null,
			"locked": true,
			"points": [
				[
					0,
					0
				],
				[
					0.7233113122549534,
					0
				],
				[
					2.8931900660101384,
					0
				],
				[
					6.50966385276809,
					-0.7233389037600789
				],
				[
					9.402853918777076,
					-0.7233389037600789
				],
				[
					15.91249018004033,
					-1.4465674414990801
				],
				[
					20.252275279054384,
					-1.4465674414990801
				],
				[
					24.592032786562452,
					-2.169906345259447
				],
				[
					28.93179029407052,
					-2.8932452490198135
				],
				[
					36.16473786758873,
					-3.616473786758815
				],
				[
					48.4607542608688,
					-4.339812690518894
				],
				[
					56.417013146641956,
					-5.063041228257895
				],
				[
					64.37324444090913,
					-5.7863801320182615
				],
				[
					81.00901834169842,
					-6.5097190357786285
				],
				[
					91.13515598122446,
					-7.232947573517342
				],
				[
					102.70786106225073,
					-7.232947573517342
				],
				[
					115.72716117628093,
					-7.956286477277708
				],
				[
					126.57658253655708,
					-7.956286477277708
				],
				[
					140.31919396284337,
					-7.956286477277708
				],
				[
					159.1248466173867,
					-8.67951501501671
				],
				[
					174.3140530766769,
					-8.67951501501671
				],
				[
					187.33338078221195,
					-9.402853918777076
				],
				[
					209.75550722351437,
					-10.849421360276157
				],
				[
					223.49811864980066,
					-10.849421360276157
				],
				[
					239.410581238335,
					-11.572760264036523
				],
				[
					253.15319266462015,
					-12.296043984786063
				],
				[
					270.5122778776644,
					-13.019327705535892
				],
				[
					284.2548341209387,
					-14.465950330045798
				],
				[
					308.8468669075012,
					-15.912517771544879
				],
				[
					324.7593846790452,
					-16.63580149229442
				],
				[
					340.6718472675795,
					-18.082424116804326
				],
				[
					365.26388005414196,
					-20.252275279053233
				],
				[
					379.0064914804271,
					-20.975558999803063
				],
				[
					395.64223778971154,
					-22.42218162431297
				],
				[
					410.1081329367468,
					-23.145465345062508
				],
				[
					426.74393442904096,
					-23.868749065812047
				],
				[
					441.20982957607623,
					-25.315371690321957
				],
				[
					465.8018623626375,
					-26.761939131821322
				],
				[
					481.7143249511719,
					-27.485222852570864
				],
				[
					498.35012644346716,
					-28.208506573320403
				],
				[
					514.2625890320015,
					-28.93184547708077
				],
				[
					535.9614317525538,
					-29.65512919783031
				],
				[
					551.8738943410881,
					-30.37841291858014
				],
				[
					564.8932220466243,
					-31.101696639329678
				],
				[
					579.3591171936596,
					-31.824980360079216
				],
				[
					591.6551059954348,
					-32.54831926383959
				],
				[
					610.460813832989,
					-32.54831926383959
				],
				[
					627.0965601422723,
					-33.27160298458912
				],
				[
					636.4994140610494,
					-33.27160298458912
				],
				[
					648.0721743250864,
					-33.27160298458912
				],
				[
					656.0283504363427,
					-33.27160298458912
				],
				[
					663.9846369136208,
					-33.27160298458912
				],
				[
					674.1107193701372,
					-32.54831926383959
				],
				[
					699.4260358774486,
					-32.54831926383959
				],
				[
					707.3823223547265,
					-32.54831926383959
				],
				[
					716.0618373697426,
					-31.824980360079216
				],
				[
					719.6783111565018,
					-31.824980360079216
				],
				[
					723.2947849432609,
					-31.101696639329678
				],
				[
					724.74135238476,
					-30.37841291858014
				],
				[
					726.1879198262591,
					-30.37841291858014
				],
				[
					726.9112587300189,
					-29.65512919783031
				],
				[
					724.74135238476,
					-30.37841291858014
				],
				[
					724.74135238476,
					-30.37841291858014
				]
			],
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
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				572.5714329310831,
				-24.00002615792414
			]
		},
		{
			"id": "3xQbE4d5ogHNdjrh8xAxy",
			"type": "freedraw",
			"x": 7044.471926337978,
			"y": 625.2854954828591,
			"width": 8.679515015017286,
			"height": 49.907349293873075,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"roundness": null,
			"seed": 1009662308,
			"version": 246,
			"versionNonce": 159239260,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230204622,
			"link": null,
			"locked": true,
			"points": [
				[
					0,
					0
				],
				[
					0.7232837207501157,
					-3.616473786758815
				],
				[
					1.4465950330050692,
					-6.509663852767802
				],
				[
					2.1698787537540336,
					-10.849421360276157
				],
				[
					2.893162474504149,
					-15.189178867784511
				],
				[
					2.1698787537540336,
					-23.145410162051682
				],
				[
					2.1698787537540336,
					-26.761883948810567
				],
				[
					2.1698787537540336,
					-28.208506573320474
				],
				[
					1.4465950330050692,
					-26.038600228060883
				],
				[
					0.7232837207501157,
					-17.359085213044246
				],
				[
					-0.7233113122549534,
					-9.402853918777076
				],
				[
					-1.446595033003918,
					-4.339757507508355
				],
				[
					-2.1698787537540336,
					-0.7232837207495401
				],
				[
					-2.893190066008987,
					1.446567441499368
				],
				[
					-3.6164737867579513,
					2.8931900660092746
				],
				[
					-3.6164737867579513,
					2.1699063452597347
				],
				[
					-2.893190066008987,
					-1.4465674414990801
				],
				[
					-0.7233113122549534,
					-7.95623129426717
				],
				[
					0.7232837207501157,
					-15.91246258853434
				],
				[
					2.1698787537540336,
					-23.868749065812047
				],
				[
					2.893162474504149,
					-29.6550740148197
				],
				[
					2.893162474504149,
					-32.54826408082883
				],
				[
					2.893162474504149,
					-28.208506573320474
				],
				[
					1.4465950330050692,
					-17.359085213044246
				],
				[
					0.7232837207501157,
					-10.849421360276157
				],
				[
					-0.7233113122549534,
					-4.339757507508355
				],
				[
					-2.893190066008987,
					5.7863801320182615
				],
				[
					-3.6164737867579513,
					10.126137639526904
				],
				[
					-4.3397850990129045,
					8.679515015016998
				],
				[
					-3.6164737867579513,
					1.446567441499368
				],
				[
					-2.893190066008987,
					-4.339757507508355
				],
				[
					-2.1698787537540336,
					-11.572705081025985
				],
				[
					-1.446595033003918,
					-22.42212644130214
				],
				[
					-1.446595033003918,
					-27.48522285257079
				],
				[
					-1.446595033003918,
					-28.208506573320474
				],
				[
					-1.446595033003918,
					-26.761883948810567
				],
				[
					-2.1698787537540336,
					-18.805652654543326
				],
				[
					-2.893190066008987,
					-5.063041228257895
				],
				[
					-4.3397850990129045,
					5.063041228258183
				],
				[
					-5.0630688197630205,
					12.295988801775525
				],
				[
					-5.786352540513136,
					16.63574630928417
				],
				[
					-5.786352540513136,
					17.359085213044246
				],
				[
					-5.786352540513136,
					16.63574630928417
				],
				[
					-5.786352540513136,
					8.679515015016998
				],
				[
					-5.0630688197630205,
					-0.7232837207495401
				],
				[
					-3.6164737867579513,
					-8.67951501501671
				],
				[
					-2.893190066008987,
					-20.252275279053233
				],
				[
					-2.893190066008987,
					-22.42212644130214
				],
				[
					-2.893190066008987,
					-18.082368933793788
				],
				[
					-3.6164737867579513,
					-12.295988801775525
				],
				[
					-3.6164737867579513,
					-4.339757507508355
				],
				[
					-3.6164737867579513,
					-2.169906345259447
				],
				[
					-3.6164737867579513,
					2.1699063452597347
				],
				[
					-3.6164737867579513,
					2.8931900660092746
				],
				[
					0,
					0
				]
			],
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
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				-2.8571428571422075,
				2.285723005022419
			]
		},
		{
			"id": "-fVB2RQtKx73ZwQaKfMfj",
			"type": "freedraw",
			"x": 7105.2286694006225,
			"y": 334.52102510065777,
			"width": 7.956258885772008,
			"height": 311.7400845650149,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"roundness": null,
			"seed": 1059871964,
			"version": 238,
			"versionNonce": 794343268,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230204622,
			"link": null,
			"locked": true,
			"points": [
				[
					0,
					0
				],
				[
					0.7233113122549534,
					-1.4466226245099068
				],
				[
					0.7233113122549534,
					-0.7233389037602947
				],
				[
					0,
					7.232947573517558
				],
				[
					0,
					12.295988801775525
				],
				[
					0,
					20.252220096042695
				],
				[
					0,
					25.315316507311415
				],
				[
					0,
					34.71811524307781
				],
				[
					-0.7232837207489645,
					44.12096916185489
				],
				[
					-1.4465674414990801,
					60.03343175038923
				],
				[
					-1.4465674414990801,
					70.15956938991592
				],
				[
					-1.4465674414990801,
					81.7322744709419
				],
				[
					-1.4465674414990801,
					99.81464340473576
				],
				[
					-1.4465674414990801,
					113.55725483102118
				],
				[
					-1.4465674414990801,
					128.0231499780563
				],
				[
					-2.1698787537540336,
					148.27542525710967
				],
				[
					-2.1698787537540336,
					160.57141405888527
				],
				[
					-2.1698787537540336,
					172.8674028606609
				],
				[
					-2.893162474502998,
					185.88673056619663
				],
				[
					-2.893162474502998,
					196.73615192647307
				],
				[
					-2.893162474502998,
					210.4787633527585
				],
				[
					-2.893162474502998,
					222.0514684337845
				],
				[
					-3.6164737867579513,
					238.68726992607904
				],
				[
					-3.6164737867579513,
					247.3667849410959
				],
				[
					-3.6164737867579513,
					253.8764487938637
				],
				[
					-3.6164737867579513,
					263.27924752963025
				],
				[
					-4.339757507508067,
					278.46848158042553
				],
				[
					-5.063041228257031,
					285.70142915394314
				],
				[
					-5.063041228257031,
					288.59456403694156
				],
				[
					-5.786352540511985,
					292.93437672746074
				],
				[
					-5.786352540511985,
					295.8275116104592
				],
				[
					-5.786352540511985,
					297.9974179557187
				],
				[
					-5.786352540511985,
					300.8906080217279
				],
				[
					-5.786352540511985,
					303.06045918397655
				],
				[
					-5.786352540511985,
					304.5070818084865
				],
				[
					-5.786352540511985,
					306.6769881537462
				],
				[
					-5.786352540511985,
					307.4002166914852
				],
				[
					-5.786352540511985,
					308.12355559524525
				],
				[
					-5.786352540511985,
					309.57012303674463
				],
				[
					-5.786352540511985,
					310.293461940505
				],
				[
					-6.5096362612621,
					309.57012303674463
				],
				[
					-6.5096362612621,
					308.84689449900566
				],
				[
					-6.5096362612621,
					307.4002166914852
				],
				[
					-6.5096362612621,
					305.2303655292363
				],
				[
					-6.5096362612621,
					300.8906080217279
				],
				[
					-7.2329475735170545,
					293.6576604482103
				],
				[
					-7.2329475735170545,
					292.2110378237004
				],
				[
					-7.2329475735170545,
					292.2110378237004
				]
			],
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
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				-5.7142857142853245,
				230.85710797991072
			]
		},
		{
			"id": "k4Nk0VBIMYB2CEYgHDHEY",
			"type": "freedraw",
			"x": 7101.612195613865,
			"y": 346.0937301816837,
			"width": 2.893190066008987,
			"height": 287.87133549920264,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"roundness": null,
			"seed": 1624048356,
			"version": 239,
			"versionNonce": 423354588,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230204622,
			"link": null,
			"locked": true,
			"points": [
				[
					0,
					0
				],
				[
					-0.7232837207501157,
					-1.4466226245099068
				],
				[
					-0.7232837207501157,
					-0.723283720749612
				],
				[
					-0.7232837207501157,
					3.616473786758815
				],
				[
					-0.7232837207501157,
					10.849421360276372
				],
				[
					-0.7232837207501157,
					17.359085213044246
				],
				[
					-0.7232837207501157,
					27.485167669560322
				],
				[
					-0.7232837207501157,
					33.9948315223282
				],
				[
					0,
					43.397685441105274
				],
				[
					0,
					52.07720045612213
				],
				[
					0,
					60.75677065414952
				],
				[
					0,
					70.8828531106656
				],
				[
					0.7233113122549534,
					80.28570702944268
				],
				[
					0.7233113122549534,
					92.5816958312182
				],
				[
					0.7233113122549534,
					101.98454974999528
				],
				[
					1.446595033003918,
					110.66406476501206
				],
				[
					1.446595033003918,
					118.62035124228991
				],
				[
					1.446595033003918,
					130.91634004406552
				],
				[
					1.446595033003918,
					139.59585505908228
				],
				[
					1.446595033003918,
					146.82880263259986
				],
				[
					1.446595033003918,
					154.78508910987762
				],
				[
					2.1699063452588714,
					164.1878878456441
				],
				[
					2.1699063452588714,
					175.76059292667009
				],
				[
					2.1699063452588714,
					182.99354050018758
				],
				[
					2.1699063452588714,
					190.94982697746542
				],
				[
					2.1699063452588714,
					198.90605827173258
				],
				[
					1.446595033003918,
					208.30885700749897
				],
				[
					1.446595033003918,
					215.54180458101646
				],
				[
					1.446595033003918,
					222.0514684337844
				],
				[
					1.446595033003918,
					228.56113228655235
				],
				[
					0.7233113122549534,
					235.0707961393203
				],
				[
					0.7233113122549534,
					241.58045999208824
				],
				[
					0,
					245.92021749959662
				],
				[
					0,
					250.25997500710497
				],
				[
					0,
					254.59973251461346
				],
				[
					0,
					261.10939636738135
				],
				[
					0,
					264.7258701541401
				],
				[
					0,
					267.61906022014915
				],
				[
					0,
					270.5122502861584
				],
				[
					0,
					272.6821014484073
				],
				[
					0,
					275.5752915144163
				],
				[
					0,
					277.745197859676
				],
				[
					0,
					279.915049021925
				],
				[
					0,
					281.36167164643484
				],
				[
					0,
					282.0849553671844
				],
				[
					0.7233113122549534,
					282.80823908793394
				],
				[
					0.7233113122549534,
					284.2548065294333
				],
				[
					0.7233113122549534,
					286.4247128746928
				],
				[
					0.7233113122549534,
					286.4247128746928
				]
			],
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
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				0.571441650390625,
				226.28570556640625
			]
		},
		{
			"id": "wCPURhtYGwsNY_g_061Qa",
			"type": "freedraw",
			"x": 7163.8155613010185,
			"y": 405.40387821132333,
			"width": 2.893190066008987,
			"height": 212.64866969801815,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"roundness": null,
			"seed": 1488460388,
			"version": 231,
			"versionNonce": 294922980,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230204622,
			"link": null,
			"locked": true,
			"points": [
				[
					0,
					0
				],
				[
					0.7232837207489645,
					0.723283720749684
				],
				[
					0.7232837207489645,
					1.4466226245099068
				],
				[
					0.7232837207489645,
					4.339757507508427
				],
				[
					0.7232837207489645,
					7.232947573517558
				],
				[
					0.7232837207489645,
					13.019327705535892
				],
				[
					0.7232837207489645,
					19.528991558303836
				],
				[
					0.7232837207489645,
					24.592032786561806
				],
				[
					0.7232837207489645,
					32.54826408082897
				],
				[
					0.7232837207489645,
					39.05792793359692
				],
				[
					1.4465674414990801,
					47.01415922786409
				],
				[
					1.4465674414990801,
					54.97039052213126
				],
				[
					1.4465674414990801,
					61.480054374899204
				],
				[
					1.4465674414990801,
					73.7760983596854
				],
				[
					2.1699063452588714,
					82.4556133747022
				],
				[
					2.1699063452588714,
					89.68856094821975
				],
				[
					2.1699063452588714,
					97.64479224248691
				],
				[
					2.1699063452588714,
					107.7709298820136
				],
				[
					2.1699063452588714,
					116.45044489703047
				],
				[
					2.1699063452588714,
					128.74648888181667
				],
				[
					2.1699063452588714,
					137.42600389683338
				],
				[
					2.1699063452588714,
					145.38223519110056
				],
				[
					2.1699063452588714,
					152.61518276461817
				],
				[
					2.1699063452588714,
					160.57146924189604
				],
				[
					2.1699063452588714,
					169.97426797766244
				],
				[
					2.1699063452588714,
					175.7606481096807
				],
				[
					2.1699063452588714,
					180.10040561718904
				],
				[
					2.1699063452588714,
					184.44016312469753
				],
				[
					2.1699063452588714,
					188.05663691145622
				],
				[
					2.1699063452588714,
					191.67311069821503
				],
				[
					1.4465674414990801,
					195.28958448497383
				],
				[
					1.4465674414990801,
					200.35268089624236
				],
				[
					1.4465674414990801,
					202.52253205849127
				],
				[
					1.4465674414990801,
					203.96915468300116
				],
				[
					1.4465674414990801,
					205.41572212450052
				],
				[
					2.1699063452588714,
					209.03219591125935
				],
				[
					2.1699063452588714,
					211.2021022565188
				],
				[
					2.1699063452588714,
					211.92538597726832
				],
				[
					2.1699063452588714,
					212.64866969801815
				],
				[
					2.893190066008987,
					212.64866969801815
				],
				[
					2.893190066008987,
					212.64866969801815
				]
			],
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
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				2.2857230050221915,
				168.00000871930814
			]
		},
		{
			"id": "TzBskays86CLJsdsA1oIM",
			"type": "freedraw",
			"x": 7163.092277580268,
			"y": 423.48624714511726,
			"width": 3.616473786759103,
			"height": 219.88156208852496,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"roundness": null,
			"seed": 390124516,
			"version": 231,
			"versionNonce": 558064988,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230204622,
			"link": null,
			"locked": true,
			"points": [
				[
					0,
					0
				],
				[
					-1.4466226245099068,
					-7.232947573517558
				],
				[
					-1.4466226245099068,
					-8.679515015016854
				],
				[
					-1.4466226245099068,
					-10.849421360276372
				],
				[
					-1.4466226245099068,
					-13.019272522525208
				],
				[
					-1.4466226245099068,
					-12.295988801775596
				],
				[
					-1.4466226245099068,
					-5.063041228258039
				],
				[
					-0.7232837207489645,
					4.339757507508355
				],
				[
					0,
					15.189178867784655
				],
				[
					0,
					23.86874906581212
				],
				[
					0.7232837207501157,
					33.271547801578514
				],
				[
					0.7232837207501157,
					41.95111799960598
				],
				[
					0.7232837207501157,
					51.353916735372444
				],
				[
					0.7232837207501157,
					61.48005437489913
				],
				[
					0.7232837207501157,
					74.49938208043496
				],
				[
					0.7232837207501157,
					82.4556133747022
				],
				[
					0.7232837207501157,
					86.79537088221055
				],
				[
					0.7232837207501157,
					95.47494108023794
				],
				[
					0.7232837207501157,
					102.70788865375557
				],
				[
					0.7232837207501157,
					109.94083622727305
				],
				[
					0.7232837207501157,
					122.96010874979827
				],
				[
					0.7232837207501157,
					130.91634004406544
				],
				[
					0.7232837207501157,
					137.42600389683338
				],
				[
					0,
					144.65895147035087
				],
				[
					0,
					152.61518276461803
				],
				[
					0.7232837207501157,
					162.7413204041448
				],
				[
					0.7232837207501157,
					168.52770053616305
				],
				[
					0.7232837207501157,
					170.69755169841196
				],
				[
					0.7232837207501157,
					182.27031196244843
				],
				[
					0.7232837207501157,
					187.3333531907066
				],
				[
					1.4465674414990801,
					190.94982697746542
				],
				[
					1.4465674414990801,
					194.56630076422422
				],
				[
					1.4465674414990801,
					198.18277455098277
				],
				[
					1.4465674414990801,
					201.07596461699202
				],
				[
					1.4465674414990801,
					203.24581577924093
				],
				[
					2.169851162249196,
					204.69243840375086
				],
				[
					2.169851162249196,
					205.41572212450038
				],
				[
					2.169851162249196,
					206.13900584524993
				],
				[
					2.169851162249196,
					206.86228956599976
				],
				[
					2.169851162249196,
					206.13900584524993
				],
				[
					2.169851162249196,
					206.13900584524993
				]
			],
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
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				1.714259556361867,
				162.85714285714272
			]
		},
		{
			"id": "K4bMImxqNMlPtvNQAP58f",
			"type": "freedraw",
			"x": 7227.465522021178,
			"y": 549.3395459609246,
			"width": 4.339812690520045,
			"height": 100.53798230849605,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"roundness": null,
			"seed": 1914871140,
			"version": 219,
			"versionNonce": 320155236,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230204622,
			"link": null,
			"locked": true,
			"points": [
				[
					0,
					0
				],
				[
					0,
					2.169906345259591
				],
				[
					0,
					5.7863801320182615
				],
				[
					0,
					8.679515015016854
				],
				[
					0,
					10.12613763952676
				],
				[
					-0.7233389037609423,
					15.91246258853434
				],
				[
					-0.7233389037609423,
					21.6988427205526
				],
				[
					-1.4466226245099068,
					28.20850657332055
				],
				[
					-2.1699063452600225,
					34.71817042608849
				],
				[
					-2.1699063452600225,
					40.50449537509621
				],
				[
					-2.8931900660101384,
					48.46072666936339
				],
				[
					-2.8931900660101384,
					56.417013146641025
				],
				[
					-2.8931900660101384,
					61.480054374899204
				],
				[
					-3.616473786759103,
					65.81981188240756
				],
				[
					-3.616473786759103,
					67.26643450691746
				],
				[
					-3.616473786759103,
					70.88290829367628
				],
				[
					-3.616473786759103,
					75.22266580118463
				],
				[
					-3.616473786759103,
					78.83913958794345
				],
				[
					-3.616473786759103,
					82.45561337470227
				],
				[
					-4.339812690520045,
					85.34880344071125
				],
				[
					-4.339812690520045,
					88.2419383237097
				],
				[
					-4.339812690520045,
					92.58169583121834
				],
				[
					-4.339812690520045,
					95.47494108023815
				],
				[
					-4.339812690520045,
					98.3680759632366
				],
				[
					-4.339812690520045,
					99.81464340473569
				],
				[
					-4.339812690520045,
					100.53798230849605
				],
				[
					-3.616473786759103,
					99.81464340473569
				],
				[
					-2.1699063452600225,
					97.6448474254976
				],
				[
					-2.1699063452600225,
					97.6448474254976
				]
			],
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
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				-1.7143031529021755,
				77.14290073939736
			]
		},
		{
			"id": "gc_0qmj9kvewxcrxC4ZH5",
			"type": "freedraw",
			"x": 7226.742183117417,
			"y": 558.0190609759414,
			"width": 4.339757507508067,
			"height": 79.56242330869298,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"roundness": null,
			"seed": 406925796,
			"version": 209,
			"versionNonce": 921065948,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230204622,
			"link": null,
			"locked": true,
			"points": [
				[
					0,
					0
				],
				[
					-0.7232837207489645,
					-0.723283720749684
				],
				[
					-0.7232837207489645,
					0.7233389037602228
				],
				[
					-0.7232837207489645,
					6.509663852767946
				],
				[
					-0.7232837207489645,
					16.63580149229456
				],
				[
					0,
					23.868749065812192
				],
				[
					-0.7232837207489645,
					33.99488670533881
				],
				[
					-1.4465674414990801,
					41.22783427885644
				],
				[
					-2.169851162249196,
					50.6306330146229
				],
				[
					-2.8931348829981602,
					55.69372942589134
				],
				[
					-3.616473786759103,
					59.31020321265015
				],
				[
					-4.339757507508067,
					62.92667699940897
				],
				[
					-4.339757507508067,
					64.37324444090834
				],
				[
					-4.339757507508067,
					66.54315078616779
				],
				[
					-4.339757507508067,
					68.71300194841669
				],
				[
					-3.616473786759103,
					70.88290829367614
				],
				[
					-3.616473786759103,
					73.05281463893559
				],
				[
					-2.8931348829981602,
					78.83913958794331
				],
				[
					-2.8931348829981602,
					78.83913958794331
				]
			],
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
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				-2.285679408481883,
				62.28572300502225
			]
		},
		{
			"id": "5vHTD-HlibR5uidfXoSMT",
			"type": "freedraw",
			"x": 7298.348375131843,
			"y": 445.18508986566985,
			"width": 5.786324949008298,
			"height": 177.93049927192953,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"roundness": null,
			"seed": 410969316,
			"version": 225,
			"versionNonce": 1420411364,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230204622,
			"link": null,
			"locked": true,
			"points": [
				[
					0,
					0
				],
				[
					0,
					0.723283720749612
				],
				[
					0,
					2.169906345259519
				],
				[
					0,
					5.7863801320183335
				],
				[
					0,
					11.572705081025912
				],
				[
					-0.7232837207501157,
					15.189178867784728
				],
				[
					-0.7232837207501157,
					20.25227527905338
				],
				[
					-0.7232837207501157,
					26.03860022806103
				],
				[
					-0.7232837207501157,
					29.655074014819842
				],
				[
					-0.7232837207501157,
					39.781211654346535
				],
				[
					-1.4465674414990801,
					44.84430806561518
				],
				[
					-1.4465674414990801,
					50.63063301462283
				],
				[
					-1.4465674414990801,
					56.41701314664117
				],
				[
					-2.169851162249196,
					62.92667699940904
				],
				[
					-2.169851162249196,
					70.88290829367621
				],
				[
					-2.893190066008987,
					80.2857070294426
				],
				[
					-3.616473786759103,
					85.34880344071132
				],
				[
					-3.616473786759103,
					91.85846729347926
				],
				[
					-3.616473786759103,
					99.09141486699676
				],
				[
					-3.616473786759103,
					105.60102353675401
				],
				[
					-4.339757507509218,
					113.55731001403187
				],
				[
					-5.063041228258183,
					118.62035124228991
				],
				[
					-5.063041228258183,
					127.29986625730676
				],
				[
					-5.063041228258183,
					133.08624638932503
				],
				[
					-5.063041228258183,
					137.42600389683338
				],
				[
					-5.063041228258183,
					141.76576140434173
				],
				[
					-5.063041228258183,
					147.55214153636015
				],
				[
					-5.063041228258183,
					151.16861532311881
				],
				[
					-5.786324949008298,
					163.46460412489455
				],
				[
					-5.786324949008298,
					172.86745804367163
				],
				[
					-5.786324949008298,
					173.59074176442118
				],
				[
					-5.786324949008298,
					175.03736438893108
				],
				[
					-5.063041228258183,
					176.48393183043015
				],
				[
					-5.063041228258183,
					177.93049927192953
				],
				[
					-5.063041228258183,
					177.93049927192953
				]
			],
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
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				-3.9999825613840585,
				140.57141985212053
			]
		},
		{
			"id": "f-hRZXoeWABoY9ziH6kyJ",
			"type": "freedraw",
			"x": 7294.731901345083,
			"y": 453.14132115993704,
			"width": 5.786324949008298,
			"height": 190.22654325671581,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"roundness": null,
			"seed": 541570020,
			"version": 232,
			"versionNonce": 1966521948,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230204622,
			"link": null,
			"locked": true,
			"points": [
				[
					0,
					0
				],
				[
					0.7232837207501157,
					-2.169851162248836
				],
				[
					0.7232837207501157,
					-1.446567441499224
				],
				[
					0.7232837207501157,
					-0.723283720749612
				],
				[
					0,
					5.7863801320183335
				],
				[
					0,
					10.12613763952669
				],
				[
					0,
					15.912517771545023
				],
				[
					0,
					27.485222852570935
				],
				[
					-0.7232837207501157,
					36.16473786758772
				],
				[
					-2.169851162249196,
					47.737498131624314
				],
				[
					-2.893190066008987,
					56.4170131466411
				],
				[
					-3.616473786759103,
					63.649960720158724
				],
				[
					-3.616473786759103,
					73.0528146389358
				],
				[
					-3.616473786759103,
					78.11585586719384
				],
				[
					-3.616473786759103,
					86.07208716146101
				],
				[
					-4.339757507508067,
					91.85846729347926
				],
				[
					-4.339757507508067,
					96.92150852173731
				],
				[
					-4.339757507508067,
					104.1544560952548
				],
				[
					-4.339757507508067,
					108.49421360276315
				],
				[
					-4.339757507508067,
					115.0038774555311
				],
				[
					-4.339757507508067,
					120.7902575875495
				],
				[
					-5.063041228258183,
					125.85329881580739
				],
				[
					-5.063041228258183,
					130.1930563233159
				],
				[
					-5.063041228258183,
					133.80953011007458
				],
				[
					-5.063041228258183,
					137.42600389683338
				],
				[
					-4.339757507508067,
					141.0424776835922
				],
				[
					-4.339757507508067,
					146.82885781561046
				],
				[
					-4.339757507508067,
					153.33852166837846
				],
				[
					-4.339757507508067,
					156.9549954551373
				],
				[
					-4.339757507508067,
					159.8481855211463
				],
				[
					-4.339757507508067,
					164.18794302865464
				],
				[
					-4.339757507508067,
					167.0811330946639
				],
				[
					-4.339757507508067,
					169.97426797766235
				],
				[
					-4.339757507508067,
					172.1441743229218
				],
				[
					-4.339757507508067,
					174.31408066818153
				],
				[
					-4.339757507508067,
					176.48393183043015
				],
				[
					-4.339757507508067,
					177.93055445494005
				],
				[
					-3.616473786759103,
					181.54702824169888
				],
				[
					-3.616473786759103,
					184.44016312469734
				],
				[
					-3.616473786759103,
					185.88678574920723
				],
				[
					-3.616473786759103,
					188.05669209446697
				],
				[
					-3.616473786759103,
					188.05669209446697
				]
			],
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
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				-2.857142857143117,
				148.5714721679688
			]
		},
		{
			"id": "D1s0VFjEnicBEfYFdginh",
			"type": "freedraw",
			"x": 7357.6585783444925,
			"y": 473.39359643899036,
			"width": 5.786324949008298,
			"height": 159.12484661738605,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"roundness": null,
			"seed": 1871608540,
			"version": 223,
			"versionNonce": 761259364,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230204622,
			"link": null,
			"locked": true,
			"points": [
				[
					0,
					0
				],
				[
					0.7232837207501157,
					0.723283720749612
				],
				[
					1.4465674414990801,
					10.12613763952669
				],
				[
					2.169851162249196,
					16.635801492294636
				],
				[
					2.169851162249196,
					23.1454101620519
				],
				[
					2.169851162249196,
					28.931790294070233
				],
				[
					2.169851162249196,
					35.441454146838176
				],
				[
					1.4465674414990801,
					42.67440172035566
				],
				[
					1.4465674414990801,
					48.46072666936339
				],
				[
					0.7232837207501157,
					55.693674242880874
				],
				[
					0,
					61.48005437489913
				],
				[
					0,
					68.71300194841676
				],
				[
					0,
					74.49938208043503
				],
				[
					0,
					81.7323296539525
				],
				[
					0,
					88.24193832370977
				],
				[
					0,
					94.02831845572818
				],
				[
					0,
					100.53798230849613
				],
				[
					0,
					106.3243072575037
				],
				[
					0,
					112.83397111027165
				],
				[
					-0.7233389037597912,
					118.62035124228991
				],
				[
					-0.7233389037597912,
					122.96010874979827
				],
				[
					-1.4466226245099068,
					128.74648888181673
				],
				[
					-1.4466226245099068,
					134.53281383082418
				],
				[
					-2.1699063452588714,
					143.21238402885172
				],
				[
					-2.1699063452588714,
					144.65895147035107
				],
				[
					-2.1699063452588714,
					146.82885781561052
				],
				[
					-2.893190066008987,
					148.27542525710962
				],
				[
					-2.893190066008987,
					151.89189904386842
				],
				[
					-2.893190066008987,
					154.06180538912815
				],
				[
					-3.616473786759103,
					156.23165655137677
				],
				[
					-3.616473786759103,
					159.12484661738605
				],
				[
					-2.893190066008987,
					152.61518276461825
				],
				[
					-2.893190066008987,
					152.61518276461825
				]
			],
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
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				-2.2857230050221915,
				120.57141985212064
			]
		},
		{
			"id": "aXRL8wJmNfn05Qds5Wu_W",
			"type": "freedraw",
			"x": 7354.042104557733,
			"y": 485.689585240766,
			"width": 7.2329475735170545,
			"height": 149.72199269860906,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"roundness": null,
			"seed": 1729791836,
			"version": 220,
			"versionNonce": 1158058716,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230204622,
			"link": null,
			"locked": true,
			"points": [
				[
					0,
					0
				],
				[
					2.169851162249196,
					-4.339757507508427
				],
				[
					2.169851162249196,
					-5.063041228258039
				],
				[
					2.8931348829993113,
					-4.339757507508427
				],
				[
					3.616473786759103,
					2.169906345259519
				],
				[
					4.339757507509218,
					12.296043984786207
				],
				[
					5.063041228258183,
					22.422181624312895
				],
				[
					5.063041228258183,
					30.378412918580064
				],
				[
					4.339757507509218,
					41.95111799960605
				],
				[
					3.616473786759103,
					50.63063301462276
				],
				[
					2.8931348829993113,
					60.033486933399836
				],
				[
					2.169851162249196,
					67.26643450691746
				],
				[
					2.169851162249196,
					73.7760983596854
				],
				[
					2.169851162249196,
					83.90223599921202
				],
				[
					1.4465674415002314,
					91.8584672934792
				],
				[
					1.4465674415002314,
					97.64479224248691
				],
				[
					0.7232837207501157,
					104.87773981600441
				],
				[
					0.7232837207501157,
					109.21755250652345
				],
				[
					0,
					114.28059373478149
				],
				[
					0,
					119.34363496303959
				],
				[
					-0.7233389037597912,
					125.85329881580739
				],
				[
					-1.4466226245099068,
					129.46977260256622
				],
				[
					-1.4466226245099068,
					133.80953011007458
				],
				[
					-1.4466226245099068,
					135.97943645533402
				],
				[
					-2.1699063452588714,
					141.0424776835922
				],
				[
					-2.1699063452588714,
					142.4891003081021
				],
				[
					-2.1699063452588714,
					143.21238402885163
				],
				[
					-2.1699063452588714,
					143.93566774960118
				],
				[
					-2.1699063452588714,
					144.658951470351
				],
				[
					-2.1699063452588714,
					144.658951470351
				]
			],
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
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				-1.714303152901266,
				114.28571428571433
			]
		},
		{
			"id": "kDUI3J6KIW4rszWt3aN1u",
			"type": "freedraw",
			"x": 7417.692010094882,
			"y": 335.2443088214074,
			"width": 6.50966385276809,
			"height": 288.59456403694156,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"roundness": null,
			"seed": 620071260,
			"version": 239,
			"versionNonce": 1652922596,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230204622,
			"link": null,
			"locked": true,
			"points": [
				[
					0,
					0
				],
				[
					0.7232837207501157,
					-0.723283720749612
				],
				[
					0.7232837207501157,
					0.723283720749612
				],
				[
					0.7232837207501157,
					6.509663852767946
				],
				[
					1.4466226245099068,
					11.572705081025912
				],
				[
					2.1699063452600225,
					19.528936375293082
				],
				[
					2.893190066008987,
					29.655074014819842
				],
				[
					2.893190066008987,
					39.781211654346535
				],
				[
					2.893190066008987,
					43.397685441105274
				],
				[
					3.616473786759103,
					52.07720045612206
				],
				[
					3.616473786759103,
					60.75677065414952
				],
				[
					4.339757507509218,
					68.71300194841669
				],
				[
					4.339757507509218,
					78.83913958794338
				],
				[
					4.339757507509218,
					88.96522204445945
				],
				[
					5.06309641126901,
					103.4311171914945
				],
				[
					5.06309641126901,
					113.55725483102127
				],
				[
					5.06309641126901,
					122.96010874979827
				],
				[
					5.786380132019125,
					135.97938127232348
				],
				[
					5.786380132019125,
					146.10551891185017
				],
				[
					5.786380132019125,
					159.12484661738605
				],
				[
					6.50966385276809,
					167.80436163240284
				],
				[
					6.50966385276809,
					177.20721555117984
				],
				[
					6.50966385276809,
					185.163446845447
				],
				[
					6.50966385276809,
					192.39639441896463
				],
				[
					5.786380132019125,
					200.35262571323182
				],
				[
					5.786380132019125,
					211.9253307942578
				],
				[
					5.786380132019125,
					218.4349946470256
				],
				[
					5.786380132019125,
					223.4980910582943
				],
				[
					5.06309641126901,
					232.17760607331118
				],
				[
					5.06309641126901,
					237.96398620532943
				],
				[
					5.06309641126901,
					243.02702743358748
				],
				[
					5.06309641126901,
					250.25997500710497
				],
				[
					4.339757507509218,
					253.87644879386377
				],
				[
					4.339757507509218,
					256.7696388598729
				],
				[
					4.339757507509218,
					261.10939636738124
				],
				[
					4.339757507509218,
					265.44915387488976
				],
				[
					4.339757507509218,
					271.2355340069081
				],
				[
					4.339757507509218,
					274.12872407291707
				],
				[
					4.339757507509218,
					275.57529151441645
				],
				[
					5.06309641126901,
					277.7451978596759
				],
				[
					5.06309641126901,
					279.1917653011753
				],
				[
					5.06309641126901,
					280.6383327426743
				],
				[
					5.06309641126901,
					281.36167164643473
				],
				[
					5.786380132019125,
					282.08495536718425
				],
				[
					5.786380132019125,
					284.25480652943315
				],
				[
					6.50966385276809,
					285.7014291539431
				],
				[
					6.50966385276809,
					287.1479965954424
				],
				[
					6.50966385276809,
					287.871280316192
				],
				[
					6.50966385276809,
					287.871280316192
				]
			],
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
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				5.1428658621653085,
				227.4285452706473
			]
		},
		{
			"id": "SVtIHXZSlj8YpPIJjwMzR",
			"type": "freedraw",
			"x": 7484.9584446018,
			"y": 494.3691554387934,
			"width": 2.8931348829981602,
			"height": 120.79020240453875,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"roundness": null,
			"seed": 1321609692,
			"version": 221,
			"versionNonce": 619173724,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230204622,
			"link": null,
			"locked": true,
			"points": [
				[
					0,
					0
				],
				[
					0,
					2.169851162248836
				],
				[
					0.7232837207489645,
					7.232947573517558
				],
				[
					1.4465674414990801,
					13.019272522525208
				],
				[
					1.4465674414990801,
					15.91246258853434
				],
				[
					1.4465674414990801,
					21.6988427205526
				],
				[
					1.4465674414990801,
					27.485167669560322
				],
				[
					1.4465674414990801,
					35.44145414683803
				],
				[
					1.4465674414990801,
					41.227779095845754
				],
				[
					1.4465674414990801,
					48.46072666936324
				],
				[
					1.4465674414990801,
					57.14029686739078
				],
				[
					1.4465674414990801,
					62.20333809564882
				],
				[
					2.1698511622480448,
					68.71300194841662
				],
				[
					2.1698511622480448,
					74.49932689742434
				],
				[
					1.4465674414990801,
					80.2857070294426
				],
				[
					1.4465674414990801,
					87.51865460296024
				],
				[
					1.4465674414990801,
					91.1351283897189
				],
				[
					1.4465674414990801,
					94.75160217647772
				],
				[
					1.4465674414990801,
					97.64479224248684
				],
				[
					0.7232837207489645,
					101.26126602924566
				],
				[
					0.7232837207489645,
					105.60102353675401
				],
				[
					0.7232837207489645,
					109.21749732351276
				],
				[
					0,
					109.94078104426231
				],
				[
					0.7232837207489645,
					112.11068738952204
				],
				[
					0,
					114.28053855177095
				],
				[
					0,
					117.17372861777993
				],
				[
					0,
					118.62035124228984
				],
				[
					-0.7232837207501157,
					119.34363496303938
				],
				[
					-0.7232837207501157,
					120.06691868378921
				],
				[
					-0.7232837207501157,
					120.79020240453875
				],
				[
					-0.7232837207501157,
					120.79020240453875
				]
			],
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
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				-0.5714198521209255,
				95.42855398995533
			]
		},
		{
			"id": "HZQ5J_px-ee0KOkn09uSm",
			"type": "freedraw",
			"x": 7481.34197081504,
			"y": 498.7089129463018,
			"width": 4.339757507508067,
			"height": 112.11068738952204,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"roundness": null,
			"seed": 642314716,
			"version": 210,
			"versionNonce": 1604901988,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230204622,
			"link": null,
			"locked": true,
			"points": [
				[
					0,
					0
				],
				[
					0,
					3.616473786758815
				],
				[
					2.169851162249196,
					15.91246258853434
				],
				[
					2.893190066008987,
					26.0386002280611
				],
				[
					3.616473786759103,
					33.99483152232827
				],
				[
					4.339757507508067,
					44.12096916185489
				],
				[
					4.339757507508067,
					56.4170131466411
				],
				[
					2.893190066008987,
					67.98971822766708
				],
				[
					2.893190066008987,
					76.66923324268393
				],
				[
					2.893190066008987,
					82.4556133747022
				],
				[
					2.893190066008987,
					87.51865460296024
				],
				[
					3.616473786759103,
					94.02831845572818
				],
				[
					3.616473786759103,
					98.36807596323654
				],
				[
					3.616473786759103,
					101.26126602924566
				],
				[
					3.616473786759103,
					104.87773981600441
				],
				[
					3.616473786759103,
					106.32430725750378
				],
				[
					3.616473786759103,
					107.77092988201368
				],
				[
					4.339757507508067,
					109.21749732351276
				],
				[
					4.339757507508067,
					112.11068738952204
				],
				[
					4.339757507508067,
					112.11068738952204
				]
			],
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
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				3.428562709263133,
				88.57142857142861
			]
		},
		{
			"id": "kh7_xJ9LXzMyUgGgoVKI0",
			"type": "freedraw",
			"x": 7538.4822676824315,
			"y": 364.89938283622723,
			"width": 0.7232837207489645,
			"height": 0.723283720749684,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"roundness": null,
			"seed": 1059347684,
			"version": 194,
			"versionNonce": 1898744796,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230204622,
			"link": null,
			"locked": true,
			"points": [
				[
					0,
					0
				],
				[
					0.7232837207489645,
					-0.723283720749684
				],
				[
					0,
					0
				]
			],
			"pressures": [
				0.1015625,
				0.0185546875,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				0.571419852120016,
				-0.5714198521205844
			]
		},
		{
			"id": "RcZmvPikcr5pMrtBRTG22",
			"type": "freedraw",
			"x": 7540.65211884468,
			"y": 362.00619277021804,
			"width": 1.4465674414990801,
			"height": 264.0025864333906,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"roundness": null,
			"seed": 1138175068,
			"version": 228,
			"versionNonce": 1855434724,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230204622,
			"link": null,
			"locked": true,
			"points": [
				[
					0,
					0
				],
				[
					-0.7232837207501157,
					0.723283720749612
				],
				[
					0,
					2.169906345259519
				],
				[
					0,
					5.063096411268722
				],
				[
					0,
					9.402853918777076
				],
				[
					0,
					18.08236893379386
				],
				[
					0,
					30.37841291858014
				],
				[
					0,
					37.611360492097695
				],
				[
					0,
					49.18406557312361
				],
				[
					-0.7232837207501157,
					58.58686430889
				],
				[
					-0.7232837207501157,
					70.88290829367628
				],
				[
					0,
					78.11585586719377
				],
				[
					0,
					86.79537088221062
				],
				[
					0.7232837207489645,
					99.09141486699683
				],
				[
					0.7232837207489645,
					110.66411994802274
				],
				[
					0.7232837207489645,
					120.06691868378914
				],
				[
					0.7232837207489645,
					128.7464888818166
				],
				[
					0.7232837207489645,
					136.70272017608377
				],
				[
					0.7232837207489645,
					150.4453316023692
				],
				[
					0.7232837207489645,
					159.12484661738605
				],
				[
					0.7232837207489645,
					169.2509842569128
				],
				[
					0.7232837207489645,
					177.20721555117998
				],
				[
					0,
					197.45949083023336
				],
				[
					0,
					213.3719534187677
				],
				[
					0,
					215.54185976402715
				],
				[
					0,
					224.221374779044
				],
				[
					0,
					230.00775491106225
				],
				[
					0,
					235.79407986006998
				],
				[
					-0.7232837207501157,
					242.30374371283773
				],
				[
					-0.7232837207501157,
					250.25997500710488
				],
				[
					-0.7232837207501157,
					253.8764487938637
				],
				[
					-0.7232837207501157,
					255.32307141837362
				],
				[
					-0.7232837207501157,
					257.4929225806225
				],
				[
					-0.7232837207501157,
					258.21626148438287
				],
				[
					-0.7232837207501157,
					262.5560189918912
				],
				[
					-0.7232837207501157,
					264.0025864333906
				],
				[
					-0.7232837207501157,
					261.10939636738135
				],
				[
					-0.7232837207501157,
					261.10939636738135
				]
			],
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
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				-0.5714198521209255,
				206.28570556640625
			]
		},
		{
			"id": "LTH65pp7sdcRyFINgzkRZ",
			"type": "freedraw",
			"x": 7082.083259238571,
			"y": 337.4142151666669,
			"width": 28.208478981815567,
			"height": 3.616473786758743,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"roundness": null,
			"seed": 1659378148,
			"version": 201,
			"versionNonce": 736538716,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230204622,
			"link": null,
			"locked": true,
			"points": [
				[
					0,
					0
				],
				[
					7.2329475735170545,
					-2.169906345259519
				],
				[
					9.402826327271088,
					-1.4466226245099068
				],
				[
					13.742583834780305,
					-0.723283720749612
				],
				[
					16.635773900789292,
					0
				],
				[
					23.145410162051395,
					0
				],
				[
					26.761883948810496,
					0
				],
				[
					28.208478981815567,
					-0.723283720749612
				],
				[
					25.315316507311415,
					0
				],
				[
					18.805652654543326,
					1.446567441499224
				],
				[
					18.805652654543326,
					1.446567441499224
				]
			],
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
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				14.857134137834692,
				1.1428397042410552
			]
		},
		{
			"id": "447YGBr1oqM-DYH0nz6Rt",
			"type": "freedraw",
			"x": 7081.359947926317,
			"y": 338.8607826081661,
			"width": 32.54826408082847,
			"height": 4.339757507508355,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"roundness": null,
			"seed": 1642880740,
			"version": 199,
			"versionNonce": 1868567396,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230204622,
			"link": null,
			"locked": true,
			"points": [
				[
					0,
					0
				],
				[
					7.232947573517053,
					-1.446567441499224
				],
				[
					9.402826327271086,
					-1.446567441499224
				],
				[
					15.912490180039175,
					-2.169851162248836
				],
				[
					21.69884272055231,
					-3.616473786758743
				],
				[
					27.485195261065446,
					-3.616473786758743
				],
				[
					30.378385327074433,
					-4.339757507508355
				],
				[
					32.54826408082847,
					-2.8931900660091308
				],
				[
					32.54826408082847,
					-2.8931900660091308
				]
			],
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
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				25.714285714285325,
				-2.285723005022305
			]
		},
		{
			"id": "MAiRkdh2CAQL5-xr12Twv",
			"type": "freedraw",
			"x": 7401.056263785598,
			"y": 335.96759254215704,
			"width": 26.038600228060382,
			"height": 2.89313488299852,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"roundness": null,
			"seed": 1851822180,
			"version": 198,
			"versionNonce": 1156072668,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230204622,
			"link": null,
			"locked": true,
			"points": [
				[
					0,
					0
				],
				[
					5.063041228258183,
					-0.723283720749612
				],
				[
					11.572705081025122,
					-1.446567441499224
				],
				[
					21.698842720552314,
					-2.169851162248908
				],
				[
					25.315316507311415,
					-2.89313488299852
				],
				[
					26.038600228060382,
					-2.89313488299852
				],
				[
					23.145410162051395,
					-2.89313488299852
				],
				[
					23.145410162051395,
					-2.89313488299852
				]
			],
			"pressures": [
				0.185546875,
				0.2470703125,
				0.2666015625,
				0.2626953125,
				0.259765625,
				0.259765625,
				0.0126953125,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				18.285696847097825,
				-2.285679408482167
			]
		},
		{
			"id": "bKuTonufW3GuYNcM_aCrk",
			"type": "freedraw",
			"x": 7400.332924881837,
			"y": 335.2443088214074,
			"width": 23.868749065812334,
			"height": 2.169851162248908,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"roundness": null,
			"seed": 493963740,
			"version": 200,
			"versionNonce": 273680100,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230204622,
			"link": null,
			"locked": true,
			"points": [
				[
					0,
					0
				],
				[
					0.7233389037609423,
					-0.723283720749612
				],
				[
					2.1699063452600225,
					-0.723283720749612
				],
				[
					5.06309641126901,
					-1.446567441499296
				],
				[
					8.679570198028111,
					-1.446567441499296
				],
				[
					17.359085213044246,
					-2.169851162248908
				],
				[
					21.698842720553465,
					-2.169851162248908
				],
				[
					23.868749065812334,
					-2.169851162248908
				],
				[
					19.52899155830427,
					0
				],
				[
					19.52899155830427,
					0
				]
			],
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
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				15.428597586495925,
				0
			]
		},
		{
			"id": "PSLYT10IT9FM8hMhL3fL8",
			"type": "freedraw",
			"x": 7724.415442223817,
			"y": 387.3821635110334,
			"width": 21.087230895940387,
			"height": 22.709348189526775,
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
			"seed": 311297756,
			"version": 94,
			"versionNonce": 731136092,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230240486,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.8110354425287984,
					-7.704960460100203
				],
				[
					-0.8110354425287984,
					-8.110478181364643
				],
				[
					-0.8110354425287984,
					-6.893894078552371
				],
				[
					-0.4055486602837555,
					-4.055239090682301
				],
				[
					0,
					1.6221018240767917
				],
				[
					0,
					6.488376357287972
				],
				[
					0.40554866028311004,
					9.732580005441395
				],
				[
					0.40554866028311004,
					10.138097726705874
				],
				[
					0.8110354425287984,
					9.732580005441395
				],
				[
					1.2165841028119084,
					5.271823193494614
				],
				[
					2.0276195453413526,
					1.2165841028123119
				],
				[
					3.6496904303989495,
					-4.866274533211181
				],
				[
					4.8662745332108575,
					-7.704960460100203
				],
				[
					5.677309975740302,
					-9.327046814667439
				],
				[
					6.8938940785522105,
					-8.921529093402999
				],
				[
					7.299442738835966,
					-6.893894078552371
				],
				[
					6.8938940785522105,
					-4.866274533211181
				],
				[
					6.488407296306522,
					-2.8386549878699894
				],
				[
					6.8938940785522105,
					-2.8386549878699894
				],
				[
					9.327062284176673,
					-4.055239090682301
				],
				[
					12.165717272046823,
					-6.893894078552371
				],
				[
					15.815407702445773,
					-11.760199550782504
				],
				[
					16.220956362729527,
					-12.5712504628209
				],
				[
					17.031991805258325,
					-11.354666360008588
				],
				[
					17.437540465541435,
					-7.299442738835723
				],
				[
					16.626505023012637,
					-3.244203648153422
				],
				[
					16.626505023012637,
					-1.2165841028122313
				],
				[
					16.220956362729527,
					0
				],
				[
					16.626505023012637,
					0.8110354425289598
				],
				[
					17.031991805258325,
					1.2165841028123119
				],
				[
					18.248575908070237,
					0.8110354425289598
				],
				[
					20.27619545341159,
					-1.622101824076711
				],
				[
					20.27619545341159,
					-1.622101824076711
				]
			],
			"pressures": [
				0.1083984375,
				0.3203125,
				0.37890625,
				0.5390625,
				0.5390625,
				0.5390625,
				0.5458984375,
				0.5498046875,
				0.5498046875,
				0.560546875,
				0.578125,
				0.5830078125,
				0.5849609375,
				0.5849609375,
				0.5849609375,
				0.5751953125,
				0.5712890625,
				0.5693359375,
				0.5693359375,
				0.5712890625,
				0.578125,
				0.5830078125,
				0.5830078125,
				0.5830078125,
				0.5830078125,
				0.5810546875,
				0.5849609375,
				0.5927734375,
				0.5947265625,
				0.564453125,
				0.49609375,
				0.3388671875,
				0.0166015625,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				28.57142857142844,
				-2.285723005022305
			]
		},
		{
			"id": "_MK1_s8vOgopFE5jaMgdI",
			"type": "freedraw",
			"x": 7751.9910804160645,
			"y": 377.64958350559203,
			"width": 17.437478587504014,
			"height": 10.94914863874419,
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
			"seed": 2027544676,
			"version": 83,
			"versionNonce": 924025700,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230240486,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-5.677371853778369,
					4.055239090682342
				],
				[
					-6.082858636023412,
					4.866305472230174
				],
				[
					-6.893894078552855,
					6.893925017571365
				],
				[
					-6.488407296307167,
					8.110478181364643
				],
				[
					-5.271823193494614,
					8.921544562912475
				],
				[
					-2.4331682056244626,
					8.921544562912475
				],
				[
					-0.4055486602837555,
					8.110478181364643
				],
				[
					1.2165841028119084,
					5.677340914759053
				],
				[
					2.027619545340707,
					3.6497213694178616
				],
				[
					2.027619545340707,
					1.622101824076711
				],
				[
					2.027619545340707,
					-0.4055177212644396
				],
				[
					2.027619545340707,
					-0.8110509120383556
				],
				[
					2.4331063275863953,
					0
				],
				[
					2.838654987870151,
					2.433137266605631
				],
				[
					4.0552390906820595,
					6.082858636023532
				],
				[
					5.271823193494614,
					7.704960460100244
				],
				[
					6.082858636023412,
					8.921544562912475
				],
				[
					6.8938940785522105,
					9.732580005441354
				],
				[
					7.7049295210810085,
					10.138097726705833
				],
				[
					8.515964963609807,
					10.138097726705833
				],
				[
					10.54358450895116,
					8.515995902629124
				],
				[
					10.54358450895116,
					8.515995902629124
				]
			],
			"pressures": [
				0.2001953125,
				0.3828125,
				0.4267578125,
				0.4833984375,
				0.49609375,
				0.49609375,
				0.5068359375,
				0.5107421875,
				0.5126953125,
				0.5205078125,
				0.533203125,
				0.544921875,
				0.5478515625,
				0.5654296875,
				0.556640625,
				0.5693359375,
				0.576171875,
				0.580078125,
				0.58203125,
				0.5439453125,
				0.4501953125,
				0.013671875,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				14.857090541294383,
				11.999991280691972
			]
		},
		{
			"id": "7DqOqvekXgGLx4bY-Cewc",
			"type": "freedraw",
			"x": 7762.12917814277,
			"y": 386.5711280685045,
			"width": 8.110478181364764,
			"height": 19.46516001088279,
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
			"seed": 1376053860,
			"version": 67,
			"versionNonce": 409195740,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230240486,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					3.2442036481539063,
					-5.6773409147590135
				],
				[
					5.271823193494614,
					-8.921544562912477
				],
				[
					7.704929521081654,
					-12.976783653594818
				],
				[
					8.110478181364764,
					-16.220971832238806
				],
				[
					5.271823193494614,
					-19.46516001088279
				],
				[
					5.271823193494614,
					-19.46516001088279
				]
			],
			"pressures": [
				0.330078125,
				0.5166015625,
				0.5234375,
				0.5048828125,
				0.3662109375,
				0.0146484375,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				7.4285888671875,
				-27.4285888671875
			]
		},
		{
			"id": "ADCE-ouKSSb9fU5bPPFB-",
			"type": "freedraw",
			"x": 7764.1567976881115,
			"y": 367.5114857788862,
			"width": 13.382301374859377,
			"height": 15.409920920200406,
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
			"seed": 2061146212,
			"version": 70,
			"versionNonce": 1880454884,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230240486,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					1.2165686333027952
				],
				[
					2.4331063275863953,
					8.5160113721386
				],
				[
					4.460725872927748,
					10.94914863874419
				],
				[
					7.299442738835966,
					12.976783653594817
				],
				[
					8.515964963610452,
					13.382301374859297
				],
				[
					10.949133169234916,
					14.598854538652574
				],
				[
					12.571204054292512,
					15.004403198936007
				],
				[
					13.382301374859377,
					15.409920920200406
				],
				[
					13.382301374859377,
					15.409920920200406
				]
			],
			"pressures": [
				0.2431640625,
				0.2685546875,
				0.51953125,
				0.5556640625,
				0.5634765625,
				0.5634765625,
				0.529296875,
				0.3671875,
				0.029296875,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				18.85716029575906,
				21.71430315290172
			]
		},
		{
			"id": "7qY_FRJtCyqNqXI079zpC",
			"type": "freedraw",
			"x": 7788.893719014451,
			"y": 382.11034031753877,
			"width": 11.354681829518025,
			"height": 2.0276195453411106,
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
			"seed": 1432561244,
			"version": 68,
			"versionNonce": 1598871900,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230240486,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					4.86633641124957,
					-1.6220708850577585
				],
				[
					8.51602684164852,
					-1.2165531637932785
				],
				[
					10.138097726706116,
					-1.2165531637932785
				],
				[
					11.354681829518025,
					-1.2165531637932785
				],
				[
					10.543646386989227,
					-1.2165531637932785
				],
				[
					8.51602684164852,
					-2.0276195453411106
				],
				[
					8.51602684164852,
					-2.0276195453411106
				]
			],
			"pressures": [
				0.318359375,
				0.509765625,
				0.525390625,
				0.533203125,
				0.53515625,
				0.21484375,
				0.0126953125,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				12.000034877232792,
				-2.857142857142776
			]
		},
		{
			"id": "gwrFQpmgpS7y-VEd5SOAE",
			"type": "freedraw",
			"x": 7791.732435880359,
			"y": 371.1612071483041,
			"width": 13.787788157104421,
			"height": 2.8386704573795467,
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
			"seed": 281160548,
			"version": 69,
			"versionNonce": 730659428,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230240486,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1.216522224774487,
					-0.8110509120383959
				],
				[
					4.8662745332108575,
					-1.6221018240767515
				],
				[
					7.299380860797899,
					-2.433152736115107
				],
				[
					8.110478181364764,
					-2.433152736115107
				],
				[
					10.138097726705471,
					-2.8386704573795467
				],
				[
					11.354619951479958,
					-2.433152736115107
				],
				[
					13.787788157104421,
					-1.6221018240767515
				],
				[
					13.787788157104421,
					-1.6221018240767515
				]
			],
			"pressures": [
				0.330078125,
				0.5244140625,
				0.552734375,
				0.5546875,
				0.5546875,
				0.5244140625,
				0.4130859375,
				0.015625,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				19.428536551338766,
				-2.285723005022362
			]
		},
		{
			"id": "URJd3fHJBudkyugIR2s1T",
			"type": "freedraw",
			"x": 7819.308012194569,
			"y": 367.9170189696601,
			"width": 24.736921326339335,
			"height": 16.626474083993767,
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
			"seed": 1871088868,
			"version": 74,
			"versionNonce": 1537297884,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230240486,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-4.460725872927748,
					10.949133169234713
				],
				[
					-0.40548678224568835,
					14.193321347878658
				],
				[
					9.732610944460427,
					13.38228590534978
				],
				[
					19.8707086711659,
					7.704944990590767
				],
				[
					20.27619545341159,
					2.83865498787007
				],
				[
					17.437540465541435,
					0.4055177212644396
				],
				[
					16.220956362729527,
					-0.8110509120383959
				],
				[
					13.382301374859377,
					-2.433152736115107
				],
				[
					9.732610944460427,
					-2.433152736115107
				],
				[
					8.516026841647873,
					-1.2165841028123119
				],
				[
					8.516026841647873,
					0
				],
				[
					9.732610944460427,
					2.0276195453411505
				],
				[
					9.732610944460427,
					2.0276195453411505
				]
			],
			"pressures": [
				0.2509765625,
				0.486328125,
				0.509765625,
				0.513671875,
				0.5400390625,
				0.564453125,
				0.5771484375,
				0.5830078125,
				0.591796875,
				0.587890625,
				0.5419921875,
				0.3115234375,
				0.013671875,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				13.714338030134058,
				2.857142857142833
			]
		},
		{
			"id": "JxazcKgfd4D0IiWGu05tI",
			"type": "freedraw",
			"x": 7996.927558620102,
			"y": 481.8692466995394,
			"width": 1.2165841028119084,
			"height": 0.4055177212644799,
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
			"seed": 882378468,
			"version": 67,
			"versionNonce": 608701924,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230240486,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					-0.4055177212644799
				],
				[
					0.40548678224568835,
					-0.4055177212644799
				],
				[
					0.8110354425287984,
					0
				],
				[
					1.2165841028119084,
					0
				],
				[
					0,
					0
				]
			],
			"pressures": [
				0.2255859375,
				0.3330078125,
				0.482421875,
				0.4658203125,
				0.0146484375,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				1.714303152901266,
				0
			]
		},
		{
			"id": "4bSY5bWPn-eVNYs82Sx6A",
			"type": "freedraw",
			"x": 7793.76011730374,
			"y": 437.6671344232981,
			"width": 3.2442036481539063,
			"height": 30.81982637089142,
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
			"seed": 435321444,
			"version": 71,
			"versionNonce": 779301468,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230240486,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.40548678224568835,
					-7.704960460100203
				],
				[
					0.8110354425287984,
					-8.921544562912475
				],
				[
					2.4331063275870406,
					-15.004403198936007
				],
				[
					2.838654987870151,
					-20.68171317467611
				],
				[
					2.4331063275870406,
					-27.98115591351187
				],
				[
					2.0276195453413526,
					-30.81982637089142
				],
				[
					2.0276195453413526,
					-30.414308649626978
				],
				[
					2.0276195453413526,
					-23.92591682282957
				],
				[
					3.2442036481539063,
					-19.46516001088279
				],
				[
					3.2442036481539063,
					-19.46516001088279
				]
			],
			"pressures": [
				0.3359375,
				0.54296875,
				0.5517578125,
				0.578125,
				0.583984375,
				0.5947265625,
				0.58203125,
				0.53125,
				0.3095703125,
				0.013671875,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				4.5714460100452925,
				-27.4285888671875
			]
		},
		{
			"id": "iLJXIXZx1qVRe9uVo9_uJ",
			"type": "freedraw",
			"x": 7811.197657769282,
			"y": 428.7455898603856,
			"width": 8.92157550193163,
			"height": 20.276195453411667,
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
			"seed": 2060738404,
			"version": 67,
			"versionNonce": 190099812,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230240486,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-5.677371853778369,
					8.110478181364643
				],
				[
					-6.488407296307167,
					8.921544562912475
				],
				[
					-8.51602684164852,
					14.598885477671528
				],
				[
					-8.92157550193163,
					17.4375404655416
				],
				[
					-6.082858636024057,
					20.276195453411667
				],
				[
					-6.082858636024057,
					20.276195453411667
				]
			],
			"pressures": [
				0.359375,
				0.5234375,
				0.5302734375,
				0.55078125,
				0.505859375,
				0.013671875,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				-8.571428571429351,
				28.571428571428555
			]
		},
		{
			"id": "bSPs3gM24pDw55cYvnpDY",
			"type": "freedraw",
			"x": 7789.299329552774,
			"y": 444.5610285018505,
			"width": 34.87501905304545,
			"height": 23.92591682282957,
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
			"seed": 1334236764,
			"version": 83,
			"versionNonce": 110397148,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230240486,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-1.622070885057597,
					4.460756811946781
				],
				[
					-1.2165841028119084,
					8.110478181364684
				],
				[
					0.4055486602837555,
					13.382301374859297
				],
				[
					1.622132763095664,
					15.004403198936007
				],
				[
					4.055239090682705,
					17.84305818680608
				],
				[
					7.704991399119721,
					19.05964228961835
				],
				[
					12.976752714576268,
					18.248575908070517
				],
				[
					15.00437225991762,
					16.626474083993767
				],
				[
					17.84308912582519,
					11.760199550782545
				],
				[
					19.059611350599678,
					9.327062284176955
				],
				[
					20.27619545341223,
					7.704960460100203
				],
				[
					20.68174411369534,
					7.704960460100203
				],
				[
					21.898328216507895,
					8.515995902629124
				],
				[
					23.520399101565495,
					10.138097726705833
				],
				[
					25.14246998662309,
					12.571234993311464
				],
				[
					26.359054089435645,
					16.220956362729325
				],
				[
					25.953567307189957,
					18.654093629334955
				],
				[
					25.548018646906847,
					21.89829727748838
				],
				[
					27.170089531964443,
					23.52039910156513
				],
				[
					29.603257737588905,
					23.92591682282957
				],
				[
					33.25294816798785,
					22.709332720017297
				],
				[
					33.25294816798785,
					22.709332720017297
				]
			],
			"pressures": [
				0.2431640625,
				0.41796875,
				0.4970703125,
				0.5185546875,
				0.521484375,
				0.5234375,
				0.5234375,
				0.5263671875,
				0.537109375,
				0.54296875,
				0.5478515625,
				0.5576171875,
				0.5634765625,
				0.5634765625,
				0.5673828125,
				0.5673828125,
				0.57421875,
				0.58203125,
				0.5751953125,
				0.5205078125,
				0.31640625,
				0.013671875,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				46.857125418527175,
				31.999991280691972
			]
		},
		{
			"id": "s1ds0oemHqjjN0MzOOobI",
			"type": "freedraw",
			"x": 7849.722429130764,
			"y": 432.3953112298035,
			"width": 30.41429318011706,
			"height": 40.14687318555894,
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
			"seed": 437759068,
			"version": 85,
			"versionNonce": 1073800420,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230240486,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1.622070885057597,
					3.649721369417902
				],
				[
					1.622070885057597,
					5.271823193494614
				],
				[
					0.8110354425287984,
					10.949164108253665
				],
				[
					-0.8110973205668656,
					15.004403198936007
				],
				[
					-4.0552390906820595,
					20.27619545341171
				],
				[
					-6.082858636023412,
					23.92591682282957
				],
				[
					-9.732610944460427,
					28.38667363477635
				],
				[
					-12.165717272046823,
					30.414293180117543
				],
				[
					-15.409920920200085,
					30.81981090138198
				],
				[
					-18.65412456835399,
					29.197740016324182
				],
				[
					-19.46516001088279,
					25.54801864690632
				],
				[
					-20.27619545341159,
					23.11488138030069
				],
				[
					-20.6817441136947,
					22.30381499875286
				],
				[
					-21.898328216507252,
					22.709332720017297
				],
				[
					-24.331434544093646,
					25.54801864690632
				],
				[
					-25.5480186469062,
					27.57563819224747
				],
				[
					-27.170151410001864,
					30.0087754588531
				],
				[
					-27.575638192247553,
					31.225359561665375
				],
				[
					-28.79222229505946,
					35.28059865234771
				],
				[
					-28.79222229505946,
					37.713735918953304
				],
				[
					-28.79222229505946,
					38.93028908274667
				],
				[
					-27.981186852530662,
					39.7413554642945
				],
				[
					-27.170151410001864,
					40.14687318555894
				],
				[
					-27.170151410001864,
					40.14687318555894
				]
			],
			"pressures": [
				0.17578125,
				0.255859375,
				0.279296875,
				0.3583984375,
				0.396484375,
				0.43359375,
				0.45703125,
				0.4931640625,
				0.513671875,
				0.5224609375,
				0.529296875,
				0.5302734375,
				0.5283203125,
				0.5263671875,
				0.5263671875,
				0.5283203125,
				0.53515625,
				0.5390625,
				0.54296875,
				0.5576171875,
				0.5654296875,
				0.552734375,
				0.48828125,
				0.0166015625,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				-38.28578404017844,
				56.57143729073664
			]
		},
		{
			"id": "1pzd-sfduqYHDezJTXgGB",
			"type": "freedraw",
			"x": 7822.5522777207625,
			"y": 519.5829516794737,
			"width": 2.4331063275870406,
			"height": 28.792222295059744,
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
			"seed": 904845020,
			"version": 83,
			"versionNonce": 1754745692,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230240486,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.40548678224568835,
					-6.893894078552412
				],
				[
					0.40554866028311004,
					-17.437509526522685
				],
				[
					0.40554866028311004,
					-23.92591682282957
				],
				[
					0.40554866028311004,
					-25.953536368170763
				],
				[
					0.40554866028311004,
					-23.92591682282957
				],
				[
					1.216584102812554,
					-17.437509526522685
				],
				[
					1.622132763095664,
					-12.571234993311464
				],
				[
					1.622132763095664,
					-7.299411799816851
				],
				[
					1.216584102812554,
					-3.2441727091345096
				],
				[
					1.216584102812554,
					-4.460756811946781
				],
				[
					1.622132763095664,
					-8.110478181364684
				],
				[
					2.0276195453413526,
					-12.571234993311464
				],
				[
					2.0276195453413526,
					-19.059611350599397
				],
				[
					2.0276195453413526,
					-20.27619545341171
				],
				[
					1.622132763095664,
					-16.626474083993806
				],
				[
					1.622132763095664,
					-11.760199550782586
				],
				[
					1.622132763095664,
					-6.488376357287972
				],
				[
					1.622132763095664,
					-2.433137266605631
				],
				[
					2.0276195453413526,
					0.811066381547832
				],
				[
					1.622132763095664,
					2.838685926888983
				],
				[
					0,
					0
				]
			],
			"pressures": [
				0.142578125,
				0.529296875,
				0.5712890625,
				0.5830078125,
				0.591796875,
				0.591796875,
				0.58203125,
				0.58203125,
				0.5576171875,
				0.5478515625,
				0.5830078125,
				0.591796875,
				0.591796875,
				0.59375,
				0.59375,
				0.595703125,
				0.59375,
				0.59375,
				0.544921875,
				0.41796875,
				0.015625,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				2.2857666015625,
				4.000026157924083
			]
		},
		{
			"id": "zwsNWl4uPilGH4c1uf771",
			"type": "freedraw",
			"x": 7862.293633185057,
			"y": 509.8503716740323,
			"width": 18.24857590807088,
			"height": 21.49277955622394,
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
			"seed": 1578298588,
			"version": 75,
			"versionNonce": 131770468,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230240486,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.40548678224568835,
					0.811066381547832
				],
				[
					-0.40548678224568835,
					1.622101824076711
				],
				[
					-0.40548678224568835,
					2.0276195453411505
				],
				[
					-0.40548678224568835,
					2.838685926888983
				],
				[
					0.8110354425287984,
					2.0276195453411505
				],
				[
					6.488407296307167,
					-3.2441727091345096
				],
				[
					10.543646386989227,
					-6.488376357287972
				],
				[
					13.382301374859377,
					-9.732549066422482
				],
				[
					15.40992092020073,
					-12.165717272047026
				],
				[
					17.031991805258325,
					-14.193336817388175
				],
				[
					17.84308912582519,
					-15.409889981181534
				],
				[
					17.031991805258325,
					-16.626474083993806
				],
				[
					14.598885477671931,
					-18.654093629334955
				],
				[
					14.598885477671931,
					-18.654093629334955
				]
			],
			"pressures": [
				0.166015625,
				0.1904296875,
				0.232421875,
				0.279296875,
				0.4462890625,
				0.505859375,
				0.541015625,
				0.546875,
				0.548828125,
				0.548828125,
				0.5322265625,
				0.4765625,
				0.30859375,
				0.013671875,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				20.571463448661234,
				-26.28570556640625
			]
		},
		{
			"id": "yu9EThE8fVYfUeOE2VTGB",
			"type": "freedraw",
			"x": 7865.132288172927,
			"y": 494.0349639715863,
			"width": 19.46516001088279,
			"height": 26.3590540894352,
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
			"seed": 955470044,
			"version": 69,
			"versionNonce": 1993179100,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230240486,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					2.0276195453413526,
					6.893894078552412
				],
				[
					8.110478181364766,
					10.949133169234713
				],
				[
					12.571265932330581,
					13.787788157104783
				],
				[
					17.032053683296397,
					17.843027247787123
				],
				[
					18.248575908070237,
					18.654093629334955
				],
				[
					19.46516001088279,
					21.08723089594059
				],
				[
					17.843089125825195,
					26.3590540894352
				],
				[
					17.843089125825195,
					26.3590540894352
				]
			],
			"pressures": [
				0.330078125,
				0.4931640625,
				0.54296875,
				0.55859375,
				0.5654296875,
				0.55859375,
				0.5126953125,
				0.0146484375,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				25.142909458705617,
				37.14285714285717
			]
		},
		{
			"id": "FfgeRTC6hC3IifycNIucc",
			"type": "freedraw",
			"x": 7929.205078181316,
			"y": 494.44048169285077,
			"width": 4.055239090682705,
			"height": 19.87067773214723,
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
			"seed": 1408845660,
			"version": 70,
			"versionNonce": 1185938404,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230240486,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.8110354425287986,
					5.677340914759053
				],
				[
					-1.2165841028125541,
					9.327031345158002
				],
				[
					-1.2165841028125541,
					11.354650890499194
				],
				[
					-0.8110354425287986,
					15.004372259917055
				],
				[
					1.2165841028119087,
					18.654093629334955
				],
				[
					2.0276195453407073,
					19.059611350599397
				],
				[
					2.8386549878701515,
					19.87067773214723
				],
				[
					2.8386549878701515,
					19.465129071863835
				],
				[
					2.8386549878701515,
					19.465129071863835
				]
			],
			"pressures": [
				0.318359375,
				0.5009765625,
				0.53125,
				0.5400390625,
				0.556640625,
				0.5546875,
				0.55078125,
				0.4765625,
				0.0126953125,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				3.9999825613840585,
				27.428545270647305
			]
		},
		{
			"id": "-ba4CfY5rZFQeJXjYHZ_-",
			"type": "freedraw",
			"x": 7930.016113623844,
			"y": 476.5974235060447,
			"width": 0.8110354425287984,
			"height": 6.488376357287972,
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
			"seed": 1000484324,
			"version": 67,
			"versionNonce": 961094748,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230240486,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.40554866028311004,
					-5.677340914759093
				],
				[
					0.40554866028311004,
					-6.488376357287972
				],
				[
					0,
					-6.082858636023532
				],
				[
					-0.40548678224568835,
					-1.2165841028123119
				],
				[
					0,
					0
				]
			],
			"pressures": [
				0.3359375,
				0.50390625,
				0.5224609375,
				0.3525390625,
				0.0146484375,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				-0.571376255580617,
				-1.7143031529018344
			]
		},
		{
			"id": "XrLo_vQzqnQGXLyplTGgR",
			"type": "freedraw",
			"x": 7827.4186141320115,
			"y": 424.6903507697033,
			"width": 14.598885477671931,
			"height": 24.736967734867925,
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
			"seed": 1368719204,
			"version": 85,
			"versionNonce": 915332964,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230240486,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.40548678224568835,
					-3.2441727091345096
				],
				[
					2.0276195453413526,
					-5.67730997574014
				],
				[
					6.4883454182691,
					-10.138097726705833
				],
				[
					6.893894078552855,
					-10.543615447970273
				],
				[
					8.110478181364764,
					-14.193336817388175
				],
				[
					6.4883454182691,
					-18.654093629334955
				],
				[
					4.055239090682705,
					-20.276179983902193
				],
				[
					1.6220708850582424,
					-19.87066226263775
				],
				[
					-0.40554866028311004,
					-17.437524996032163
				],
				[
					-1.622132763095664,
					-13.787788157104783
				],
				[
					-1.622132763095664,
					-10.949133169234754
				],
				[
					0.40548678224568835,
					-7.704929521081291
				],
				[
					2.838654987870151,
					-6.488376357287972
				],
				[
					7.299380860797899,
					-4.460756811946781
				],
				[
					9.32700040613925,
					-3.2441727091345096
				],
				[
					10.138097726706116,
					-1.6220708850577985
				],
				[
					8.921513623893562,
					0
				],
				[
					3.6496904303989495,
					1.2165841028122715
				],
				[
					-0.40554866028311004,
					1.622101824076711
				],
				[
					-2.8387168659075726,
					1.622101824076711
				],
				[
					-4.0552390906820595,
					2.433168205624543
				],
				[
					-4.460787750965815,
					4.460787750965734
				],
				[
					0,
					0
				]
			],
			"pressures": [
				0.177734375,
				0.384765625,
				0.4697265625,
				0.4951171875,
				0.4951171875,
				0.4970703125,
				0.5048828125,
				0.5087890625,
				0.521484375,
				0.5361328125,
				0.546875,
				0.5498046875,
				0.5517578125,
				0.546875,
				0.5390625,
				0.5302734375,
				0.53125,
				0.544921875,
				0.560546875,
				0.568359375,
				0.5380859375,
				0.435546875,
				0.015625,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				-6.2857491629465585,
				6.285749162946445
			]
		},
		{
			"id": "VPJb2gpjenWMKU4IMkent",
			"type": "freedraw",
			"x": 7803.898215030446,
			"y": 588.5220162210735,
			"width": 3.6496904303989495,
			"height": 25.54798770788741,
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
			"seed": 943373540,
			"version": 73,
			"versionNonce": 1708931292,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230240486,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.4055486602837555,
					-4.460756811946781
				],
				[
					-0.4055486602837555,
					-8.515995902629163
				],
				[
					-0.8110354425287984,
					-15.409889981181534
				],
				[
					-0.8110354425287984,
					-19.870677732147268
				],
				[
					-1.216584102812554,
					-23.11485044128174
				],
				[
					-1.216584102812554,
					-25.142469986622928
				],
				[
					-1.216584102812554,
					-25.54798770788741
				],
				[
					-0.8110354425287984,
					-25.142469986622928
				],
				[
					0,
					-23.11485044128174
				],
				[
					1.2165841028119084,
					-19.870677732147268
				],
				[
					2.4331063275863953,
					-16.62647408399385
				],
				[
					2.4331063275863953,
					-16.62647408399385
				]
			],
			"pressures": [
				0.29296875,
				0.50390625,
				0.541015625,
				0.5751953125,
				0.583984375,
				0.591796875,
				0.587890625,
				0.5859375,
				0.533203125,
				0.47265625,
				0.2958984375,
				0.0146484375,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				3.4285191127228245,
				-23.428562709263474
			]
		},
		{
			"id": "z_Irxm5eSxoTVZV6eCReo",
			"type": "freedraw",
			"x": 7822.1467909385165,
			"y": 589.7386003238856,
			"width": 1.6220708850582424,
			"height": 2.8386859268889424,
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
			"seed": 545187172,
			"version": 68,
			"versionNonce": 533025508,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230240486,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.40548678224568835,
					-1.2165841028122313
				],
				[
					1.216584102812554,
					-2.0276195453411106
				],
				[
					1.216584102812554,
					-2.4331372666055904
				],
				[
					1.6220708850582424,
					-2.8386859268889424
				],
				[
					1.6220708850582424,
					-2.4331372666055904
				],
				[
					0,
					0
				]
			],
			"pressures": [
				0.2646484375,
				0.486328125,
				0.498046875,
				0.498046875,
				0.5,
				0.501953125,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				2.2856794084827925,
				-3.4285627092633604
			]
		},
		{
			"id": "JnRw8z8lJnHCItUFuZh-R",
			"type": "freedraw",
			"x": 7824.174410483858,
			"y": 584.466777130391,
			"width": 3.6497523084370163,
			"height": 11.760199550782586,
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
			"seed": 649675996,
			"version": 65,
			"versionNonce": 672709980,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230240486,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-3.6497523084370163,
					9.732580005441475
				],
				[
					-3.244203648153261,
					11.760199550782586
				],
				[
					-1.216584102812554,
					10.949164108253706
				],
				[
					-1.216584102812554,
					10.949164108253706
				]
			],
			"pressures": [
				0.2802734375,
				0.5263671875,
				0.5263671875,
				0.015625,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				-1.7143031529021755,
				15.428597586495584
			]
		},
		{
			"id": "u8uNXN4wU4E5wGg2Rrlg6",
			"type": "freedraw",
			"x": 7843.234021834458,
			"y": 556.0801034956147,
			"width": 12.976752714575621,
			"height": 28.38667363477635,
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
			"seed": 25076316,
			"version": 78,
			"versionNonce": 283203172,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230240486,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-2.433168205625108,
					7.704960460100284
				],
				[
					-2.433168205625108,
					8.921544562912516
				],
				[
					-4.055239090682705,
					15.815438641464887
				],
				[
					-4.866274533211503,
					18.654093629334955
				],
				[
					-5.271823193494614,
					24.33143454409405
				],
				[
					-4.055239090682705,
					27.98115591351195
				],
				[
					-0.8110354425294439,
					28.38667363477635
				],
				[
					2.027619545340707,
					27.170120470983072
				],
				[
					6.488407296306522,
					23.92591682282957
				],
				[
					7.7049295210810085,
					21.49277955622398
				],
				[
					6.082858636023412,
					18.248575908070556
				],
				[
					2.4331682056244626,
					17.43754046554168
				],
				[
					0.40554866028311004,
					17.84305818680608
				],
				[
					-1.216584102812554,
					20.681713174676148
				],
				[
					-1.216584102812554,
					24.33143454409405
				],
				[
					0,
					28.38667363477635
				],
				[
					0,
					28.38667363477635
				]
			],
			"pressures": [
				0.2880859375,
				0.4716796875,
				0.4892578125,
				0.5205078125,
				0.5234375,
				0.5361328125,
				0.5390625,
				0.5302734375,
				0.5185546875,
				0.505859375,
				0.5,
				0.5087890625,
				0.541015625,
				0.556640625,
				0.5546875,
				0.4833984375,
				0.0166015625,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				0,
				40
			]
		},
		{
			"id": "j-T4REPgchIGbk853jxcd",
			"type": "freedraw",
			"x": 7799.43742727948,
			"y": 605.9595566866151,
			"width": 23.925885883810537,
			"height": 24.33143454409405,
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
			"seed": 1392791780,
			"version": 84,
			"versionNonce": 1766896092,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230240486,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.40548678224568835,
					0
				],
				[
					-0.40548678224568835,
					1.216553163793359
				],
				[
					0,
					4.460756811946781
				],
				[
					2.0276195453413526,
					8.515995902629163
				],
				[
					3.244203648153261,
					11.354650890499233
				],
				[
					4.866274533211503,
					13.382270435840343
				],
				[
					8.516026841647873,
					15.004372259917055
				],
				[
					12.165717272046823,
					14.193336817388175
				],
				[
					14.193336817388175,
					12.165717272047065
				],
				[
					15.40992092020073,
					7.704960460100284
				],
				[
					16.220956362729527,
					4.460756811946781
				],
				[
					17.84308912582519,
					2.027619545341191
				],
				[
					18.65412456835399,
					2.027619545341191
				],
				[
					20.27619545341159,
					4.055239090682382
				],
				[
					21.492779556224143,
					6.488376357287972
				],
				[
					21.898328216507252,
					9.327031345158042
				],
				[
					22.30381499875294,
					10.543615447970273
				],
				[
					22.70936365903605,
					12.976752714575944
				],
				[
					23.11485044128174,
					16.62647408399385
				],
				[
					23.11485044128174,
					17.84305818680608
				],
				[
					23.11485044128174,
					20.681713174676148
				],
				[
					23.52039910156485,
					24.33143454409405
				],
				[
					23.52039910156485,
					24.33143454409405
				]
			],
			"pressures": [
				0.232421875,
				0.4091796875,
				0.4541015625,
				0.4833984375,
				0.494140625,
				0.4970703125,
				0.5,
				0.4970703125,
				0.4970703125,
				0.4970703125,
				0.4970703125,
				0.5,
				0.5087890625,
				0.5205078125,
				0.5185546875,
				0.5126953125,
				0.5126953125,
				0.5126953125,
				0.5126953125,
				0.515625,
				0.51953125,
				0.4365234375,
				0.015625,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				33.142874581472825,
				34.285714285714334
			]
		},
		{
			"id": "G9XmCQmLeN2qQxcWY3FUD",
			"type": "freedraw",
			"x": 7849.316880470481,
			"y": 598.6601139477793,
			"width": 26.764540871680687,
			"height": 37.71373591895327,
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
			"seed": 958133596,
			"version": 85,
			"versionNonce": 380692964,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230240486,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.8110354425287984,
					4.460756811946781
				],
				[
					0.8110354425287984,
					4.866305472230134
				],
				[
					0.40554866028311004,
					8.515995902629083
				],
				[
					-1.216584102812554,
					10.949164108253626
				],
				[
					-4.055239090682705,
					15.815438641464887
				],
				[
					-7.299442738835966,
					19.05964228961831
				],
				[
					-9.732549066422362,
					20.276195453411667
				],
				[
					-11.760168611763714,
					20.681713174676066
				],
				[
					-13.787788157105066,
					19.87067773214719
				],
				[
					-15.40992092020073,
					16.626474083993767
				],
				[
					-16.220956362729527,
					14.193336817388175
				],
				[
					-17.031991805258325,
					12.571234993311384
				],
				[
					-17.843027247787123,
					12.571234993311384
				],
				[
					-18.65412456835399,
					12.976783653594817
				],
				[
					-19.87064679312848,
					14.598854538652574
				],
				[
					-22.30381499875294,
					18.654093629334955
				],
				[
					-23.520399101565495,
					21.0872618349595
				],
				[
					-25.5480186469062,
					25.1425009256418
				],
				[
					-25.95350542915189,
					27.575638192247393
				],
				[
					-25.5480186469062,
					30.41429318011746
				],
				[
					-24.736983204377403,
					32.44191272545865
				],
				[
					-24.331434544094293,
					34.469532270799846
				],
				[
					-25.14246998662309,
					37.71373591895327
				],
				[
					-25.14246998662309,
					37.71373591895327
				]
			],
			"pressures": [
				0.2412109375,
				0.3359375,
				0.3466796875,
				0.39453125,
				0.4091796875,
				0.4423828125,
				0.4736328125,
				0.4921875,
				0.5078125,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.5146484375,
				0.521484375,
				0.5146484375,
				0.5185546875,
				0.5341796875,
				0.5400390625,
				0.5400390625,
				0.498046875,
				0.33984375,
				0.0146484375,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				-35.42855398995562,
				53.142874581473166
			]
		},
		{
			"id": "rTnytCKGDwlQPiuaoNaxE",
			"type": "freedraw",
			"x": 7822.1467909385165,
			"y": 670.8433821375324,
			"width": 4.055239090682705,
			"height": 26.359054089435162,
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
			"seed": 1814855644,
			"version": 77,
			"versionNonce": 412489308,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230240486,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.8110354425287986,
					-4.460756811946781
				],
				[
					0.8110354425287986,
					-6.893925017571324
				],
				[
					1.6220708850582426,
					-12.976783653594817
				],
				[
					1.6220708850582426,
					-18.248575908070478
				],
				[
					1.2165841028125541,
					-20.276195453411667
				],
				[
					1.2165841028125541,
					-17.84305818680608
				],
				[
					0.8110354425287986,
					-14.598854538652656
				],
				[
					0.8110354425287986,
					-12.571234993311464
				],
				[
					0.40548678224568846,
					-8.921544562912516
				],
				[
					-0.8110354425287986,
					-2.4331372666055904
				],
				[
					-1.6221327630956643,
					0.8110354425288792
				],
				[
					-2.0276195453407073,
					3.6496904303989495
				],
				[
					-2.433168205624463,
					5.271823193494614
				],
				[
					-2.433168205624463,
					6.082858636023492
				],
				[
					0,
					0
				]
			],
			"pressures": [
				0.2255859375,
				0.4404296875,
				0.466796875,
				0.509765625,
				0.53515625,
				0.5390625,
				0.5498046875,
				0.54296875,
				0.541015625,
				0.541015625,
				0.541015625,
				0.541015625,
				0.5390625,
				0.498046875,
				0.4375,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				-3.4286063058034415,
				8.571428571428555
			]
		},
		{
			"id": "aSjrdN8pPRnjCxI7IArN2",
			"type": "freedraw",
			"x": 7873.648315014575,
			"y": 672.0599662403447,
			"width": 8.110478181364764,
			"height": 27.98115591351195,
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
			"seed": 458819676,
			"version": 68,
			"versionNonce": 1950485860,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230240486,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					2.4331682056244626,
					-7.299442738835804
				],
				[
					3.6496904303989495,
					-9.732580005441395
				],
				[
					6.082858636023412,
					-14.19336775640713
				],
				[
					8.110478181364764,
					-19.059642289618388
				],
				[
					8.110478181364764,
					-21.89829727748846
				],
				[
					4.866274533211503,
					-27.98115591351195
				],
				[
					4.866274533211503,
					-27.98115591351195
				]
			],
			"pressures": [
				0.3359375,
				0.46875,
				0.48046875,
				0.48046875,
				0.4580078125,
				0.341796875,
				0.0146484375,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				6.8571254185271755,
				-39.42858014787953
			]
		},
		{
			"id": "DVyxRMo-0vCYCt5klDp2x",
			"type": "freedraw",
			"x": 7874.053863674859,
			"y": 652.1892885081975,
			"width": 14.193336817388175,
			"height": 20.276164514392715,
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
			"seed": 1032087908,
			"version": 69,
			"versionNonce": 1924852444,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230240486,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					3.6496904303989495,
					6.893894078552371
				],
				[
					5.677309975739656,
					8.515995902629083
				],
				[
					8.921513623893562,
					10.949133169234754
				],
				[
					9.732549066422362,
					12.165717272046985
				],
				[
					12.571204054292512,
					16.626474083993767
				],
				[
					12.976752714575621,
					18.654093629334955
				],
				[
					14.193336817388175,
					20.276164514392715
				],
				[
					14.193336817388175,
					20.276164514392715
				]
			],
			"pressures": [
				0.353515625,
				0.515625,
				0.5361328125,
				0.5400390625,
				0.5400390625,
				0.4365234375,
				0.29296875,
				0.013671875,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				20,
				28.57138497488836
			]
		},
		{
			"id": "q5PBMxwoCmIAlYQeuCKJ1",
			"type": "freedraw",
			"x": 7923.527768205575,
			"y": 641.2401243999439,
			"width": 2.4331063275863953,
			"height": 21.0872618349595,
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
			"seed": 1696729828,
			"version": 70,
			"versionNonce": 1524809956,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230240486,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.40548678224568835,
					2.8386859268889424
				],
				[
					0.40548678224568835,
					7.704960460100203
				],
				[
					0,
					14.193336817388095
				],
				[
					0.40548678224568835,
					19.05964228961831
				],
				[
					0.40548678224568835,
					19.87067773214719
				],
				[
					1.216584102812554,
					21.0872618349595
				],
				[
					2.0276195453413526,
					19.05964228961831
				],
				[
					2.4331063275863953,
					15.815438641464887
				],
				[
					2.4331063275863953,
					15.815438641464887
				]
			],
			"pressures": [
				0.359375,
				0.5546875,
				0.5712890625,
				0.5927734375,
				0.6064453125,
				0.6083984375,
				0.5830078125,
				0.3388671875,
				0.0146484375,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				3.4285191127228245,
				22.285723005022305
			]
		},
		{
			"id": "mpghVcBIfWEn-NiIpZj5l",
			"type": "freedraw",
			"x": 7921.500148660234,
			"y": 623.3970662131378,
			"width": 1.2165841028119084,
			"height": 0.811066381547832,
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
			"seed": 836283356,
			"version": 66,
			"versionNonce": 1246834524,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230240486,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.8110354425287984,
					-0.4055177212644799
				],
				[
					-0.8110354425287984,
					0
				],
				[
					-1.2165841028119084,
					0.4055486602833521
				],
				[
					0,
					0
				]
			],
			"pressures": [
				0.3359375,
				0.48046875,
				0.48828125,
				0.3447265625,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				-1.714303152901266,
				0.5714634486606656
			]
		},
		{
			"id": "E573hfwYI00fZDqdz_EV4",
			"type": "freedraw",
			"x": 8014.365099085645,
			"y": 405.63073941910386,
			"width": 17.437540465541435,
			"height": 27.981140444002435,
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
			"seed": 350710372,
			"version": 82,
			"versionNonce": 572589156,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230240487,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-7.299442738835965,
					-4.460772281456258
				],
				[
					-6.488345418269099,
					-5.677340914759053
				],
				[
					0.40554866028311,
					-14.598870008162091
				],
				[
					2.8386549878701506,
					-21.087246365450024
				],
				[
					2.0276195453407064,
					-23.114865910791213
				],
				[
					-0.4054867822456883,
					-23.114865910791213
				],
				[
					-2.43310632758704,
					-21.492764086714505
				],
				[
					-2.43310632758704,
					-17.03200727476772
				],
				[
					2.0276195453407064,
					-12.165717272047026
				],
				[
					5.271823193494613,
					-8.92152909340304
				],
				[
					8.921513623893562,
					-6.488391826797408
				],
				[
					10.13809772670547,
					-4.055239090682342
				],
				[
					7.704991399119074,
					-1.622101824076711
				],
				[
					4.460787750965814,
					0
				],
				[
					2.8386549878701506,
					0.8110509120383556
				],
				[
					0,
					1.6220863545672346
				],
				[
					-1.6220708850582422,
					1.6220863545672346
				],
				[
					-0.8110354425287983,
					3.244188178643986
				],
				[
					1.2165841028119082,
					4.866274533211221
				],
				[
					0,
					0
				]
			],
			"pressures": [
				0.1630859375,
				0.5205078125,
				0.5224609375,
				0.5224609375,
				0.4990234375,
				0.4990234375,
				0.5087890625,
				0.5283203125,
				0.5380859375,
				0.5361328125,
				0.5302734375,
				0.5283203125,
				0.5244140625,
				0.5302734375,
				0.5537109375,
				0.5625,
				0.576171875,
				0.5791015625,
				0.390625,
				0.0146484375,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				1.714303152901266,
				6.857125418526778
			]
		},
		{
			"id": "zdeNK0ay0T9QuDPbmznWD",
			"type": "freedraw",
			"x": 8039.913117732551,
			"y": 397.5202612377392,
			"width": 6.8938940785522105,
			"height": 15.004372259917055,
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
			"seed": 1678753628,
			"version": 66,
			"versionNonce": 1336599516,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230240487,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-6.8938940785522105,
					8.92152909340304
				],
				[
					-6.488407296307167,
					12.571234993311464
				],
				[
					-6.082858636023412,
					14.598854538652615
				],
				[
					-4.055239090682705,
					15.004372259917055
				],
				[
					-4.055239090682705,
					15.004372259917055
				]
			],
			"pressures": [
				0.333984375,
				0.5224609375,
				0.486328125,
				0.33984375,
				0.0146484375,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				-5.714285714286234,
				21.142839704241055
			]
		},
		{
			"id": "RZ1Ufpti9pqqvKfQrXwUO",
			"type": "freedraw",
			"x": 8067.894242707043,
			"y": 378.05511669636587,
			"width": 12.165717272046823,
			"height": 23.925901353320093,
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
			"seed": 98672356,
			"version": 77,
			"versionNonce": 2143999972,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230240487,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-3.6496904303989495,
					1.2165686333027952
				],
				[
					-7.7049295210810085,
					6.082858636023492
				],
				[
					-10.138097726705471,
					12.976752714575904
				],
				[
					-9.327000406138605,
					17.437524996032163
				],
				[
					-7.7049295210810085,
					19.059611350599397
				],
				[
					-2.8386549878695053,
					19.87066226263775
				],
				[
					0,
					19.059611350599397
				],
				[
					1.622132763095664,
					17.437524996032163
				],
				[
					2.0276195453413526,
					16.626474083993806
				],
				[
					0.8110973205668656,
					14.598854538652615
				],
				[
					-1.622070885057597,
					14.598854538652615
				],
				[
					-6.488345418268454,
					17.031991805258247
				],
				[
					-8.110478181364119,
					19.465144541373313
				],
				[
					-7.7049295210810085,
					21.492764086714505
				],
				[
					-4.460725872927748,
					23.925901353320093
				],
				[
					-4.460725872927748,
					23.925901353320093
				]
			],
			"pressures": [
				0.1875,
				0.3779296875,
				0.4580078125,
				0.494140625,
				0.5068359375,
				0.5068359375,
				0.5009765625,
				0.4970703125,
				0.4970703125,
				0.4970703125,
				0.5107421875,
				0.5166015625,
				0.537109375,
				0.537109375,
				0.48828125,
				0.0166015625,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				-6.2856619698659415,
				33.71427263532365
			]
		},
		{
			"id": "Jg685-Xu5D6F5IbYdySTq",
			"type": "freedraw",
			"x": 8009.498824552433,
			"y": 414.95780170328084,
			"width": 35.28056771332856,
			"height": 30.819810901381942,
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
			"seed": 322993764,
			"version": 81,
			"versionNonce": 1490683996,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230240487,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-4.055239090682059,
					5.6773099757400995
				],
				[
					-3.6496904303989486,
					9.327031345158002
				],
				[
					-0.40554866028311,
					15.004372259917055
				],
				[
					2.433168205624462,
					17.031991805258205
				],
				[
					7.299442738835965,
					17.843027247787123
				],
				[
					12.165717272046821,
					16.220956362729325
				],
				[
					15.81540770244577,
					14.193336817388175
				],
				[
					19.059611350599678,
					11.354650890499153
				],
				[
					22.709363659036047,
					6.488376357287932
				],
				[
					23.925885883810533,
					4.055239090682301
				],
				[
					24.7369832043774,
					4.055239090682301
				],
				[
					26.359054089434995,
					8.110478181364643
				],
				[
					27.57563819224755,
					12.976752714575865
				],
				[
					27.981124974493238,
					17.031991805258205
				],
				[
					27.981124974493238,
					20.68171317467611
				],
				[
					27.981124974493238,
					24.33143454409401
				],
				[
					27.981124974493238,
					27.98112497449296
				],
				[
					28.792222295060103,
					30.414293180117504
				],
				[
					31.225328622646497,
					30.819810901381942
				],
				[
					31.225328622646497,
					30.819810901381942
				]
			],
			"pressures": [
				0.2255859375,
				0.3955078125,
				0.439453125,
				0.4853515625,
				0.494140625,
				0.49609375,
				0.49609375,
				0.498046875,
				0.5,
				0.5078125,
				0.509765625,
				0.515625,
				0.5234375,
				0.5341796875,
				0.5458984375,
				0.5517578125,
				0.5537109375,
				0.5263671875,
				0.361328125,
				0.0146484375,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				43.99998256138406,
				43.42856270926336
			]
		},
		{
			"id": "oYoTSBCFDAsuB8iH_AFrb",
			"type": "freedraw",
			"x": 8075.599234106163,
			"y": 408.87492759774784,
			"width": 37.71373591895367,
			"height": 40.95792409759725,
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
			"seed": 575718628,
			"version": 80,
			"versionNonce": 1072577380,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230240487,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-4.460787750965815,
					10.94914863874419
				],
				[
					-9.732610944460427,
					19.87066226263775
				],
				[
					-14.598885477671931,
					22.709348189526736
				],
				[
					-20.68174411369534,
					25.142485456132366
				],
				[
					-23.520399101565495,
					25.142485456132366
				],
				[
					-24.736983204377403,
					24.736967734867925
				],
				[
					-26.764602749718755,
					22.709348189526736
				],
				[
					-27.575638192247553,
					19.059626820108832
				],
				[
					-26.764602749718755,
					15.81542317195541
				],
				[
					-26.764602749718755,
					16.220971832238803
				],
				[
					-27.575638192247553,
					18.248591377579952
				],
				[
					-31.630877282930257,
					23.520383632055616
				],
				[
					-34.87508093108352,
					26.764587280209078
				],
				[
					-37.30818725866991,
					32.036379534684734
				],
				[
					-37.71373591895367,
					35.68610090410264
				],
				[
					-37.30818725866991,
					37.71372044944379
				],
				[
					-36.49715181614111,
					39.33582227352054
				],
				[
					-36.90270047642487,
					40.95792409759725
				],
				[
					-36.90270047642487,
					40.95792409759725
				]
			],
			"pressures": [
				0.23046875,
				0.4091796875,
				0.4912109375,
				0.51171875,
				0.5263671875,
				0.53125,
				0.53515625,
				0.537109375,
				0.5302734375,
				0.5244140625,
				0.5205078125,
				0.5205078125,
				0.525390625,
				0.5400390625,
				0.560546875,
				0.5625,
				0.52734375,
				0.3955078125,
				0.0146484375,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				-52.00003487723279,
				57.714298793247735
			]
		},
		{
			"id": "pDZcksg6UYJW15aTDZ-Br",
			"type": "freedraw",
			"x": 8037.885498187209,
			"y": 470.5145648700212,
			"width": 12.165717272046823,
			"height": 23.114881380300652,
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
			"seed": 47196252,
			"version": 81,
			"versionNonce": 699440348,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230240487,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.8110354425287984,
					-3.6497213694178616
				],
				[
					0.4055486602837555,
					-3.244203648153422
				],
				[
					-0.40554866028311004,
					-0.8110354425288792
				],
				[
					-1.2165841028119084,
					6.082858636023532
				],
				[
					-1.622070885057597,
					11.354681829518146
				],
				[
					-1.2165841028119084,
					16.626474083993806
				],
				[
					0,
					19.059611350599397
				],
				[
					1.216584102812554,
					19.46516001088279
				],
				[
					3.6496904303989495,
					19.46516001088279
				],
				[
					8.516026841647873,
					17.031991805258247
				],
				[
					10.543646386989227,
					14.193336817388175
				],
				[
					9.732549066422362,
					11.760199550782586
				],
				[
					6.082858636023412,
					10.138097726705833
				],
				[
					1.622070885057597,
					10.543615447970314
				],
				[
					-0.40554866028311004,
					12.165717272047026
				],
				[
					-1.622070885057597,
					14.193336817388175
				],
				[
					-1.2165841028119084,
					15.815438641464928
				],
				[
					0,
					17.031991805258247
				],
				[
					1.216584102812554,
					19.46516001088279
				],
				[
					1.216584102812554,
					19.46516001088279
				]
			],
			"pressures": [
				0.1630859375,
				0.2734375,
				0.4765625,
				0.51171875,
				0.53125,
				0.5478515625,
				0.5556640625,
				0.5556640625,
				0.5556640625,
				0.5556640625,
				0.5595703125,
				0.5546875,
				0.5576171875,
				0.5654296875,
				0.5751953125,
				0.5859375,
				0.5869140625,
				0.5341796875,
				0.38671875,
				0.0146484375,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				1.7143031529021755,
				27.4285888671875
			]
		},
		{
			"id": "GQ6D70q44yH2JQitnjNF_",
			"type": "freedraw",
			"x": 8085.737331832868,
			"y": 485.11341940867385,
			"width": 17.843027247787123,
			"height": 25.95353636817072,
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
			"seed": 1791859164,
			"version": 68,
			"versionNonce": 2094608100,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230240487,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					4.460725872927747,
					-4.866274533211221
				],
				[
					8.51596496361045,
					-9.327031345158002
				],
				[
					16.626443144975212,
					-16.626474083993767
				],
				[
					17.843027247787123,
					-19.465129071863835
				],
				[
					17.031991805258325,
					-22.709332720017258
				],
				[
					12.57120405429251,
					-25.95353636817072
				],
				[
					12.57120405429251,
					-25.95353636817072
				]
			],
			"pressures": [
				0.27734375,
				0.513671875,
				0.5224609375,
				0.5244140625,
				0.486328125,
				0.30078125,
				0.013671875,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				17.7142333984375,
				-36.57143729073658
			]
		},
		{
			"id": "Y5hvH6vJB8TgmlNISJKPZ",
			"type": "freedraw",
			"x": 8093.036774571705,
			"y": 464.8372239552622,
			"width": 11.354619951479958,
			"height": 21.49277955622398,
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
			"seed": 1667526628,
			"version": 69,
			"versionNonce": 1002479964,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230240487,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.40548678224568835,
					4.460756811946781
				],
				[
					0.8110354425287984,
					6.082858636023492
				],
				[
					3.6496904303989495,
					10.543615447970273
				],
				[
					8.110478181364764,
					14.193336817388175
				],
				[
					9.32700040613925,
					15.409920920200447
				],
				[
					11.354619951479958,
					18.654093629334955
				],
				[
					11.354619951479958,
					21.49277955622398
				],
				[
					11.354619951479958,
					21.49277955622398
				]
			],
			"pressures": [
				0.294921875,
				0.4169921875,
				0.4677734375,
				0.541015625,
				0.5537109375,
				0.5537109375,
				0.4287109375,
				0.05859375,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				15.999930245535325,
				30.28573172433039
			]
		},
		{
			"id": "NT4bssMST75PxeGyASjEQ",
			"type": "freedraw",
			"x": 8148.593537738444,
			"y": 466.86484350060334,
			"width": 4.460725872927748,
			"height": 1.216553163793359,
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
			"seed": 1989552100,
			"version": 66,
			"versionNonce": 1461301860,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230240487,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					2.4331063275870406,
					-0.4055177212644799
				],
				[
					2.838654987870151,
					-0.8110354425289195
				],
				[
					4.460725872927748,
					-1.216553163793359
				],
				[
					0,
					0
				]
			],
			"pressures": [
				0.2041015625,
				0.234375,
				0.232421875,
				0.013671875,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				6.2856619698659415,
				-1.7142595563616396
			]
		},
		{
			"id": "7pK1BtNXjl0OR5IGZtPLu",
			"type": "freedraw",
			"x": 8140.888546339325,
			"y": 452.2659889619507,
			"width": 3.244203648153261,
			"height": 27.57563819224747,
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
			"seed": 1271645660,
			"version": 71,
			"versionNonce": 106698204,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230240487,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					10.949133169234754
				],
				[
					0.4055486602837555,
					12.976752714575904
				],
				[
					1.216584102812554,
					18.248575908070517
				],
				[
					2.0276195453413526,
					21.89829727748842
				],
				[
					2.4331682056244626,
					25.142469986622928
				],
				[
					2.838716865908218,
					26.76457181069964
				],
				[
					2.838716865908218,
					27.17008953196408
				],
				[
					2.838716865908218,
					27.57563819224747
				],
				[
					3.244203648153261,
					26.76457181069964
				],
				[
					3.244203648153261,
					26.76457181069964
				]
			],
			"pressures": [
				0.333984375,
				0.50390625,
				0.5185546875,
				0.548828125,
				0.560546875,
				0.56640625,
				0.56640625,
				0.5556640625,
				0.513671875,
				0.0146484375,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				4.571446010044383,
				37.714276994977695
			]
		},
		{
			"id": "hLogpcEpqNZr65sUQ_bWe",
			"type": "freedraw",
			"x": 8146.565918193104,
			"y": 464.02618851273326,
			"width": 15.409920920200085,
			"height": 12.571234993311464,
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
			"seed": 30191836,
			"version": 78,
			"versionNonce": 763217380,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230240487,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					4.460725872927748,
					-0.811066381547832
				],
				[
					10.949133169234269,
					-3.2442036481534626
				],
				[
					11.760168611763067,
					-4.055239090682342
				],
				[
					12.165717272046823,
					-4.460756811946781
				],
				[
					12.165717272046823,
					-6.082858636023492
				],
				[
					10.949133169234269,
					-8.110478181364684
				],
				[
					8.110478181364119,
					-6.893925017571324
				],
				[
					5.271823193494614,
					-4.460756811946781
				],
				[
					2.4331063275863953,
					-0.4055177212644396
				],
				[
					2.8386549878695053,
					2.83865498787007
				],
				[
					6.082858636023412,
					4.460756811946781
				],
				[
					10.138097726705471,
					4.460756811946781
				],
				[
					12.165717272046823,
					4.055239090682342
				],
				[
					14.193336817388175,
					3.649721369417902
				],
				[
					14.598823599633219,
					3.649721369417902
				],
				[
					15.409920920200085,
					3.2441727091345096
				],
				[
					15.409920920200085,
					3.2441727091345096
				]
			],
			"pressures": [
				0.30859375,
				0.431640625,
				0.4619140625,
				0.4599609375,
				0.46484375,
				0.466796875,
				0.4453125,
				0.4580078125,
				0.4873046875,
				0.5234375,
				0.556640625,
				0.5703125,
				0.5810546875,
				0.5810546875,
				0.533203125,
				0.4482421875,
				0.1220703125,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				21.714303152901266,
				4.571402413504472
			]
		},
		{
			"id": "5GavZ6GWfbwJK3NSdrR7A",
			"type": "freedraw",
			"x": 8164.408945440891,
			"y": 470.10904714875676,
			"width": 11.760230489801135,
			"height": 14.193336817388175,
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
			"seed": 1046723172,
			"version": 71,
			"versionNonce": 1184168540,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230240487,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					4.8662745332108575,
					-8.921544562912516
				],
				[
					8.516026841647873,
					-12.976783653594817
				],
				[
					8.921513623893562,
					-13.787819096123735
				],
				[
					10.138097726705471,
					-10.949164108253665
				],
				[
					10.138097726705471,
					-6.893925017571324
				],
				[
					10.949133169234916,
					-3.244203648153422
				],
				[
					11.35468182951738,
					-1.622101824076711
				],
				[
					11.35468182951738,
					0.4055177212644396
				],
				[
					11.760230489801135,
					0.4055177212644396
				],
				[
					11.760230489801135,
					0.4055177212644396
				]
			],
			"pressures": [
				0.359375,
				0.5361328125,
				0.5380859375,
				0.5380859375,
				0.5380859375,
				0.55859375,
				0.5673828125,
				0.5673828125,
				0.5078125,
				0.021484375,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				16.571480887276266,
				0.5714198521205276
			]
		},
		{
			"id": "AN8igTJIHh3mJASp5yHoy",
			"type": "freedraw",
			"x": 8195.22878728129,
			"y": 446.58864804719167,
			"width": 16.220956362728238,
			"height": 25.14250092564184,
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
			"seed": 1767219044,
			"version": 73,
			"versionNonce": 1427335524,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230240487,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-9.327062284176026,
					0.811066381547832
				],
				[
					-13.787850035142487,
					0.811066381547832
				],
				[
					-13.787850035142487,
					0.4055177212644396
				],
				[
					-12.165717272046823,
					0
				],
				[
					-11.35468182951738,
					3.649721369417902
				],
				[
					-13.787850035142487,
					8.921544562912516
				],
				[
					-16.220956362728238,
					16.220956362729368
				],
				[
					-13.787850035142487,
					23.11488138030069
				],
				[
					-10.949133169233624,
					24.73695226535849
				],
				[
					-9.732610944459783,
					25.14250092564184
				],
				[
					-6.488407296306522,
					23.52039910156513
				],
				[
					-6.488407296306522,
					23.52039910156513
				]
			],
			"pressures": [
				0.2802734375,
				0.4677734375,
				0.5380859375,
				0.5517578125,
				0.544921875,
				0.515625,
				0.51953125,
				0.5537109375,
				0.572265625,
				0.578125,
				0.548828125,
				0.0146484375,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				-9.142892020088766,
				33.14287458147322
			]
		},
		{
			"id": "W1ehrXjabRKrRj_onxPyr",
			"type": "freedraw",
			"x": 8204.555849565468,
			"y": 458.3488475979742,
			"width": 3.6496904303989495,
			"height": 12.976752714575904,
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
			"seed": 430544868,
			"version": 70,
			"versionNonce": 1195200220,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230240487,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.4055486602837555,
					-0.8110354425289195
				],
				[
					0,
					0.4055177212644396
				],
				[
					0,
					4.055239090682342
				],
				[
					-1.622132763095664,
					8.110478181364643
				],
				[
					-2.433168205623817,
					10.543615447970273
				],
				[
					-2.0276195453413526,
					11.760199550782545
				],
				[
					-1.622132763095664,
					12.165717272046985
				],
				[
					1.2165222247751322,
					10.543615447970273
				],
				[
					1.2165222247751322,
					10.543615447970273
				]
			],
			"pressures": [
				0.26953125,
				0.47265625,
				0.513671875,
				0.5341796875,
				0.55859375,
				0.5673828125,
				0.5693359375,
				0.5205078125,
				0.013671875,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				1.714215959822468,
				14.857134137834805
			]
		},
		{
			"id": "JLM4-Vdn_iLHehNADfbGk",
			"type": "freedraw",
			"x": 8204.961336347715,
			"y": 436.45055032048583,
			"width": 3.6496904303989495,
			"height": 2.0276195453411505,
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
			"seed": 593661660,
			"version": 67,
			"versionNonce": 1361616100,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230240487,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-1.622070885057597,
					-1.622101824076711
				],
				[
					-1.622070885057597,
					-2.0276195453411505
				],
				[
					-2.4331063275870406,
					-1.622101824076711
				],
				[
					-3.6496904303989495,
					-1.2165531637933187
				],
				[
					0,
					0
				]
			],
			"pressures": [
				0.2880859375,
				0.5029296875,
				0.490234375,
				0.375,
				0.109375,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				-5.142822265625,
				-1.7142595563615828
			]
		},
		{
			"id": "zmjNre4yGMXihurgXgN3B",
			"type": "freedraw",
			"x": 8223.615399038028,
			"y": 446.9941657684561,
			"width": 3.244203648153261,
			"height": 15.409920920200447,
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
			"seed": 1043272932,
			"version": 68,
			"versionNonce": 686232412,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230240487,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.8110973205662201,
					5.271823193494614
				],
				[
					1.622132763095664,
					8.110478181364643
				],
				[
					2.433168205623817,
					10.949164108253665
				],
				[
					2.8387168659075726,
					13.382301374859257
				],
				[
					3.244203648153261,
					15.004403198935968
				],
				[
					3.244203648153261,
					15.409920920200447
				],
				[
					3.244203648153261,
					15.409920920200447
				]
			],
			"pressures": [
				0.2900390625,
				0.5146484375,
				0.53515625,
				0.552734375,
				0.552734375,
				0.5009765625,
				0.4833984375,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				4.571446010044383,
				21.714303152901778
			]
		},
		{
			"id": "h_V_sjutAWdWVZpjlhhLl",
			"type": "freedraw",
			"x": 8220.371257267912,
			"y": 454.69912622855634,
			"width": 13.382239496820665,
			"height": 1.622101824076711,
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
			"seed": 2050854236,
			"version": 70,
			"versionNonce": 189489252,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230240487,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.4054867822443975,
					0
				],
				[
					3.244141770115194,
					0
				],
				[
					6.488345418268454,
					-0.4055177212644396
				],
				[
					9.732549066421715,
					0
				],
				[
					11.354619951479313,
					0
				],
				[
					12.165717272046823,
					0
				],
				[
					12.571204054292512,
					0.4055177212644396
				],
				[
					13.382239496820665,
					1.2165841028122715
				],
				[
					13.382239496820665,
					1.2165841028122715
				]
			],
			"pressures": [
				0.2109375,
				0.419921875,
				0.5087890625,
				0.513671875,
				0.513671875,
				0.4931640625,
				0.4033203125,
				0.189453125,
				0.0126953125,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				18.857073102677532,
				1.7143031529017776
			]
		},
		{
			"id": "hFc7IXlQ-ls6L1BLLQzeG",
			"type": "freedraw",
			"x": 8239.430868618512,
			"y": 442.53340895650933,
			"width": 5.271823193494614,
			"height": 21.08723089594059,
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
			"seed": 1660749796,
			"version": 72,
			"versionNonce": 702826460,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230240487,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.40548678224568835,
					-0.8110354425289195
				],
				[
					1.2165841028119084,
					4.866305472230134
				],
				[
					2.0276195453413526,
					12.571234993311425
				],
				[
					2.4331063275870406,
					14.193336817388136
				],
				[
					3.244203648153261,
					17.4375404655416
				],
				[
					3.244203648153261,
					18.654093629334916
				],
				[
					3.6496904303989495,
					19.465160010882748
				],
				[
					4.055239090682705,
					20.276195453411667
				],
				[
					4.460725872927102,
					20.276195453411667
				],
				[
					5.271823193494614,
					19.87067773214723
				],
				[
					5.271823193494614,
					19.87067773214723
				]
			],
			"pressures": [
				0.2880859375,
				0.47265625,
				0.5341796875,
				0.56640625,
				0.5732421875,
				0.58984375,
				0.587890625,
				0.5439453125,
				0.45703125,
				0.0654296875,
				0.0126953125,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				7.4285888671875,
				28.000008719308028
			]
		},
		{
			"id": "5Hce9D18YlL-tannuj77A",
			"type": "freedraw",
			"x": 8243.891594491439,
			"y": 435.6395148779569,
			"width": 16.220956362729527,
			"height": 37.30818725866991,
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
			"seed": 1951654748,
			"version": 81,
			"versionNonce": 189379556,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230240487,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					7.704991399119721,
					-2.0276195453411505
				],
				[
					11.760230489802426,
					-2.8386859268889824
				],
				[
					13.787850035143778,
					-3.6497213694179016
				],
				[
					14.193336817388175,
					-3.6497213694179016
				],
				[
					14.193336817388175,
					-4.055239090682341
				],
				[
					15.004434137955688,
					-2.0276195453411505
				],
				[
					15.004434137955688,
					2.8386549878700698
				],
				[
					15.815469580483839,
					11.354650890499192
				],
				[
					16.220956362729527,
					19.46512907186383
				],
				[
					15.815469580483839,
					25.953536368170717
				],
				[
					15.004434137955688,
					30.00877545885306
				],
				[
					14.193336817388175,
					30.81981090138194
				],
				[
					12.976814592614334,
					32.441912725458685
				],
				[
					10.949195047272982,
					33.25294816798757
				],
				[
					10.138097726706762,
					33.25294816798757
				],
				[
					8.11047818136541,
					33.25294816798757
				],
				[
					7.299442738835966,
					33.25294816798757
				],
				[
					6.082858636024057,
					32.441912725458685
				],
				[
					5.677371853778369,
					31.225328622646416
				],
				[
					5.677371853778369,
					31.225328622646416
				]
			],
			"pressures": [
				0.234375,
				0.3408203125,
				0.4140625,
				0.4482421875,
				0.4658203125,
				0.4921875,
				0.5234375,
				0.5234375,
				0.525390625,
				0.525390625,
				0.5419921875,
				0.56640625,
				0.568359375,
				0.580078125,
				0.5947265625,
				0.59765625,
				0.5869140625,
				0.5439453125,
				0.439453125,
				0.015625,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				8.000052315848734,
				43.999982561383945
			]
		},
		{
			"id": "0XThFINIGcXfP8i6P5EwR",
			"type": "freedraw",
			"x": 8274.305887671557,
			"y": 450.23836941660954,
			"width": 15.409920920201374,
			"height": 1.622101824076711,
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
			"seed": 1736193244,
			"version": 68,
			"versionNonce": 1850141788,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230240487,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					4.055239090682705,
					-0.4055177212644396
				],
				[
					5.271823193494614,
					-0.8110354425288792
				],
				[
					10.543646386989227,
					-1.2165841028122715
				],
				[
					13.787850035142487,
					-1.2165841028122715
				],
				[
					15.409920920201374,
					-1.622101824076711
				],
				[
					14.598885477671931,
					-1.2165841028122715
				],
				[
					14.598885477671931,
					-1.2165841028122715
				]
			],
			"pressures": [
				0.2880859375,
				0.53515625,
				0.546875,
				0.5537109375,
				0.5556640625,
				0.525390625,
				0.015625,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				20.571463448661234,
				-1.7143031529017776
			]
		},
		{
			"id": "ulAFfG5i4S5sUy7g4fDjC",
			"type": "freedraw",
			"x": 8311.614136808264,
			"y": 465.64832127582895,
			"width": 5.677309975740302,
			"height": 34.469532270799846,
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
			"seed": 156140772,
			"version": 72,
			"versionNonce": 791779172,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230240487,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1.622070885057597,
					-6.082858636023492
				],
				[
					1.2165222247751322,
					-13.787819096123696
				],
				[
					-0.4055486602837555,
					-21.89829727748838
				],
				[
					-2.0276195453413526,
					-28.38667363477635
				],
				[
					-2.433168205623817,
					-31.225359561665336
				],
				[
					-2.8387168659075726,
					-34.469532270799846
				],
				[
					-3.244203648153261,
					-34.469532270799846
				],
				[
					-3.6497523084370163,
					-31.630877282929774
				],
				[
					-4.055239090682705,
					-26.7645718106996
				],
				[
					-2.433168205623817,
					-21.49277955622394
				],
				[
					-2.433168205623817,
					-21.49277955622394
				]
			],
			"pressures": [
				0.234375,
				0.4765625,
				0.5537109375,
				0.5791015625,
				0.5830078125,
				0.5830078125,
				0.5771484375,
				0.55859375,
				0.4375,
				0.2578125,
				0.013671875,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				-3.428606305802532,
				-30.285731724330333
			]
		},
		{
			"id": "K7KQ-q1fzzDi9t3RRL2OB",
			"type": "freedraw",
			"x": 8322.157721317217,
			"y": 446.994227646494,
			"width": 19.059611350600324,
			"height": 15.815407702445974,
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
			"seed": 1403680348,
			"version": 85,
			"versionNonce": 1205928156,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230240487,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					4.866274533212149,
					-2.838685926888983
				],
				[
					4.46078775096646,
					-4.055239090682301
				],
				[
					3.6497523084370163,
					-4.460787750965694
				],
				[
					0.4055486602837555,
					-4.866305472230134
				],
				[
					-2.43310632758575,
					-2.0276195453411505
				],
				[
					-3.6496904303989495,
					2.433137266605631
				],
				[
					-2.8386549878695053,
					4.866274533211262
				],
				[
					-1.622070885057597,
					7.299411799816851
				],
				[
					0.8110354425294439,
					8.921513623893562
				],
				[
					3.244203648153261,
					9.732549066422482
				],
				[
					6.4884072963078125,
					8.921513623893562
				],
				[
					6.4884072963078125,
					7.299411799816851
				],
				[
					6.4884072963078125,
					5.67730997574014
				],
				[
					6.8938940785522105,
					2.83865498787007
				],
				[
					8.921513623893562,
					-3.244203648153422
				],
				[
					11.760230489802426,
					-6.082858636023492
				],
				[
					12.976752714576268,
					-4.866305472230134
				],
				[
					12.976752714576268,
					-1.622101824076711
				],
				[
					12.57126593233058,
					2.433137266605631
				],
				[
					13.382301374860022,
					6.082858636023532
				],
				[
					13.787850035142487,
					7.299411799816851
				],
				[
					14.193336817388175,
					8.515995902629124
				],
				[
					15.409920920201374,
					9.732549066422482
				],
				[
					15.409920920201374,
					9.732549066422482
				]
			],
			"pressures": [
				0.26953125,
				0.376953125,
				0.435546875,
				0.455078125,
				0.48046875,
				0.5,
				0.5205078125,
				0.5234375,
				0.525390625,
				0.5048828125,
				0.423828125,
				0.013671875,
				0.060546875,
				0.1796875,
				0.3623046875,
				0.4990234375,
				0.5126953125,
				0.5341796875,
				0.55078125,
				0.5615234375,
				0.568359375,
				0.55859375,
				0.51171875,
				0.03125,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				21.714303152903085,
				13.714250837053612
			]
		},
		{
			"id": "LIg0AMI7iWU15i4hzYBtm",
			"type": "freedraw",
			"x": 8358.249386351112,
			"y": 430.77327128376464,
			"width": 15.004434137955688,
			"height": 26.359054089435162,
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
			"seed": 64577756,
			"version": 76,
			"versionNonce": 1666255588,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230240487,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-11.35468182951867,
					0.4055177212644396
				],
				[
					-10.949195047272982,
					-0.811066381547832
				],
				[
					-8.92157550193163,
					-0.4055486602833924
				],
				[
					-8.92157550193163,
					0.8110354425288792
				],
				[
					-13.382301374860022,
					9.327031345158002
				],
				[
					-15.004434137955688,
					14.598854538652615
				],
				[
					-15.004434137955688,
					15.815407702445974
				],
				[
					-13.382301374860022,
					17.437509526522685
				],
				[
					-8.11047818136541,
					20.68171317467611
				],
				[
					-6.082858636024057,
					23.11485044128174
				],
				[
					-6.082858636024057,
					23.520368162546177
				],
				[
					-5.271823193494614,
					24.33143454409401
				],
				[
					-4.46078775096646,
					25.14246998662289
				],
				[
					-3.6497523084370163,
					25.54798770788733
				],
				[
					-3.6497523084370163,
					25.54798770788733
				]
			],
			"pressures": [
				0.330078125,
				0.5009765625,
				0.5107421875,
				0.49609375,
				0.49609375,
				0.498046875,
				0.5126953125,
				0.5166015625,
				0.5166015625,
				0.5224609375,
				0.525390625,
				0.517578125,
				0.4716796875,
				0.3310546875,
				0.2255859375,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				-5.142909458705617,
				35.99997384207586
			]
		},
		{
			"id": "iIE-uMsdAfkI2ixO5eQMI",
			"type": "freedraw",
			"x": 8369.604006302592,
			"y": 440.5058203501871,
			"width": 1.622132763095664,
			"height": 15.815438641464887,
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
			"seed": 1170900708,
			"version": 66,
			"versionNonce": 2118419804,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230240487,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.8110354425294439,
					8.921544562912516
				],
				[
					-0.40548678224568835,
					10.543646386989227
				],
				[
					0,
					13.382301374859297
				],
				[
					0.8110973205662201,
					15.815438641464887
				],
				[
					0.8110973205662201,
					15.815438641464887
				]
			],
			"pressures": [
				0.353515625,
				0.51171875,
				0.51171875,
				0.5009765625,
				0.123046875,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				1.142926897320649,
				22.285723005022305
			]
		},
		{
			"id": "uzwnbEGzkF9VUj6MGDjgy",
			"type": "freedraw",
			"x": 8369.198519520347,
			"y": 426.3124835327989,
			"width": 4.055239090682705,
			"height": 2.027619545341191,
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
			"seed": 1874753244,
			"version": 66,
			"versionNonce": 1513492068,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230240487,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-1.2165841028131996,
					-0.4055177212644396
				],
				[
					-0.811035442529444,
					0
				],
				[
					2.8386549878695058,
					1.6221018240767515
				],
				[
					0,
					0
				]
			],
			"pressures": [
				0.359375,
				0.4306640625,
				0.4560546875,
				0.0126953125,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				3.999982561383149,
				2.285723005022362
			]
		},
		{
			"id": "vE60MRSkh2kNkUOTosOpK",
			"type": "freedraw",
			"x": 8375.28137815637,
			"y": 419.0130562634726,
			"width": 17.843027247787123,
			"height": 42.580025921674,
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
			"seed": 227929956,
			"version": 76,
			"versionNonce": 381909468,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230240487,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					7.299442738835965,
					2.0276195453411905
				],
				[
					13.38230137486002,
					1.2165841028123117
				],
				[
					15.409920920201372,
					0.4055331907739159
				],
				[
					15.409920920201372,
					1.6221018240767513
				],
				[
					15.004372259917618,
					6.0828741055330084
				],
				[
					15.004372259917618,
					11.76021502029206
				],
				[
					16.626443144975212,
					22.303830468262333
				],
				[
					17.843027247787123,
					28.792206825550302
				],
				[
					16.220956362729524,
					34.46954774030935
				],
				[
					12.976752714576266,
					38.524786830991694
				],
				[
					11.354681829518668,
					40.14688865506841
				],
				[
					9.327062284177316,
					40.957924097597285
				],
				[
					7.704929521081652,
					41.76895954012617
				],
				[
					0.4054867822456883,
					42.580025921674
				],
				[
					0.4054867822456883,
					42.580025921674
				]
			],
			"pressures": [
				0.357421875,
				0.4140625,
				0.4443359375,
				0.462890625,
				0.513671875,
				0.5205078125,
				0.5224609375,
				0.5224609375,
				0.5224609375,
				0.5263671875,
				0.5498046875,
				0.5615234375,
				0.55859375,
				0.5078125,
				0.013671875,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				0.571376255580617,
				60.0000217982701
			]
		},
		{
			"id": "yd0RcWq9zPf8zZSmGRYvN",
			"type": "freedraw",
			"x": 8152.243166290804,
			"y": 529.7210803451985,
			"width": 3.2442036481539063,
			"height": 30.41429318011746,
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
			"seed": 829590748,
			"version": 86,
			"versionNonce": 1152295396,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230240487,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.4055486602837555,
					1.2165841028123119
				],
				[
					1.216584102812554,
					-2.83865498787007
				],
				[
					0.8110354425294439,
					-9.327031345158042
				],
				[
					0.4055486602837555,
					-16.626474083993806
				],
				[
					-0.40548678224568835,
					-24.73695226535849
				],
				[
					-0.8110354425287984,
					-27.17008953196408
				],
				[
					-0.8110354425287984,
					-26.3590540894352
				],
				[
					-0.40548678224568835,
					-14.193336817388175
				],
				[
					0.4055486602837555,
					-4.055239090682301
				],
				[
					0.4055486602837555,
					2.4331372666055904
				],
				[
					0.4055486602837555,
					2.8386859268889424
				],
				[
					-0.8110354425287984,
					1.622101824076711
				],
				[
					-1.622070885057597,
					-6.082858636023532
				],
				[
					-2.0276195453413526,
					-12.165717272047026
				],
				[
					-2.0276195453413526,
					-15.815438641464928
				],
				[
					-1.622070885057597,
					-25.953536368170763
				],
				[
					-1.2165841028119084,
					-27.57560725322852
				],
				[
					-0.40548678224568835,
					-24.73695226535849
				],
				[
					0,
					-19.059611350599436
				],
				[
					0,
					-15.815438641464928
				],
				[
					0.4055486602837555,
					-8.921513623893562
				],
				[
					0.8110354425294439,
					-4.055239090682301
				],
				[
					1.216584102812554,
					2.8386859268889424
				],
				[
					0,
					0
				]
			],
			"pressures": [
				0.17578125,
				0.1943359375,
				0.509765625,
				0.5546875,
				0.5703125,
				0.572265625,
				0.578125,
				0.5703125,
				0.5439453125,
				0.5244140625,
				0.5146484375,
				0.5126953125,
				0.5712890625,
				0.6005859375,
				0.60546875,
				0.60546875,
				0.59765625,
				0.595703125,
				0.580078125,
				0.5693359375,
				0.5673828125,
				0.5146484375,
				0.3740234375,
				0.0146484375,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				1.7143031529021755,
				4.000026157924026
			]
		},
		{
			"id": "sXGjA7Rvj4DnYh_pM_1vJ",
			"type": "freedraw",
			"x": 8140.482935801003,
			"y": 511.06698671586355,
			"width": 10.138097726705471,
			"height": 11.354681829518105,
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
			"seed": 162843748,
			"version": 70,
			"versionNonce": 477093468,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230240487,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					3.244203648153261,
					-2.83865498787007
				],
				[
					6.8938940785522105,
					-6.488376357287932
				],
				[
					7.299442738835966,
					-6.893894078552371
				],
				[
					9.732610944460427,
					-10.543615447970273
				],
				[
					10.138097726705471,
					-10.949133169234713
				],
				[
					10.138097726705471,
					-11.354681829518105
				],
				[
					9.327062284176673,
					-10.138097726705833
				],
				[
					8.110478181364764,
					-6.893894078552371
				],
				[
					8.110478181364764,
					-6.893894078552371
				]
			],
			"pressures": [
				0.224609375,
				0.4375,
				0.5078125,
				0.5107421875,
				0.5234375,
				0.525390625,
				0.51171875,
				0.361328125,
				0.0146484375,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				11.428571428571558,
				-9.71426827566961
			]
		},
		{
			"id": "g5P1YH9ms2WcPd1D7l-62",
			"type": "freedraw",
			"x": 8139.671900358474,
			"y": 532.9652839933519,
			"width": 29.603257737588905,
			"height": 6.082858636023573,
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
			"seed": 1980674652,
			"version": 72,
			"versionNonce": 164152676,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230240487,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-3.2442036481539063,
					0.4055177212644799
				],
				[
					3.244203648153261,
					-1.2165841028123119
				],
				[
					5.677309975739656,
					-2.027619545341191
				],
				[
					12.571265932329933,
					-3.244203648153422
				],
				[
					20.6817441136947,
					-4.460756811946781
				],
				[
					22.30381499875294,
					-5.271823193494614
				],
				[
					25.142469986622444,
					-5.677340914759093
				],
				[
					25.95350542915189,
					-5.677340914759093
				],
				[
					26.359054089435,
					-5.677340914759093
				],
				[
					25.95350542915189,
					-5.271823193494614
				],
				[
					25.95350542915189,
					-5.271823193494614
				]
			],
			"pressures": [
				0.2490234375,
				0.3876953125,
				0.513671875,
				0.5185546875,
				0.5146484375,
				0.5234375,
				0.5234375,
				0.5234375,
				0.5107421875,
				0.4970703125,
				0.015625,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				36.57139369419656,
				-7.4285888671875
			]
		},
		{
			"id": "b-yCgBKSxjTWuNwenmfW1",
			"type": "freedraw",
			"x": 8018.014727638001,
			"y": 583.6558035659001,
			"width": 20.68174411369534,
			"height": 26.76457181069964,
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
			"seed": 1398658660,
			"version": 81,
			"versionNonce": 1746645724,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230240487,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					2.4331682056251074,
					-1.622101824076711
				],
				[
					3.6496904303989486,
					-2.8386859268889424
				],
				[
					7.299442738835965,
					-7.704960460100203
				],
				[
					7.704929521081652,
					-11.354681829518105
				],
				[
					7.299442738835965,
					-12.571234993311464
				],
				[
					3.6496904303989486,
					-15.815438641464887
				],
				[
					1.2165841028125537,
					-17.4375404655416
				],
				[
					1.6220708850582422,
					-16.220956362729286
				],
				[
					6.082858636024056,
					-10.543615447970273
				],
				[
					15.004372259917618,
					-4.460756811946781
				],
				[
					20.276195453412228,
					0
				],
				[
					18.248575908070876,
					4.055239090682382
				],
				[
					12.976752714576266,
					6.488376357287972
				],
				[
					9.732549066423005,
					7.299411799816851
				],
				[
					4.866274533211502,
					8.110478181364684
				],
				[
					0.8110354425294437,
					8.110478181364684
				],
				[
					0,
					8.110478181364684
				],
				[
					-0.40554866028311,
					8.515995902629163
				],
				[
					2.027619545341352,
					9.327031345158042
				],
				[
					2.027619545341352,
					9.327031345158042
				]
			],
			"pressures": [
				0.1923828125,
				0.2939453125,
				0.330078125,
				0.38671875,
				0.40625,
				0.427734375,
				0.4921875,
				0.5302734375,
				0.5517578125,
				0.533203125,
				0.5263671875,
				0.5224609375,
				0.5322265625,
				0.57421875,
				0.595703125,
				0.6162109375,
				0.62109375,
				0.61328125,
				0.5595703125,
				0.015625,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				2.857142857143117,
				13.142830984933084
			]
		},
		{
			"id": "TVoEdEbCM_9HL0NzI3rPh",
			"type": "freedraw",
			"x": 8043.968233067153,
			"y": 586.8999762750346,
			"width": 4.8662745332108575,
			"height": 22.303814998752777,
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
			"seed": 712318180,
			"version": 66,
			"versionNonce": 2127722724,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230240487,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-3.6496904303989495,
					10.543646386989227
				],
				[
					-4.460725872927748,
					13.382301374859297
				],
				[
					-4.8662745332108575,
					17.032022744277118
				],
				[
					-4.460725872927748,
					22.303814998752777
				],
				[
					-4.460725872927748,
					22.303814998752777
				]
			],
			"pressures": [
				0.322265625,
				0.50390625,
				0.5107421875,
				0.4931640625,
				0.0146484375,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				-6.2856619698659415,
				31.42857142857133
			]
		},
		{
			"id": "xURppJZ2zORDHOij--W6E",
			"type": "freedraw",
			"x": 8070.7328358168725,
			"y": 588.1165603778469,
			"width": 13.382301374859377,
			"height": 27.98115591351187,
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
			"seed": 1464631516,
			"version": 73,
			"versionNonce": 1750660956,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230240487,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-7.299442738835966,
					-2.0276195453411106
				],
				[
					-8.516026841647873,
					-5.677340914759013
				],
				[
					-5.271823193494614,
					-9.732580005441395
				],
				[
					-1.622070885057597,
					-12.571234993311464
				],
				[
					0.8110354425287984,
					-17.84305818680608
				],
				[
					-1.622070885057597,
					-23.52039910156509
				],
				[
					-8.110478181364764,
					-26.76457181069964
				],
				[
					-11.760168611763714,
					-27.98115591351187
				],
				[
					-12.165717272046823,
					-27.57563819224747
				],
				[
					-12.57126593233058,
					-26.359054089435162
				],
				[
					-11.760168611763714,
					-24.73695226535845
				],
				[
					-11.760168611763714,
					-24.73695226535845
				]
			],
			"pressures": [
				0.2255859375,
				0.462890625,
				0.5224609375,
				0.5283203125,
				0.5234375,
				0.5029296875,
				0.5,
				0.5244140625,
				0.5439453125,
				0.53515625,
				0.3974609375,
				0.0146484375,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				-16.57139369419656,
				-34.857134137834805
			]
		},
		{
			"id": "fuV4lTqaobHVUh57aoASX",
			"type": "freedraw",
			"x": 8015.98710809266,
			"y": 603.9319990193118,
			"width": 34.87508093108352,
			"height": 26.35905408943524,
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
			"seed": 552292444,
			"version": 81,
			"versionNonce": 525974628,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230240487,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.4055486602837555,
					1.216553163793359
				],
				[
					0.40554866028311004,
					4.460756811946781
				],
				[
					1.622070885057597,
					8.515995902629163
				],
				[
					2.838654987870151,
					11.354650890499233
				],
				[
					3.244203648153261,
					12.165717272047065
				],
				[
					6.082858636023412,
					14.598854538652656
				],
				[
					10.138097726705471,
					15.004372259917055
				],
				[
					16.220956362728884,
					12.571234993311464
				],
				[
					20.6817441136947,
					8.515995902629163
				],
				[
					23.11485044128174,
					5.271792254475661
				],
				[
					24.331434544093646,
					4.460756811946781
				],
				[
					26.359054089435,
					7.299411799816851
				],
				[
					28.38667363477635,
					10.543615447970273
				],
				[
					29.19770907730515,
					12.165717272047065
				],
				[
					30.008744519833947,
					15.815438641464887
				],
				[
					29.60325773758826,
					20.276195453411667
				],
				[
					30.008744519833947,
					23.11485044128174
				],
				[
					31.2253286226465,
					25.54798770788741
				],
				[
					34.46953227079976,
					26.35905408943524
				],
				[
					34.46953227079976,
					26.35905408943524
				]
			],
			"pressures": [
				0.2060546875,
				0.4091796875,
				0.4521484375,
				0.4658203125,
				0.474609375,
				0.4765625,
				0.48046875,
				0.482421875,
				0.4951171875,
				0.4970703125,
				0.4970703125,
				0.505859375,
				0.5087890625,
				0.5087890625,
				0.5087890625,
				0.513671875,
				0.521484375,
				0.49609375,
				0.330078125,
				0.013671875,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				48.57142857142844,
				37.142857142857224
			]
		},
		{
			"id": "RzvHZJwakcofJ1z8UyTL6",
			"type": "freedraw",
			"x": 8080.059898101048,
			"y": 597.0380740017404,
			"width": 33.65849682827096,
			"height": 38.52477136148222,
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
			"seed": 624017884,
			"version": 80,
			"versionNonce": 1769581532,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230240487,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-2.8386549878695053,
					7.299442738835804
				],
				[
					-6.8938940785522105,
					12.571265932330418
				],
				[
					-10.949133169234269,
					14.598885477671608
				],
				[
					-15.815469580483839,
					13.787819096123776
				],
				[
					-17.843089125824548,
					11.760199550782586
				],
				[
					-18.654124568353346,
					10.138097726705874
				],
				[
					-19.059611350599035,
					9.327062284176995
				],
				[
					-20.27619545341159,
					9.327062284176995
				],
				[
					-22.70936365903605,
					11.354681829518105
				],
				[
					-26.359054089435,
					16.220956362729368
				],
				[
					-30.008806397872014,
					20.6817441136951
				],
				[
					-30.41429318011706,
					21.89829727748838
				],
				[
					-32.84746138574152,
					25.953536368170763
				],
				[
					-33.65849682827096,
					30.819841840400894
				],
				[
					-32.03642594321272,
					33.65849682827096
				],
				[
					-30.41429318011706,
					35.28059865234768
				],
				[
					-29.19770907730515,
					36.091634094876554
				],
				[
					-27.575638192246906,
					38.52477136148222
				],
				[
					-27.575638192246906,
					38.52477136148222
				]
			],
			"pressures": [
				0.2255859375,
				0.3623046875,
				0.4345703125,
				0.4873046875,
				0.4990234375,
				0.5078125,
				0.509765625,
				0.509765625,
				0.509765625,
				0.501953125,
				0.5,
				0.515625,
				0.5185546875,
				0.52734375,
				0.5400390625,
				0.54296875,
				0.5224609375,
				0.4521484375,
				0.0126953125,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				-38.85716029575815,
				54.285714285714334
			]
		},
		{
			"id": "sxVRDtBZcPNcY63bXJ_b3",
			"type": "freedraw",
			"x": 8057.350534442012,
			"y": 678.1428558153872,
			"width": 22.303814998752294,
			"height": 25.54798770788733,
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
			"seed": 1937018084,
			"version": 74,
			"versionNonce": 1160548324,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230240487,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-9.327000406138605,
					-0.4055177212644799
				],
				[
					-12.976752714575621,
					-2.4331372666055904
				],
				[
					-13.38223949682131,
					-4.460756811946781
				],
				[
					-10.949133169234269,
					-8.921513623893562
				],
				[
					-6.8938940785522105,
					-13.382270435840343
				],
				[
					-6.082858636023412,
					-19.870646793128316
				],
				[
					-11.760168611763067,
					-23.925885883810697
				],
				[
					-15.815407702445773,
					-25.142469986622928
				],
				[
					-21.087230895940387,
					-25.54798770788733
				],
				[
					-22.303814998752294,
					-25.54798770788733
				],
				[
					-21.898266338469185,
					-25.142469986622928
				],
				[
					-15.409859042162017,
					-23.11485044128174
				],
				[
					-15.409859042162017,
					-23.11485044128174
				]
			],
			"pressures": [
				0.232421875,
				0.5166015625,
				0.5751953125,
				0.5986328125,
				0.5927734375,
				0.57421875,
				0.5419921875,
				0.56640625,
				0.587890625,
				0.60546875,
				0.599609375,
				0.5546875,
				0.0146484375,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				-21.71421595982065,
				-32.5714111328125
			]
		},
		{
			"id": "g4H665RdUrKG4TLJWV-mm",
			"type": "freedraw",
			"x": 8089.792447167471,
			"y": 676.115236270046,
			"width": 19.46516001088279,
			"height": 22.70933272001734,
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
			"seed": 1725481692,
			"version": 66,
			"versionNonce": 1569706076,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230240487,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					9.73261094446043,
					-9.327031345157963
				],
				[
					18.248575908070237,
					-16.626474083993767
				],
				[
					19.46516001088279,
					-19.465129071863835
				],
				[
					13.78785003514249,
					-22.70933272001734
				],
				[
					13.78785003514249,
					-22.70933272001734
				]
			],
			"pressures": [
				0.3359375,
				0.5107421875,
				0.513671875,
				0.3740234375,
				0.0146484375,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				19.428623744419383,
				-31.99999128069203
			]
		},
		{
			"id": "CpDK5moiwhQyj0m3tvw0V",
			"type": "freedraw",
			"x": 8096.280854463777,
			"y": 655.0280053741054,
			"width": 18.24857590807088,
			"height": 19.059611350599358,
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
			"seed": 670753636,
			"version": 67,
			"versionNonce": 1616442212,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230240487,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					8.110478181364764,
					9.327062284176916
				],
				[
					13.382301374859377,
					12.571234993311386
				],
				[
					15.815407702446418,
					14.598854538652578
				],
				[
					17.031991805258325,
					17.03199180525817
				],
				[
					18.24857590807088,
					19.059611350599358
				],
				[
					18.24857590807088,
					19.059611350599358
				]
			],
			"pressures": [
				0.4453125,
				0.548828125,
				0.5517578125,
				0.5126953125,
				0.369140625,
				0.0146484375,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				25.714285714286234,
				26.85712541852672
			]
		},
		{
			"id": "o_Ss_yzZttvGqj0cLHcH_",
			"type": "freedraw",
			"x": 8148.593475860402,
			"y": 671.2489617368348,
			"width": 3.244203648153261,
			"height": 34.064014549535365,
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
			"seed": 495718756,
			"version": 70,
			"versionNonce": 611149020,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230240487,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1.622132763095664,
					-7.299442738835804
				],
				[
					1.622132763095664,
					-13.787819096123696
				],
				[
					0.40554866028311004,
					-22.709332720017258
				],
				[
					-1.216584102812554,
					-31.225359561665293
				],
				[
					-1.622070885057597,
					-34.064014549535365
				],
				[
					-1.622070885057597,
					-32.84743044672313
				],
				[
					-1.622070885057597,
					-29.60325773758858
				],
				[
					-1.216584102812554,
					-23.11488138030069
				],
				[
					-1.216584102812554,
					-23.11488138030069
				]
			],
			"pressures": [
				0.2060546875,
				0.4521484375,
				0.54296875,
				0.5654296875,
				0.5673828125,
				0.54296875,
				0.4384765625,
				0.3076171875,
				0.0146484375,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				-1.7143031529021755,
				-32.571454729352695
			]
		},
		{
			"id": "bdqdVG3HFi6nycVj3qn4e",
			"type": "freedraw",
			"x": 8159.948157689921,
			"y": 658.27217808324,
			"width": 23.11491231932045,
			"height": 15.004372259917055,
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
			"seed": 1717787996,
			"version": 84,
			"versionNonce": 791471844,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230240487,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					5.677309975740302,
					-3.24417270913455
				],
				[
					8.921513623893562,
					-5.271792254475661
				],
				[
					6.8938940785522105,
					-6.488376357287972
				],
				[
					3.244203648153261,
					-6.893894078552371
				],
				[
					-0.40554866028311004,
					-4.460756811946781
				],
				[
					-2.4331682056244626,
					-0.8110354425288792
				],
				[
					-2.4331682056244626,
					2.433168205624543
				],
				[
					-2.0276195453413526,
					3.649721369417902
				],
				[
					0,
					5.271823193494614
				],
				[
					2.0276195453413526,
					7.299442738835804
				],
				[
					5.677309975740302,
					8.110478181364684
				],
				[
					6.082858636024057,
					5.677340914759013
				],
				[
					6.488407296307167,
					2.838685926889023
				],
				[
					9.327062284177318,
					-2.83865498787007
				],
				[
					10.543646386989227,
					-4.460756811946781
				],
				[
					12.57126593233058,
					-6.488376357287972
				],
				[
					13.78778815710571,
					-6.082858636023492
				],
				[
					15.00437225991762,
					-2.027619545341191
				],
				[
					15.815407702445773,
					2.433168205624543
				],
				[
					17.031991805258972,
					4.055239090682301
				],
				[
					17.843027247787123,
					5.271823193494614
				],
				[
					20.681744113695988,
					4.055239090682301
				],
				[
					20.681744113695988,
					4.055239090682301
				]
			],
			"pressures": [
				0.294921875,
				0.451171875,
				0.4482421875,
				0.4345703125,
				0.4580078125,
				0.5068359375,
				0.5341796875,
				0.5478515625,
				0.54296875,
				0.521484375,
				0.43359375,
				0.0126953125,
				0.2041015625,
				0.4150390625,
				0.5146484375,
				0.521484375,
				0.5244140625,
				0.53125,
				0.5361328125,
				0.5439453125,
				0.529296875,
				0.4521484375,
				0.013671875,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				29.142892020090585,
				5.714285714285666
			]
		},
		{
			"id": "WT9KRRnQFDTCSD11XgeZf",
			"type": "freedraw",
			"x": 8252.002072672802,
			"y": 627.452367181858,
			"width": 18.24857590807088,
			"height": 39.33580680401102,
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
			"seed": 1110125148,
			"version": 76,
			"versionNonce": 961943260,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230240487,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					11.35468182951867,
					-3.6497213694179016
				],
				[
					13.787850035142487,
					-5.27179225447566
				],
				[
					16.220956362729527,
					-3.2441727091345496
				],
				[
					17.031991805258972,
					2.838685926888942
				],
				[
					17.84308912582519,
					10.949164108253624
				],
				[
					18.24857590807088,
					17.437540465541595
				],
				[
					18.24857590807088,
					21.898297277488375
				],
				[
					16.220956362729527,
					27.170120470982987
				],
				[
					13.787850035142487,
					31.22535956166529
				],
				[
					12.165717272046823,
					32.84743044672313
				],
				[
					10.138097726706762,
					34.06401454953536
				],
				[
					7.704991399119721,
					34.06401454953536
				],
				[
					7.299442738835966,
					33.65849682827096
				],
				[
					7.704991399119721,
					32.44191272545865
				],
				[
					7.704991399119721,
					32.44191272545865
				]
			],
			"pressures": [
				0.2626953125,
				0.326171875,
				0.3359375,
				0.3916015625,
				0.4443359375,
				0.49609375,
				0.5087890625,
				0.529296875,
				0.5546875,
				0.5703125,
				0.5810546875,
				0.5888671875,
				0.587890625,
				0.54296875,
				0.0146484375,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				10.857195172991851,
				45.714285714285666
			]
		},
		{
			"id": "VMrhRMYQUjMANQbIQeyD_",
			"type": "freedraw",
			"x": 8284.44398539826,
			"y": 643.6733235445872,
			"width": 15.00437225991762,
			"height": 2.4331372666055904,
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
			"seed": 1344116068,
			"version": 65,
			"versionNonce": 1071666404,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230240487,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					7.704991399119721,
					-0.8110354425288792
				],
				[
					13.382301374858733,
					-2.0276195453411106
				],
				[
					15.00437225991762,
					-2.4331372666055904
				],
				[
					15.00437225991762,
					-2.4331372666055904
				]
			],
			"pressures": [
				0.2568359375,
				0.47265625,
				0.498046875,
				0.4609375,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				21.14283970424185,
				-3.4285627092633604
			]
		},
		{
			"id": "gdO5BIkPVOz7vXCNH0DmS",
			"type": "freedraw",
			"x": 8316.88589812372,
			"y": 647.7285626352697,
			"width": 2.0276195453413526,
			"height": 27.17008953196412,
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
			"seed": 1945329636,
			"version": 68,
			"versionNonce": 1822874460,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230240487,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-1.2165841028131996,
					-10.949133169234754
				],
				[
					-1.2165841028131996,
					-19.870677732147268
				],
				[
					-1.2165841028131996,
					-22.30381499875286
				],
				[
					-0.811035442529444,
					-27.17008953196412
				],
				[
					-0.811035442529444,
					-26.76457181069964
				],
				[
					0.8110354425281531,
					-23.11485044128174
				],
				[
					0.8110354425281531,
					-23.11485044128174
				]
			],
			"pressures": [
				0.4365234375,
				0.5625,
				0.5673828125,
				0.5673828125,
				0.478515625,
				0.291015625,
				0.013671875,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				1.142839704240032,
				-32.5714111328125
			]
		},
		{
			"id": "QKQVB8miZZpdfdddzr9s2",
			"type": "freedraw",
			"x": 8333.10685448645,
			"y": 640.0236021751695,
			"width": 12.165717272046823,
			"height": 15.409889981181534,
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
			"seed": 1868362332,
			"version": 72,
			"versionNonce": 978065508,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230240487,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					2.433168205623817,
					-3.6496904303989495
				],
				[
					0,
					-5.271792254475741
				],
				[
					-3.244203648154552,
					-4.055239090682382
				],
				[
					-4.866274533212149,
					-2.83865498787007
				],
				[
					-8.11047818136541,
					0
				],
				[
					-9.732549066423006,
					4.055239090682301
				],
				[
					-8.515964963611097,
					8.110478181364602
				],
				[
					-5.677309975740302,
					10.138097726705794
				],
				[
					-2.0276195453413526,
					10.138097726705794
				],
				[
					2.0276195453400616,
					9.732580005441395
				],
				[
					2.0276195453400616,
					9.732580005441395
				]
			],
			"pressures": [
				0.2724609375,
				0.3232421875,
				0.3916015625,
				0.40625,
				0.4296875,
				0.48046875,
				0.5107421875,
				0.5126953125,
				0.494140625,
				0.341796875,
				0.0146484375,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				2.857142857141298,
				13.71429443359375
			]
		},
		{
			"id": "B7-ZGViglu9C4cAP3aPDo",
			"type": "freedraw",
			"x": 8337.567642237414,
			"y": 648.5396290168175,
			"width": 15.409920920200085,
			"height": 10.138097726705874,
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
			"seed": 969119332,
			"version": 71,
			"versionNonce": 1919619036,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230240487,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					2.0276195453413526,
					-4.460787750965734
				],
				[
					5.677309975740302,
					-8.921544562912516
				],
				[
					8.921513623893562,
					-10.138097726705874
				],
				[
					10.138097726705471,
					-8.516026841648035
				],
				[
					10.138097726705471,
					-6.893925017571324
				],
				[
					10.54358450895116,
					-5.677340914759093
				],
				[
					10.949133169234916,
					-4.460787750965734
				],
				[
					13.382301374858733,
					-4.460787750965734
				],
				[
					15.409920920200085,
					-6.893925017571324
				],
				[
					15.409920920200085,
					-6.893925017571324
				]
			],
			"pressures": [
				0.1533203125,
				0.474609375,
				0.53515625,
				0.5556640625,
				0.5771484375,
				0.5830078125,
				0.5732421875,
				0.5224609375,
				0.2646484375,
				0.013671875,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				21.714303152901266,
				-9.714311872209805
			]
		},
		{
			"id": "QdMRL8SaY78RSHGMOJKY2",
			"type": "freedraw",
			"x": 8370.009554962873,
			"y": 622.9916103699112,
			"width": 18.654124568354636,
			"height": 26.76457181069964,
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
			"seed": 1780513636,
			"version": 78,
			"versionNonce": 158559204,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230240487,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-12.165717272046823,
					4.866274533211181
				],
				[
					-17.031991805258972,
					8.110478181364684
				],
				[
					-18.654124568354636,
					8.921513623893562
				],
				[
					-18.24857590807088,
					8.921513623893562
				],
				[
					-16.626505023013284,
					9.327062284176915
				],
				[
					-16.220956362729527,
					12.165717272046985
				],
				[
					-16.220956362729527,
					15.815438641464887
				],
				[
					-16.220956362729527,
					19.46516001088279
				],
				[
					-14.193336817388175,
					21.89829727748838
				],
				[
					-10.949133169234916,
					23.92591682282957
				],
				[
					-8.516026841647873,
					25.14246998662285
				],
				[
					-8.11047818136541,
					25.14246998662285
				],
				[
					-7.704991399119721,
					25.14246998662285
				],
				[
					-6.4884072963078125,
					26.359054089435162
				],
				[
					-6.082858636024057,
					26.76457181069964
				],
				[
					-3.244203648153261,
					26.76457181069964
				],
				[
					-3.244203648153261,
					26.76457181069964
				]
			],
			"pressures": [
				0.310546875,
				0.5205078125,
				0.564453125,
				0.580078125,
				0.578125,
				0.5517578125,
				0.5380859375,
				0.5380859375,
				0.5458984375,
				0.5458984375,
				0.5517578125,
				0.5537109375,
				0.5537109375,
				0.5537109375,
				0.48828125,
				0.30859375,
				0.013671875,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				-4.571446010044383,
				37.714276994977695
			]
		},
		{
			"id": "HMnXb2D4OCzuHCn7Zy-ts",
			"type": "freedraw",
			"x": 8377.30899770171,
			"y": 639.618084453905,
			"width": 2.433168205625108,
			"height": 13.382301374859297,
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
			"seed": 694043996,
			"version": 66,
			"versionNonce": 179614812,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230240487,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-2.433168205625108,
					9.327062284176915
				],
				[
					-2.433168205625108,
					10.949164108253626
				],
				[
					-2.433168205625108,
					12.976783653594817
				],
				[
					-2.433168205625108,
					13.382301374859297
				],
				[
					-2.433168205625108,
					13.382301374859297
				]
			],
			"pressures": [
				0.353515625,
				0.5205078125,
				0.525390625,
				0.52734375,
				0.52734375,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				-3.428606305804351,
				18.857160295758945
			]
		},
		{
			"id": "gU5-MgCC1NA0aLHrt_YhF",
			"type": "freedraw",
			"x": 8378.120033144238,
			"y": 624.6137121939879,
			"width": 3.6496904303989495,
			"height": 1.2165841028123119,
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
			"seed": 593279204,
			"version": 67,
			"versionNonce": 795103076,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230240488,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.40548678224568835,
					-0.811066381547832
				],
				[
					1.2165841028119084,
					-1.2165841028123119
				],
				[
					2.4331063275870406,
					-1.2165841028123119
				],
				[
					3.6496904303989495,
					-0.811066381547832
				],
				[
					0,
					0
				]
			],
			"pressures": [
				0.37109375,
				0.44921875,
				0.3349609375,
				0.234375,
				0.0146484375,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				5.142822265625,
				-1.14288330078125
			]
		},
		{
			"id": "P0I6o2h02MezugHW5YJvi",
			"type": "freedraw",
			"x": 8388.258130870943,
			"y": 618.9363712792288,
			"width": 15.409859042163308,
			"height": 36.902669537405515,
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
			"seed": 479667940,
			"version": 76,
			"versionNonce": 592824540,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230240488,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					6.082858636024057,
					0
				],
				[
					12.976814592614334,
					2.027619545341191
				],
				[
					14.193336817388175,
					3.244203648153503
				],
				[
					12.976814592614334,
					5.677340914759093
				],
				[
					13.382239496821956,
					11.354681829518105
				],
				[
					15.004434137955688,
					17.84305818680608
				],
				[
					15.409859042163308,
					19.059611350599436
				],
				[
					15.004434137955688,
					24.33143454409405
				],
				[
					12.165717272048115,
					29.603257737588663
				],
				[
					7.299442738835966,
					33.65849682827096
				],
				[
					6.893894078553501,
					34.06401454953544
				],
				[
					5.271823193494614,
					35.28056771332872
				],
				[
					4.866274533212149,
					36.091634094876554
				],
				[
					3.244203648154552,
					36.902669537405515
				],
				[
					3.244203648154552,
					36.902669537405515
				]
			],
			"pressures": [
				0.3662109375,
				0.4541015625,
				0.48046875,
				0.50390625,
				0.5361328125,
				0.5498046875,
				0.546875,
				0.546875,
				0.5625,
				0.5830078125,
				0.609375,
				0.609375,
				0.611328125,
				0.5703125,
				0.0166015625,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				4.571446010046202,
				51.99999128069203
			]
		},
		{
			"id": "1N-n5MASWvVg6_n56PAcW",
			"type": "freedraw",
			"x": 8211.159585468971,
			"y": 622.6111015487394,
			"width": 20.571376255579708,
			"height": 31.428571428571445,
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
			"seed": 786781284,
			"version": 20,
			"versionNonce": 141139036,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230279082,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-10.285731724330617,
					-1.1428397042410552
				],
				[
					-10.857107979909415,
					-1.1428397042410552
				],
				[
					-14.285714285713766,
					-1.1428397042410552
				],
				[
					-13.714250837052532,
					0
				],
				[
					-17.142857142856883,
					9.14284842354914
				],
				[
					-18.285696847096915,
					11.428571428571445
				],
				[
					-20.571376255579708,
					18.28569684709828
				],
				[
					-20.571376255579708,
					20
				],
				[
					-18.85716029575815,
					23.999982561383945
				],
				[
					-13.714250837052532,
					28.000008719308084
				],
				[
					-11.999947684151266,
					29.14284842354914
				],
				[
					-10.857107979909415,
					29.714268275669724
				],
				[
					-10.285731724330617,
					30.28573172433039
				],
				[
					-9.142804827008149,
					30.28573172433039
				],
				[
					-7.4285888671875,
					30.28573172433039
				],
				[
					-4.571446010044383,
					30.28573172433039
				],
				[
					-2.857142857143117,
					29.714268275669724
				],
				[
					-2.857142857143117,
					29.714268275669724
				]
			],
			"pressures": [
				0.2822265625,
				0.509765625,
				0.51953125,
				0.5439453125,
				0.5009765625,
				0.49609375,
				0.49609375,
				0.501953125,
				0.5078125,
				0.5107421875,
				0.5107421875,
				0.5205078125,
				0.5234375,
				0.5234375,
				0.5234375,
				0.48828125,
				0.271484375,
				0.013671875,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				-2.857142857143117,
				29.714268275669724
			]
		},
		{
			"id": "E-h7yUx_ZG9wiq-K6Ct3L",
			"type": "freedraw",
			"x": 8224.873923499106,
			"y": 636.8968158344537,
			"width": 10.285731724330617,
			"height": 24.57144601004461,
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
			"seed": 1104275300,
			"version": 9,
			"versionNonce": 1640043876,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230279557,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					3.999982561383149,
					11.428571428571445
				],
				[
					6.285661969865032,
					20
				],
				[
					0.571376255580617,
					24.57144601004461
				],
				[
					-2.2857666015625,
					23.999982561383945
				],
				[
					-4.000069754465585,
					21.71430315290172
				],
				[
					-2.857142857143117,
					12.5714111328125
				],
				[
					-2.857142857143117,
					12.5714111328125
				]
			],
			"pressures": [
				0.2509765625,
				0.4755859375,
				0.498046875,
				0.5390625,
				0.5576171875,
				0.537109375,
				0.013671875,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				-2.857142857143117,
				12.5714111328125
			]
		},
		{
			"id": "kTLLgys0zHPfF56QcDYCZ",
			"type": "freedraw",
			"x": 8224.873923499106,
			"y": 618.6111189873556,
			"width": 3.999982561383149,
			"height": 1.14288330078125,
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
			"seed": 1720738524,
			"version": 7,
			"versionNonce": 637698140,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230279736,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.571376255580617,
					-0.5714634486607792
				],
				[
					1.142839704240032,
					-1.14288330078125
				],
				[
					3.999982561383149,
					-0.5714634486607792
				],
				[
					0,
					0
				]
			],
			"pressures": [
				0.39453125,
				0.412109375,
				0.40234375,
				0.0146484375,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				3.999982561383149,
				-0.5714634486607792
			]
		},
		{
			"id": "u7aga8sZgDIstUAPKhwn_",
			"type": "freedraw",
			"x": 8182.016846036771,
			"y": 715.1825562780921,
			"width": 27.428501674106883,
			"height": 33.14287458147328,
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
			"seed": 829908060,
			"version": 22,
			"versionNonce": 1941926500,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230304344,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.571376255580617,
					0.5714198521204708
				],
				[
					3.4285191127228245,
					2.285723005022305
				],
				[
					6.857125418526266,
					2.8571428571428896
				],
				[
					14.285714285713766,
					2.285723005022305
				],
				[
					21.142839704240032,
					0.5714198521204708
				],
				[
					26.857125418526266,
					-2.8571428571428896
				],
				[
					27.428501674106883,
					-6.857125418526721
				],
				[
					25.142822265625,
					-9.14284842354914
				],
				[
					22.285679408481883,
					-11.99999128069203
				],
				[
					21.71421595982065,
					-14.28571428571422
				],
				[
					23.428519112723734,
					-16.57143729073664
				],
				[
					26.857125418526266,
					-21.14283970424117
				],
				[
					26.857125418526266,
					-23.42856270926336
				],
				[
					22.857142857143117,
					-26.85712541852672
				],
				[
					16.57139369419565,
					-29.14284842354914
				],
				[
					12.5714111328125,
					-30.28573172433039
				],
				[
					10.28564453125,
					-30.28573172433039
				],
				[
					10.28564453125,
					-29.14284842354914
				],
				[
					11.428571428570649,
					-27.4285888671875
				],
				[
					11.428571428570649,
					-27.4285888671875
				]
			],
			"pressures": [
				0.2529296875,
				0.4580078125,
				0.4970703125,
				0.5087890625,
				0.51171875,
				0.51171875,
				0.517578125,
				0.5166015625,
				0.5166015625,
				0.5263671875,
				0.541015625,
				0.5400390625,
				0.521484375,
				0.5126953125,
				0.5283203125,
				0.5537109375,
				0.5732421875,
				0.57421875,
				0.529296875,
				0.013671875,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				11.428571428570649,
				-27.4285888671875
			]
		},
		{
			"id": "mxLw2ThWiwh29p6Eyvuve",
			"type": "freedraw",
			"x": 8273.445417465342,
			"y": 699.7540022881367,
			"width": 27.999965122768117,
			"height": 6.857125418526721,
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
			"seed": 1072846300,
			"version": 9,
			"versionNonce": 1180338140,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230305273,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					6.285661969866851,
					1.1428397042411689
				],
				[
					14.285714285715585,
					3.4285627092633604
				],
				[
					19.428536551340585,
					4.571402413504529
				],
				[
					24.571358816965585,
					5.142822265625
				],
				[
					27.999965122768117,
					5.714285714285779
				],
				[
					25.714285714286234,
					6.857125418526721
				],
				[
					25.714285714286234,
					6.857125418526721
				]
			],
			"pressures": [
				0.234375,
				0.4833984375,
				0.5166015625,
				0.5166015625,
				0.513671875,
				0.4931640625,
				0.0146484375,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				25.714285714286234,
				6.857125418526721
			]
		},
		{
			"id": "TiuSYF0TSkH3lmfuFkjcZ",
			"type": "freedraw",
			"x": 8351.159825249943,
			"y": 680.3254221402572,
			"width": 2.285679408481883,
			"height": 37.14285714285711,
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
			"seed": 1761342820,
			"version": 12,
			"versionNonce": 127547740,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230317803,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1.142839704241851,
					5.714285714285779
				],
				[
					1.142839704241851,
					8.571428571428669
				],
				[
					1.714215959822468,
					14.28571428571422
				],
				[
					2.285679408481883,
					17.14285714285711
				],
				[
					2.285679408481883,
					26.28570556640625
				],
				[
					2.285679408481883,
					31.99999128069203
				],
				[
					1.142839704241851,
					35.99997384207586
				],
				[
					0.571376255580617,
					37.14285714285711
				],
				[
					0,
					37.14285714285711
				],
				[
					0,
					37.14285714285711
				]
			],
			"pressures": [
				0.302734375,
				0.470703125,
				0.48828125,
				0.5078125,
				0.50390625,
				0.5068359375,
				0.5068359375,
				0.5009765625,
				0.4853515625,
				0.3857421875,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				0,
				37.14285714285711
			]
		},
		{
			"id": "HeYOxerdBu1aixHgWeIYX",
			"type": "freedraw",
			"x": 8272.302664954184,
			"y": 782.0396816966188,
			"width": 32.00003487723188,
			"height": 41.71425955636164,
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
			"seed": 754812132,
			"version": 16,
			"versionNonce": 1378110172,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230319949,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-17.142857142856883,
					-3.999982561383945
				],
				[
					-22.2857666015625,
					-9.71426827566961
				],
				[
					-20,
					-14.857134137834919
				],
				[
					-16.571480887278085,
					-18.85711669921875
				],
				[
					-12.5714111328125,
					-22.28572300502242
				],
				[
					-8.571428571429351,
					-29.71426827566961
				],
				[
					-11.428571428572468,
					-33.71429443359375
				],
				[
					-16.571480887278085,
					-37.14285714285711
				],
				[
					-21.14283970424185,
					-39.42858014787953
				],
				[
					-26.285749162947468,
					-41.14283970424117
				],
				[
					-28.57142857142935,
					-41.71425955636164
				],
				[
					-30.85719517299185,
					-41.71425955636164
				],
				[
					-32.00003487723188,
					-40
				],
				[
					-32.00003487723188,
					-40
				]
			],
			"pressures": [
				0.2822265625,
				0.525390625,
				0.5791015625,
				0.5693359375,
				0.537109375,
				0.494140625,
				0.4541015625,
				0.4921875,
				0.55859375,
				0.591796875,
				0.59375,
				0.5732421875,
				0.4921875,
				0.0166015625,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				-32.00003487723188,
				-40
			]
		},
		{
			"id": "CG6K32D5xMV1HRl1HLDda",
			"type": "freedraw",
			"x": 8023.731367172373,
			"y": 848.8968507116856,
			"width": 24.571446010044383,
			"height": 37.14285714285711,
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
			"seed": 155148516,
			"version": 21,
			"versionNonce": 207508452,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230344980,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					2.857142857143117,
					-9.71426827566961
				],
				[
					6.2856619698659415,
					-18.285696847098052
				],
				[
					6.8571254185271755,
					-20.57141985212047
				],
				[
					6.2856619698659415,
					-24.57144601004461
				],
				[
					3.428519112723734,
					-29.142848423548912
				],
				[
					0.571376255580617,
					-30.85715157645086
				],
				[
					-0.5714634486603245,
					-26.85712541852672
				],
				[
					2.285679408481883,
					-21.71430315290172
				],
				[
					10.285731724330617,
					-10.285731724330162
				],
				[
					15.428553989955617,
					1.1428397042411689
				],
				[
					13.142874581473734,
					2.285723005022419
				],
				[
					5.714285714286234,
					5.1428658621653085
				],
				[
					-1.714303152901266,
					6.28570556640625
				],
				[
					-6.2857491629465585,
					5.714285714285779
				],
				[
					-9.142892020088766,
					5.1428658621653085
				],
				[
					-7.4285888671875,
					4.571446010044838
				],
				[
					-0.5714634486603245,
					3.9999825613840585
				],
				[
					0,
					0
				]
			],
			"pressures": [
				0.2490234375,
				0.451171875,
				0.4794921875,
				0.482421875,
				0.4931640625,
				0.5029296875,
				0.5244140625,
				0.5302734375,
				0.5166015625,
				0.501953125,
				0.513671875,
				0.5302734375,
				0.572265625,
				0.58984375,
				0.5927734375,
				0.5732421875,
				0.2265625,
				0.0126953125,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				-0.5714634486603245,
				3.9999825613840585
			]
		},
		{
			"id": "qo_qOGSeuv0F58tnCsmGk",
			"type": "freedraw",
			"x": 8063.159903723713,
			"y": 847.7540110074447,
			"width": 13.142874581473734,
			"height": 28.57142857142844,
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
			"seed": 776752220,
			"version": 8,
			"versionNonce": 1181958628,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230345527,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-8.571428571428442,
					11.99999128069203
				],
				[
					-12.5714111328125,
					20.57141985212047
				],
				[
					-13.142874581473734,
					24.571402413504302
				],
				[
					-12.5714111328125,
					27.42854527064719
				],
				[
					-11.999947684152175,
					28.57142857142844
				],
				[
					-11.999947684152175,
					28.57142857142844
				]
			],
			"pressures": [
				0.34375,
				0.5,
				0.521484375,
				0.466796875,
				0.234375,
				0.0126953125,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				-11.999947684152175,
				28.57142857142844
			]
		},
		{
			"id": "IRUu9YYs2Dij1_R3cHURP",
			"type": "freedraw",
			"x": 8092.874084806302,
			"y": 836.8967722379134,
			"width": 32.00003487723188,
			"height": 45.142865862165195,
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
			"seed": 2126855772,
			"version": 18,
			"versionNonce": 1542635876,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230356036,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					9.71435546875,
					-20.57141985212047
				],
				[
					6.857212611606883,
					-30.85710797991078
				],
				[
					4.571446010044383,
					-32.5714111328125
				],
				[
					1.1429268973215585,
					-34.285714285714334
				],
				[
					-3.4285191127228245,
					-30.85710797991078
				],
				[
					-3.9999825613840585,
					-29.14284842354914
				],
				[
					-1.1428397042409415,
					-16.57139369419656
				],
				[
					7.4285888671875,
					-7.99996512276789
				],
				[
					18.28578404017844,
					-0.5714198521204708
				],
				[
					18.28578404017844,
					3.4286063058034415
				],
				[
					8.000052315847825,
					6.285749162946331
				],
				[
					-2.857142857143117,
					7.4285888671875
				],
				[
					-9.142804827009058,
					8.00000871930797
				],
				[
					-13.714250837053442,
					8.571428571428442
				],
				[
					-12.5714111328125,
					10.85715157645086
				],
				[
					-12.5714111328125,
					10.85715157645086
				]
			],
			"pressures": [
				0.2822265625,
				0.388671875,
				0.40625,
				0.4248046875,
				0.478515625,
				0.5107421875,
				0.5107421875,
				0.5078125,
				0.4970703125,
				0.470703125,
				0.4794921875,
				0.529296875,
				0.5556640625,
				0.533203125,
				0.447265625,
				0.0126953125,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				-12.5714111328125,
				10.85715157645086
			]
		},
		{
			"id": "g9ziS7pWHLRwb0hMozmTF",
			"type": "freedraw",
			"x": 8045.445495939113,
			"y": 944.8968681503018,
			"width": 26.28566196986594,
			"height": 34.85713413783492,
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
			"seed": 580875996,
			"version": 22,
			"versionNonce": 290645988,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230360882,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1.1428397042409415,
					-5.1428658621653085
				],
				[
					2.857142857143117,
					-7.4285888671875
				],
				[
					7.4285888671875,
					-14.857177734375
				],
				[
					9.142892020088766,
					-18.28574044363836
				],
				[
					10.285731724330617,
					-26.85716901506703
				],
				[
					5.7142857142853245,
					-32.00003487723211
				],
				[
					3.9999825613840585,
					-32.57145472935281
				],
				[
					-0.571376255580617,
					-31.42857142857156
				],
				[
					0.5714634486603245,
					-26.28574916294656
				],
				[
					7.4285888671875,
					-17.14285714285711
				],
				[
					18.85716029575906,
					-8.571428571428669
				],
				[
					25.714285714285325,
					-3.428606305803669
				],
				[
					22.857142857143117,
					-0.5714634486607792
				],
				[
					13.142874581472825,
					1.7142595563616396
				],
				[
					6.2857491629465585,
					1.7142595563616396
				],
				[
					5.142909458705617,
					1.7142595563616396
				],
				[
					4.571446010044383,
					1.7142595563616396
				],
				[
					7.4285888671875,
					2.2856794084821104
				],
				[
					0,
					0
				]
			],
			"pressures": [
				0.1513671875,
				0.380859375,
				0.419921875,
				0.4609375,
				0.4677734375,
				0.478515625,
				0.5185546875,
				0.537109375,
				0.583984375,
				0.583984375,
				0.560546875,
				0.517578125,
				0.501953125,
				0.521484375,
				0.5810546875,
				0.603515625,
				0.603515625,
				0.546875,
				0.013671875,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				7.4285888671875,
				2.2856794084821104
			]
		},
		{
			"id": "-lsO545JKJPC7yQ2LdQvF",
			"type": "freedraw",
			"x": 8110.016941949158,
			"y": 948.8968507116856,
			"width": 14.857177734375,
			"height": 30.85715157645086,
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
			"seed": 261814364,
			"version": 7,
			"versionNonce": 2139293148,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230361415,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1.7143031529021755,
					-3.999982561383831
				],
				[
					9.142892020089675,
					-10.28573172433039
				],
				[
					12.000034877231883,
					-13.142874581473052
				],
				[
					14.857177734375,
					-30.85715157645086
				],
				[
					14.857177734375,
					-30.85715157645086
				]
			],
			"pressures": [
				0.3935546875,
				0.517578125,
				0.552734375,
				0.552734375,
				0.013671875,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				14.857177734375,
				-30.85715157645086
			]
		},
		{
			"id": "rFDcQlXsq87PhI5AEWt6i",
			"type": "freedraw",
			"x": 8112.3026213576395,
			"y": 918.0396991352347,
			"width": 28.57142857142935,
			"height": 28.00000871930797,
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
			"seed": 1920849380,
			"version": 7,
			"versionNonce": 965046372,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230361603,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					11.428571428571558,
					14.857134137834919
				],
				[
					14.857177734375,
					17.71427699497781
				],
				[
					22.2857666015625,
					22.85714285714289
				],
				[
					28.57142857142935,
					28.00000871930797
				],
				[
					28.57142857142935,
					28.00000871930797
				]
			],
			"pressures": [
				0.3515625,
				0.53515625,
				0.546875,
				0.435546875,
				0.0126953125,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				28.57142857142935,
				28.00000871930797
			]
		},
		{
			"id": "_AgS5Cqi2S8nmbv8RJiMm",
			"type": "freedraw",
			"x": 8205.445495939113,
			"y": 922.6111015487393,
			"width": 1.142839704240032,
			"height": 38.28569684709805,
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
			"seed": 538130396,
			"version": 8,
			"versionNonce": 1390943844,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230363019,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.571463448659415,
					12.5714111328125
				],
				[
					0,
					21.14283970424094
				],
				[
					0,
					26.85712541852672
				],
				[
					0.571463448659415,
					32.5714111328125
				],
				[
					1.142839704240032,
					38.28569684709805
				],
				[
					1.142839704240032,
					38.28569684709805
				]
			],
			"pressures": [
				0.359375,
				0.4755859375,
				0.4970703125,
				0.4970703125,
				0.4365234375,
				0.0166015625,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				1.142839704240032,
				38.28569684709805
			]
		},
		{
			"id": "7eQ2i21jRZlCRxvA-PVoB",
			"type": "freedraw",
			"x": 8220.874049929069,
			"y": 947.7539674109044,
			"width": 5.714285714286234,
			"height": 24.57144601004461,
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
			"seed": 1174039004,
			"version": 8,
			"versionNonce": 1719913572,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230363359,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-2.857142857143117,
					-9.714311872209692
				],
				[
					-5.142822265625,
					-19.42858014787953
				],
				[
					-5.714285714286234,
					-24.00002615792414
				],
				[
					-3.999982561384968,
					-24.57144601004461
				],
				[
					-1.142839704241851,
					-18.85716029575883
				],
				[
					-1.142839704241851,
					-18.85716029575883
				]
			],
			"pressures": [
				0.333984375,
				0.5068359375,
				0.5595703125,
				0.556640625,
				0.39453125,
				0.0146484375,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				-1.142839704241851,
				-18.85716029575883
			]
		},
		{
			"id": "voy4AU5dsQXxcv5DChfUe",
			"type": "freedraw",
			"x": 8231.159781653398,
			"y": 934.0396729773106,
			"width": 28.57142857142935,
			"height": 18.85716029575906,
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
			"seed": 230202332,
			"version": 23,
			"versionNonce": 1733639516,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230363915,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-2.285679408481883,
					-5.714285714285779
				],
				[
					-5.142822265625,
					-3.4285627092633604
				],
				[
					-6.285749162945649,
					1.7143031529017208
				],
				[
					-6.285749162945649,
					2.8571428571428896
				],
				[
					-5.142822265625,
					8.571428571428669
				],
				[
					-2.857142857141298,
					10.85715157645086
				],
				[
					0.571463448661234,
					11.428571428571558
				],
				[
					0.571463448661234,
					10.85715157645086
				],
				[
					2.857142857143117,
					8.571428571428669
				],
				[
					3.428606305804351,
					7.4285888671875
				],
				[
					4.571446010046202,
					4.57144601004461
				],
				[
					4.571446010046202,
					3.9999825613840585
				],
				[
					7.4285888671875,
					-1.1428397042409415
				],
				[
					11.428571428572468,
					-6.28570556640625
				],
				[
					14.857177734375,
					-7.4285888671875
				],
				[
					17.142857142858702,
					-1.7143031529017208
				],
				[
					17.714320591518117,
					5.1428658621653085
				],
				[
					18.285696847098734,
					8.571428571428669
				],
				[
					19.428536551340585,
					10.28573172433039
				],
				[
					22.285679408483702,
					9.14284842354914
				],
				[
					22.285679408483702,
					9.14284842354914
				]
			],
			"pressures": [
				0.2041015625,
				0.263671875,
				0.3857421875,
				0.44921875,
				0.4521484375,
				0.4521484375,
				0.4443359375,
				0.41796875,
				0.4130859375,
				0.25,
				0.1796875,
				0.1181640625,
				0.15625,
				0.3310546875,
				0.4521484375,
				0.50390625,
				0.5185546875,
				0.5185546875,
				0.4912109375,
				0.296875,
				0.013671875,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				22.285679408483702,
				9.14284842354914
			]
		},
		{
			"id": "5Lby-Z1E58ZKs7WJvwKYh",
			"type": "freedraw",
			"x": 8273.445461061881,
			"y": 908.8968071151455,
			"width": 21.142839704240032,
			"height": 37.14285714285711,
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
			"seed": 1370281572,
			"version": 18,
			"versionNonce": 1435014620,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230364375,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-13.714250837054351,
					3.4285627092633604
				],
				[
					-17.7142333984375,
					4.00002615792414
				],
				[
					-20.571376255580617,
					3.4285627092633604
				],
				[
					-20,
					2.8571428571428896
				],
				[
					-18.285696847098734,
					2.2857230050221915
				],
				[
					-16.571393694197468,
					5.714285714285552
				],
				[
					-17.142857142858702,
					13.142874581473052
				],
				[
					-18.85707310267935,
					18.85716029575883
				],
				[
					-20,
					26.28570556640625
				],
				[
					-18.285696847098734,
					30.85715157645086
				],
				[
					-14.857090541296202,
					34.28571428571422
				],
				[
					-11.428571428572468,
					35.42859758649547
				],
				[
					-8.571428571429351,
					36.00001743861594
				],
				[
					-5.142822265625,
					37.14285714285711
				],
				[
					0.571463448659415,
					34.85713413783469
				],
				[
					0.571463448659415,
					34.85713413783469
				]
			],
			"pressures": [
				0.2626953125,
				0.439453125,
				0.5,
				0.5361328125,
				0.5390625,
				0.5263671875,
				0.5224609375,
				0.5205078125,
				0.5185546875,
				0.5185546875,
				0.529296875,
				0.53515625,
				0.537109375,
				0.52734375,
				0.4873046875,
				0.013671875,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				0.571463448659415,
				34.85713413783469
			]
		},
		{
			"id": "RPXWhl6NgB35xlSlYLXW-",
			"type": "freedraw",
			"x": 8284.302656234871,
			"y": 936.8968158344535,
			"width": 6.857125418526266,
			"height": 18.28569684709828,
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
			"seed": 358172132,
			"version": 10,
			"versionNonce": 832793692,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230364737,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					3.428519112723734,
					10.85715157645086
				],
				[
					2.285679408481883,
					15.42855398995539
				],
				[
					-1.714303152901266,
					18.28569684709828
				],
				[
					-2.857142857143117,
					18.28569684709828
				],
				[
					-3.428606305802532,
					14.857134137834919
				],
				[
					-2.857142857143117,
					5.714285714285779
				],
				[
					0,
					0
				]
			],
			"pressures": [
				0.3837890625,
				0.490234375,
				0.517578125,
				0.55078125,
				0.5361328125,
				0.341796875,
				0.013671875,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				-2.857142857143117,
				5.714285714285779
			]
		},
		{
			"id": "uTMAZYnuUmK1wxYjS8dFL",
			"type": "freedraw",
			"x": 8280.302673673488,
			"y": 912.8968332730697,
			"width": 5.714285714284415,
			"height": 2.285723005022419,
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
			"seed": 1037899620,
			"version": 7,
			"versionNonce": 2030707172,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230364897,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1.714215959820649,
					-1.7143031529019481
				],
				[
					3.999982561383149,
					-2.285723005022419
				],
				[
					5.714285714284415,
					-1.7143031529019481
				],
				[
					0,
					0
				]
			],
			"pressures": [
				0.3994140625,
				0.439453125,
				0.341796875,
				0.0146484375,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				5.714285714284415,
				-1.7143031529019481
			]
		},
		{
			"id": "676eDOk38MUM5mbR0y5mN",
			"type": "freedraw",
			"x": 8297.445530816345,
			"y": 903.7539412529802,
			"width": 21.142839704240032,
			"height": 41.71430315290195,
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
			"seed": 227303004,
			"version": 15,
			"versionNonce": 615734748,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230365337,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					9.142804827008149,
					1.7143031529019481
				],
				[
					14.857090541294383,
					0.5714634486607792
				],
				[
					15.428553989955617,
					2.8571428571428896
				],
				[
					14.857090541294383,
					9.714311872209919
				],
				[
					17.7142333984375,
					22.28572300502242
				],
				[
					21.142839704240032,
					31.42857142857156
				],
				[
					21.142839704240032,
					33.14287458147328
				],
				[
					18.857073102677532,
					36.57143729073664
				],
				[
					12.5714111328125,
					40
				],
				[
					7.999965122768117,
					41.14288330078125
				],
				[
					6.857125418526266,
					41.71430315290195
				],
				[
					5.714285714286234,
					41.71430315290195
				],
				[
					5.714285714286234,
					41.71430315290195
				]
			],
			"pressures": [
				0.3876953125,
				0.4287109375,
				0.439453125,
				0.48828125,
				0.5126953125,
				0.5244140625,
				0.5244140625,
				0.5244140625,
				0.5244140625,
				0.54296875,
				0.5498046875,
				0.46484375,
				0.0166015625,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				5.714285714286234,
				41.71430315290195
			]
		},
		{
			"id": "eP-lKzHii6qM7j2unrTWl",
			"type": "freedraw",
			"x": 8257.445312833646,
			"y": 976.3253523857927,
			"width": 22.2857666015625,
			"height": 33.71429443359375,
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
			"seed": 958332388,
			"version": 20,
			"versionNonce": 1333328604,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230375006,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-5.142909458705617,
					-1.14288330078125
				],
				[
					-10.857195172991851,
					5.142822265625
				],
				[
					-11.428571428572468,
					6.857125418526721
				],
				[
					-14.857177734375,
					18.85711669921875
				],
				[
					-16.00001743861685,
					22.85714285714289
				],
				[
					-16.571480887276266,
					28.57142857142844
				],
				[
					-13.714338030134968,
					32.5714111328125
				],
				[
					-6.857212611606883,
					31.42857142857133
				],
				[
					2.285679408481883,
					26.28570556640625
				],
				[
					5.714285714286234,
					20.57141985212047
				],
				[
					4.571358816963766,
					15.99997384207586
				],
				[
					3.428519112723734,
					14.857134137834692
				],
				[
					-3.428606305804351,
					14.857134137834692
				],
				[
					-10.857195172991851,
					18.85711669921875
				],
				[
					-14.285714285713766,
					22.28567940848211
				],
				[
					-15.428641183036234,
					25.142822265625
				],
				[
					-14.285714285713766,
					27.99996512276789
				],
				[
					-14.285714285713766,
					27.99996512276789
				]
			],
			"pressures": [
				0.2568359375,
				0.40234375,
				0.4736328125,
				0.4765625,
				0.4990234375,
				0.5078125,
				0.515625,
				0.5185546875,
				0.513671875,
				0.498046875,
				0.4873046875,
				0.49609375,
				0.49609375,
				0.515625,
				0.5244140625,
				0.5244140625,
				0.4873046875,
				0.013671875,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				-14.285714285713766,
				27.99996512276789
			]
		},
		{
			"id": "7d00OdSkXLcmrj_9ipWCC",
			"type": "freedraw",
			"x": 8340.87383194637,
			"y": 920.8967547992972,
			"width": 25.714285714284415,
			"height": 1.1428397042411689,
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
			"seed": 1020113124,
			"version": 9,
			"versionNonce": 1506549476,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230376379,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					8.000052315846915,
					-0.5714198521206981
				],
				[
					15.428553989953798,
					0.5714198521204708
				],
				[
					21.714303152901266,
					0.5714198521204708
				],
				[
					22.857142857141298,
					0.5714198521204708
				],
				[
					25.142909458703798,
					0
				],
				[
					25.714285714284415,
					0
				],
				[
					25.714285714284415,
					0
				]
			],
			"pressures": [
				0.26953125,
				0.515625,
				0.5234375,
				0.5205078125,
				0.509765625,
				0.392578125,
				0.03125,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				25.714285714284415,
				0
			]
		},
		{
			"id": "PKvdczNw95R9_XaefJe-O",
			"type": "freedraw",
			"x": 8419.73099224213,
			"y": 998.0396555386947,
			"width": 2.857142857141298,
			"height": 35.99997384207586,
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
			"seed": 263500124,
			"version": 9,
			"versionNonce": 441656156,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230383235,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-1.142839704240032,
					-14.28571428571422
				],
				[
					-1.142839704240032,
					-23.42856270926336
				],
				[
					-0.571376255580617,
					-30.28568812779008
				],
				[
					0,
					-34.857134137834805
				],
				[
					0.571463448661234,
					-35.99997384207586
				],
				[
					1.714303152901266,
					-34.28571428571422
				],
				[
					1.714303152901266,
					-34.28571428571422
				]
			],
			"pressures": [
				0.3046875,
				0.5283203125,
				0.548828125,
				0.54296875,
				0.513671875,
				0.4296875,
				0.0126953125,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				1.714303152901266,
				-34.28571428571422
			]
		},
		{
			"id": "Uf_iEeI7wdOxdbHaW_M7_",
			"type": "freedraw",
			"x": 8400.873919139452,
			"y": 930.0396468193867,
			"width": 9.142892020090585,
			"height": 42.85714285714289,
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
			"seed": 1114132580,
			"version": 11,
			"versionNonce": 1001755108,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230385042,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.571463448661234,
					-1.1428397042411689
				],
				[
					-4.000069754465585,
					-6.857125418526721
				],
				[
					-8.000052315848734,
					-20
				],
				[
					-8.571428571429351,
					-32.5714111328125
				],
				[
					-9.142892020090585,
					-41.71425955636164
				],
				[
					-8.000052315848734,
					-42.85714285714289
				],
				[
					-7.4285888671875,
					-42.85714285714289
				],
				[
					-3.428606305804351,
					-39.42853655133922
				],
				[
					-3.428606305804351,
					-39.42853655133922
				]
			],
			"pressures": [
				0.1630859375,
				0.3359375,
				0.490234375,
				0.5498046875,
				0.5498046875,
				0.52734375,
				0.4931640625,
				0.33984375,
				0.0146484375,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				-3.428606305804351,
				-39.42853655133922
			]
		},
		{
			"id": "3lLYUTK4u4M2Y9vrSV07Q",
			"type": "freedraw",
			"x": 8408.873884262219,
			"y": 908.8968071151455,
			"width": 28.57142857142935,
			"height": 18.285740443638474,
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
			"seed": 831516252,
			"version": 24,
			"versionNonce": 1536318436,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230385588,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					4.571446010046202,
					-7.4285888671875
				],
				[
					0.571463448661234,
					-10.285731724330276
				],
				[
					-3.999982561383149,
					-8.571428571428442
				],
				[
					-6.285749162945649,
					-5.142865862165081
				],
				[
					-6.285749162945649,
					0.5714198521206981
				],
				[
					-3.999982561383149,
					3.428562709263474
				],
				[
					-1.142839704240032,
					5.1428658621653085
				],
				[
					2.285679408483702,
					5.1428658621653085
				],
				[
					7.999965122768117,
					0.5714198521206981
				],
				[
					11.428571428572468,
					-5.142865862165081
				],
				[
					14.285714285715585,
					-9.142848423549026
				],
				[
					15.428553989955617,
					-10.285731724330276
				],
				[
					17.142857142858702,
					-8.00000871930797
				],
				[
					18.285696847098734,
					-4.57144601004461
				],
				[
					18.857160295759968,
					-3.999982561383831
				],
				[
					20.571463448661234,
					-3.4285627092633604
				],
				[
					21.714303152903085,
					-2.857142857142776
				],
				[
					22.285679408483702,
					-1.7143031529017208
				],
				[
					21.714303152903085,
					1.1428397042411689
				],
				[
					20,
					6.857125418526948
				],
				[
					21.14283970424185,
					8.000008719308198
				],
				[
					21.14283970424185,
					8.000008719308198
				]
			],
			"pressures": [
				0.2578125,
				0.3232421875,
				0.3486328125,
				0.3935546875,
				0.443359375,
				0.4462890625,
				0.4013671875,
				0.2822265625,
				0.1630859375,
				0.21484375,
				0.3984375,
				0.4931640625,
				0.5078125,
				0.52734375,
				0.537109375,
				0.537109375,
				0.5390625,
				0.5390625,
				0.5087890625,
				0.466796875,
				0.3173828125,
				0.0146484375,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				21.14283970424185,
				8.000008719308198
			]
		},
		{
			"id": "_UwnbfxLBmQSDx2JGwES7",
			"type": "freedraw",
			"x": 8454.016706527844,
			"y": 890.0396468193867,
			"width": 17.142857142856883,
			"height": 34.28571428571422,
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
			"seed": 574407772,
			"version": 17,
			"versionNonce": 1546496092,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230386234,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-14.285714285713766,
					5.142865862165081
				],
				[
					-13.714250837052532,
					5.714285714285779
				],
				[
					-10.28564453125,
					6.857169015067029
				],
				[
					-9.142804827008149,
					8.571428571428555
				],
				[
					-9.142804827008149,
					13.71429443359375
				],
				[
					-12.5714111328125,
					19.42858014787953
				],
				[
					-13.714250837052532,
					24.00002615792414
				],
				[
					-12.5714111328125,
					26.85716901506703
				],
				[
					-11.428571428570649,
					28.00000871930797
				],
				[
					-9.142804827008149,
					30.28573172433039
				],
				[
					-4.571358816963766,
					33.14287458147328
				],
				[
					-1.142839704240032,
					34.28571428571422
				],
				[
					1.142926897322468,
					33.71429443359375
				],
				[
					2.857142857143117,
					30.85715157645086
				],
				[
					2.857142857143117,
					30.85715157645086
				]
			],
			"pressures": [
				0.2255859375,
				0.37109375,
				0.373046875,
				0.369140625,
				0.369140625,
				0.388671875,
				0.4208984375,
				0.447265625,
				0.46875,
				0.4775390625,
				0.4814453125,
				0.4814453125,
				0.478515625,
				0.4013671875,
				0.015625,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				2.857142857143117,
				30.85715157645086
			]
		},
		{
			"id": "zmNOZAaoFQyQSQEdJwa6h",
			"type": "freedraw",
			"x": 8471.159563670702,
			"y": 906.6110841101233,
			"width": 11.428571428570649,
			"height": 20.57141985212047,
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
			"seed": 86285156,
			"version": 9,
			"versionNonce": 471452004,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230386609,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					3.428606305802532,
					6.857169015066916
				],
				[
					2.857142857141298,
					12.571454729352581
				],
				[
					-2.857142857143117,
					18.85716029575883
				],
				[
					-6.285661969866851,
					20
				],
				[
					-7.999965122768117,
					20.57141985212047
				],
				[
					-7.999965122768117,
					17.14285714285711
				],
				[
					-7.999965122768117,
					17.14285714285711
				]
			],
			"pressures": [
				0.2568359375,
				0.3935546875,
				0.4619140625,
				0.51953125,
				0.5400390625,
				0.544921875,
				0.0166015625,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				-7.999965122768117,
				17.14285714285711
			]
		},
		{
			"id": "s_v5td5uKoIaNNHYtyu3q",
			"type": "freedraw",
			"x": 8465.445277956416,
			"y": 885.4682444058822,
			"width": 2.2857666015625,
			"height": 3.428562709263474,
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
			"seed": 575467228,
			"version": 7,
			"versionNonce": 737840220,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230386804,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.571463448661234,
					-2.8571428571428896
				],
				[
					0.571463448661234,
					-2.2857230050221915
				],
				[
					2.2857666015625,
					0.5714198521205844
				],
				[
					0,
					0
				]
			],
			"pressures": [
				0.333984375,
				0.3623046875,
				0.216796875,
				0.0126953125,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				2.2857666015625,
				0.5714198521205844
			]
		},
		{
			"id": "QaVXb_7ig4CUo0kjdrpeu",
			"type": "freedraw",
			"x": 8485.445277956416,
			"y": 885.4682444058822,
			"width": 21.714303152901266,
			"height": 43.42856270926336,
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
			"seed": 268957540,
			"version": 17,
			"versionNonce": 1020220260,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230387556,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					13.142874581473734,
					-1.14288330078125
				],
				[
					20,
					-3.4285627092633604
				],
				[
					21.714303152901266,
					-3.4285627092633604
				],
				[
					21.14292689732065,
					3.9999825613840585
				],
				[
					20.571463448661234,
					13.142830984933084
				],
				[
					20,
					23.99998256138406
				],
				[
					20,
					26.28570556640625
				],
				[
					18.85716029575815,
					30.28568812779031
				],
				[
					15.428641183036234,
					34.85713413783492
				],
				[
					12.571498325893117,
					35.99997384207586
				],
				[
					10.857195172990032,
					36.57143729073664
				],
				[
					8.571428571427532,
					37.14285714285711
				],
				[
					5.714285714286234,
					37.71427699497781
				],
				[
					1.714303152901266,
					40
				],
				[
					1.714303152901266,
					40
				]
			],
			"pressures": [
				0.30859375,
				0.3701171875,
				0.3896484375,
				0.39453125,
				0.4541015625,
				0.474609375,
				0.482421875,
				0.482421875,
				0.4912109375,
				0.515625,
				0.5302734375,
				0.533203125,
				0.5107421875,
				0.400390625,
				0.015625,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				1.714303152901266,
				40
			]
		},
		{
			"id": "HCxPQj5EccxVGLu5bilWE",
			"type": "freedraw",
			"x": 8320.302455690791,
			"y": 988.325387263025,
			"width": 32.00003487723188,
			"height": 2.8571428571428896,
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
			"seed": 957154524,
			"version": 9,
			"versionNonce": 824555228,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230393084,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					14.857177734375,
					-0.5714198521204708
				],
				[
					17.714320591518117,
					-0.5714198521204708
				],
				[
					26.28574916294565,
					0
				],
				[
					29.714268275669383,
					0
				],
				[
					31.42857142857065,
					-1.14288330078125
				],
				[
					32.00003487723188,
					-2.8571428571428896
				],
				[
					32.00003487723188,
					-2.8571428571428896
				]
			],
			"pressures": [
				0.3203125,
				0.5126953125,
				0.5185546875,
				0.513671875,
				0.4990234375,
				0.3154296875,
				0.0810546875,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				32.00003487723188,
				-2.8571428571428896
			]
		},
		{
			"id": "ngExDEdK59q9Wi30OnJhU",
			"type": "freedraw",
			"x": 8284.873901700836,
			"y": 1080.325378543717,
			"width": 34.285714285713766,
			"height": 37.71427699497781,
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
			"seed": 643478756,
			"version": 19,
			"versionNonce": 1139856484,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230394384,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1.142839704241851,
					1.7143031529017208
				],
				[
					2.285679408481883,
					2.2857230050221915
				],
				[
					6.285661969866851,
					2.8571428571428896
				],
				[
					15.428553989955617,
					2.2857230050221915
				],
				[
					17.142857142856883,
					1.7143031529017208
				],
				[
					20.571376255580617,
					-1.1428397042411689
				],
				[
					20,
					-8.571428571428669
				],
				[
					17.142857142856883,
					-14.285714285714448
				],
				[
					11.428571428570649,
					-20.571419852120698
				],
				[
					10.857107979911234,
					-25.14286586216531
				],
				[
					16.00001743861685,
					-29.14284842354914
				],
				[
					22.857142857143117,
					-33.14287458147328
				],
				[
					28.57142857142935,
					-34.85713413783492
				],
				[
					31.999947684151266,
					-34.85713413783492
				],
				[
					33.71425083705435,
					-33.71429443359375
				],
				[
					34.285714285713766,
					-31.42857142857156
				],
				[
					34.285714285713766,
					-31.42857142857156
				]
			],
			"pressures": [
				0.2724609375,
				0.4892578125,
				0.5029296875,
				0.51171875,
				0.51953125,
				0.521484375,
				0.5234375,
				0.5234375,
				0.5234375,
				0.544921875,
				0.5869140625,
				0.603515625,
				0.603515625,
				0.5966796875,
				0.548828125,
				0.439453125,
				0.015625,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				34.285714285713766,
				-31.42857142857156
			]
		},
		{
			"id": "EkXsBvGx3N7Xfcp3uf-rC",
			"type": "freedraw",
			"x": 8142.0167588436925,
			"y": 1112.8967896765294,
			"width": 8.571428571428442,
			"height": 37.14285714285688,
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
			"seed": 1333793756,
			"version": 12,
			"versionNonce": 1824995684,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230406146,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.571376255580617,
					-1.7142595563614123
				],
				[
					1.7143031529021755,
					-7.999965122767662
				],
				[
					2.857142857143117,
					-13.714250837053442
				],
				[
					2.857142857143117,
					-20
				],
				[
					2.285679408481883,
					-29.142848423548912
				],
				[
					1.7143031529021755,
					-31.999991280691802
				],
				[
					2.857142857143117,
					-37.14285714285688
				],
				[
					5.142822265625,
					-36.57139369419633
				],
				[
					8.571428571428442,
					-33.14283098493297
				],
				[
					8.571428571428442,
					-33.14283098493297
				]
			],
			"pressures": [
				0.189453125,
				0.4404296875,
				0.517578125,
				0.5400390625,
				0.552734375,
				0.5556640625,
				0.5556640625,
				0.4736328125,
				0.314453125,
				0.0263671875,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				8.571428571428442,
				-33.14283098493297
			]
		},
		{
			"id": "GAHdEuUOT3uBk-nKZpAjY",
			"type": "freedraw",
			"x": 8151.159563670702,
			"y": 1087.7539674109044,
			"width": 23.99998256138406,
			"height": 30.85710797991078,
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
			"seed": 292454108,
			"version": 17,
			"versionNonce": 169665244,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230406550,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-6.8571254185271755,
					1.1428397042413962
				],
				[
					-11.999947684152175,
					4.571402413504529
				],
				[
					-15.999930245535325,
					7.428545270647646
				],
				[
					-18.285696847097825,
					7.999965122768117
				],
				[
					-21.14283970424094,
					6.857125418526948
				],
				[
					-23.428519112722825,
					1.714259556361867
				],
				[
					-23.99998256138406,
					-5.714285714285552
				],
				[
					-23.428519112722825,
					-14.28571428571422
				],
				[
					-22.857142857143117,
					-19.428580147879302
				],
				[
					-21.71421595982156,
					-22.28572300502219
				],
				[
					-20.571376255580617,
					-22.857142857142662
				],
				[
					-19.428536551339675,
					-22.28572300502219
				],
				[
					-17.7142333984375,
					-19.428580147879302
				],
				[
					-17.142857142856883,
					-12.571454729352581
				],
				[
					-17.142857142856883,
					-12.571454729352581
				]
			],
			"pressures": [
				0.212890625,
				0.341796875,
				0.419921875,
				0.47265625,
				0.5,
				0.5283203125,
				0.55859375,
				0.56640625,
				0.56640625,
				0.564453125,
				0.556640625,
				0.53515625,
				0.43359375,
				0.26171875,
				0.013671875,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				-17.142857142856883,
				-12.571454729352581
			]
		},
		{
			"id": "QhzG4HSSH8zNQfFod36sL",
			"type": "freedraw",
			"x": 8166.588204853737,
			"y": 1075.1825126815518,
			"width": 25.142822265625,
			"height": 33.71429443359398,
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
			"seed": 1555843300,
			"version": 20,
			"versionNonce": 1571831772,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230408033,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-5.1429094587047075,
					6.28570556640625
				],
				[
					-5.7142857142853245,
					9.14284842354914
				],
				[
					-5.7142857142853245,
					15.428597586495698
				],
				[
					-1.714303152901266,
					21.142883300781477
				],
				[
					8.571428571429351,
					21.142883300781477
				],
				[
					14.285714285714675,
					17.71427699497758
				],
				[
					17.7142333984375,
					12.571454729352581
				],
				[
					19.428536551339675,
					8.000008719308198
				],
				[
					17.7142333984375,
					0.5714198521206981
				],
				[
					14.857090541295292,
					-5.714285714285552
				],
				[
					9.714268275670292,
					-11.999991280691802
				],
				[
					5.714285714286234,
					-12.5714111328125
				],
				[
					2.2856794084827925,
					-9.71426827566961
				],
				[
					1.142839704241851,
					-5.142865862165081
				],
				[
					1.7142159598215585,
					-0.5714198521204708
				],
				[
					3.9999825613840585,
					4.57144601004461
				],
				[
					0,
					0
				]
			],
			"pressures": [
				0.234375,
				0.4072265625,
				0.4287109375,
				0.44921875,
				0.4658203125,
				0.4658203125,
				0.46875,
				0.4775390625,
				0.4892578125,
				0.5263671875,
				0.548828125,
				0.5537109375,
				0.5595703125,
				0.552734375,
				0.5126953125,
				0.3408203125,
				0.0146484375,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				3.9999825613840585,
				4.57144601004461
			]
		},
		{
			"id": "JFj5GE8o",
			"type": "text",
			"x": 6956.302429532867,
			"y": 772.3253698244091,
			"width": 149,
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
			"seed": 756031332,
			"version": 12,
			"versionNonce": 265023324,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230423441,
			"link": null,
			"locked": false,
			"text": "WALKTHROUGH",
			"rawText": "WALKTHROUGH",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "left",
			"verticalAlign": "top",
			"baseline": 17,
			"containerId": null,
			"originalText": "WALKTHROUGH",
			"lineHeight": 1.25
		},
		{
			"id": "DNPxkTHc",
			"type": "text",
			"x": 7504.302438252177,
			"y": 776.8968158344537,
			"width": 151,
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
			"seed": 2075437412,
			"version": 12,
			"versionNonce": 2040481116,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230493153,
			"link": null,
			"locked": false,
			"text": "BRUTEFORECE",
			"rawText": "BRUTEFORECE",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "left",
			"verticalAlign": "top",
			"baseline": 17,
			"containerId": null,
			"originalText": "BRUTEFORECE",
			"lineHeight": 1.25
		},
		{
			"id": "EEkgMBz4",
			"type": "text",
			"x": 6998.5881089413515,
			"y": 863.1825649974002,
			"width": 415,
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
			"seed": 270179932,
			"version": 266,
			"versionNonce": 279620452,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686230811521,
			"link": null,
			"locked": false,
			"text": "- currMaxArea = 0\n- iterate height i = 0\n    - iterate height j = i + 1\n        -  currArear = \n           Min of  (len[i], len[j]) x (j - i) \n        - if currArea > currMaxArea\n            - currMaxAea = currArea\n- return currMaxArea ",
			"rawText": "- currMaxArea = 0\n- iterate height i = 0\n    - iterate height j = i + 1\n        -  currArear = \n           Min of  (len[i], len[j]) x (j - i) \n        - if currArea > currMaxArea\n            - currMaxAea = currArea\n- return currMaxArea ",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "left",
			"verticalAlign": "top",
			"baseline": 192,
			"containerId": null,
			"originalText": "- currMaxArea = 0\n- iterate height i = 0\n    - iterate height j = i + 1\n        -  currArear = \n           Min of  (len[i], len[j]) x (j - i) \n        - if currArea > currMaxArea\n            - currMaxAea = currArea\n- return currMaxArea ",
			"lineHeight": 1.25
		},
		{
			"id": "w6wR1Ty0wW0bz6-HPJGsl",
			"type": "freedraw",
			"x": 7050.016723966455,
			"y": 594.0396729773109,
			"width": 47.42854527064719,
			"height": 5.714285714285666,
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
			"seed": 1977024484,
			"version": 14,
			"versionNonce": 1768909660,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686231225744,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					4.571402413504984,
					-1.7143031529017208
				],
				[
					14.285714285714675,
					-3.4285627092633604
				],
				[
					22.285679408481883,
					-4.57144601004461
				],
				[
					33.142830984933425,
					-4.57144601004461
				],
				[
					35.99997384207563,
					-4.57144601004461
				],
				[
					42.28567940848188,
					-5.142865862165081
				],
				[
					45.142822265625,
					-5.714285714285666
				],
				[
					45.714285714286234,
					-5.714285714285666
				],
				[
					46.857125418527175,
					-5.714285714285666
				],
				[
					47.42854527064719,
					-5.714285714285666
				],
				[
					47.42854527064719,
					-4.57144601004461
				],
				[
					47.42854527064719,
					-4.57144601004461
				]
			],
			"pressures": [
				0.2822265625,
				0.5107421875,
				0.51953125,
				0.5234375,
				0.525390625,
				0.525390625,
				0.525390625,
				0.529296875,
				0.529296875,
				0.4921875,
				0.4228515625,
				0.013671875,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				47.42854527064719,
				-4.57144601004461
			]
		},
		{
			"id": "UKqIZfZxCRUTz7JltHmlM",
			"type": "freedraw",
			"x": 7053.445286675718,
			"y": 596.3253959823334,
			"width": 13.71429443359375,
			"height": 26.85712541852672,
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
			"seed": 940869732,
			"version": 8,
			"versionNonce": 1809898844,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686231227418,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-10.285731724329708,
					14.28571428571422
				],
				[
					-11.428571428570649,
					16.571437290736526
				],
				[
					-13.142874581472825,
					21.714259556361526
				],
				[
					-13.71429443359375,
					26.85712541852672
				],
				[
					-9.142848423548458,
					23.42856270926336
				],
				[
					-9.142848423548458,
					23.42856270926336
				]
			],
			"pressures": [
				0.2255859375,
				0.41015625,
				0.4375,
				0.453125,
				0.453125,
				0.0146484375,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				-9.142848423548458,
				23.42856270926336
			]
		},
		{
			"id": "RghPOjE1kdD4GUHdHJwo7",
			"type": "freedraw",
			"x": 7066.016697808531,
			"y": 594.6110928294315,
			"width": 22.28572300502219,
			"height": 35.42859758649547,
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
			"seed": 1697330788,
			"version": 8,
			"versionNonce": 1493782364,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686231227675,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-7.4285452706471915,
					9.714311872209805
				],
				[
					-15.428553989954708,
					20
				],
				[
					-21.14283970424094,
					31.428571428571445
				],
				[
					-22.28572300502219,
					35.42859758649547
				],
				[
					-17.142857142856883,
					29.142848423549026
				],
				[
					-17.142857142856883,
					29.142848423549026
				]
			],
			"pressures": [
				0.2548828125,
				0.3544921875,
				0.4345703125,
				0.4462890625,
				0.41015625,
				0.0146484375,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				-17.142857142856883,
				29.142848423549026
			]
		},
		{
			"id": "Baggizc3tkV2qfl3kyS3U",
			"type": "freedraw",
			"x": 7076.873849384982,
			"y": 591.1825301201682,
			"width": 26.28570556640625,
			"height": 43.42856270926336,
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
			"seed": 310043748,
			"version": 7,
			"versionNonce": 1090457316,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686231227899,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-9.142848423549367,
					15.428553989955276
				],
				[
					-16.571437290736867,
					27.428588867187386
				],
				[
					-26.28570556640625,
					43.42856270926336
				],
				[
					-20,
					41.142839704241055
				],
				[
					-20,
					41.142839704241055
				]
			],
			"pressures": [
				0.23046875,
				0.3828125,
				0.4482421875,
				0.466796875,
				0.0146484375,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				-20,
				41.142839704241055
			]
		},
		{
			"id": "OqHqE09oD0rwpi48bG18J",
			"type": "freedraw",
			"x": 7091.159563670696,
			"y": 594.6110928294315,
			"width": 26.857125418526266,
			"height": 46.857169015066916,
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
			"seed": 493404508,
			"version": 9,
			"versionNonce": 1702835036,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686231228124,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-8.000008719307516,
					11.428571428571445
				],
				[
					-16.571437290735958,
					22.85714285714289
				],
				[
					-23.428562709263133,
					37.714276994977695
				],
				[
					-26.857125418526266,
					44.57144601004461
				],
				[
					-25.714285714285325,
					46.857169015066916
				],
				[
					-18.85716029575906,
					39.428580147879416
				],
				[
					-18.85716029575906,
					39.428580147879416
				]
			],
			"pressures": [
				0.2109375,
				0.3388671875,
				0.4365234375,
				0.4912109375,
				0.494140625,
				0.298828125,
				0.013671875,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				-18.85716029575906,
				39.428580147879416
			]
		},
		{
			"id": "zHf7KFvTmNpUJQc4ndqvl",
			"type": "freedraw",
			"x": 7097.445269237102,
			"y": 611.1825301201682,
			"width": 24.571402413504075,
			"height": 46.85712541852672,
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
			"seed": 465911908,
			"version": 10,
			"versionNonce": 1346869724,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686231228351,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-6.28570556640625,
					13.142874581473166
				],
				[
					-9.142848423548458,
					17.14285714285711
				],
				[
					-18.285696847097825,
					28.571428571428555
				],
				[
					-20.571419852120016,
					32.571411132812386
				],
				[
					-22.857142857142208,
					40.57141985212047
				],
				[
					-24.571402413504075,
					45.714285714285666
				],
				[
					-24.571402413504075,
					46.85712541852672
				],
				[
					-24.571402413504075,
					46.85712541852672
				]
			],
			"pressures": [
				0.21875,
				0.3193359375,
				0.365234375,
				0.478515625,
				0.48046875,
				0.4609375,
				0.259765625,
				0.1904296875,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				-24.571402413504075,
				46.85712541852672
			]
		},
		{
			"id": "gXBmmcTTk5IrH1zzcJPQA",
			"type": "freedraw",
			"x": 7049.445260517795,
			"y": 592.3253698244092,
			"width": 106.28574916294656,
			"height": 10.285688127790195,
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
			"seed": 1828487652,
			"version": 23,
			"versionNonce": 721811556,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686231232070,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					6.8571690150665745,
					-1.1428397042410552
				],
				[
					14.857177734375,
					-1.7142595563616396
				],
				[
					16.00001743861594,
					-1.7142595563616396
				],
				[
					20.571463448660325,
					-2.2856794084821104
				],
				[
					28.000008719307516,
					-3.4285627092633604
				],
				[
					36.57143729073596,
					-4.571402413504529
				],
				[
					43.42860630580344,
					-5.142822265625
				],
				[
					50.28573172432971,
					-6.28570556640625
				],
				[
					59.428580147879075,
					-6.857125418526834
				],
				[
					66.28574916294656,
					-7.428545270647305
				],
				[
					72.57145472935281,
					-7.99996512276789
				],
				[
					76.57143729073596,
					-7.99996512276789
				],
				[
					84.00002615792346,
					-8.571428571428555
				],
				[
					90.85715157645063,
					-8.571428571428555
				],
				[
					96.00001743861594,
					-9.14284842354914
				],
				[
					100,
					-10.285688127790195
				],
				[
					102.28572300502219,
					-10.285688127790195
				],
				[
					104.57144601004438,
					-10.285688127790195
				],
				[
					105.71428571428532,
					-9.71426827566961
				],
				[
					106.28574916294656,
					-9.14284842354914
				],
				[
					106.28574916294656,
					-9.14284842354914
				]
			],
			"pressures": [
				0.1943359375,
				0.2509765625,
				0.2880859375,
				0.298828125,
				0.3447265625,
				0.380859375,
				0.39453125,
				0.4072265625,
				0.412109375,
				0.4140625,
				0.412109375,
				0.400390625,
				0.4091796875,
				0.412109375,
				0.423828125,
				0.4384765625,
				0.44921875,
				0.4521484375,
				0.4482421875,
				0.1005859375,
				0.0146484375,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				106.28574916294656,
				-9.14284842354914
			]
		},
		{
			"id": "Jer7guGDkNgXyYQnUGy4l",
			"type": "freedraw",
			"x": 7112.302403374937,
			"y": 600.3253785437172,
			"width": 24.571402413504075,
			"height": 26.85716901506703,
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
			"seed": 1790914524,
			"version": 7,
			"versionNonce": 455634268,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686231233729,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-18.285696847097825,
					17.142857142857224
				],
				[
					-23.99998256138315,
					25.71428571428578
				],
				[
					-24.571402413504075,
					26.85716901506703
				],
				[
					-21.14283970424094,
					22.85714285714289
				],
				[
					-21.14283970424094,
					22.85714285714289
				]
			],
			"pressures": [
				0.171875,
				0.2158203125,
				0.197265625,
				0.14453125,
				0.0126953125,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				-21.14283970424094,
				22.85714285714289
			]
		},
		{
			"id": "zkDKmvuGAN3xvF7QxtGUs",
			"type": "freedraw",
			"x": 7124.87385810429,
			"y": 582.6111015487396,
			"width": 44.00002615792346,
			"height": 53.142874581473166,
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
			"seed": 1541711460,
			"version": 10,
			"versionNonce": 1928106972,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686231233990,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-7.4285888671875,
					9.142848423549026
				],
				[
					-18.285740443638133,
					21.71430315290172
				],
				[
					-29.71431187220969,
					36.571437290736526
				],
				[
					-33.71429443359375,
					41.71430315290172
				],
				[
					-41.14288330078125,
					50.285731724330276
				],
				[
					-44.00002615792346,
					53.142874581473166
				],
				[
					-35.428597586495016,
					49.142848423549026
				],
				[
					-35.428597586495016,
					49.142848423549026
				]
			],
			"pressures": [
				0.1533203125,
				0.28125,
				0.3583984375,
				0.37109375,
				0.37109375,
				0.3232421875,
				0.2412109375,
				0.013671875,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				-35.428597586495016,
				49.142848423549026
			]
		},
		{
			"id": "K5tFVfMQRJzGmOlfx9uJV",
			"type": "freedraw",
			"x": 7139.1595723900045,
			"y": 588.3253872630253,
			"width": 40.571419852120925,
			"height": 43.999982561383945,
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
			"seed": 1857824740,
			"version": 8,
			"versionNonce": 1665517020,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686231234219,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-22.28572300502219,
					23.42856270926336
				],
				[
					-36.00001743861594,
					38.285696847098166
				],
				[
					-38.85716029575906,
					41.71430315290172
				],
				[
					-40.571419852120925,
					43.999982561383945
				],
				[
					-26.28570556640625,
					34.857134137834805
				],
				[
					-26.28570556640625,
					34.857134137834805
				]
			],
			"pressures": [
				0.1923828125,
				0.4052734375,
				0.4716796875,
				0.4775390625,
				0.4775390625,
				0.015625,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				-26.28570556640625,
				34.857134137834805
			]
		},
		{
			"id": "wSmaQbjlyWgo5yVtkrHha",
			"type": "freedraw",
			"x": 7150.016723966455,
			"y": 591.7539499722886,
			"width": 30.285731724330617,
			"height": 42.285723005022305,
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
			"seed": 826742244,
			"version": 9,
			"versionNonce": 2011890660,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686231234438,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-9.714311872209692,
					16.57143729073664
				],
				[
					-22.28572300502219,
					29.714311872209805
				],
				[
					-28.000008719307516,
					37.714276994977695
				],
				[
					-30.285731724330617,
					42.285723005022305
				],
				[
					-29.142892020088766,
					42.285723005022305
				],
				[
					-19.428580147879075,
					34.857134137834805
				],
				[
					-19.428580147879075,
					34.857134137834805
				]
			],
			"pressures": [
				0.1923828125,
				0.37109375,
				0.455078125,
				0.4697265625,
				0.4521484375,
				0.3349609375,
				0.0146484375,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				-19.428580147879075,
				34.857134137834805
			]
		},
		{
			"id": "FarVpWaJIrXEYH6MFOEFp",
			"type": "freedraw",
			"x": 7153.445286675718,
			"y": 606.039664258003,
			"width": 21.14288330078125,
			"height": 30.85715157645086,
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
			"seed": 321035356,
			"version": 9,
			"versionNonce": 1576242780,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686231234638,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-2.8571428571422075,
					5.714285714285666
				],
				[
					-9.142848423548458,
					14.857134137834805
				],
				[
					-17.142857142856883,
					26.28570556640625
				],
				[
					-20,
					28.571428571428555
				],
				[
					-21.14288330078125,
					30.85715157645086
				],
				[
					-8.571428571428442,
					22.285723005022305
				],
				[
					-8.571428571428442,
					22.285723005022305
				]
			],
			"pressures": [
				0.171875,
				0.255859375,
				0.3642578125,
				0.416015625,
				0.4189453125,
				0.38671875,
				0.013671875,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				-8.571428571428442,
				22.285723005022305
			]
		},
		{
			"id": "IqZKSlxt17QZX-01dhT-B",
			"type": "freedraw",
			"x": 7159.730992242125,
			"y": 619.1825388394761,
			"width": 13.142874581472825,
			"height": 17.714276994977695,
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
			"seed": 1469584740,
			"version": 6,
			"versionNonce": 2069584860,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686231234754,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-7.4285888671875,
					8.571428571428555
				],
				[
					-10.285731724329708,
					13.142830984933084
				],
				[
					-13.142874581472825,
					17.714276994977695
				],
				[
					-13.142874581472825,
					17.714276994977695
				]
			],
			"pressures": [
				0.173828125,
				0.1923828125,
				0.1455078125,
				0.0126953125,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				-13.142874581472825,
				17.714276994977695
			]
		},
		{
			"id": "DfoK0zq5VzAUZhsA_myB7",
			"type": "freedraw",
			"x": 7155.731009680741,
			"y": 584.8968245537619,
			"width": 69.14284842354846,
			"height": 8.571428571428555,
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
			"seed": 2138955748,
			"version": 19,
			"versionNonce": 448503652,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686231236546,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					10.285688127789399,
					-1.14288330078125
				],
				[
					14.285714285713766,
					-1.7143031529018344
				],
				[
					18.85711669921875,
					-2.285723005022305
				],
				[
					24.571402413504075,
					-2.8571428571428896
				],
				[
					26.28570556640625,
					-2.8571428571428896
				],
				[
					34.85713413783469,
					-3.428562709263474
				],
				[
					40.571419852120016,
					-4.571446010044724
				],
				[
					41.71425955636096,
					-5.142865862165195
				],
				[
					49.14284842354846,
					-6.857169015067029
				],
				[
					56.57139369419565,
					-8.000008719308084
				],
				[
					60.571419852120016,
					-8.571428571428555
				],
				[
					64.57140241350407,
					-8.571428571428555
				],
				[
					65.71428571428532,
					-8.000008719308084
				],
				[
					68.57142857142844,
					-8.000008719308084
				],
				[
					69.14284842354846,
					-8.000008719308084
				],
				[
					69.14284842354846,
					-6.857169015067029
				],
				[
					69.14284842354846,
					-6.857169015067029
				]
			],
			"pressures": [
				0.1865234375,
				0.2568359375,
				0.2861328125,
				0.3291015625,
				0.3525390625,
				0.3564453125,
				0.365234375,
				0.3671875,
				0.369140625,
				0.3818359375,
				0.3955078125,
				0.3984375,
				0.423828125,
				0.435546875,
				0.453125,
				0.4658203125,
				0.013671875,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				69.14284842354846,
				-6.857169015067029
			]
		},
		{
			"id": "C1UeuSNkguyidM6-fA-ue",
			"type": "freedraw",
			"x": 7176.873849384982,
			"y": 584.3254047016413,
			"width": 19.428580147879984,
			"height": 33.142830984933084,
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
			"seed": 937130204,
			"version": 9,
			"versionNonce": 723135196,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686231237049,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-13.142874581473734,
					21.142839704241055
				],
				[
					-17.142857142857792,
					27.428545270647305
				],
				[
					-19.428580147879984,
					31.428571428571445
				],
				[
					-18.285696847098734,
					33.142830984933084
				],
				[
					-13.71429443359375,
					31.428571428571445
				],
				[
					-5.714285714286234,
					25.142822265625
				],
				[
					-5.714285714286234,
					25.142822265625
				]
			],
			"pressures": [
				0.2431640625,
				0.3955078125,
				0.421875,
				0.40625,
				0.3388671875,
				0.197265625,
				0.0126953125,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				-5.714285714286234,
				25.142822265625
			]
		},
		{
			"id": "F47PitYFZ7RORsGhf3mxK",
			"type": "freedraw",
			"x": 7198.588152537884,
			"y": 582.6111015487396,
			"width": 22.857142857142208,
			"height": 41.71430315290172,
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
			"seed": 1259831524,
			"version": 7,
			"versionNonce": 458947428,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686231237267,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-5.1428658621653085,
					8.00000871930797
				],
				[
					-12.571454729352808,
					21.71430315290172
				],
				[
					-22.857142857142208,
					34.857134137834805
				],
				[
					-22.28572300502219,
					41.71430315290172
				],
				[
					-22.28572300502219,
					41.71430315290172
				]
			],
			"pressures": [
				0.2109375,
				0.3154296875,
				0.384765625,
				0.4072265625,
				0.013671875,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				-22.28572300502219,
				41.71430315290172
			]
		},
		{
			"id": "VZ0n7ikYWH3ES2-j8nmxD",
			"type": "freedraw",
			"x": 7210.588143818576,
			"y": 590.0396904159271,
			"width": 23.428562709264042,
			"height": 41.714259556361526,
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
			"seed": 409984220,
			"version": 8,
			"versionNonce": 874522980,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1686231237476,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-11.999991280692484,
					18.285696847098166
				],
				[
					-19.428580147879984,
					29.142848423549026
				],
				[
					-21.714303152902175,
					33.71425083705344
				],
				[
					-23.428562709264042,
					41.714259556361526
				],
				[
					-16.00001743861594,
					35.99997384207586
				],
				[
					-16.00001743861594,
					35.99997384207586
				]
			],
			"pressures": [
				0.212890625,
				0.423828125,
				0.470703125,
				0.474609375,
				0.28125,
				0.013671875,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				-16.00001743861594,
				35.99997384207586
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
		"scrollX": -6630.3024120942455,
		"scrollY": -105.71823786640142,
		"zoom": {
			"value": 0.7000000000000001
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