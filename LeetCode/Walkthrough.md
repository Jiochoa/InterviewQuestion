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

Info ^CuJHrOKm

- int[] nums: Array of integers
- int target: integer
- One solution
- don't use same element twice

> int[] twoSum (int[] nums, int target) <  ^4bKTrt45

Example ^KtihYIHC

Walkthrough ^xwmves8c

t ^5UZHxEyp

f ^UFySeXJW

return new int[] {i, j} ^GpTQ957t

return NULL ^dSX0TpvP

loop the nums (i = 0) ^riUQ2AqO

loop the nums (j = i + 1) ^jb8P1ZSP

if target == nums[i] + nums[j] ^MoAtt0Bz

Bruteforce ^SiIIpeqI

- loop nums
    - loop nums (start one after the i )
        - if both nums are == target return them ^m0e83AsJ

Optimization ^XL5Rzdin

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

Implementation ^v4OfmmPE

[[LeetCode/Questions#Solution 1]] ^4DszYKaL

## 2. Add Two Numbers
 ^CjwqNKbu

Info ^k7qRZbC9

- given two reversed non-negative integers made into Link List
    -  ex. 234 => 4-> 3-> 2
- return the sum of these numbers in reverse
- no leading zeros
    - ex. 034 ^YiC895uq

Example ^SnaKSG0t

Input: l1 = [2,4,3], l2 = [5,6,4]
Output: [7,0,8]
Explanation: 342 + 465 = 807. ^3mh7wTWn

Walkthrough ^oDIhD1vm

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

Bruteforce  ^4pQSL374

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

Optimization ^VCCU9bsz

- Save space by overwriting l1 to place the results
 ^WzD1RNLk

Implementation ^KHAjE5i0

[[LeetCode/Questions#Solution 2]] ^8HEJKyGR

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
			"version": 316,
			"versionNonce": 935382718,
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
			"updated": 1685715167494,
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
			"version": 312,
			"versionNonce": 1015481378,
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
			"updated": 1685715167494,
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
			"version": 304,
			"versionNonce": 1987331838,
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
			"updated": 1685715167494,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 280,
			"versionNonce": 253112290,
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
			"updated": 1685715167494,
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
			"version": 356,
			"versionNonce": 948877118,
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
			"updated": 1685715167494,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 324,
			"versionNonce": 1716118434,
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
			"updated": 1685715167494,
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
			"version": 398,
			"versionNonce": 1718689662,
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
			"updated": 1685715167494,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 371,
			"versionNonce": 1280384866,
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
			"updated": 1685715167494,
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
			"version": 408,
			"versionNonce": 878477246,
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
			"updated": 1685715167495,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 509,
			"versionNonce": 763028258,
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
			"updated": 1685715167495,
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
			"version": 313,
			"versionNonce": 644995070,
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
			"updated": 1685715167495,
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
			"version": 375,
			"versionNonce": 339095266,
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
			"updated": 1685715167495,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 340,
			"versionNonce": 347220030,
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
			"updated": 1685715167495,
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
			"version": 861,
			"versionNonce": 1607530601,
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
			"updated": 1685721101580,
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
			"version": 894,
			"versionNonce": 566756169,
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
			"updated": 1685721101580,
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
			"version": 66,
			"versionNonce": 448618082,
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
			"width": 41,
			"height": 25,
			"seed": 434069263,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685715167495,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Info",
			"rawText": "Info",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Info",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 175,
			"versionNonce": 18329790,
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
			"updated": 1685715167495,
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
			"version": 112,
			"versionNonce": 34030114,
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
			"width": 76,
			"height": 25,
			"seed": 456646927,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685715167495,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Example",
			"rawText": "Example",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Example",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 153,
			"versionNonce": 1990125822,
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
			"width": 115,
			"height": 25,
			"seed": 1094953775,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685715167496,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Walkthrough",
			"rawText": "Walkthrough",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Walkthrough",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "line",
			"version": 1039,
			"versionNonce": 1977527778,
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
			"updated": 1685715167496,
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
			"version": 800,
			"versionNonce": 1595218238,
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
			"updated": 1685715167496,
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
			"version": 1067,
			"versionNonce": 458400162,
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
			"updated": 1685715167496,
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
			"version": 965,
			"versionNonce": 1910194558,
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
			"updated": 1685715167496,
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
			"version": 879,
			"versionNonce": 496115042,
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
			"updated": 1685715167496,
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
			"version": 631,
			"versionNonce": 1379033534,
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
			"updated": 1685715167496,
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
			"version": 823,
			"versionNonce": 1777082658,
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
			"updated": 1685715167496,
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
			"version": 732,
			"versionNonce": 322664958,
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
			"updated": 1685715167496,
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
			"version": 1385,
			"versionNonce": 1808772322,
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
			"updated": 1685715167496,
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
			"version": 504,
			"versionNonce": 1006078526,
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
			"updated": 1685715167496,
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
			"version": 1557,
			"versionNonce": 1221312674,
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
			"updated": 1685715167496,
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
			"version": 407,
			"versionNonce": 1262981758,
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
			"updated": 1685715167496,
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
			"version": 342,
			"versionNonce": 479157346,
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
			"updated": 1685715167496,
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
			"version": 381,
			"versionNonce": 1005359806,
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
			"updated": 1685715167496,
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
			"version": 400,
			"versionNonce": 887717922,
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
			"updated": 1685715167496,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 386,
			"versionNonce": 143100670,
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
			"updated": 1685715167496,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 346,
			"versionNonce": 1305029602,
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
			"updated": 1685715167496,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 362,
			"versionNonce": 798587710,
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
			"updated": 1685715167497,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 412,
			"versionNonce": 1295867810,
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
			"updated": 1685715167497,
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
			"version": 487,
			"versionNonce": 931357566,
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
			"updated": 1685715167497,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 374,
			"versionNonce": 2138381154,
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
			"updated": 1685715167497,
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
			"version": 413,
			"versionNonce": 847659966,
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
			"updated": 1685715167497,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 435,
			"versionNonce": 1388273442,
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
			"updated": 1685715167497,
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
			"version": 350,
			"versionNonce": 1120082942,
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
			"updated": 1685715167497,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 193,
			"versionNonce": 327887586,
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
			"width": 108,
			"height": 25,
			"seed": 231449188,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685715167497,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Bruteforce",
			"rawText": "Bruteforce",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Bruteforce",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 212,
			"versionNonce": 507178046,
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
			"updated": 1685715167497,
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
			"version": 103,
			"versionNonce": 677871266,
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
			"width": 116,
			"height": 25,
			"seed": 1077618788,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685715167497,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Optimization",
			"rawText": "Optimization",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Optimization",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 81,
			"versionNonce": 315536510,
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
			"updated": 1685715167497,
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
			"version": 77,
			"versionNonce": 1308842594,
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
			"updated": 1685715167497,
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
			"version": 114,
			"versionNonce": 171930814,
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
			"updated": 1685715167497,
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
			"version": 197,
			"versionNonce": 1395506722,
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
			"updated": 1685715167497,
			"link": null,
			"locked": false
		},
		{
			"type": "line",
			"version": 209,
			"versionNonce": 237907198,
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
			"updated": 1685715167497,
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
			"version": 225,
			"versionNonce": 1423288802,
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
			"updated": 1685715167497,
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
			"version": 173,
			"versionNonce": 1276894526,
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
			"updated": 1685715167497,
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
			"version": 229,
			"versionNonce": 2047483298,
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
			"updated": 1685715167498,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 402,
			"versionNonce": 426345854,
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
			"updated": 1685715167498,
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
			"version": 207,
			"versionNonce": 804919650,
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
			"updated": 1685715167498,
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
			"version": 58,
			"versionNonce": 2002265534,
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
			"updated": 1685715167498,
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
			"version": 122,
			"versionNonce": 1710529826,
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
			"updated": 1685715167498,
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
			"version": 114,
			"versionNonce": 386448894,
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
			"updated": 1685715167498,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 145,
			"versionNonce": 1231595746,
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
			"updated": 1685715167498,
			"link": null,
			"locked": false
		},
		{
			"type": "arrow",
			"version": 585,
			"versionNonce": 1568427582,
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
			"updated": 1685715167498,
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
			"version": 56,
			"versionNonce": 31800482,
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
			"updated": 1685715167498,
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
			"version": 291,
			"versionNonce": 1737741950,
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
			"updated": 1685715167498,
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
			"version": 243,
			"versionNonce": 1830377570,
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
			"updated": 1685715167498,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 138,
			"versionNonce": 235951806,
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
			"updated": 1685715167498,
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
			"version": 235,
			"versionNonce": 1523842082,
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
			"updated": 1685715167498,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 257,
			"versionNonce": 1771228926,
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
			"updated": 1685715167498,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 285,
			"versionNonce": 1225009122,
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
			"updated": 1685715167498,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 355,
			"versionNonce": 1453080382,
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
			"updated": 1685715167498,
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
			"version": 347,
			"versionNonce": 532208546,
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
			"updated": 1685715167498,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 323,
			"versionNonce": 2039326590,
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
			"updated": 1685715167498,
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
			"version": 402,
			"versionNonce": 1830885218,
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
			"updated": 1685715167498,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 367,
			"versionNonce": 1118308286,
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
			"updated": 1685715167498,
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
			"version": 441,
			"versionNonce": 562813730,
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
			"updated": 1685715167498,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 414,
			"versionNonce": 1913413630,
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
			"updated": 1685715167498,
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
			"version": 451,
			"versionNonce": 1265116898,
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
			"updated": 1685715167498,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 552,
			"versionNonce": 465285182,
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
			"updated": 1685715167498,
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
			"version": 356,
			"versionNonce": 1397029538,
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
			"updated": 1685715167498,
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
			"version": 421,
			"versionNonce": 731314302,
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
			"updated": 1685715167499,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 383,
			"versionNonce": 936466018,
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
			"updated": 1685715167499,
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
			"version": 254,
			"versionNonce": 1767848126,
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
			"updated": 1685715167499,
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
			"version": 262,
			"versionNonce": 1239169570,
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
			"updated": 1685715167499,
			"link": null,
			"locked": false
		},
		{
			"type": "arrow",
			"version": 882,
			"versionNonce": 2092265726,
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
			"updated": 1685715167499,
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
			"version": 117,
			"versionNonce": 1750377954,
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
			"updated": 1685715167499,
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
			"version": 431,
			"versionNonce": 1897570622,
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
			"updated": 1685715167499,
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
			"version": 438,
			"versionNonce": 1011456418,
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
			"updated": 1685715167499,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 480,
			"versionNonce": 972015998,
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
			"updated": 1685715167499,
			"link": null,
			"locked": false
		},
		{
			"type": "arrow",
			"version": 433,
			"versionNonce": 1961497954,
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
			"updated": 1685715167499,
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
			"version": 128,
			"versionNonce": 913697214,
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
			"updated": 1685715167499,
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
			"version": 704,
			"versionNonce": 779388169,
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
			"updated": 1685721101595,
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
			"version": 285,
			"versionNonce": 902693374,
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
			"updated": 1685715167499,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 209,
			"versionNonce": 1468638434,
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
			"updated": 1685715167499,
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
			"version": 167,
			"versionNonce": 2063143486,
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
			"updated": 1685715167499,
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
			"version": 121,
			"versionNonce": 445036706,
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
			"updated": 1685715167500,
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
			"version": 189,
			"versionNonce": 1087904382,
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
			"updated": 1685715167500,
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
			"version": 214,
			"versionNonce": 1814778978,
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
			"updated": 1685715167500,
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
			"version": 112,
			"versionNonce": 1043077822,
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
			"updated": 1685715167500,
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
			"version": 59,
			"versionNonce": 507934754,
			"isDeleted": false,
			"id": "v4OfmmPE",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -429.33972492683324,
			"y": 1571.7204419200566,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 142,
			"height": 25,
			"seed": 629827804,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685715167500,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Implementation",
			"rawText": "Implementation",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Implementation",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 122,
			"versionNonce": 697701118,
			"isDeleted": false,
			"id": "4DszYKaL",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -379.30299777220455,
			"y": 1619.3113367930803,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 366,
			"height": 25,
			"seed": 1529320804,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685715167500,
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
			"version": 210,
			"versionNonce": 1892099042,
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
			"updated": 1685715167500,
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
			"version": 91,
			"versionNonce": 1033306942,
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
			"updated": 1685715167500,
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
			"version": 48,
			"versionNonce": 1304188834,
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
			"width": 41,
			"height": 25,
			"seed": 752181604,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685715167500,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Info",
			"rawText": "Info",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Info",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 215,
			"versionNonce": 1016064894,
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
			"updated": 1685715167500,
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
			"version": 51,
			"versionNonce": 89461602,
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
			"width": 76,
			"height": 25,
			"seed": 1934118364,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685715167500,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Example",
			"rawText": "Example",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Example",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 45,
			"versionNonce": 1958857662,
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
			"updated": 1685715167500,
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
			"version": 89,
			"versionNonce": 165697314,
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
			"width": 115,
			"height": 25,
			"seed": 610995556,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685715167500,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Walkthrough",
			"rawText": "Walkthrough",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Walkthrough",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 1410,
			"versionNonce": 1140290302,
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
			"updated": 1685715408549,
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
			"version": 581,
			"versionNonce": 727749026,
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
			"updated": 1685715167502,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 423,
			"versionNonce": 635720062,
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
			"updated": 1685715167502,
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
			"version": 519,
			"versionNonce": 1449266530,
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
			"updated": 1685715167502,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 409,
			"versionNonce": 1117352382,
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
			"updated": 1685715167502,
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
			"version": 471,
			"versionNonce": 1665012002,
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
			"updated": 1685715167502,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 383,
			"versionNonce": 71338494,
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
			"updated": 1685715167502,
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
			"version": 1170,
			"versionNonce": 1539020489,
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
			"updated": 1685721101600,
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
			"version": 733,
			"versionNonce": 8705607,
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
			"updated": 1685721101600,
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
			"version": 696,
			"versionNonce": 711045282,
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
			"updated": 1685715167502,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 641,
			"versionNonce": 1783145086,
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
			"updated": 1685715167502,
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
			"version": 628,
			"versionNonce": 904350818,
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
			"updated": 1685715167502,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 601,
			"versionNonce": 2018222782,
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
			"updated": 1685715167502,
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
			"version": 698,
			"versionNonce": 1036218402,
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
			"updated": 1685715167502,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 652,
			"versionNonce": 109353726,
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
			"updated": 1685715167502,
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
			"version": 582,
			"versionNonce": 98900962,
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
			"updated": 1685715167502,
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
			"version": 1187,
			"versionNonce": 1469044137,
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
			"updated": 1685721101606,
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
			"version": 567,
			"versionNonce": 2086358946,
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
			"updated": 1685715167503,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 525,
			"versionNonce": 92042110,
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
			"updated": 1685715167503,
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
			"version": 584,
			"versionNonce": 1968507746,
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
			"updated": 1685715167503,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 562,
			"versionNonce": 2128434110,
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
			"updated": 1685715167503,
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
			"version": 571,
			"versionNonce": 1730236194,
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
			"updated": 1685715167503,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 550,
			"versionNonce": 297282558,
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
			"updated": 1685715167503,
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
			"version": 1027,
			"versionNonce": 171996519,
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
			"updated": 1685721101610,
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
			"version": 521,
			"versionNonce": 1812855870,
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
			"updated": 1685715167503,
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
			"version": 276,
			"versionNonce": 554528418,
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
			"updated": 1685715167503,
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
			"version": 274,
			"versionNonce": 1405076606,
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
			"updated": 1685715167503,
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
			"version": 276,
			"versionNonce": 476793442,
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
			"updated": 1685715167503,
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
			"version": 276,
			"versionNonce": 713983166,
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
			"updated": 1685715167503,
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
			"version": 269,
			"versionNonce": 1863822882,
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
			"updated": 1685715167503,
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
			"version": 273,
			"versionNonce": 1914387710,
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
			"updated": 1685715167503,
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
			"version": 353,
			"versionNonce": 1040292322,
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
			"updated": 1685715167504,
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
			"version": 365,
			"versionNonce": 1340534078,
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
			"updated": 1685715167504,
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
			"version": 351,
			"versionNonce": 943197602,
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
			"updated": 1685715167504,
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
			"version": 349,
			"versionNonce": 290624894,
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
			"updated": 1685715167504,
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
			"version": 338,
			"versionNonce": 1391069538,
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
			"updated": 1685715167504,
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
			"version": 337,
			"versionNonce": 798963134,
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
			"updated": 1685715167504,
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
			"version": 134,
			"versionNonce": 799785954,
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
			"width": 118,
			"height": 25,
			"seed": 1148148090,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685715408549,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Bruteforce ",
			"rawText": "Bruteforce ",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Bruteforce ",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 307,
			"versionNonce": 1154245438,
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
			"updated": 1685715408549,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 315,
			"versionNonce": 118290338,
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
			"updated": 1685715408549,
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
			"version": 321,
			"versionNonce": 1981369214,
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
			"updated": 1685715408549,
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
			"version": 544,
			"versionNonce": 194098018,
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
			"updated": 1685715408549,
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
			"version": 152,
			"versionNonce": 1981754302,
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
			"updated": 1685715408549,
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
			"version": 187,
			"versionNonce": 1602811682,
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
			"updated": 1685715408549,
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
			"version": 315,
			"versionNonce": 1929315326,
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
			"updated": 1685715408549,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 287,
			"versionNonce": 56738530,
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
			"updated": 1685715408549,
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
			"version": 399,
			"versionNonce": 296425122,
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
			"updated": 1685715408549,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 374,
			"versionNonce": 53517438,
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
			"updated": 1685715408549,
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
			"version": 1010,
			"versionNonce": 360394887,
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
			"updated": 1685721101618,
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
			"version": 249,
			"versionNonce": 1114330658,
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
			"updated": 1685715408549,
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
			"version": 962,
			"versionNonce": 1542555559,
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
			"updated": 1685721101621,
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
			"version": 307,
			"versionNonce": 950026722,
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
			"updated": 1685715408549,
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
			"version": 369,
			"versionNonce": 1374078270,
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
			"updated": 1685715408549,
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
			"version": 290,
			"versionNonce": 1972858238,
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
			"updated": 1685715408549,
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
			"version": 209,
			"versionNonce": 1703480766,
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
			"updated": 1685715408549,
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
			"version": 371,
			"versionNonce": 1571173666,
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
			"updated": 1685715408549,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 357,
			"versionNonce": 1591518718,
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
			"updated": 1685715408549,
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
			"version": 1247,
			"versionNonce": 735050439,
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
			"updated": 1685721101623,
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
			"version": 200,
			"versionNonce": 1007735970,
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
			"updated": 1685715408549,
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
			"version": 497,
			"versionNonce": 1770897022,
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
			"updated": 1685715408549,
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
			"version": 411,
			"versionNonce": 143474366,
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
			"updated": 1685715408549,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 359,
			"versionNonce": 16356386,
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
			"updated": 1685715408549,
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
			"version": 1425,
			"versionNonce": 1504905703,
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
			"updated": 1685721101626,
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
			"version": 252,
			"versionNonce": 889136958,
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
			"updated": 1685715408549,
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
			"version": 451,
			"versionNonce": 2069394338,
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
			"updated": 1685715408549,
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
			"version": 107,
			"versionNonce": 1628286818,
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
			"updated": 1685715408549,
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
			"version": 99,
			"versionNonce": 1131474878,
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
			"updated": 1685715408549,
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
			"version": 107,
			"versionNonce": 472216354,
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
			"updated": 1685715408549,
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
			"version": 100,
			"versionNonce": 964184062,
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
			"updated": 1685715408549,
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
			"version": 227,
			"versionNonce": 1863237346,
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
			"updated": 1685715408549,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 215,
			"versionNonce": 1567266878,
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
			"updated": 1685715408549,
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
			"version": 290,
			"versionNonce": 1985516194,
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
			"updated": 1685715408549,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 277,
			"versionNonce": 656990334,
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
			"updated": 1685715408549,
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
			"version": 233,
			"versionNonce": 1785995454,
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
			"updated": 1685715408549,
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
			"version": 251,
			"versionNonce": 1525504254,
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
			"updated": 1685715408549,
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
			"version": 448,
			"versionNonce": 342404514,
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
			"updated": 1685715408554,
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
			"version": 155,
			"versionNonce": 1288778146,
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
			"updated": 1685715408549,
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
			"version": 792,
			"versionNonce": 1923560711,
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
			"updated": 1685721101631,
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
			"version": 241,
			"versionNonce": 1086238050,
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
			"updated": 1685715408549,
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
			"version": 410,
			"versionNonce": 836161982,
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
			"updated": 1685715408549,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 424,
			"versionNonce": 419868962,
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
			"updated": 1685715408549,
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
			"version": 316,
			"versionNonce": 1900018238,
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
			"updated": 1685715408549,
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
			"version": 580,
			"versionNonce": 774437927,
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
			"updated": 1685721101634,
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
			"version": 92,
			"versionNonce": 1022618722,
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
			"updated": 1685715408549,
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
			"version": 266,
			"versionNonce": 769196734,
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
			"updated": 1685715408549,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 356,
			"versionNonce": 2050756642,
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
			"updated": 1685715408549,
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
			"version": 460,
			"versionNonce": 720854631,
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
			"updated": 1685721101638,
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
			"version": 89,
			"versionNonce": 724299682,
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
			"updated": 1685715408549,
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
			"version": 211,
			"versionNonce": 1636160382,
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
			"updated": 1685715408549,
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
			"version": 487,
			"versionNonce": 829225351,
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
			"updated": 1685721101639,
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
			"version": 89,
			"versionNonce": 1380577058,
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
			"updated": 1685715408549,
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
			"version": 237,
			"versionNonce": 1122601982,
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
			"updated": 1685715408549,
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
			"version": 211,
			"versionNonce": 1665383138,
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
			"updated": 1685715408549,
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
			"version": 138,
			"versionNonce": 806575166,
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
			"updated": 1685715408549,
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
			"version": 156,
			"versionNonce": 493984034,
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
			"width": 116,
			"height": 25,
			"seed": 1711394814,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685715414477,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Optimization",
			"rawText": "Optimization",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Optimization",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 211,
			"versionNonce": 567326782,
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
			"updated": 1685715426792,
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
			"version": 27,
			"versionNonce": 1713948322,
			"isDeleted": false,
			"id": "KHAjE5i0",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 521.9922148747943,
			"y": 1678.2711418877705,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 142,
			"height": 25,
			"seed": 1105104226,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685715745783,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Implementation",
			"rawText": "Implementation",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Implementation",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 233,
			"versionNonce": 44428414,
			"isDeleted": false,
			"id": "8HEJKyGR",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 549.7452323931591,
			"y": 1738.8325365132189,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 375,
			"height": 25,
			"seed": 1665386558,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685715745783,
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
			"version": 225,
			"versionNonce": 1569865982,
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
			"updated": 1685715770316,
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
		"scrollX": -1222.1445394530938,
		"scrollY": 654.7790026837012,
		"zoom": {
			"value": 0.7396070534130323
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