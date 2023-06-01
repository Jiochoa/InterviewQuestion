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

- find the longest one and loop it
    - add the values = sum
    - if sum > 9
        - sum = sum - 10
        - carry = true
    - solutionLL add link value sum   ^suDg5Eqb

Bruteforce ^pym91Zhn

largestSize += 1 ^KGwjUGcJ

largestSize = 0 ^AFZ3ZRWc

llSolution; ^378lKNzK

valuel1 = 0 ^SIm5WW90

valuel2 = 0 ^24AzcU4z

T ^8hlovFyI

value1 = l1.value ^ljKeKlyW

value2 = l2.value ^eTV2buH5

while either l1_temp or l2_temp are not null ^ZQt3LQf8

for largestSize ^f1S00YO4

if both values not null ^xQxY3kzC

if sum < 9 ^yoIAIXuZ

if carry == true ^cUn8HeKJ

T ^j208RnMj

sum += 1 ^YitmxPR5

T ^wslASSB1

llSolution.value = sum ^XWCHqCBa

else ^CN2nYge6

carry = true ^xElYFQwW

sum -= 10 ^WKOQFTNw

carry = false ^ASXx62SK

llSolution.value = sum ^bXM31pbp

llSolution = next ^UvoTTpgF

llSolution = next ^hPdW1Xdk

2 ^bQ9Kjc4G

4 ^LrJzMGg3

3 ^BY3tMLOh

5 ^q7xmGnTH

6 ^y3MQq29Y

4 ^RqHOIK5i

7 ^RzKJ3NZ7

0 ^W1G5e9CW

8 ^ebTfCNkg

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
			"version": 296,
			"versionNonce": 30964078,
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
			"updated": 1685655862514,
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
			"version": 292,
			"versionNonce": 18390130,
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
			"updated": 1685655862514,
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
			"version": 284,
			"versionNonce": 799218606,
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
			"updated": 1685655862514,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 260,
			"versionNonce": 1685077554,
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
			"updated": 1685655862514,
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
			"version": 336,
			"versionNonce": 140473838,
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
			"updated": 1685655862514,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 304,
			"versionNonce": 1206757362,
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
			"updated": 1685655862514,
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
			"version": 378,
			"versionNonce": 890669102,
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
			"updated": 1685655862514,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 351,
			"versionNonce": 865589682,
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
			"updated": 1685655862514,
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
			"version": 388,
			"versionNonce": 1437684334,
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
			"updated": 1685655862514,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 489,
			"versionNonce": 378917746,
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
			"updated": 1685655862514,
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
			"version": 293,
			"versionNonce": 620287150,
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
			"updated": 1685655862514,
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
			"version": 355,
			"versionNonce": 1663997234,
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
			"updated": 1685655862514,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 320,
			"versionNonce": 479596270,
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
			"updated": 1685655862514,
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
			"version": 789,
			"versionNonce": 717823730,
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
			"updated": 1685655862514,
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
			"version": 822,
			"versionNonce": 420610350,
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
			"updated": 1685655862514,
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
			"version": 46,
			"versionNonce": 971796658,
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
			"updated": 1685655862514,
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
			"version": 155,
			"versionNonce": 2111155054,
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
			"updated": 1685655862514,
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
			"version": 92,
			"versionNonce": 876579442,
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
			"updated": 1685655862514,
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
			"version": 133,
			"versionNonce": 1495928238,
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
			"updated": 1685655862514,
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
			"version": 1019,
			"versionNonce": 814312498,
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
			"updated": 1685655862514,
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
			"version": 780,
			"versionNonce": 137897966,
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
			"updated": 1685655862514,
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
			"version": 1047,
			"versionNonce": 1420891634,
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
			"updated": 1685655862515,
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
			"version": 945,
			"versionNonce": 1527314990,
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
			"updated": 1685655862515,
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
			"version": 859,
			"versionNonce": 1908246450,
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
			"updated": 1685655862515,
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
			"version": 611,
			"versionNonce": 948274286,
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
			"updated": 1685655862515,
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
			"version": 803,
			"versionNonce": 534102386,
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
			"updated": 1685655862515,
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
			"version": 712,
			"versionNonce": 1115080366,
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
			"updated": 1685655862515,
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
			"version": 1365,
			"versionNonce": 1514193714,
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
			"updated": 1685655862515,
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
			"version": 484,
			"versionNonce": 2038808814,
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
			"updated": 1685655862515,
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
			"version": 1537,
			"versionNonce": 459640050,
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
			"updated": 1685655862515,
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
			"version": 387,
			"versionNonce": 1631286062,
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
			"updated": 1685655862515,
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
			"version": 322,
			"versionNonce": 2026577586,
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
			"updated": 1685655862515,
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
			"version": 361,
			"versionNonce": 604036462,
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
			"updated": 1685655862515,
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
			"version": 380,
			"versionNonce": 1058568306,
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
			"updated": 1685655862515,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 366,
			"versionNonce": 924778414,
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
			"updated": 1685655862515,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 326,
			"versionNonce": 236231218,
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
			"updated": 1685655862515,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 342,
			"versionNonce": 2126436846,
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
			"updated": 1685655862515,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 392,
			"versionNonce": 1957069810,
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
			"updated": 1685655862515,
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
			"version": 467,
			"versionNonce": 1911122990,
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
			"updated": 1685655862515,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 354,
			"versionNonce": 215299506,
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
			"updated": 1685655862515,
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
			"version": 393,
			"versionNonce": 1049081454,
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
			"updated": 1685655862515,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 415,
			"versionNonce": 398962546,
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
			"updated": 1685655862515,
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
			"version": 330,
			"versionNonce": 1835186350,
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
			"updated": 1685655862515,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 173,
			"versionNonce": 432337202,
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
			"updated": 1685655862515,
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
			"version": 192,
			"versionNonce": 102986478,
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
			"updated": 1685655862515,
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
			"version": 83,
			"versionNonce": 1983118066,
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
			"updated": 1685655862515,
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
			"version": 61,
			"versionNonce": 861070638,
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
			"updated": 1685655862515,
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
			"version": 57,
			"versionNonce": 194759858,
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
			"updated": 1685655862515,
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
			"version": 94,
			"versionNonce": 1717178222,
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
			"updated": 1685655862515,
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
			"version": 177,
			"versionNonce": 1336108658,
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
			"updated": 1685655862515,
			"link": null,
			"locked": false
		},
		{
			"type": "line",
			"version": 189,
			"versionNonce": 2072113582,
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
			"updated": 1685655862515,
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
			"version": 205,
			"versionNonce": 1796327474,
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
			"updated": 1685655862515,
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
			"version": 153,
			"versionNonce": 1576242158,
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
			"updated": 1685655862515,
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
			"version": 209,
			"versionNonce": 1439560178,
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
			"updated": 1685655862515,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 382,
			"versionNonce": 733470254,
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
			"updated": 1685655862515,
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
			"version": 187,
			"versionNonce": 1927209906,
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
			"updated": 1685655862515,
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
			"version": 38,
			"versionNonce": 1505224814,
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
			"updated": 1685655862515,
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
			"version": 102,
			"versionNonce": 745250162,
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
			"updated": 1685655862515,
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
			"version": 94,
			"versionNonce": 1471982254,
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
			"updated": 1685655862515,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 125,
			"versionNonce": 263921458,
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
			"updated": 1685655862515,
			"link": null,
			"locked": false
		},
		{
			"type": "arrow",
			"version": 565,
			"versionNonce": 879699182,
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
			"updated": 1685655862515,
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
			"version": 36,
			"versionNonce": 1765042418,
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
			"updated": 1685655862516,
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
			"version": 271,
			"versionNonce": 1096308526,
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
			"updated": 1685655862516,
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
			"version": 223,
			"versionNonce": 1616804530,
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
			"updated": 1685655862516,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 118,
			"versionNonce": 920732014,
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
			"updated": 1685655862516,
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
			"version": 215,
			"versionNonce": 333468786,
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
			"updated": 1685655862516,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 237,
			"versionNonce": 1481827246,
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
			"updated": 1685655862516,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 265,
			"versionNonce": 897644082,
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
			"updated": 1685655862516,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 335,
			"versionNonce": 399916526,
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
			"updated": 1685655862516,
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
			"version": 327,
			"versionNonce": 640114674,
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
			"updated": 1685655862516,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 303,
			"versionNonce": 980701230,
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
			"updated": 1685655862516,
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
			"version": 382,
			"versionNonce": 299536818,
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
			"updated": 1685655862516,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 347,
			"versionNonce": 2081823342,
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
			"updated": 1685655862516,
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
			"version": 421,
			"versionNonce": 197233522,
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
			"updated": 1685655862516,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 394,
			"versionNonce": 864328878,
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
			"updated": 1685655862516,
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
			"version": 431,
			"versionNonce": 706956594,
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
			"updated": 1685655862516,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 532,
			"versionNonce": 1986582254,
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
			"updated": 1685655862516,
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
			"version": 336,
			"versionNonce": 577165042,
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
			"updated": 1685655862516,
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
			"version": 401,
			"versionNonce": 1028376878,
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
			"updated": 1685655862516,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 363,
			"versionNonce": 1695754418,
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
			"updated": 1685655862516,
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
			"version": 234,
			"versionNonce": 127300462,
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
			"updated": 1685655862516,
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
			"version": 242,
			"versionNonce": 969884274,
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
			"updated": 1685655862516,
			"link": null,
			"locked": false
		},
		{
			"type": "arrow",
			"version": 862,
			"versionNonce": 2140263854,
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
			"updated": 1685655862516,
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
			"version": 97,
			"versionNonce": 1533158450,
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
			"updated": 1685655862516,
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
			"version": 411,
			"versionNonce": 510062574,
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
			"updated": 1685655862516,
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
			"version": 418,
			"versionNonce": 330485234,
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
			"updated": 1685655862516,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 460,
			"versionNonce": 1344193070,
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
			"updated": 1685655862516,
			"link": null,
			"locked": false
		},
		{
			"type": "arrow",
			"version": 413,
			"versionNonce": 1472741298,
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
			"updated": 1685655862516,
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
			"version": 108,
			"versionNonce": 396512366,
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
			"updated": 1685655862516,
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
			"version": 632,
			"versionNonce": 1674148210,
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
			"updated": 1685655862516,
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
			"version": 265,
			"versionNonce": 851087022,
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
			"updated": 1685655862516,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 189,
			"versionNonce": 1459452722,
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
			"updated": 1685655862516,
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
			"version": 147,
			"versionNonce": 1041271022,
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
			"updated": 1685655862516,
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
			"version": 101,
			"versionNonce": 1338721522,
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
			"updated": 1685655862516,
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
			"version": 169,
			"versionNonce": 1496136494,
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
			"updated": 1685655862516,
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
			"version": 194,
			"versionNonce": 129619634,
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
			"updated": 1685655862516,
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
			"version": 92,
			"versionNonce": 1249486190,
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
			"updated": 1685655862516,
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
			"version": 39,
			"versionNonce": 1869623410,
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
			"updated": 1685655862516,
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
			"version": 102,
			"versionNonce": 591316910,
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
			"updated": 1685655862516,
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
			"version": 190,
			"versionNonce": 1253397042,
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
			"updated": 1685655862516,
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
			"version": 71,
			"versionNonce": 1671799278,
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
			"updated": 1685655862516,
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
			"version": 28,
			"versionNonce": 1282423794,
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
			"updated": 1685655862516,
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
			"version": 195,
			"versionNonce": 515322926,
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
			"updated": 1685655862517,
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
			"version": 31,
			"versionNonce": 849866162,
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
			"updated": 1685655862517,
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
			"version": 25,
			"versionNonce": 509378158,
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
			"updated": 1685655862517,
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
			"version": 35,
			"versionNonce": 1652778866,
			"isDeleted": false,
			"id": "oDIhD1vm",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 501.1456148208066,
			"y": -35.275551696952675,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 115,
			"height": 25,
			"seed": 610995556,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862517,
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
			"version": 232,
			"versionNonce": 123633838,
			"isDeleted": false,
			"id": "suDg5Eqb",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 627.8122814874732,
			"y": 53.057781636380696,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 363,
			"height": 150,
			"seed": 1666972252,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862517,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "- find the longest one and loop it\n    - add the values = sum\n    - if sum > 9\n        - sum = sum - 10\n        - carry = true\n    - solutionLL add link value sum  ",
			"rawText": "- find the longest one and loop it\n    - add the values = sum\n    - if sum > 9\n        - sum = sum - 10\n        - carry = true\n    - solutionLL add link value sum  ",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "- find the longest one and loop it\n    - add the values = sum\n    - if sum > 9\n        - sum = sum - 10\n        - carry = true\n    - solutionLL add link value sum  ",
			"lineHeight": 1.25,
			"baseline": 142
		},
		{
			"type": "freedraw",
			"version": 573,
			"versionNonce": 1035054642,
			"isDeleted": false,
			"id": "WJDIeTcU2R3RIIz6TmKnL",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1161.1635651776598,
			"y": 697.834256783325,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 13.366254283233957,
			"height": 28.475976411997085,
			"seed": 953311196,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862517,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					0.29056688983853357
				],
				[
					-0.29054472100589407,
					2.6151463462121307
				],
				[
					-0.29054472100589407,
					7.554849979965218
				],
				[
					0,
					12.203986723879773
				],
				[
					0.8717228383482402,
					19.177702924167924
				],
				[
					1.1623118970194133,
					21.792849270380106
				],
				[
					1.1623118970194133,
					22.373983050057173
				],
				[
					0.5811337796770671,
					22.08341616021864
				],
				[
					-1.1622675593541343,
					20.049425762516215
				],
				[
					-2.9057132360507136,
					14.819133070091903
				],
				[
					-3.777436074398954,
					10.460563216015883
				],
				[
					-4.067980795404848,
					4.939703633753088
				],
				[
					-2.9057132360507136,
					-1.1622897281868232
				],
				[
					0.5811337796770671,
					-4.649136743914554
				],
				[
					4.358569854076021,
					-6.101993361939911
				],
				[
					7.554872148797908,
					-6.101993361939911
				],
				[
					9.298273487829109,
					-5.520859582262844
				],
				[
					9.298273487829109,
					-3.777436074398954
				],
				[
					6.392560251778395,
					-1.1622897281868232
				],
				[
					6.392560251778395,
					-1.1622897281868232
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.1630859375,
				0.248046875,
				0.265625,
				0.2724609375,
				0.3017578125,
				0.322265625,
				0.3310546875,
				0.353515625,
				0.4326171875,
				0.486328125,
				0.5048828125,
				0.5078125,
				0.501953125,
				0.5,
				0.5087890625,
				0.51171875,
				0.51171875,
				0.4921875,
				0.3291015625,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 558,
			"versionNonce": 1915553262,
			"isDeleted": false,
			"id": "VrhQuhaoHz9ezqlggD5NY",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1154.7710049258815,
			"y": 708.0042531095022,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 15.40028901860171,
			"height": 1.4528566180253568,
			"seed": 647070044,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862517,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					2.3245794563736464,
					1.4528566180253568
				],
				[
					5.811426472101427,
					1.4528566180253568
				],
				[
					11.041719164525688,
					1.1622897281868232
				],
				[
					15.40028901860171,
					0.8717006695156007
				],
				[
					15.40028901860171,
					0.8717006695156007
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2626953125,
				0.275390625,
				0.2783203125,
				0.2841796875,
				0.0146484375,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 617,
			"versionNonce": 1468078066,
			"isDeleted": false,
			"id": "zcBt_-BHk1v45w_uMnpHU",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1171.6241505625085,
			"y": 706.8419633813156,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 8.42655064948077,
			"height": 5.811426472101328,
			"seed": 1172946148,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862517,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-1.4528566180253073,
					2.6151463462121303
				],
				[
					-1.7434456766964803,
					3.4868470157277307
				],
				[
					-1.4528566180253073,
					4.358569854076021
				],
				[
					-0.8717228383482402,
					4.649136743914554
				],
				[
					0.8717228383483393,
					5.2302926924242605
				],
				[
					3.486847015727781,
					4.649136743914554
				],
				[
					6.1019711931072225,
					2.905713236050664
				],
				[
					5.520837413430155,
					1.7434235078638407
				],
				[
					3.486847015727781,
					0.581133779677067
				],
				[
					0.29054472100589407,
					-0.581133779677067
				],
				[
					-1.4528566180253073,
					-0.2905668898385335
				],
				[
					-2.3245794563735473,
					0.2905668898385335
				],
				[
					-2.0339903977023743,
					1.452856618025307
				],
				[
					1.1622675593541343,
					2.905713236050664
				],
				[
					2.6151241773795406,
					3.196280125889197
				],
				[
					0,
					0
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2880859375,
				0.36328125,
				0.3876953125,
				0.419921875,
				0.43359375,
				0.44921875,
				0.462890625,
				0.46875,
				0.4873046875,
				0.498046875,
				0.513671875,
				0.5146484375,
				0.5126953125,
				0.482421875,
				0.0859375,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 623,
			"versionNonce": 783423534,
			"isDeleted": false,
			"id": "_Uq9k58F-05MSS1QKVCMZ",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1180.3412902706605,
			"y": 709.4571097275276,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 5.811426472101328,
			"height": 12.494575782550996,
			"seed": 1524534236,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862517,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-1.162311897019413,
					-0.5811559485097562
				],
				[
					-1.452856618025307,
					-0.8717228383482897
				],
				[
					-1.452856618025307,
					-1.1622897281868232
				],
				[
					-1.74344567669648,
					-1.1622897281868232
				],
				[
					-1.74344567669648,
					-1.4528566180253568
				],
				[
					-1.74344567669648,
					-1.7434235078638904
				],
				[
					-1.74344567669648,
					-1.4528566180253568
				],
				[
					-1.452856618025307,
					0
				],
				[
					-0.87172283834824,
					1.7434235078638904
				],
				[
					0,
					2.6151463462121307
				],
				[
					0.8717228383483392,
					3.1962801258891975
				],
				[
					1.452856618025406,
					3.1962801258891975
				],
				[
					2.3245794563736464,
					1.7434235078638904
				],
				[
					2.0339903977024734,
					0.29056688983853357
				],
				[
					1.452856618025406,
					-1.7434235078638904
				],
				[
					0.8717228383483392,
					-4.358569854076021
				],
				[
					0.8717228383483392,
					-6.973716200288152
				],
				[
					1.452856618025406,
					-9.007706597990575
				],
				[
					2.3245794563736464,
					-9.298295656661798
				],
				[
					3.1962579570566074,
					-9.298295656661798
				],
				[
					4.067980795404847,
					-8.717139708152041
				],
				[
					4.067980795404847,
					-6.392582420611085
				],
				[
					4.067980795404847,
					-6.392582420611085
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2490234375,
				0.3369140625,
				0.3759765625,
				0.431640625,
				0.4443359375,
				0.453125,
				0.453125,
				0.46484375,
				0.4765625,
				0.4814453125,
				0.4814453125,
				0.4814453125,
				0.4931640625,
				0.5048828125,
				0.5185546875,
				0.515625,
				0.5234375,
				0.529296875,
				0.5390625,
				0.5390625,
				0.5390625,
				0.5205078125,
				0.015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 613,
			"versionNonce": 1597852082,
			"isDeleted": false,
			"id": "3mz686EklQxpGGx-Edacm",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1197.3586805847947,
			"y": 683.2882729342472,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 11.622852944202755,
			"height": 29.92885519885508,
			"seed": 1466268132,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862517,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.5811781173424452,
					0
				],
				[
					-2.3245794563736464,
					1.1622897281867985
				],
				[
					-4.358569854076021,
					4.649136743914554
				],
				[
					-6.9737383691208406,
					10.460563216015933
				],
				[
					-10.751174443519794,
					19.468291982839148
				],
				[
					-11.622852944202755,
					24.1174287267537
				],
				[
					-11.041719164525688,
					26.732575072965883
				],
				[
					-8.136005928474974,
					29.057132360506788
				],
				[
					-6.102015530772601,
					29.92885519885508
				],
				[
					-4.939747971418466,
					29.92885519885508
				],
				[
					-2.9057132360507136,
					29.057132360506788
				],
				[
					-2.9057132360507136,
					29.057132360506788
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.21875,
				0.2685546875,
				0.3076171875,
				0.34375,
				0.3857421875,
				0.4462890625,
				0.470703125,
				0.478515625,
				0.474609375,
				0.4423828125,
				0.3251953125,
				0.0146484375,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 610,
			"versionNonce": 895148654,
			"isDeleted": false,
			"id": "I0I-vDVFPvG8YF20GJnq5",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1237.5838321533258,
			"y": 705.3891067632902,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 3.486847015727781,
			"height": 17.14371252646555,
			"seed": 1536180836,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862517,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.290589058671173,
					-2.6151463462121307
				],
				[
					-0.290589058671173,
					-5.520859582262844
				],
				[
					-0.290589058671173,
					-8.136005928474974
				],
				[
					-0.5811337796770671,
					-11.041719164525638
				],
				[
					-0.5811337796770671,
					-12.78514267238953
				],
				[
					-0.8717228383482402,
					-15.690855908440193
				],
				[
					-0.290589058671173,
					-17.14371252646555
				],
				[
					0.29058905867127216,
					-17.14371252646555
				],
				[
					2.6151241773795406,
					-14.819133070091953
				],
				[
					2.6151241773795406,
					-14.819133070091953
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.171875,
				0.326171875,
				0.4404296875,
				0.5,
				0.513671875,
				0.515625,
				0.50390625,
				0.4365234375,
				0.294921875,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 616,
			"versionNonce": 202195826,
			"isDeleted": false,
			"id": "8t-wpftq0rCEmgm7xsuBD",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1240.1989563307054,
			"y": 694.6379766574356,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 17.434279416304083,
			"height": 14.237999290414885,
			"seed": 763111268,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862517,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-3.7773917367336747,
					0.5811337796770671
				],
				[
					-5.520837413430155,
					0.8717006695156007
				],
				[
					-8.717139708152041,
					1.4528566180253568
				],
				[
					-13.947388062911024,
					2.033990397702424
				],
				[
					-16.271967519284672,
					2.033990397702424
				],
				[
					-17.14369035763291,
					2.033990397702424
				],
				[
					-17.434279416304083,
					1.4528566180253568
				],
				[
					-16.271967519284672,
					-1.4528566180253073
				],
				[
					-15.109699959930536,
					-4.358569854076021
				],
				[
					-13.947388062911024,
					-7.264283090126685
				],
				[
					-12.78512050355689,
					-9.87942943633884
				],
				[
					-12.203986723879822,
					-11.622852944202705
				],
				[
					-12.203986723879822,
					-12.204008892712462
				],
				[
					-12.203986723879822,
					-11.913442002873929
				],
				[
					-11.913397665208649,
					-10.751152274687104
				],
				[
					-11.913397665208649,
					-10.751152274687104
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2109375,
				0.251953125,
				0.294921875,
				0.390625,
				0.4921875,
				0.5029296875,
				0.51171875,
				0.52734375,
				0.5390625,
				0.5498046875,
				0.560546875,
				0.5634765625,
				0.55859375,
				0.5185546875,
				0.208984375,
				0.0126953125,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 592,
			"versionNonce": 2029020334,
			"isDeleted": false,
			"id": "oUPeoXqQrfnBswnN9blw-",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1237.874421211997,
			"y": 676.3319744027834,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 20.3399926523547,
			"height": 37.48370517882032,
			"seed": 940930788,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862517,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					-0.29056688983853357
				],
				[
					1.1622675593541343,
					-0.29056688983853357
				],
				[
					5.811426472101328,
					1.7434235078638656
				],
				[
					9.298273487829109,
					4.649136743914554
				],
				[
					13.65684334190513,
					8.717139708152041
				],
				[
					17.724824137309877,
					13.075709562228088
				],
				[
					20.3399926523547,
					19.758858872677706
				],
				[
					20.049403593683525,
					23.53627277824397
				],
				[
					18.88713603432939,
					27.313708852642925
				],
				[
					15.400244680936332,
					31.091122758209238
				],
				[
					11.332263885531484,
					33.415702214582836
				],
				[
					8.717139708152041,
					34.868558832608194
				],
				[
					6.392560251778395,
					36.030848560794965
				],
				[
					3.7773917367335756,
					36.90254923031057
				],
				[
					0.290544721005795,
					37.19313828898179
				],
				[
					0.290544721005795,
					37.19313828898179
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.212890625,
				0.2353515625,
				0.349609375,
				0.3564453125,
				0.3564453125,
				0.353515625,
				0.35546875,
				0.3720703125,
				0.40234375,
				0.4501953125,
				0.5009765625,
				0.517578125,
				0.51953125,
				0.47265625,
				0.25390625,
				0.0126953125,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 617,
			"versionNonce": 406324530,
			"isDeleted": false,
			"id": "BWIcQh5Jn7P3ty5m6s3lf",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1210.2701454695155,
			"y": 740.2576434270654,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 14.52856618025337,
			"height": 15.690855908440243,
			"seed": 1474317660,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862517,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-2.0340347353677526,
					0
				],
				[
					-4.068025133070127,
					0.5811559485097562
				],
				[
					-5.5208817510955335,
					1.4528566180253568
				],
				[
					-6.9737383691208406,
					2.9057132360507136
				],
				[
					-7.84546120746908,
					4.649158912747244
				],
				[
					-6.683149310449667,
					7.264283090126734
				],
				[
					-4.939747971418466,
					8.717139708152041
				],
				[
					-2.9057132360507136,
					11.913442002873929
				],
				[
					-4.358569854076021,
					13.075709562228063
				],
				[
					-6.683149310449667,
					14.237999290414885
				],
				[
					-12.204031061545102,
					15.690855908440243
				],
				[
					-12.78516484122217,
					15.690855908440243
				],
				[
					-14.238021459247575,
					15.690855908440243
				],
				[
					-14.52856618025337,
					15.690855908440243
				],
				[
					-13.947432400576304,
					15.690855908440243
				],
				[
					-9.879451605171553,
					14.528566180253419
				],
				[
					-9.879451605171553,
					14.528566180253419
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.21875,
				0.2666015625,
				0.35546875,
				0.42578125,
				0.482421875,
				0.498046875,
				0.4931640625,
				0.484375,
				0.482421875,
				0.4931640625,
				0.4990234375,
				0.51171875,
				0.51171875,
				0.515625,
				0.5185546875,
				0.3095703125,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 615,
			"versionNonce": 723230446,
			"isDeleted": false,
			"id": "9_hDNU-R2r0_B2CMnedzL",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1213.1758587055663,
			"y": 747.521926517192,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 4.649114575081816,
			"height": 7.554872148797908,
			"seed": 1821980132,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862517,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.290544721005795,
					1.7434456766965298
				],
				[
					0.290544721005795,
					3.4868691845604203
				],
				[
					0.5811337796770671,
					4.358569854076021
				],
				[
					1.1622675593541343,
					5.811426472101328
				],
				[
					1.7434013390312013,
					7.264283090126685
				],
				[
					2.0339903977023743,
					7.554872148797908
				],
				[
					2.9057132360506146,
					6.973716200288152
				],
				[
					3.196257957056509,
					5.230292692424261
				],
				[
					3.196257957056509,
					2.6151463462121307
				],
				[
					3.196257957056509,
					0.8717228383482402
				],
				[
					3.196257957056509,
					0.5811559485097066
				],
				[
					3.486847015727682,
					0.5811559485097066
				],
				[
					3.7773917367335756,
					2.324579456373597
				],
				[
					4.649114575081816,
					5.230292692424261
				],
				[
					4.649114575081816,
					5.230292692424261
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.29296875,
				0.326171875,
				0.3369140625,
				0.3564453125,
				0.388671875,
				0.3974609375,
				0.3974609375,
				0.4248046875,
				0.474609375,
				0.5078125,
				0.5107421875,
				0.5107421875,
				0.4716796875,
				0.3125,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 618,
			"versionNonce": 1562676978,
			"isDeleted": false,
			"id": "-2snDgmnljHVIxHU9tOrt",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1220.7306865166986,
			"y": 753.3333529892934,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 10.16999632617735,
			"height": 8.136005928474974,
			"seed": 175337052,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862517,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.8717228383482402,
					-2.905713236050664
				],
				[
					1.7434456766965793,
					-4.358569854076021
				],
				[
					2.6151685150448194,
					-5.230270523591621
				],
				[
					3.1963022947218866,
					-5.520837413430154
				],
				[
					3.486847015727781,
					-5.811426472101328
				],
				[
					4.939703633753088,
					-6.101993361939861
				],
				[
					6.392560251778395,
					-6.973694031455461
				],
				[
					8.136005928474974,
					-7.845416869803751
				],
				[
					9.007728766823215,
					-7.264283090126684
				],
				[
					9.298273487829109,
					-5.520837413430154
				],
				[
					9.298273487829109,
					-4.0679807954047975
				],
				[
					9.588862546500282,
					-3.196280125889197
				],
				[
					9.879451605171553,
					-2.615124177379441
				],
				[
					9.879451605171553,
					-2.3245572875409075
				],
				[
					10.16999632617735,
					-2.0339903977023743
				],
				[
					10.16999632617735,
					-0.8717006695156005
				],
				[
					9.879451605171553,
					0.29058905867122253
				],
				[
					9.879451605171553,
					0.29058905867122253
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.181640625,
				0.2470703125,
				0.3271484375,
				0.396484375,
				0.4697265625,
				0.4794921875,
				0.4833984375,
				0.486328125,
				0.4951171875,
				0.5078125,
				0.5126953125,
				0.5234375,
				0.5390625,
				0.537109375,
				0.5302734375,
				0.486328125,
				0.3623046875,
				0.0146484375,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 608,
			"versionNonce": 1617269038,
			"isDeleted": false,
			"id": "Ep-Th7lpiIVtKycVHXpkJ",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1239.3272778300222,
			"y": 750.7182288119141,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 11.622852944202656,
			"height": 3.4868691845604203,
			"seed": 913730396,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862517,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1.743401339031201,
					0
				],
				[
					3.4868470157276814,
					-0.2905890586712226
				],
				[
					7.264283090126635,
					-1.1622897281868232
				],
				[
					8.717139708152041,
					-1.4528566180253568
				],
				[
					10.751130105854415,
					-1.7434456766965793
				],
				[
					11.622852944202656,
					-2.3245794563736464
				],
				[
					10.169996326177348,
					-3.4868691845604203
				],
				[
					10.169996326177348,
					-3.4868691845604203
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2724609375,
				0.349609375,
				0.4111328125,
				0.4658203125,
				0.4677734375,
				0.4296875,
				0.2373046875,
				0.0126953125,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 608,
			"versionNonce": 1868161202,
			"isDeleted": false,
			"id": "g2q8KUd1Qv6wHffwLRilI",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1241.0706791690534,
			"y": 742.2916559936004,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 12.494575782550996,
			"height": 0.8717228383482897,
			"seed": 129749468,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862517,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.290589058671173,
					0
				],
				[
					1.4528566180253073,
					-0.29056688983853357
				],
				[
					3.1963022947218866,
					-0.5811559485097562
				],
				[
					5.520881751095434,
					-0.8717228383482897
				],
				[
					8.136005928474974,
					-0.8717228383482897
				],
				[
					10.16999632617735,
					-0.8717228383482897
				],
				[
					12.494575782550996,
					-0.8717228383482897
				],
				[
					12.494575782550996,
					-0.8717228383482897
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.310546875,
				0.34375,
				0.3779296875,
				0.416015625,
				0.453125,
				0.4599609375,
				0.462890625,
				0.015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 619,
			"versionNonce": 876034926,
			"isDeleted": false,
			"id": "K8w7siWcBXXqSn5WG2ULw",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1266.6409645138326,
			"y": 734.446216954964,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 9.588862546500382,
			"height": 17.434279416304083,
			"seed": 1137651556,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862517,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.29058905867127216,
					-0.8717006695156007
				],
				[
					-0.29058905867127216,
					-0.29056688983853357
				],
				[
					-0.29058905867127216,
					2.0340125665350635
				],
				[
					-0.29058905867127216,
					4.358569854076021
				],
				[
					-0.5811337796770671,
					7.264283090126685
				],
				[
					-0.5811337796770671,
					11.622852944202705
				],
				[
					-0.8717228383483393,
					14.237999290414837
				],
				[
					-0.5811337796770671,
					15.690855908440193
				],
				[
					-0.8717228383483393,
					16.27201185694995
				],
				[
					-0.8717228383483393,
					16.562578746788482
				],
				[
					-0.5811337796770671,
					16.562578746788482
				],
				[
					0.8717228383482402,
					16.562578746788482
				],
				[
					1.4528566180253073,
					16.27201185694995
				],
				[
					4.067980795404749,
					15.690855908440193
				],
				[
					5.520837413430155,
					15.40028901860166
				],
				[
					6.392560251778395,
					15.690855908440193
				],
				[
					6.973694031455462,
					15.690855908440193
				],
				[
					8.717139708152041,
					15.690855908440193
				],
				[
					8.717139708152041,
					15.690855908440193
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.189453125,
				0.2373046875,
				0.33984375,
				0.36328125,
				0.37109375,
				0.373046875,
				0.3935546875,
				0.3984375,
				0.3984375,
				0.41015625,
				0.43359375,
				0.48046875,
				0.48046875,
				0.48046875,
				0.484375,
				0.484375,
				0.455078125,
				0.384765625,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 616,
			"versionNonce": 981400178,
			"isDeleted": false,
			"id": "1gFMqsxyVN45Y7fPhF5h7",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1281.1695306940858,
			"y": 729.506513321211,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 9.298273487829109,
			"height": 17.434279416304083,
			"seed": 2028783068,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862517,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					0.8717228383482402
				],
				[
					0,
					2.0339903977023743
				],
				[
					-0.290589058671173,
					6.683149310449618
				],
				[
					-0.5811337796770671,
					10.16999632617735
				],
				[
					-0.8717228383482402,
					12.78514267238953
				],
				[
					-1.1622675593541343,
					15.981422798278727
				],
				[
					-1.4528566180253073,
					16.853145636627016
				],
				[
					-1.1622675593541343,
					17.434279416304083
				],
				[
					-0.8717228383482402,
					17.434279416304083
				],
				[
					0.8717228383482402,
					17.14371252646555
				],
				[
					2.3245794563736464,
					16.562556577955792
				],
				[
					4.067980795404848,
					15.981422798278727
				],
				[
					5.811426472101328,
					15.690855908440193
				],
				[
					6.973694031455462,
					15.690855908440193
				],
				[
					7.845416869803802,
					15.981422798278727
				],
				[
					7.845416869803802,
					15.981422798278727
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.3203125,
				0.3662109375,
				0.3701171875,
				0.400390625,
				0.4306640625,
				0.44140625,
				0.4560546875,
				0.4677734375,
				0.4814453125,
				0.494140625,
				0.5068359375,
				0.509765625,
				0.509765625,
				0.51171875,
				0.47265625,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 645,
			"versionNonce": 1826201006,
			"isDeleted": false,
			"id": "Z-XmvVEWnoUrahwNpWcBE",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1293.9546511976428,
			"y": 735.6085066831508,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 12.203986723879723,
			"height": 21.502282380541573,
			"seed": 800755292,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862517,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1.7434456766964803,
					-1.4528566180253075
				],
				[
					3.1963022947218866,
					-3.196280125889198
				],
				[
					4.358569854076021,
					-4.939703633753089
				],
				[
					4.939747971418367,
					-6.392560251778396
				],
				[
					5.520881751095434,
					-7.264283090126686
				],
				[
					5.520881751095434,
					-7.845416869803753
				],
				[
					5.520881751095434,
					-6.101993361939862
				],
				[
					5.520881751095434,
					-3.777413905566265
				],
				[
					5.230292692424261,
					1.7434235078638907
				],
				[
					4.358569854076021,
					4.649136743914555
				],
				[
					3.777436074398954,
					6.973716200288202
				],
				[
					3.1963022947218866,
					8.717139708152043
				],
				[
					2.9057132360506146,
					10.1699963261774
				],
				[
					2.3245794563735473,
					11.622852944202757
				],
				[
					2.3245794563735473,
					11.91341983404129
				],
				[
					2.0340347353677526,
					11.91341983404129
				],
				[
					2.0340347353677526,
					12.204008892712464
				],
				[
					1.4528566180253073,
					12.204008892712464
				],
				[
					0.8717228383482402,
					12.494575782550998
				],
				[
					0.581178117342346,
					12.785142672389531
				],
				[
					0.290589058671173,
					12.785142672389531
				],
				[
					0.581178117342346,
					12.494575782550998
				],
				[
					0.8717228383482402,
					12.204008892712464
				],
				[
					1.4528566180253073,
					11.91341983404129
				],
				[
					3.777436074398954,
					11.332286054364223
				],
				[
					6.392604589443773,
					10.751152274687156
				],
				[
					8.426594987146148,
					10.1699963261774
				],
				[
					9.588862546500282,
					9.879429436338867
				],
				[
					10.16999632617735,
					9.879429436338867
				],
				[
					10.460585384848523,
					9.879429436338867
				],
				[
					9.879451605171456,
					10.1699963261774
				],
				[
					8.426594987146148,
					10.751152274687156
				],
				[
					6.102015530772501,
					11.622852944202757
				],
				[
					3.777436074398954,
					12.494575782550998
				],
				[
					2.0340347353677526,
					12.785142672389531
				],
				[
					0.581178117342346,
					13.366276452066598
				],
				[
					-0.29054472100589407,
					13.366276452066598
				],
				[
					-1.4528566180254063,
					13.65686551073782
				],
				[
					-1.7434013390312013,
					13.65686551073782
				],
				[
					-1.4528566180254063,
					13.65686551073782
				],
				[
					-1.1622675593541343,
					13.366276452066598
				],
				[
					-0.5811337796770671,
					13.075709562228065
				],
				[
					0.290589058671173,
					12.785142672389531
				],
				[
					1.7434456766964803,
					12.204008892712464
				],
				[
					1.7434456766964803,
					12.204008892712464
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.142578125,
				0.2158203125,
				0.25390625,
				0.279296875,
				0.322265625,
				0.353515625,
				0.380859375,
				0.4443359375,
				0.4443359375,
				0.4482421875,
				0.46484375,
				0.4853515625,
				0.4951171875,
				0.5068359375,
				0.51953125,
				0.517578125,
				0.5234375,
				0.52734375,
				0.52734375,
				0.5244140625,
				0.5244140625,
				0.5244140625,
				0.5166015625,
				0.5146484375,
				0.5126953125,
				0.5107421875,
				0.5107421875,
				0.5126953125,
				0.5126953125,
				0.5126953125,
				0.5126953125,
				0.5224609375,
				0.5244140625,
				0.5244140625,
				0.5244140625,
				0.5244140625,
				0.5244140625,
				0.5244140625,
				0.5244140625,
				0.5263671875,
				0.5166015625,
				0.4990234375,
				0.4287109375,
				0.2724609375,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 608,
			"versionNonce": 492493874,
			"isDeleted": false,
			"id": "uy2x6tYQRepjKYYPxmgbw",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1310.5172521132638,
			"y": 736.1896626316604,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 11.622852944202755,
			"height": 3.1963022947218866,
			"seed": 2003535332,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862517,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1.4528566180253073,
					0
				],
				[
					3.7773917367335756,
					0
				],
				[
					7.264283090126734,
					-0.5811559485097562
				],
				[
					9.588818208835002,
					-1.1622897281868232
				],
				[
					10.460541047183243,
					-1.1622897281868232
				],
				[
					11.622852944202755,
					-1.7434456766965298
				],
				[
					11.332263885531484,
					-3.1963022947218866
				],
				[
					11.332263885531484,
					-3.1963022947218866
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2255859375,
				0.3603515625,
				0.3916015625,
				0.412109375,
				0.4267578125,
				0.4267578125,
				0.3955078125,
				0.015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 613,
			"versionNonce": 527808494,
			"isDeleted": false,
			"id": "ed4SmjxlF17bq3UvaJ5X-",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1318.3626689830678,
			"y": 730.3782361595594,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 2.3245794563735473,
			"height": 13.366276452066597,
			"seed": 1283938148,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862517,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.290544721005795,
					0.5811337796770671
				],
				[
					0.8717228383482402,
					1.4528566180253568
				],
				[
					1.7434013390312013,
					3.1962801258892473
				],
				[
					2.0339903977023743,
					5.8114264721013775
				],
				[
					1.7434013390312013,
					7.845416869803802
				],
				[
					1.4528566180253073,
					9.879407267506176
				],
				[
					1.1622675593541343,
					11.913419834041289
				],
				[
					1.1622675593541343,
					12.494553613718356
				],
				[
					1.4528566180253073,
					12.78512050355689
				],
				[
					1.4528566180253073,
					13.075709562228063
				],
				[
					1.7434013390312013,
					13.366276452066597
				],
				[
					2.3245794563735473,
					12.78512050355689
				],
				[
					2.3245794563735473,
					12.78512050355689
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2880859375,
				0.3740234375,
				0.4453125,
				0.48828125,
				0.4970703125,
				0.513671875,
				0.5146484375,
				0.5126953125,
				0.5126953125,
				0.5029296875,
				0.4111328125,
				0.37890625,
				0.0126953125,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 618,
			"versionNonce": 97814002,
			"isDeleted": false,
			"id": "-Hi8YWWJm5godkX7Xu6HN",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1332.891235163321,
			"y": 718.7553832153566,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 11.041719164525688,
			"height": 23.24570588840546,
			"seed": 117313628,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862518,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.290589058671173,
					2.033990397702424
				],
				[
					-1.1623118970195123,
					6.101993361939911
				],
				[
					-1.7434456766965793,
					13.075709562228063
				],
				[
					-2.3245794563736464,
					17.434279416304083
				],
				[
					-2.6151685150448194,
					20.049403593683575
				],
				[
					-2.9057132360507136,
					21.502260211708883
				],
				[
					-2.9057132360507136,
					22.664549939895707
				],
				[
					-2.9057132360507136,
					22.955116829734237
				],
				[
					-3.1963022947218866,
					23.24570588840546
				],
				[
					-2.9057132360507136,
					23.24570588840546
				],
				[
					-0.290589058671173,
					23.24570588840546
				],
				[
					2.0339903977023743,
					22.955116829734237
				],
				[
					4.649114575081915,
					22.664549939895707
				],
				[
					5.520837413430155,
					22.664549939895707
				],
				[
					7.264283090126734,
					22.664549939895707
				],
				[
					7.5548278111325295,
					22.664549939895707
				],
				[
					7.845416869803802,
					22.664549939895707
				],
				[
					7.845416869803802,
					22.664549939895707
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.328125,
				0.3876953125,
				0.4169921875,
				0.47265625,
				0.486328125,
				0.4931640625,
				0.4990234375,
				0.5205078125,
				0.5234375,
				0.529296875,
				0.537109375,
				0.5478515625,
				0.5537109375,
				0.5537109375,
				0.5537109375,
				0.5048828125,
				0.48828125,
				0.0126953125,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 621,
			"versionNonce": 1410632238,
			"isDeleted": false,
			"id": "7UdFAsEY3OuKwgVPsD2sr",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1349.1632026826057,
			"y": 717.8836603770084,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 9.298317825494488,
			"height": 22.373983050057173,
			"seed": 8293724,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862518,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.29054472100579504,
					0.29056688983853357
				],
				[
					-0.8716785006828622,
					4.649136743914555
				],
				[
					-1.7434013390312015,
					9.29827348782911
				],
				[
					-2.905713236050615,
					13.656843341905132
				],
				[
					-3.777391736733576,
					17.434279416304086
				],
				[
					-4.358569854076022,
					20.049425762516265
				],
				[
					-4.358569854076022,
					21.502282380541573
				],
				[
					-4.358569854076022,
					22.373983050057173
				],
				[
					-4.0679807954047495,
					22.373983050057173
				],
				[
					-3.4868470157276823,
					22.373983050057173
				],
				[
					-3.196257957056509,
					22.08341616021864
				],
				[
					-2.0339903977023748,
					21.792849270380106
				],
				[
					-0.5811337796770671,
					21.21171549070304
				],
				[
					1.1623118970195125,
					20.921126432031866
				],
				[
					2.905713236050714,
					20.630559542193332
				],
				[
					3.196302294721887,
					20.630559542193332
				],
				[
					3.7774360743989543,
					20.630559542193332
				],
				[
					4.358569854076022,
					20.630559542193332
				],
				[
					4.649158912747294,
					20.3399926523548
				],
				[
					4.939747971418467,
					20.049425762516265
				],
				[
					4.939747971418467,
					20.049425762516265
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2626953125,
				0.412109375,
				0.4482421875,
				0.4736328125,
				0.4892578125,
				0.494140625,
				0.5078125,
				0.5185546875,
				0.525390625,
				0.5400390625,
				0.5419921875,
				0.544921875,
				0.5498046875,
				0.5537109375,
				0.5556640625,
				0.5517578125,
				0.54296875,
				0.51953125,
				0.4404296875,
				0.3076171875,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 621,
			"versionNonce": 217249714,
			"isDeleted": false,
			"id": "H3PMoZEnqTz4b0evF7cHr",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1371.5372300703277,
			"y": 734.1556500651254,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 12.78516484122217,
			"height": 18.015413195981175,
			"seed": 1051053284,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862518,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.5811781173424452,
					0
				],
				[
					-3.1963022947218866,
					0
				],
				[
					-5.230292692424261,
					0.29056688983853357
				],
				[
					-7.554872148797908,
					0
				],
				[
					-9.007728766823215,
					-0.29056688983853357
				],
				[
					-8.426594987146148,
					-1.1622897281868232
				],
				[
					-6.392604589443773,
					-2.3245572875409577
				],
				[
					-4.358569854076021,
					-3.486847015727781
				],
				[
					-2.6151685150448194,
					-4.649136743914554
				],
				[
					-1.4528566180253073,
					-5.8114264721013775
				],
				[
					-1.1623118970195123,
					-7.845416869803802
				],
				[
					-1.7434456766965793,
					-9.007706597990575
				],
				[
					-2.6151685150448194,
					-10.460563216015933
				],
				[
					-3.777436074398954,
					-11.622852944202755
				],
				[
					-6.102015530772601,
					-13.65684334190513
				],
				[
					-8.136005928474974,
					-14.819133070091953
				],
				[
					-10.46058538484862,
					-15.690855908440243
				],
				[
					-11.622852944202755,
					-16.562556577955842
				],
				[
					-11.913442002873929,
					-16.562556577955842
				],
				[
					-12.78516484122217,
					-17.72484630614264
				],
				[
					-12.78516484122217,
					-17.72484630614264
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.17578125,
				0.30078125,
				0.4228515625,
				0.478515625,
				0.5166015625,
				0.5361328125,
				0.5380859375,
				0.5283203125,
				0.5224609375,
				0.5029296875,
				0.4951171875,
				0.5,
				0.513671875,
				0.533203125,
				0.5576171875,
				0.5771484375,
				0.5849609375,
				0.5849609375,
				0.5849609375,
				0.58203125,
				0.0166015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 611,
			"versionNonce": 698291310,
			"isDeleted": false,
			"id": "PY7tC2rWqtTKuVGl5NN0S",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1199.8095600846673,
			"y": 788.201889653069,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 2.6151685150448194,
			"height": 13.075709562228063,
			"seed": 879804508,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862518,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					-0.5811337796770671
				],
				[
					0.2905890586712721,
					-0.29056688983853357
				],
				[
					0.8717228383483392,
					0.8717228383482897
				],
				[
					1.452856618025406,
					4.068002964237487
				],
				[
					1.7434456766965791,
					7.554872148797908
				],
				[
					2.3245794563736464,
					10.460585384848573
				],
				[
					2.3245794563736464,
					11.332286054364172
				],
				[
					2.6151685150448194,
					11.913442002873929
				],
				[
					2.6151685150448194,
					12.494575782550996
				],
				[
					2.3245794563736464,
					12.204008892712462
				],
				[
					2.3245794563736464,
					12.204008892712462
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2490234375,
				0.2900390625,
				0.37890625,
				0.3974609375,
				0.41796875,
				0.4365234375,
				0.443359375,
				0.4521484375,
				0.4541015625,
				0.3837890625,
				0.015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 610,
			"versionNonce": 316486002,
			"isDeleted": false,
			"id": "gILL8ko5uvOKRw7EV1aIh",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1196.6133021276107,
			"y": 778.6130492754014,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 2.3245794563736464,
			"height": 3.4868691845604203,
			"seed": 1919297636,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862518,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.290589058671173,
					-0.5811559485097562
				],
				[
					-0.5811781173424451,
					-0.8717228383482897
				],
				[
					0,
					-0.29056688983853357
				],
				[
					0.29054472100589407,
					0.5811337796770671
				],
				[
					0.581133779677067,
					1.4528566180253568
				],
				[
					0.581133779677067,
					2.3245572875409577
				],
				[
					0.8716785006829612,
					2.6151463462121307
				],
				[
					1.743401339031201,
					2.6151463462121307
				],
				[
					0,
					0
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2158203125,
				0.279296875,
				0.3662109375,
				0.49609375,
				0.494140625,
				0.494140625,
				0.494140625,
				0.47265625,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 621,
			"versionNonce": 2044614318,
			"isDeleted": false,
			"id": "LarNa5vOYvAp80gdrjjGK",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1203.296407100395,
			"y": 783.843319798993,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 12.78516484122217,
			"height": 30.219422088693612,
			"seed": 1613598052,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862518,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.290589058671173,
					1.4528566180253568
				],
				[
					0.8717228383482402,
					4.358569854076021
				],
				[
					1.4528566180253073,
					5.8114264721013775
				],
				[
					2.9057132360507136,
					9.879429436338866
				],
				[
					4.939747971418466,
					14.819155238924592
				],
				[
					6.102015530772601,
					15.981422798278727
				],
				[
					6.392604589443773,
					16.27201185694995
				],
				[
					6.102015530772601,
					14.819155238924592
				],
				[
					4.939747971418466,
					11.913442002873929
				],
				[
					3.4868913533930597,
					4.358569854076021
				],
				[
					2.9057132360507136,
					-1.7434235078638904
				],
				[
					2.6151685150448194,
					-7.264283090126685
				],
				[
					3.1963022947218866,
					-10.460563216015933
				],
				[
					6.392604589443773,
					-13.366276452066597
				],
				[
					9.298317825494488,
					-13.947410231743664
				],
				[
					11.332308223196861,
					-13.65684334190513
				],
				[
					12.494575782550996,
					-12.203986723879773
				],
				[
					12.78516484122217,
					-10.460563216015933
				],
				[
					11.622852944202755,
					-7.845416869803752
				],
				[
					8.717139708152041,
					-5.230270523591622
				],
				[
					8.717139708152041,
					-5.230270523591622
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2705078125,
				0.3203125,
				0.345703125,
				0.359375,
				0.384765625,
				0.396484375,
				0.40234375,
				0.4052734375,
				0.490234375,
				0.53125,
				0.568359375,
				0.5791015625,
				0.5771484375,
				0.5712890625,
				0.56640625,
				0.56640625,
				0.5576171875,
				0.541015625,
				0.47265625,
				0.2529296875,
				0.0126953125,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 609,
			"versionNonce": 1524249394,
			"isDeleted": false,
			"id": "cNqh-lkOLAqRd6CfD1Uy9",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1204.7492637184203,
			"y": 784.4244757475026,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 11.913442002873929,
			"height": 1.1622897281867737,
			"seed": 1772317788,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862518,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					0.29056688983853357
				],
				[
					0.29058905867127216,
					0.5811337796770671
				],
				[
					2.0340347353677526,
					0.5811337796770671
				],
				[
					4.939747971418466,
					0.29056688983853357
				],
				[
					7.84546120746918,
					0
				],
				[
					9.879451605171553,
					0
				],
				[
					11.041719164525688,
					0.5811337796770671
				],
				[
					11.913442002873929,
					1.1622897281867737
				],
				[
					11.913442002873929,
					1.1622897281867737
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.345703125,
				0.3828125,
				0.4033203125,
				0.458984375,
				0.4951171875,
				0.5078125,
				0.4931640625,
				0.3291015625,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 618,
			"versionNonce": 2105233646,
			"isDeleted": false,
			"id": "6wqH3Vh4t-mASVIv7K6uk",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1251.2406754952312,
			"y": 780.3564727832652,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 20.63058171102597,
			"height": 18.88713603432939,
			"seed": 978188516,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862518,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-6.392560251778395,
					2.324579456373597
				],
				[
					-9.588818208835002,
					5.230292692424261
				],
				[
					-10.751130105854417,
					8.426572818313508
				],
				[
					-9.298273487829109,
					10.16999632617735
				],
				[
					-6.392560251778395,
					11.622852944202705
				],
				[
					-1.4528566180253073,
					13.65684334190513
				],
				[
					1.4528566180253073,
					15.109699959930436
				],
				[
					1.7434456766965793,
					15.690855908440193
				],
				[
					0.5811781173424452,
					16.853145636627016
				],
				[
					-2.9057132360507136,
					17.434279416304083
				],
				[
					-7.5548278111325295,
					17.434279416304083
				],
				[
					-13.075709562228063,
					17.724846306142616
				],
				[
					-16.85310129896164,
					18.01541319598115
				],
				[
					-18.01541319598115,
					18.01541319598115
				],
				[
					-18.88713603432939,
					18.306002254652324
				],
				[
					-17.14369035763291,
					18.88713603432939
				],
				[
					-11.913397665208551,
					18.596569144490857
				],
				[
					-11.913397665208551,
					18.596569144490857
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2548828125,
				0.3642578125,
				0.4755859375,
				0.49609375,
				0.4921875,
				0.486328125,
				0.4755859375,
				0.4677734375,
				0.462890625,
				0.4658203125,
				0.4990234375,
				0.53125,
				0.5546875,
				0.5546875,
				0.5546875,
				0.525390625,
				0.353515625,
				0.0146484375,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 616,
			"versionNonce": 659619058,
			"isDeleted": false,
			"id": "eD41_7Z7gkElzHDzCZnLP",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1260.5389933207257,
			"y": 786.458466145205,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 12.203986723879822,
			"height": 12.204008892712462,
			"seed": 1217326052,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862518,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-1.4528566180254063,
					3.4868691845604203
				],
				[
					-1.4528566180254063,
					4.939725802585777
				],
				[
					-1.1623118970195123,
					8.136005928474974
				],
				[
					0,
					10.460563216015933
				],
				[
					1.7434013390312013,
					11.913419834041289
				],
				[
					4.067980795404749,
					12.204008892712462
				],
				[
					5.811426472101328,
					11.332286054364221
				],
				[
					6.973694031455462,
					9.298295656661798
				],
				[
					7.5548278111325295,
					6.683149310449667
				],
				[
					8.42655064948077,
					2.9057132360507136
				],
				[
					9.007684429157838,
					1.4528566180253568
				],
				[
					9.298273487829109,
					0.5811559485097562
				],
				[
					9.588818208834905,
					1.1622897281868232
				],
				[
					9.879407267506176,
					2.9057132360507136
				],
				[
					10.751130105854417,
					6.101993361939911
				],
				[
					10.751130105854417,
					6.101993361939911
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.328125,
				0.36328125,
				0.3740234375,
				0.4228515625,
				0.45703125,
				0.4609375,
				0.4775390625,
				0.4921875,
				0.49609375,
				0.5078125,
				0.5283203125,
				0.5400390625,
				0.5458984375,
				0.5029296875,
				0.3671875,
				0.0146484375,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 617,
			"versionNonce": 1878983470,
			"isDeleted": false,
			"id": "JOXUYCUjyoOkGXZhlZj_o",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1273.614702882954,
			"y": 796.337895581544,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 17.724824137309877,
			"height": 8.717139708152041,
			"seed": 1149184868,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862518,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.581133779677067,
					-2.324579456373597
				],
				[
					2.0339903977023743,
					-4.939703633753088
				],
				[
					3.4868470157276814,
					-6.973716200288152
				],
				[
					4.358569854076021,
					-8.426572818313508
				],
				[
					5.230248354758882,
					-8.717139708152041
				],
				[
					5.520837413430154,
					-8.426572818313508
				],
				[
					6.101971193107222,
					-7.845416869803752
				],
				[
					7.845416869803701,
					-7.264283090126685
				],
				[
					11.332263885531482,
					-8.136005928474974
				],
				[
					13.366254283233856,
					-8.426572818313508
				],
				[
					14.528566180253367,
					-7.845416869803752
				],
				[
					15.109699959930435,
					-6.101993361939911
				],
				[
					15.690833739607502,
					-3.486847015727731
				],
				[
					16.562556577955743,
					-1.7434235078638904
				],
				[
					17.14369035763281,
					-0.8717228383482897
				],
				[
					17.724824137309877,
					-0.29056688983853357
				],
				[
					17.724824137309877,
					-0.29056688983853357
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.333984375,
				0.4453125,
				0.501953125,
				0.5126953125,
				0.5126953125,
				0.5126953125,
				0.5126953125,
				0.5126953125,
				0.5126953125,
				0.5126953125,
				0.51953125,
				0.521484375,
				0.52734375,
				0.5478515625,
				0.552734375,
				0.4541015625,
				0.015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 616,
			"versionNonce": 1439207090,
			"isDeleted": false,
			"id": "b-1MeF27gw2K0H-2Hi5gD",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1299.184988227733,
			"y": 784.7150204685086,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 25.860830065784953,
			"height": 11.913419834041239,
			"seed": 1227396444,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862518,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.5811337796770671,
					0
				],
				[
					2.0339903977023743,
					-0.8717006695156007
				],
				[
					5.811426472101328,
					-2.6151241773794416
				],
				[
					8.717139708152041,
					-4.358569854076021
				],
				[
					12.78512050355689,
					-6.101993361939861
				],
				[
					16.853145636627016,
					-7.845416869803752
				],
				[
					19.75885887267773,
					-9.298273487829109
				],
				[
					22.955116829734237,
					-10.460563216015883
				],
				[
					24.11742872675375,
					-11.04169699569295
				],
				[
					24.989107227436612,
					-11.332263885531484
				],
				[
					25.57028534477906,
					-11.622852944202705
				],
				[
					25.860830065784953,
					-11.913419834041239
				],
				[
					25.279696286107885,
					-11.913419834041239
				],
				[
					23.826839668082478,
					-10.751130105854417
				],
				[
					21.502260211708933,
					-8.717139708152041
				],
				[
					21.502260211708933,
					-8.717139708152041
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2568359375,
				0.3916015625,
				0.43359375,
				0.4677734375,
				0.4697265625,
				0.4697265625,
				0.4697265625,
				0.4697265625,
				0.4697265625,
				0.47265625,
				0.48046875,
				0.48046875,
				0.482421875,
				0.4306640625,
				0.2119140625,
				0.0126953125,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 616,
			"versionNonce": 869428590,
			"isDeleted": false,
			"id": "q2fvrHZyjTmFqb4YwooRO",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1301.8001124051123,
			"y": 782.9715969606445,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 24.11742872675375,
			"height": 9.298273487829109,
			"seed": 1666772444,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862518,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1.4528566180254063,
					-0.29056688983853357
				],
				[
					1.7434456766965793,
					-0.29056688983853357
				],
				[
					3.1963022947218866,
					-0.29056688983853357
				],
				[
					4.358569854076021,
					0
				],
				[
					6.102015530772601,
					0.8717228383482402
				],
				[
					10.169996326177449,
					4.068002964237487
				],
				[
					13.366298620899334,
					5.811426472101328
				],
				[
					16.27201185694995,
					6.973716200288152
				],
				[
					18.596591313323596,
					7.264283090126685
				],
				[
					20.63058171102597,
					7.554849979965218
				],
				[
					22.083438329051376,
					7.845439038636441
				],
				[
					22.955161167399616,
					8.136005928474974
				],
				[
					23.24570588840551,
					8.426572818313508
				],
				[
					23.826839668082577,
					8.717139708152041
				],
				[
					24.11742872675375,
					9.007706597990575
				],
				[
					24.11742872675375,
					9.007706597990575
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2509765625,
				0.3076171875,
				0.318359375,
				0.3701171875,
				0.4111328125,
				0.4482421875,
				0.4833984375,
				0.4990234375,
				0.509765625,
				0.5205078125,
				0.525390625,
				0.525390625,
				0.5166015625,
				0.462890625,
				0.3310546875,
				0.095703125,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 625,
			"versionNonce": 2062018674,
			"isDeleted": false,
			"id": "OWbjXO8KmABVDma-mKXNC",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1356.1369410517266,
			"y": 790.2358800507714,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 14.819155238924543,
			"height": 24.11740655792106,
			"seed": 1387902556,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862518,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					-0.29056688983853357
				],
				[
					0,
					-0.8717006695156007
				],
				[
					0.290589058671173,
					-2.905713236050664
				],
				[
					0.581178117342346,
					-5.520859582262844
				],
				[
					1.1623118970194133,
					-9.879429436338866
				],
				[
					1.4528566180253073,
					-12.78514267238953
				],
				[
					1.7434456766964803,
					-14.819133070091953
				],
				[
					1.7434456766964803,
					-15.690855908440193
				],
				[
					0,
					-13.65684334190513
				],
				[
					-2.6151241773795406,
					-11.913419834041239
				],
				[
					-6.973694031455562,
					-11.332286054364172
				],
				[
					-9.879407267506176,
					-11.913419834041239
				],
				[
					-11.913397665208649,
					-13.65684334190513
				],
				[
					-12.78512050355689,
					-15.981422798278727
				],
				[
					-13.075709562228063,
					-18.305980085819684
				],
				[
					-12.494531444885716,
					-19.75883670384504
				],
				[
					-11.04167482686031,
					-21.21169332187035
				],
				[
					-8.135961590809696,
					-22.955138998566927
				],
				[
					-5.811426472101427,
					-23.536272778243994
				],
				[
					-3.486847015727781,
					-24.11740655792106
				],
				[
					-2.6151241773795406,
					-24.11740655792106
				],
				[
					-1.4528566180254063,
					-23.826839668082528
				],
				[
					-1.1622675593541343,
					-23.536272778243994
				],
				[
					-0.29054472100589407,
					-21.792849270380106
				],
				[
					-0.29054472100589407,
					-21.792849270380106
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.173828125,
				0.25390625,
				0.3076171875,
				0.4296875,
				0.5009765625,
				0.5263671875,
				0.53515625,
				0.537109375,
				0.5322265625,
				0.5126953125,
				0.5078125,
				0.50390625,
				0.5185546875,
				0.5517578125,
				0.576171875,
				0.5830078125,
				0.5927734375,
				0.5947265625,
				0.5947265625,
				0.587890625,
				0.587890625,
				0.587890625,
				0.5400390625,
				0.3681640625,
				0.0146484375,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 609,
			"versionNonce": 1983811502,
			"isDeleted": false,
			"id": "4CZ2nF8O7nGydOLZKzXzz",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1239.9084116096997,
			"y": 830.6253206344752,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 0.8717228383482402,
			"height": 14.237999290414885,
			"seed": 95506404,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862518,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					1.4528566180253568
				],
				[
					-0.29054472100589407,
					4.068002964237487
				],
				[
					-0.5811337796770671,
					6.392560251778445
				],
				[
					-0.29054472100589407,
					9.588840377667642
				],
				[
					0,
					11.041696995693
				],
				[
					0,
					11.913419834041239
				],
				[
					0.290589058671173,
					13.366276452066597
				],
				[
					0,
					14.237999290414885
				],
				[
					0,
					14.237999290414885
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.302734375,
				0.396484375,
				0.4482421875,
				0.482421875,
				0.49609375,
				0.49609375,
				0.49609375,
				0.390625,
				0.0146484375,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 607,
			"versionNonce": 2121665074,
			"isDeleted": false,
			"id": "c-t3FEMXpUXeFexR6RK4B",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1235.2592970346177,
			"y": 823.07047065451,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 0.8717228383482402,
			"height": 4.068002964237487,
			"seed": 536172252,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862518,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.290589058671173,
					-0.8717228383482896
				],
				[
					-0.290589058671173,
					-1.1622897281868232
				],
				[
					-0.290589058671173,
					-0.8717228383482896
				],
				[
					0,
					0.581133779677067
				],
				[
					0.5811337796770671,
					2.905713236050664
				],
				[
					0,
					0
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.3046875,
				0.359375,
				0.447265625,
				0.4404296875,
				0.2666015625,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 618,
			"versionNonce": 1399613934,
			"isDeleted": false,
			"id": "vkVKJAfOc9DSeYD72uUjF",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1247.7538728171687,
			"y": 832.0781772525004,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 12.78512050355689,
			"height": 19.468269814006508,
			"seed": 33653476,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862518,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					3.1962801258891975
				],
				[
					0.29054472100589407,
					5.520859582262795
				],
				[
					0.8716785006829613,
					7.554849979965218
				],
				[
					1.4528566180253073,
					8.717139708152041
				],
				[
					1.7434013390312013,
					9.298273487829109
				],
				[
					2.3245351187082686,
					9.298273487829109
				],
				[
					3.196257957056509,
					6.683127141616929
				],
				[
					3.196257957056509,
					4.068002964237487
				],
				[
					3.196257957056509,
					0.5811337796770671
				],
				[
					3.196257957056509,
					-2.9057132360507136
				],
				[
					4.939703633753088,
					-7.264283090126734
				],
				[
					7.5548278111325295,
					-9.007706597990575
				],
				[
					9.879407267506176,
					-10.1699963261774
				],
				[
					11.913397665208551,
					-10.1699963261774
				],
				[
					12.78512050355689,
					-9.588862546500332
				],
				[
					12.494531444885618,
					-7.845439038636441
				],
				[
					9.879407267506176,
					-5.520859582262844
				],
				[
					9.879407267506176,
					-5.520859582262844
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2724609375,
				0.318359375,
				0.357421875,
				0.380859375,
				0.390625,
				0.3984375,
				0.41796875,
				0.486328125,
				0.513671875,
				0.5283203125,
				0.5439453125,
				0.5615234375,
				0.5634765625,
				0.5634765625,
				0.5634765625,
				0.533203125,
				0.4140625,
				0.015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 609,
			"versionNonce": 928642034,
			"isDeleted": false,
			"id": "Apxz1jQCN2b0Hl-BcydZ_",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1249.787863214871,
			"y": 829.7535977961268,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 11.913397665208649,
			"height": 0.8717228383482897,
			"seed": 1530787300,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862518,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.29054472100589407,
					0.29056688983853357
				],
				[
					0.581133779677067,
					0.5811559485097562
				],
				[
					2.0339903977024734,
					0.8717228383482897
				],
				[
					4.939703633753087,
					0.5811559485097562
				],
				[
					7.554827811132628,
					0.5811559485097562
				],
				[
					9.298273487829109,
					0.5811559485097562
				],
				[
					10.460541047183241,
					0.5811559485097562
				],
				[
					11.913397665208649,
					0.29056688983853357
				],
				[
					11.913397665208649,
					0.29056688983853357
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.35546875,
				0.3935546875,
				0.4541015625,
				0.5029296875,
				0.521484375,
				0.5244140625,
				0.4794921875,
				0.2587890625,
				0.0126953125,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 611,
			"versionNonce": 2053438510,
			"isDeleted": false,
			"id": "LpTvRiV6HY0g9fy8CGCAg",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1278.5544065167069,
			"y": 825.6855948318894,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 12.494575782550996,
			"height": 13.656865510737818,
			"seed": 247058652,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862518,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-5.23029269242436,
					4.649158912747243
				],
				[
					-6.683149310449667,
					7.8454390386364405
				],
				[
					-7.264283090126734,
					10.169996326177397
				],
				[
					-6.973694031455562,
					11.913442002873927
				],
				[
					-5.811426472101427,
					12.785142672389528
				],
				[
					-4.358569854076021,
					13.366298620899284
				],
				[
					-2.6151241773795406,
					13.366298620899284
				],
				[
					-0.5811337796770671,
					13.656865510737818
				],
				[
					2.0339903977023743,
					13.366298620899284
				],
				[
					5.230292692424261,
					12.785142672389528
				],
				[
					5.230292692424261,
					12.785142672389528
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2783203125,
				0.447265625,
				0.48828125,
				0.5126953125,
				0.5185546875,
				0.5205078125,
				0.5205078125,
				0.5205078125,
				0.5029296875,
				0.404296875,
				0.015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 615,
			"versionNonce": 127575474,
			"isDeleted": false,
			"id": "L5kBVUrnMWuMjCmGv7ePl",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1289.0149919015555,
			"y": 829.1724640164498,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 13.075709562228063,
			"height": 7.845416869803802,
			"seed": 1780793316,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862518,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-1.7434456766964803,
					3.1962801258892473
				],
				[
					-2.0339903977023743,
					4.068002964237487
				],
				[
					-2.3245794563735473,
					6.101993361939911
				],
				[
					-2.0339903977023743,
					7.264283090126734
				],
				[
					-1.7434456766964803,
					7.554849979965268
				],
				[
					-0.8717228383482402,
					7.845416869803802
				],
				[
					0.5811337796770671,
					7.264283090126734
				],
				[
					3.486847015727781,
					4.649136743914554
				],
				[
					5.23029269242436,
					2.61514634621218
				],
				[
					6.1019711931072225,
					1.1622897281868232
				],
				[
					7.554827811132629,
					2.9057132360507136
				],
				[
					8.426550649480868,
					5.230270523591622
				],
				[
					9.007684429157935,
					6.101993361939911
				],
				[
					10.751130105854516,
					7.554849979965268
				],
				[
					10.751130105854516,
					7.554849979965268
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.251953125,
				0.328125,
				0.359375,
				0.3974609375,
				0.3974609375,
				0.3974609375,
				0.3974609375,
				0.404296875,
				0.4443359375,
				0.4638671875,
				0.486328125,
				0.517578125,
				0.515625,
				0.501953125,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 618,
			"versionNonce": 1360086638,
			"isDeleted": false,
			"id": "BXxM4S_O-QjB70ww6MjFo",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1299.7661220074099,
			"y": 832.6593110321776,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 10.46058538484862,
			"height": 11.041719164525688,
			"seed": 1221035100,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862518,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					0.29056688983853357
				],
				[
					-0.2905890586712721,
					1.743423507863841
				],
				[
					0,
					2.905713236050664
				],
				[
					0.290589058671173,
					3.4868691845604203
				],
				[
					0.290589058671173,
					3.777436074398954
				],
				[
					0.581133779677067,
					3.4868691845604203
				],
				[
					1.162267559354134,
					1.743423507863841
				],
				[
					1.74344567669648,
					-1.4528566180253568
				],
				[
					2.3245794563735473,
					-3.486847015727781
				],
				[
					3.4868470157276814,
					-4.939703633753088
				],
				[
					5.2302926924242605,
					-6.101993361939911
				],
				[
					6.973694031455461,
					-6.973716200288201
				],
				[
					8.426550649480768,
					-7.264283090126734
				],
				[
					9.298273487829109,
					-6.973716200288201
				],
				[
					9.879407267506174,
					-6.683127141616978
				],
				[
					9.879407267506174,
					-6.392560251778445
				],
				[
					10.169996326177348,
					-5.8114264721013775
				],
				[
					10.169996326177348,
					-5.8114264721013775
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2587890625,
				0.2861328125,
				0.328125,
				0.38671875,
				0.3984375,
				0.3984375,
				0.4609375,
				0.5146484375,
				0.5400390625,
				0.552734375,
				0.5625,
				0.5673828125,
				0.5673828125,
				0.5673828125,
				0.5625,
				0.50390625,
				0.2841796875,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 618,
			"versionNonce": 2019499890,
			"isDeleted": false,
			"id": "ZXFS18tGC0NJlOjcQ5pFZ",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1311.9701087312897,
			"y": 825.3950279420508,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 13.075709562228063,
			"height": 11.622852944202705,
			"seed": 1925644636,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862518,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.5811337796770671,
					1.4528566180253568
				],
				[
					-0.8717228383482402,
					2.61514634621218
				],
				[
					-0.8717228383482402,
					4.358569854076021
				],
				[
					-0.5811337796770671,
					7.264283090126734
				],
				[
					-0.290544721005795,
					9.298295656661798
				],
				[
					-0.290544721005795,
					10.1699963261774
				],
				[
					0,
					10.1699963261774
				],
				[
					0.8717228383483393,
					8.426572818313508
				],
				[
					1.4528566180254063,
					6.101993361939911
				],
				[
					2.6151685150448194,
					3.777436074398954
				],
				[
					5.23029269242436,
					0.5811559485097562
				],
				[
					7.554872148797908,
					-0.5811337796770671
				],
				[
					9.588862546500382,
					-1.1622897281867737
				],
				[
					11.041719164525688,
					-1.4528566180253073
				],
				[
					11.913442002873929,
					-1.4528566180253073
				],
				[
					12.203986723879822,
					-1.1622897281867737
				],
				[
					12.203986723879822,
					-0.29056688983853357
				],
				[
					12.203986723879822,
					-0.29056688983853357
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.310546875,
				0.35546875,
				0.3828125,
				0.41796875,
				0.4384765625,
				0.4423828125,
				0.4521484375,
				0.4970703125,
				0.517578125,
				0.5380859375,
				0.548828125,
				0.5546875,
				0.5546875,
				0.5546875,
				0.5546875,
				0.515625,
				0.318359375,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 607,
			"versionNonce": 406472878,
			"isDeleted": false,
			"id": "mlK4Nb2DAi5-eaJEYvBok",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1327.6609868085625,
			"y": 823.9421713240256,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 10.460585384848523,
			"height": 11.913419834041239,
			"seed": 821968476,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862518,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					1.4528566180253073
				],
				[
					-0.5811781173423461,
					3.4868691845604203
				],
				[
					-1.1623118970194133,
					6.392582420611085
				],
				[
					-0.8717228383482403,
					11.041719164525638
				],
				[
					2.615124177379541,
					11.913419834041239
				],
				[
					9.29827348782911,
					8.426572818313508
				],
				[
					9.29827348782911,
					8.426572818313508
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2587890625,
				0.515625,
				0.533203125,
				0.552734375,
				0.56640625,
				0.5166015625,
				0.0166015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 607,
			"versionNonce": 1441685810,
			"isDeleted": false,
			"id": "DP2gWkLsQiol0HRIn2wTo",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1346.5481228428919,
			"y": 826.5573176702376,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 31.091167095874592,
			"height": 27.894842632320017,
			"seed": 1502647140,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862518,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-2.9057132360507136,
					0.29056688983853357
				],
				[
					-8.426594987146247,
					4.068002964237487
				],
				[
					-11.913442002873929,
					6.973716200288152
				],
				[
					-22.083438329051376,
					16.853145636627016
				],
				[
					-27.023141962804466,
					22.955138998566927
				],
				[
					-31.091167095874592,
					27.894842632320017
				],
				[
					-31.091167095874592,
					27.894842632320017
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.29296875,
				0.44140625,
				0.5234375,
				0.5341796875,
				0.515625,
				0.3212890625,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 723,
			"versionNonce": 260637422,
			"isDeleted": false,
			"id": "Wi7bcqHcc0bsYF6kjwQiq",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1237.7582919989259,
			"y": 913.3800256164186,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 14.296130403448714,
			"height": 24.059310915019477,
			"seed": 1245394148,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862518,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					0.6973605356124806
				],
				[
					0,
					2.0921082094366485
				],
				[
					0,
					5.578964092697466
				],
				[
					-0.3487068704054473,
					7.671072302134114
				],
				[
					0,
					13.250036394831579
				],
				[
					0.3486536652070333,
					16.388212010286157
				],
				[
					0.3486536652070333,
					19.17770735793449
				],
				[
					0.3486536652070333,
					21.26981556737114
				],
				[
					0,
					21.967176102983622
				],
				[
					-0.3487068704054473,
					22.31588297338907
				],
				[
					1.7434279416304084,
					21.61849583517738
				],
				[
					5.230283824891226,
					21.61849583517738
				],
				[
					9.763207114169969,
					21.967176102983622
				],
				[
					11.855288721007412,
					22.31588297338907
				],
				[
					12.90135612702534,
					22.66456324119531
				],
				[
					13.59871666263782,
					23.013243509001548
				],
				[
					13.947423533043267,
					24.059310915019477
				],
				[
					13.947423533043267,
					24.059310915019477
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2158203125,
				0.283203125,
				0.306640625,
				0.3359375,
				0.357421875,
				0.384765625,
				0.392578125,
				0.40234375,
				0.43359375,
				0.4619140625,
				0.4833984375,
				0.5,
				0.5,
				0.5,
				0.5,
				0.501953125,
				0.48046875,
				0.03125,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 724,
			"versionNonce": 1269787378,
			"isDeleted": false,
			"id": "VVarZAHVMcWK-L2zjq0Z9",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1253.7977971388066,
			"y": 912.6826384782071,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 9.763207114169969,
			"height": 23.361950379406995,
			"seed": 1415653348,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862518,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.34870687040544723,
					2.440815079842096
				],
				[
					0.34870687040544723,
					6.276351230909153
				],
				[
					0.34870687040544723,
					10.11188738197621
				],
				[
					0,
					14.993490939061195
				],
				[
					-0.3486536652070332,
					17.78298628670953
				],
				[
					-0.3486536652070332,
					19.87509449614618
				],
				[
					-0.6973605356124805,
					21.26984216997035
				],
				[
					-0.6973605356124805,
					21.967202705582828
				],
				[
					-0.3486536652070332,
					23.013270111600757
				],
				[
					1.0460674060179278,
					23.361950379406995
				],
				[
					3.4868558832608163,
					23.013270111600757
				],
				[
					5.927697565702119,
					22.31588297338907
				],
				[
					7.671125507332527,
					21.967202705582828
				],
				[
					8.717139708152041,
					21.618522437776587
				],
				[
					9.065846578557489,
					21.618522437776587
				],
				[
					9.065846578557489,
					21.967202705582828
				],
				[
					9.065846578557489,
					22.66456324119531
				],
				[
					9.065846578557489,
					23.361950379406995
				],
				[
					9.065846578557489,
					23.361950379406995
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2880859375,
				0.39453125,
				0.416015625,
				0.4248046875,
				0.4345703125,
				0.458984375,
				0.4794921875,
				0.4921875,
				0.4970703125,
				0.5048828125,
				0.51171875,
				0.5185546875,
				0.521484375,
				0.521484375,
				0.525390625,
				0.5224609375,
				0.5224609375,
				0.2333984375,
				0.0556640625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 723,
			"versionNonce": 428242222,
			"isDeleted": false,
			"id": "0B8qcVmgD3vNbLoJ5H6HE",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1278.9032020624434,
			"y": 921.3997781863591,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 14.296130403448714,
			"height": 14.644810671254955,
			"seed": 224343388,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862518,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-5.230283824891226,
					0.3487068704054473
				],
				[
					-8.019779172539561,
					1.3947476738241682
				],
				[
					-9.763207114169969,
					3.1381756154545766
				],
				[
					-10.111913984575416,
					4.184243021472504
				],
				[
					-8.368486042945008,
					5.927670963102913
				],
				[
					-4.532923289278744,
					7.322418636927081
				],
				[
					-1.394774276423375,
					8.717139708152041
				],
				[
					1.046014200819514,
					9.763207114169969
				],
				[
					2.4407884772428887,
					10.809274520187898
				],
				[
					2.4407884772428887,
					11.506635055800379
				],
				[
					1.046014200819514,
					12.901382729624546
				],
				[
					-2.0921348120358556,
					13.598743265237026
				],
				[
					-5.92769756570212,
					13.947423533043267
				],
				[
					-9.065846578557489,
					13.947423533043267
				],
				[
					-10.809274520187898,
					14.296130403448714
				],
				[
					-11.855341926205826,
					14.644810671254955
				],
				[
					-8.368486042945008,
					14.296130403448714
				],
				[
					-8.368486042945008,
					14.296130403448714
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.1923828125,
				0.302734375,
				0.408203125,
				0.4794921875,
				0.4921875,
				0.494140625,
				0.494140625,
				0.4921875,
				0.486328125,
				0.4912109375,
				0.4931640625,
				0.4990234375,
				0.5166015625,
				0.53515625,
				0.5576171875,
				0.55859375,
				0.466796875,
				0.0166015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 723,
			"versionNonce": 2702514,
			"isDeleted": false,
			"id": "NTJanmZIe8KDBrLCrDM2n",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1286.9229280297843,
			"y": 929.4195573588986,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 9.065846578557489,
			"height": 8.717139708152041,
			"seed": 212169308,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862518,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-2.7894421424499223,
					2.4407884772428887
				],
				[
					-3.1381490128553695,
					3.1381756154545766
				],
				[
					-3.1381490128553695,
					3.835536151067057
				],
				[
					-0.6973605356124806,
					4.8816035570849845
				],
				[
					1.7434279416304084,
					4.184216418873297
				],
				[
					4.184269624071711,
					3.4868558832608167
				],
				[
					5.578990695296673,
					1.7434279416304084
				],
				[
					5.92769756570212,
					0.3486802678062403
				],
				[
					4.881630159684192,
					-1.3947476738241682
				],
				[
					3.4868558832608167,
					-2.7894953476483364
				],
				[
					1.394774276423375,
					-3.4868558832608167
				],
				[
					-0.3486536652070333,
					-3.835536151067057
				],
				[
					-1.3947210712249611,
					-3.835536151067057
				],
				[
					-1.7434279416304084,
					-3.1381756154545766
				],
				[
					-1.3947210712249611,
					-2.4407884772428887
				],
				[
					1.394774276423375,
					-1.0460674060179278
				],
				[
					0,
					0
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2900390625,
				0.3955078125,
				0.4365234375,
				0.4775390625,
				0.482421875,
				0.482421875,
				0.4658203125,
				0.447265625,
				0.4501953125,
				0.4716796875,
				0.4873046875,
				0.4990234375,
				0.5078125,
				0.5078125,
				0.4990234375,
				0.40625,
				0.015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 714,
			"versionNonce": 1604034414,
			"isDeleted": false,
			"id": "LlGJSrQj1fy_ezUSsTx-p",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1297.7322025499723,
			"y": 934.3011609159835,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 3.1381490128553695,
			"height": 23.361950379406995,
			"seed": 2058579804,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862518,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.3487068704054473,
					-5.927670963102913
				],
				[
					-0.3487068704054473,
					-7.671098904733321
				],
				[
					-0.3487068704054473,
					-9.763207114169969
				],
				[
					-0.6973605356124806,
					-13.947423533043267
				],
				[
					-0.6973605356124806,
					-16.388238612885363
				],
				[
					-1.3947210712249611,
					-20.921135299564902
				],
				[
					-2.4407884772428887,
					-22.66456324119531
				],
				[
					-3.1381490128553695,
					-23.361950379406995
				],
				[
					-3.1381490128553695,
					-23.361950379406995
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.30859375,
				0.4970703125,
				0.5302734375,
				0.5537109375,
				0.5712890625,
				0.5712890625,
				0.5263671875,
				0.3544921875,
				0.0146484375,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 710,
			"versionNonce": 822269554,
			"isDeleted": false,
			"id": "Edbd4UJUsyA1s1WvSEW-I",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1307.8440633293494,
			"y": 925.5840212078315,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 2.0921348120358556,
			"height": 0.6973871382116875,
			"seed": 910656996,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862518,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-1.046014200819514,
					-0.3486802678062403
				],
				[
					-1.3947210712249611,
					-0.3486802678062403
				],
				[
					0.6974137408108946,
					-0.6973871382116875
				],
				[
					0,
					0
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.421875,
				0.4970703125,
				0.4970703125,
				0.0166015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 720,
			"versionNonce": 1980858798,
			"isDeleted": false,
			"id": "rSaNEpQF3ZHT464l1swSH",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1312.7256934890336,
			"y": 925.5840212078315,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 11.506635055800379,
			"height": 11.157928185394931,
			"seed": 633243612,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862518,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					3.835536151067057
				],
				[
					0,
					4.184216418873297
				],
				[
					0,
					4.532896686679537
				],
				[
					0.6973605356124806,
					2.7894687450491293
				],
				[
					1.7434279416304084,
					0
				],
				[
					2.7894953476483364,
					-2.7894953476483364
				],
				[
					4.184216418873297,
					-4.8816035570849845
				],
				[
					5.927644360503706,
					-6.625031498715393
				],
				[
					8.019779172539561,
					-6.625031498715393
				],
				[
					10.809221314989484,
					-3.835536151067057
				],
				[
					11.157928185394931,
					-3.1381756154545766
				],
				[
					10.809221314989484,
					0
				],
				[
					10.111860779377002,
					1.7434279416304084
				],
				[
					11.506635055800379,
					2.4407884772428887
				],
				[
					11.506635055800379,
					2.4407884772428887
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.1611328125,
				0.2314453125,
				0.279296875,
				0.294921875,
				0.4287109375,
				0.46484375,
				0.4775390625,
				0.482421875,
				0.490234375,
				0.49609375,
				0.5146484375,
				0.517578125,
				0.5234375,
				0.525390625,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 721,
			"versionNonce": 1325611058,
			"isDeleted": false,
			"id": "wm6DpQO2B2Crq7h7x85Bj",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1333.9954824538056,
			"y": 923.1432061279895,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 10.809221314989484,
			"height": 8.717139708152041,
			"seed": 1700155364,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862518,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					3.138202218053784,
					-1.7434279416304084
				],
				[
					3.8355627536662644,
					-2.4407884772428887
				],
				[
					3.486855883260817,
					-3.4868558832608167
				],
				[
					2.092134812035856,
					-4.184216418873297
				],
				[
					-1.3947210712249614,
					-3.835536151067057
				],
				[
					-3.486855883260817,
					-2.4407884772428887
				],
				[
					-4.881576954485778,
					-0.3486802678062403
				],
				[
					-5.578937490098259,
					1.3947476738241682
				],
				[
					-5.578937490098259,
					3.1381756154545766
				],
				[
					-4.881576954485778,
					3.835562753666264
				],
				[
					-3.486855883260817,
					4.184243021472504
				],
				[
					-1.3947210712249614,
					4.184243021472504
				],
				[
					2.7894953476483364,
					4.184243021472504
				],
				[
					5.230283824891226,
					4.532923289278744
				],
				[
					0,
					0
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2509765625,
				0.3134765625,
				0.34765625,
				0.3896484375,
				0.396484375,
				0.4326171875,
				0.482421875,
				0.50390625,
				0.525390625,
				0.5498046875,
				0.552734375,
				0.560546875,
				0.55859375,
				0.4111328125,
				0.015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 710,
			"versionNonce": 1121262,
			"isDeleted": false,
			"id": "6CZZJcfCvfFQZ3tRDLE-5",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1341.666607961138,
			"y": 928.7221968232861,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 5.927644360503706,
			"height": 17.085599148497842,
			"seed": 1184239460,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862518,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					2.4407884772428887,
					-5.230283824891225
				],
				[
					4.53287008408033,
					-8.019779172539561
				],
				[
					5.927644360503706,
					-11.855315323606616
				],
				[
					4.53287008408033,
					-17.085599148497842
				],
				[
					4.53287008408033,
					-17.085599148497842
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.302734375,
				0.4833984375,
				0.4970703125,
				0.412109375,
				0.015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 713,
			"versionNonce": 437346802,
			"isDeleted": false,
			"id": "cK5epojg3H5z_vOxEkHbX",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1343.4100359027682,
			"y": 912.6826384782071,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 9.065793373359075,
			"height": 12.552702461818306,
			"seed": 246146652,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862518,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					4.532923289278744
				],
				[
					0.3486536652070332,
					6.276351230909153
				],
				[
					1.0460142008195137,
					7.671098904733321
				],
				[
					2.0920816068374415,
					9.41452684636373
				],
				[
					3.138149012855369,
					10.11188738197621
				],
				[
					5.230283824891225,
					11.506635055800379
				],
				[
					9.065793373359075,
					12.552702461818306
				],
				[
					9.065793373359075,
					12.552702461818306
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2509765625,
				0.37109375,
				0.4501953125,
				0.501953125,
				0.52734375,
				0.52734375,
				0.4853515625,
				0.0166015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 717,
			"versionNonce": 1403219502,
			"isDeleted": false,
			"id": "dC41692y00hdSaPG1in6U",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1358.0548199714242,
			"y": 925.5840212078315,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 18.829000487529044,
			"height": 18.480346822322012,
			"seed": 136604892,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862518,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.6973605356124805,
					-3.1381756154545766
				],
				[
					-2.0921348120358556,
					-6.276351230909153
				],
				[
					-3.8355627536662635,
					-10.460567649782451
				],
				[
					-6.973711766521633,
					-16.388238612885363
				],
				[
					-6.6250581013145995,
					-17.434279416304083
				],
				[
					-5.578990695296672,
					-18.13166655451577
				],
				[
					-3.138202218053783,
					-18.480346822322012
				],
				[
					1.394721071224961,
					-18.13166655451577
				],
				[
					3.138149012855369,
					-17.782959684110324
				],
				[
					7.322365431728666,
					-17.085599148497842
				],
				[
					11.85528872100741,
					-16.039531742479916
				],
				[
					11.85528872100741,
					-16.039531742479916
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.4111328125,
				0.486328125,
				0.4970703125,
				0.4482421875,
				0.3251953125,
				0.4384765625,
				0.509765625,
				0.5361328125,
				0.53515625,
				0.5302734375,
				0.42578125,
				0.015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 715,
			"versionNonce": 1026839474,
			"isDeleted": false,
			"id": "pynsKkBoJdAA8Ji7cuaRb",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1372.350897169674,
			"y": 922.445845592377,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 16.039558345079122,
			"height": 3.1381756154545766,
			"seed": 472169564,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862518,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.3487068704054473,
					0
				],
				[
					1.0460674060179278,
					0
				],
				[
					3.1382022180537836,
					-0.3486802678062403
				],
				[
					4.532923289278744,
					-0.3486802678062403
				],
				[
					8.368486042945008,
					-0.6973605356124806
				],
				[
					12.552702461818306,
					-1.3947476738241682
				],
				[
					13.598769867836234,
					-1.7434279416304084
				],
				[
					15.342197809466642,
					-2.0921082094366485
				],
				[
					16.039558345079122,
					-3.1381756154545766
				],
				[
					16.039558345079122,
					-3.1381756154545766
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.25,
				0.35546875,
				0.4033203125,
				0.46484375,
				0.482421875,
				0.49609375,
				0.4921875,
				0.4853515625,
				0.3359375,
				0.0146484375,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 710,
			"versionNonce": 498169966,
			"isDeleted": false,
			"id": "07j7mjc8GcHW-xNfWfhmr",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1376.1864599233406,
			"y": 908.84710232714,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 13.947423533043267,
			"height": 1.3947476738241682,
			"seed": 698009436,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862518,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					8.717139708152041,
					-1.046040803418721
				],
				[
					10.111860779377002,
					-1.3947476738241682
				],
				[
					12.203995591412859,
					-1.046040803418721
				],
				[
					13.947423533043267,
					-0.6973605356124807
				],
				[
					13.947423533043267,
					-0.6973605356124807
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.41015625,
				0.47265625,
				0.4775390625,
				0.48046875,
				0.3818359375,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 763,
			"versionNonce": 1788022130,
			"isDeleted": false,
			"id": "12XQbvWbaQHcdBMZ6fZpI",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1404.4299606546342,
			"y": 898.3865612799566,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 9.414500243764522,
			"height": 27.894847066086534,
			"seed": 1581127396,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862518,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					0.3486802678062403
				],
				[
					0,
					1.7434279416304084
				],
				[
					0,
					9.065819975958282
				],
				[
					-0.3486536652070332,
					13.947423533043267
				],
				[
					-0.3486536652070332,
					20.22377476395242
				],
				[
					-0.3486536652070332,
					23.013243509001548
				],
				[
					0,
					24.75667145063196
				],
				[
					0,
					25.802738856649885
				],
				[
					0.34870687040544723,
					26.151419124456126
				],
				[
					1.394774276423375,
					26.151419124456126
				],
				[
					3.138202218053783,
					25.802738856649885
				],
				[
					6.6250581013145995,
					25.802738856649885
				],
				[
					8.368486042945008,
					26.151419124456126
				],
				[
					8.717139708152041,
					26.151419124456126
				],
				[
					9.065846578557489,
					27.197486530474052
				],
				[
					9.065846578557489,
					27.894847066086534
				],
				[
					8.717139708152041,
					27.894847066086534
				],
				[
					8.717139708152041,
					27.894847066086534
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2509765625,
				0.3271484375,
				0.341796875,
				0.3671875,
				0.37890625,
				0.38671875,
				0.4033203125,
				0.4306640625,
				0.4423828125,
				0.4716796875,
				0.521484375,
				0.5244140625,
				0.5263671875,
				0.5263671875,
				0.5263671875,
				0.48828125,
				0.30078125,
				0.23828125,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 765,
			"versionNonce": 100940462,
			"isDeleted": false,
			"id": "hrzMXiirWyJ_ejRSTcVEQ",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1420.8181726649202,
			"y": 894.2023448610835,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 7.671072302134114,
			"height": 33.12513089097776,
			"seed": 1217497572,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862518,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					-0.3487068704054473
				],
				[
					-0.3486536652070333,
					1.3947210712249611
				],
				[
					-0.6973605356124806,
					5.230283824891226
				],
				[
					-1.046014200819514,
					11.855288721007412
				],
				[
					-1.3947210712249611,
					20.57242842915945
				],
				[
					-1.3947210712249611,
					24.407991182825718
				],
				[
					-1.046014200819514,
					28.940887869505254
				],
				[
					-1.046014200819514,
					29.986955275523183
				],
				[
					-1.046014200819514,
					31.032996078941903
				],
				[
					-1.046014200819514,
					32.07906348495983
				],
				[
					-1.046014200819514,
					32.42774375276607
				],
				[
					-0.6973605356124806,
					32.776424020572314
				],
				[
					0.3487068704054473,
					32.42774375276607
				],
				[
					1.7434279416304084,
					32.07906348495983
				],
				[
					2.440841682441303,
					32.07906348495983
				],
				[
					3.835562753666264,
					31.73038321715359
				],
				[
					4.184269624071711,
					31.73038321715359
				],
				[
					4.532923289278744,
					32.07906348495983
				],
				[
					6.276351230909153,
					32.42774375276607
				],
				[
					6.276351230909153,
					32.42774375276607
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2900390625,
				0.3759765625,
				0.41796875,
				0.44921875,
				0.47265625,
				0.4873046875,
				0.5,
				0.521484375,
				0.52734375,
				0.53515625,
				0.548828125,
				0.5556640625,
				0.5556640625,
				0.578125,
				0.5810546875,
				0.5810546875,
				0.583984375,
				0.5224609375,
				0.501953125,
				0.0146484375,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 757,
			"versionNonce": 2004127538,
			"isDeleted": false,
			"id": "oe-P3NNjYXhKwRj-e8MNZ",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1445.9235775885568,
			"y": 897.6892007443441,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 13.947423533043267,
			"height": 27.546140195681087,
			"seed": 2127560804,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862518,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-5.578990695296673,
					2.7894687450491293
				],
				[
					-10.460567649782451,
					9.763180511570763
				],
				[
					-12.203995591412859,
					14.644784068655747
				],
				[
					-12.901409332223754,
					19.17770735793449
				],
				[
					-11.855341926205826,
					23.71060404461403
				],
				[
					-9.065846578557489,
					25.80271225405068
				],
				[
					-6.9737117665216335,
					26.848779660068605
				],
				[
					-3.4868558832608167,
					27.197459927874846
				],
				[
					-1.394774276423375,
					27.546140195681087
				],
				[
					0,
					27.197459927874846
				],
				[
					1.046014200819514,
					27.546140195681087
				],
				[
					1.046014200819514,
					27.546140195681087
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2041015625,
				0.248046875,
				0.380859375,
				0.462890625,
				0.4873046875,
				0.513671875,
				0.52734375,
				0.5361328125,
				0.5302734375,
				0.46875,
				0.2919921875,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 766,
			"versionNonce": 1397011694,
			"isDeleted": false,
			"id": "1Su12RMwkzqRsQcuH2YPA",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1463.3578570048612,
			"y": 907.8010615237213,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 10.111860779377002,
			"height": 16.039558345079122,
			"seed": 332077284,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862518,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-3.138202218053783,
					0
				],
				[
					-6.276351230909152,
					0.3487068704054473
				],
				[
					-9.065846578557489,
					1.3947476738241682
				],
				[
					-8.717139708152041,
					1.7434279416304084
				],
				[
					-7.32241863692708,
					3.4868558832608167
				],
				[
					-4.532923289278744,
					4.8816035570849845
				],
				[
					-2.0921348120358556,
					6.625031498715393
				],
				[
					-0.34870687040544723,
					8.368459440345802
				],
				[
					0.6973605356124805,
					10.460567649782451
				],
				[
					1.0460142008195137,
					12.203995591412859
				],
				[
					0.6973605356124805,
					12.901382729624546
				],
				[
					-0.6974137408108945,
					13.947423533043267
				],
				[
					-2.0921348120358556,
					14.296130403448714
				],
				[
					-4.184269624071711,
					14.644810671254955
				],
				[
					-6.6250581013145995,
					14.993490939061195
				],
				[
					-8.019779172539561,
					15.342171206867436
				],
				[
					-8.368486042945008,
					15.690851474673675
				],
				[
					-8.019779172539561,
					15.690851474673675
				],
				[
					-7.671125507332527,
					16.039558345079122
				],
				[
					-3.8355627536662635,
					15.690851474673675
				],
				[
					-3.8355627536662635,
					15.690851474673675
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2431640625,
				0.2890625,
				0.380859375,
				0.470703125,
				0.4833984375,
				0.48046875,
				0.48046875,
				0.4736328125,
				0.4716796875,
				0.4736328125,
				0.482421875,
				0.501953125,
				0.5400390625,
				0.5625,
				0.5791015625,
				0.58984375,
				0.58984375,
				0.5869140625,
				0.4228515625,
				0.3720703125,
				0.0146484375,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 762,
			"versionNonce": 2017450226,
			"isDeleted": false,
			"id": "1iy9LkJ2vLPQV3YdKco_f",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1470.6802224365902,
			"y": 910.2418766035632,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 10.809221314989484,
			"height": 9.763180511570763,
			"seed": 1532176604,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862518,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-1.046067406017928,
					1.3947476738241682
				],
				[
					-1.3947210712249614,
					2.0921082094366485
				],
				[
					-1.3947210712249614,
					3.4868558832608167
				],
				[
					-1.046067406017928,
					4.8816035570849845
				],
				[
					0,
					6.625031498715393
				],
				[
					1.7434279416304086,
					8.368459440345802
				],
				[
					3.486855883260817,
					9.414500243764522
				],
				[
					4.8816301596841924,
					9.763180511570763
				],
				[
					6.276351230909154,
					9.763180511570763
				],
				[
					6.973711766521634,
					8.717139708152041
				],
				[
					7.671072302134115,
					6.9737117665216335
				],
				[
					8.717139708152043,
					4.532896686679537
				],
				[
					9.414500243764524,
					2.4407884772428887
				],
				[
					9.414500243764524,
					2.0921082094366485
				],
				[
					9.414500243764524,
					3.1381756154545766
				],
				[
					9.414500243764524,
					3.4868558832608167
				],
				[
					9.414500243764524,
					3.4868558832608167
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2109375,
				0.265625,
				0.2939453125,
				0.36328125,
				0.3974609375,
				0.404296875,
				0.4296875,
				0.4482421875,
				0.470703125,
				0.4833984375,
				0.498046875,
				0.517578125,
				0.5498046875,
				0.5634765625,
				0.5654296875,
				0.244140625,
				0.05859375,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 768,
			"versionNonce": 251389742,
			"isDeleted": false,
			"id": "Cpi8nrXXNB6PK-XdA9FRf",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1483.9302854340212,
			"y": 910.9392371391757,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 15.690851474673675,
			"height": 11.506635055800379,
			"seed": 557302372,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862518,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.3487068704054473,
					1.3947476738241682
				],
				[
					-0.3487068704054473,
					1.7434279416304084
				],
				[
					-0.3487068704054473,
					3.4868558832608167
				],
				[
					-0.3487068704054473,
					4.8816035570849845
				],
				[
					-0.3487068704054473,
					6.625031498715393
				],
				[
					0.3487068704054473,
					6.625031498715393
				],
				[
					2.7894953476483364,
					4.532923289278744
				],
				[
					4.881576954485777,
					2.7894953476483364
				],
				[
					7.322418636927081,
					0.6973871382116875
				],
				[
					7.671072302134114,
					0.3486802678062403
				],
				[
					8.019779172539561,
					0.6973871382116875
				],
				[
					8.368432837746594,
					1.3947476738241682
				],
				[
					9.414500243764522,
					1.7434279416304084
				],
				[
					11.157928185394931,
					1.7434279416304084
				],
				[
					12.90135612702534,
					2.0921082094366485
				],
				[
					13.59871666263782,
					3.835536151067057
				],
				[
					13.59871666263782,
					5.927670963102913
				],
				[
					13.59871666263782,
					8.368459440345802
				],
				[
					13.947423533043267,
					9.41452684636373
				],
				[
					14.296130403448714,
					10.460567649782451
				],
				[
					14.993490939061195,
					11.157954787994138
				],
				[
					15.342144604268228,
					11.506635055800379
				],
				[
					15.342144604268228,
					11.506635055800379
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2255859375,
				0.2685546875,
				0.3037109375,
				0.376953125,
				0.4130859375,
				0.4443359375,
				0.4990234375,
				0.5224609375,
				0.52734375,
				0.5244140625,
				0.5244140625,
				0.5244140625,
				0.52734375,
				0.537109375,
				0.5458984375,
				0.5537109375,
				0.5537109375,
				0.55859375,
				0.5791015625,
				0.58203125,
				0.5634765625,
				0.4248046875,
				0.015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 571,
			"versionNonce": 1551624882,
			"isDeleted": false,
			"id": "JSke0cbrlsoPfEhoebSI_",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1503.805406532766,
			"y": 895.2483856645022,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 12.552649256619892,
			"height": 39.052775251481464,
			"seed": 1630344540,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862518,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					-1.0460408034187207
				],
				[
					0,
					-2.4407884772428887
				],
				[
					0.6973605356124806,
					-3.1381490128553695
				],
				[
					3.4868558832608167,
					-2.4407884772428887
				],
				[
					5.578937490098259,
					0.6973871382116875
				],
				[
					7.671072302134114,
					4.8816035570849845
				],
				[
					9.763153908971555,
					9.41452684636373
				],
				[
					11.157928185394931,
					16.388238612885363
				],
				[
					12.203995591412859,
					19.87509449614618
				],
				[
					12.552649256619892,
					23.013270111600757
				],
				[
					12.552649256619892,
					25.454058588843644
				],
				[
					11.506581850601965,
					29.98698187812239
				],
				[
					10.460567649782451,
					32.427770355365276
				],
				[
					9.763153908971555,
					33.822518029189446
				],
				[
					9.763153908971555,
					34.51987856480193
				],
				[
					9.763153908971555,
					34.868558832608166
				],
				[
					9.763153908971555,
					35.565945970819854
				],
				[
					10.111860779377002,
					35.9146262386261
				],
				[
					10.111860779377002,
					35.9146262386261
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.1923828125,
				0.2431640625,
				0.3017578125,
				0.3466796875,
				0.37890625,
				0.3740234375,
				0.369140625,
				0.37109375,
				0.3798828125,
				0.39453125,
				0.41796875,
				0.44921875,
				0.4873046875,
				0.5029296875,
				0.513671875,
				0.5185546875,
				0.521484375,
				0.4853515625,
				0.47265625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 574,
			"versionNonce": 697487726,
			"isDeleted": false,
			"id": "tENyq8jaLYbkAe5srCRAJ",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1291.1071976538562,
			"y": 864.2153895855602,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 8.717139708152041,
			"height": 13.598743265237026,
			"seed": 893292900,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862518,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-3.1382022180537836,
					-0.6973871382116875
				],
				[
					-3.835562753666264,
					-1.0460674060179278
				],
				[
					-4.532923289278744,
					-1.0460674060179278
				],
				[
					-5.230283824891226,
					-0.3487068704054473
				],
				[
					-5.230283824891226,
					1.0460408034187207
				],
				[
					-4.532923289278744,
					3.1381490128553695
				],
				[
					-3.4868558832608167,
					5.230283824891226
				],
				[
					-2.440841682441303,
					7.322392034327874
				],
				[
					-0.6974137408108946,
					9.763180511570763
				],
				[
					0,
					10.460567649782451
				],
				[
					0.3486536652070333,
					11.157928185394931
				],
				[
					0,
					11.50660845320117
				],
				[
					-1.7434279416304084,
					12.552675859219098
				],
				[
					-3.4868558832608167,
					12.552675859219098
				],
				[
					-5.230283824891226,
					12.552675859219098
				],
				[
					-6.9737117665216335,
					12.203995591412859
				],
				[
					-8.368486042945008,
					11.855288721007412
				],
				[
					-8.368486042945008,
					11.50660845320117
				],
				[
					-8.368486042945008,
					10.80924791758869
				],
				[
					-7.322418636927081,
					10.460567649782451
				],
				[
					-5.578990695296673,
					10.460567649782451
				],
				[
					-5.578990695296673,
					10.460567649782451
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2001953125,
				0.3251953125,
				0.390625,
				0.416015625,
				0.453125,
				0.4384765625,
				0.423828125,
				0.4140625,
				0.412109375,
				0.412109375,
				0.412109375,
				0.416015625,
				0.4501953125,
				0.4970703125,
				0.5146484375,
				0.521484375,
				0.5263671875,
				0.529296875,
				0.5263671875,
				0.4658203125,
				0.2109375,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 571,
			"versionNonce": 181388402,
			"isDeleted": false,
			"id": "9MMRIC9PS5BQwFzBxr2-G",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1301.5677653036387,
			"y": 865.6101106567851,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 11.855288721007412,
			"height": 11.506635055800379,
			"seed": 906500964,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862518,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					1.0460674060179278
				],
				[
					0,
					1.7434279416304084
				],
				[
					0,
					3.1381756154545766
				],
				[
					0,
					4.184243021472504
				],
				[
					0.6973605356124806,
					5.927670963102913
				],
				[
					1.046014200819514,
					7.671098904733321
				],
				[
					1.7434279416304084,
					8.717139708152041
				],
				[
					2.7894421424499223,
					9.41452684636373
				],
				[
					5.230283824891226,
					9.065846578557489
				],
				[
					6.9737117665216335,
					8.019779172539561
				],
				[
					8.368432837746594,
					6.625031498715393
				],
				[
					9.763153908971555,
					4.8816035570849845
				],
				[
					10.460567649782451,
					3.1381756154545766
				],
				[
					11.157928185394931,
					0.6973871382116875
				],
				[
					11.506581850601965,
					-0.3486802678062403
				],
				[
					11.506581850601965,
					-1.7434279416304084
				],
				[
					11.506581850601965,
					-2.0921082094366485
				],
				[
					11.855288721007412,
					0
				],
				[
					11.855288721007412,
					0
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.1923828125,
				0.21484375,
				0.224609375,
				0.259765625,
				0.265625,
				0.2978515625,
				0.3251953125,
				0.3349609375,
				0.341796875,
				0.3681640625,
				0.3916015625,
				0.408203125,
				0.4306640625,
				0.4501953125,
				0.46484375,
				0.46484375,
				0.4619140625,
				0.455078125,
				0.0146484375,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 572,
			"versionNonce": 508720046,
			"isDeleted": false,
			"id": "RzNB5QTUVR36Z-EXb13tX",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1317.9559773139247,
			"y": 864.5640698533664,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 16.03950513988071,
			"height": 8.717139708152041,
			"seed": 1930402268,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862518,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					2.0921082094366485
				],
				[
					0.34865366520703334,
					5.230283824891226
				],
				[
					0.34865366520703334,
					5.927644360503706
				],
				[
					0.6973605356124807,
					5.230283824891226
				],
				[
					1.3947210712249614,
					3.4868558832608167
				],
				[
					2.7894953476483364,
					1.0460408034187207
				],
				[
					3.486855883260817,
					0.3486802678062403
				],
				[
					4.184216418873298,
					0.6973605356124806
				],
				[
					5.230283824891226,
					1.7434279416304084
				],
				[
					6.276351230909154,
					2.4407884772428887
				],
				[
					8.368432837746596,
					2.4407884772428887
				],
				[
					10.111860779377004,
					1.3947476738241682
				],
				[
					11.506635055800379,
					0.6973605356124806
				],
				[
					12.552649256619894,
					2.0921082094366485
				],
				[
					12.901356127025341,
					3.4868558832608167
				],
				[
					13.598716662637822,
					6.625031498715393
				],
				[
					14.644784068655749,
					8.019752569940355
				],
				[
					15.34214460426823,
					8.717139708152041
				],
				[
					16.03950513988071,
					8.717139708152041
				],
				[
					16.03950513988071,
					8.717139708152041
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.1865234375,
				0.3095703125,
				0.3203125,
				0.330078125,
				0.419921875,
				0.4375,
				0.4501953125,
				0.4501953125,
				0.4501953125,
				0.4443359375,
				0.4423828125,
				0.44921875,
				0.45703125,
				0.4619140625,
				0.4638671875,
				0.47265625,
				0.4931640625,
				0.498046875,
				0.4599609375,
				0.0166015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 560,
			"versionNonce": 2097309234,
			"isDeleted": false,
			"id": "_8sFELEUNYTWVVSLCUR6Y",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1338.179752077877,
			"y": 865.6101106567851,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 11.157928185394931,
			"height": 3.4868558832608167,
			"seed": 1422326620,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862519,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					2.0920816068374415,
					-0.3486802678062403
				],
				[
					5.230283824891226,
					-0.6973605356124806
				],
				[
					7.322365431728667,
					-1.0460408034187207
				],
				[
					9.414500243764522,
					-1.3947210712249611
				],
				[
					10.809221314989484,
					-1.7434279416304084
				],
				[
					11.157928185394931,
					-1.7434279416304084
				],
				[
					10.460567649782451,
					-3.4868558832608167
				],
				[
					10.460567649782451,
					-3.4868558832608167
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2109375,
				0.3515625,
				0.416015625,
				0.423828125,
				0.423828125,
				0.4169921875,
				0.3359375,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 560,
			"versionNonce": 392416750,
			"isDeleted": false,
			"id": "mMI1fEYD5rWNz4sByoFsf",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1343.7586895679754,
			"y": 858.6363988902635,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 4.184216418873297,
			"height": 14.993490939061195,
			"seed": 1370644956,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862519,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.6973605356124806,
					3.835562753666264
				],
				[
					2.0921348120358556,
					7.671098904733321
				],
				[
					2.7894953476483364,
					10.11188738197621
				],
				[
					3.4868558832608167,
					11.855315323606618
				],
				[
					3.835562753666264,
					12.901382729624546
				],
				[
					3.835562753666264,
					13.947423533043267
				],
				[
					4.184216418873297,
					14.993490939061195
				],
				[
					4.184216418873297,
					14.993490939061195
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2548828125,
				0.400390625,
				0.482421875,
				0.4921875,
				0.4892578125,
				0.482421875,
				0.3955078125,
				0.015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 562,
			"versionNonce": 1543163890,
			"isDeleted": false,
			"id": "qCuXTwt8tJiN0Dg2Hjj8G",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1356.311392029793,
			"y": 863.5180024473484,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 10.111860779377002,
			"height": 2.7894687450491293,
			"seed": 1580054620,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862519,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1.394721071224961,
					0
				],
				[
					2.0920816068374415,
					0
				],
				[
					3.8355095484678494,
					-0.3486802678062403
				],
				[
					5.578937490098258,
					-0.3486802678062403
				],
				[
					6.973711766521633,
					0
				],
				[
					8.717139708152041,
					0
				],
				[
					9.763207114169969,
					0.3486802678062403
				],
				[
					10.111860779377002,
					-0.3486802678062403
				],
				[
					9.414500243764522,
					-2.4407884772428887
				],
				[
					9.414500243764522,
					-2.4407884772428887
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2060546875,
				0.30078125,
				0.3388671875,
				0.38671875,
				0.39453125,
				0.39453125,
				0.39453125,
				0.375,
				0.2119140625,
				0.0126953125,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 560,
			"versionNonce": 298836014,
			"isDeleted": false,
			"id": "qX_sfqjirg4kC53Fc4z-G",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1356.311392029793,
			"y": 854.103502203584,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 11.855288721007412,
			"height": 1.3947476738241682,
			"seed": 1740030812,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862519,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					2.4407884772428887,
					0
				],
				[
					5.230283824891226,
					0.6973605356124807
				],
				[
					6.276351230909153,
					1.046040803418721
				],
				[
					9.065793373359075,
					1.3947476738241682
				],
				[
					10.809221314989484,
					1.3947476738241682
				],
				[
					11.157928185394931,
					1.3947476738241682
				],
				[
					11.855288721007412,
					1.046040803418721
				],
				[
					11.855288721007412,
					1.046040803418721
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2587890625,
				0.3603515625,
				0.4150390625,
				0.427734375,
				0.439453125,
				0.44140625,
				0.40625,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 577,
			"versionNonce": 465568178,
			"isDeleted": false,
			"id": "2wySTLx4xmMqPEeR0IwK3",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1377.9298878649709,
			"y": 851.662687123742,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 13.59871666263782,
			"height": 19.875067893546973,
			"seed": 767896028,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862519,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					3.1381490128553695,
					-3.835536151067057
				],
				[
					4.184216418873297,
					-5.578964092697466
				],
				[
					4.532923289278744,
					-6.9737117665216335
				],
				[
					4.532923289278744,
					-8.019752569940355
				],
				[
					4.184216418873297,
					-8.368432837746594
				],
				[
					3.835562753666264,
					-8.019752569940355
				],
				[
					3.4868558832608167,
					-5.927644360503706
				],
				[
					3.4868558832608167,
					0.3487068704054473
				],
				[
					3.1381490128553695,
					3.835562753666264
				],
				[
					2.0921348120358556,
					6.625031498715393
				],
				[
					0.6973605356124806,
					8.717139708152041
				],
				[
					-0.6973605356124806,
					10.11188738197621
				],
				[
					-1.7434279416304084,
					10.809274520187898
				],
				[
					-2.0921348120358556,
					11.157954787994138
				],
				[
					-2.4407884772428887,
					11.506635055800379
				],
				[
					-2.0921348120358556,
					11.506635055800379
				],
				[
					-1.0460674060179278,
					11.157954787994138
				],
				[
					0.3487068704054473,
					10.809274520187898
				],
				[
					1.7434279416304084,
					10.460567649782451
				],
				[
					3.835562753666264,
					10.460567649782451
				],
				[
					5.927644360503706,
					10.460567649782451
				],
				[
					8.717139708152041,
					10.460567649782451
				],
				[
					10.111860779377002,
					10.460567649782451
				],
				[
					11.157928185394931,
					10.11188738197621
				],
				[
					11.157928185394931,
					10.11188738197621
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2509765625,
				0.3515625,
				0.3984375,
				0.4208984375,
				0.44921875,
				0.462890625,
				0.4794921875,
				0.462890625,
				0.4443359375,
				0.439453125,
				0.4462890625,
				0.4599609375,
				0.4716796875,
				0.5048828125,
				0.5224609375,
				0.525390625,
				0.5478515625,
				0.55078125,
				0.55078125,
				0.55078125,
				0.548828125,
				0.548828125,
				0.53125,
				0.4384765625,
				0.015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 574,
			"versionNonce": 25143918,
			"isDeleted": false,
			"id": "cSWFHEU3j_X3KQ_rdlEwC",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1202.889786371516,
			"y": 966.728931271349,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 17.085572545898636,
			"height": 16.736918880691604,
			"seed": 1030987620,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862519,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1.0460674060179278,
					-0.34868026780624034
				],
				[
					1.7434279416304084,
					-0.34868026780624034
				],
				[
					3.835562753666264,
					-1.3947210712249614
				],
				[
					7.671072302134114,
					-2.7894687450491293
				],
				[
					10.809274520187898,
					-4.532896686679538
				],
				[
					11.157928185394931,
					-4.881576954485778
				],
				[
					10.460567649782451,
					-5.578964092697466
				],
				[
					6.9737117665216335,
					-5.230283824891226
				],
				[
					5.927644360503706,
					-4.881576954485778
				],
				[
					-1.7434279416304084,
					-1.046040803418721
				],
				[
					-4.184216418873297,
					2.092134812035856
				],
				[
					-5.927644360503706,
					5.578990695296673
				],
				[
					-5.927644360503706,
					9.06584657855749
				],
				[
					-4.184216418873297,
					10.111887381976212
				],
				[
					-1.7434279416304084,
					10.809274520187898
				],
				[
					1.0460674060179278,
					10.809274520187898
				],
				[
					4.184216418873297,
					10.809274520187898
				],
				[
					9.065846578557489,
					10.460567649782451
				],
				[
					10.111860779377002,
					10.460567649782451
				],
				[
					10.460567649782451,
					10.460567649782451
				],
				[
					10.460567649782451,
					11.15795478799414
				],
				[
					10.460567649782451,
					11.15795478799414
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.1943359375,
				0.27734375,
				0.2900390625,
				0.3154296875,
				0.3544921875,
				0.37890625,
				0.3837890625,
				0.39453125,
				0.3798828125,
				0.373046875,
				0.345703125,
				0.388671875,
				0.431640625,
				0.4619140625,
				0.466796875,
				0.474609375,
				0.478515625,
				0.482421875,
				0.4951171875,
				0.4970703125,
				0.4970703125,
				0.302734375,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 560,
			"versionNonce": 393804658,
			"isDeleted": false,
			"id": "iNq35oCcxK0VkMF-5t49H",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1224.1596285414867,
			"y": 975.446070979501,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 2.0920816068374415,
			"height": 20.57242842915945,
			"seed": 47720804,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862519,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.6973605356124805,
					-7.322392034327873
				],
				[
					0.6973605356124805,
					-11.506608453201169
				],
				[
					0.6973605356124805,
					-16.736892278092395
				],
				[
					0.6973605356124805,
					-19.52638762574073
				],
				[
					0.6973605356124805,
					-20.57242842915945
				],
				[
					0.6973605356124805,
					-19.17770735793449
				],
				[
					2.0920816068374415,
					-15.342144604268226
				],
				[
					2.0920816068374415,
					-15.342144604268226
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2412109375,
				0.4501953125,
				0.5029296875,
				0.509765625,
				0.509765625,
				0.51171875,
				0.4150390625,
				0.015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 566,
			"versionNonce": 1966877870,
			"isDeleted": false,
			"id": "nXCJ3rvGpw5RBS31kiVAh",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1236.7122777981065,
			"y": 961.1499671786514,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 7.322365431728667,
			"height": 17.434279416304083,
			"seed": 505268964,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862519,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-4.881576954485777,
					3.1381756154545766
				],
				[
					-4.881576954485777,
					4.8816035570849845
				],
				[
					-3.4868558832608167,
					7.322392034327874
				],
				[
					-1.7434279416304084,
					9.41452684636373
				],
				[
					0.3487068704054473,
					11.157954787994138
				],
				[
					2.0921348120358556,
					12.901382729624546
				],
				[
					2.4407884772428887,
					14.296103800849508
				],
				[
					0.3487068704054473,
					16.039531742479916
				],
				[
					-2.4407884772428887,
					17.085599148497842
				],
				[
					-3.83550954846785,
					17.434279416304083
				],
				[
					-4.184216418873297,
					17.434279416304083
				],
				[
					-3.83550954846785,
					17.085599148497842
				],
				[
					-1.3947210712249611,
					16.388238612885363
				],
				[
					-1.3947210712249611,
					16.388238612885363
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2431640625,
				0.4150390625,
				0.45703125,
				0.4560546875,
				0.4462890625,
				0.4443359375,
				0.4443359375,
				0.4443359375,
				0.453125,
				0.4736328125,
				0.482421875,
				0.4638671875,
				0.314453125,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 568,
			"versionNonce": 762101042,
			"isDeleted": false,
			"id": "Uu192M0NjXyL_vNOD-dSq",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1246.126778041871,
			"y": 974.4000301760823,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 13.947423533043267,
			"height": 10.80924791758869,
			"seed": 1094297316,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862519,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					2.7894953476483364,
					-1.7434279416304084
				],
				[
					5.230283824891226,
					-4.8816035570849845
				],
				[
					5.230283824891226,
					-5.927670963102913
				],
				[
					3.835562753666264,
					-8.019779172539561
				],
				[
					2.0921348120358556,
					-7.671098904733321
				],
				[
					0,
					-5.578964092697466
				],
				[
					-1.046014200819514,
					-3.1381756154545766
				],
				[
					-1.3947210712249611,
					-0.6973871382116875
				],
				[
					-0.6973605356124806,
					1.0460408034187207
				],
				[
					1.394774276423375,
					2.4407884772428887
				],
				[
					3.4868558832608167,
					2.7894687450491293
				],
				[
					4.184269624071711,
					2.7894687450491293
				],
				[
					6.276351230909153,
					2.7894687450491293
				],
				[
					8.717139708152041,
					2.7894687450491293
				],
				[
					12.552702461818306,
					2.4407884772428887
				],
				[
					12.552702461818306,
					2.4407884772428887
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.181640625,
				0.2197265625,
				0.3369140625,
				0.357421875,
				0.384765625,
				0.3916015625,
				0.4267578125,
				0.46875,
				0.4931640625,
				0.5068359375,
				0.5126953125,
				0.51953125,
				0.5146484375,
				0.4921875,
				0.3818359375,
				0.0146484375,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 568,
			"versionNonce": 984508142,
			"isDeleted": false,
			"id": "AAvnByissBgwRdor5U57_",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1252.7518361431855,
			"y": 1005.4331060628217,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 17.08562575109705,
			"height": 16.388212010286157,
			"seed": 1758430820,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862519,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-1.7434279416304084,
					-0.34868026780624034
				],
				[
					-4.881630159684192,
					0.34868026780624034
				],
				[
					-7.671125507332528,
					1.3947476738241682
				],
				[
					-10.460567649782451,
					3.138175615454577
				],
				[
					-13.250062997430787,
					6.276324628309947
				],
				[
					-15.690851474673675,
					9.414500243764524
				],
				[
					-17.08562575109705,
					12.20399559141286
				],
				[
					-15.342197809466642,
					14.644784068655749
				],
				[
					-12.901409332223754,
					15.690851474673677
				],
				[
					-10.460567649782451,
					16.039531742479916
				],
				[
					-6.9737117665216335,
					15.342171206867437
				],
				[
					-4.881630159684192,
					14.99346433646199
				],
				[
					-4.184269624071711,
					14.99346433646199
				],
				[
					-2.7894953476483364,
					14.644784068655749
				],
				[
					-1.7434279416304084,
					14.644784068655749
				],
				[
					-1.7434279416304084,
					14.644784068655749
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.1875,
				0.2548828125,
				0.322265625,
				0.380859375,
				0.435546875,
				0.4833984375,
				0.50390625,
				0.5185546875,
				0.5205078125,
				0.5205078125,
				0.5205078125,
				0.5205078125,
				0.517578125,
				0.5087890625,
				0.4052734375,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 572,
			"versionNonce": 1526875890,
			"isDeleted": false,
			"id": "O5CYWcz-FmPj3dz72fVy6",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1260.4229084453198,
			"y": 1007.8738945400646,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 16.388212010286157,
			"height": 12.203995591412859,
			"seed": 2029385188,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862519,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-3.138202218053784,
					2.440815079842096
				],
				[
					-4.532923289278745,
					5.230283824891226
				],
				[
					-5.578990695296673,
					8.368459440345802
				],
				[
					-5.578990695296673,
					10.80924791758869
				],
				[
					-4.8816301596841924,
					11.855315323606618
				],
				[
					-4.184216418873298,
					12.203995591412859
				],
				[
					-1.046067406017928,
					11.506635055800379
				],
				[
					1.3947210712249614,
					10.11188738197621
				],
				[
					3.13814901285537,
					8.019779172539561
				],
				[
					3.8355095484678503,
					4.8816035570849845
				],
				[
					3.8355095484678503,
					3.1381756154545766
				],
				[
					3.486855883260817,
					4.184243021472504
				],
				[
					3.8355095484678503,
					6.276351230909153
				],
				[
					4.532923289278745,
					8.019779172539561
				],
				[
					6.625004896116187,
					10.11188738197621
				],
				[
					6.973711766521634,
					10.80924791758869
				],
				[
					8.019779172539563,
					11.855315323606618
				],
				[
					8.717139708152043,
					12.203995591412859
				],
				[
					10.809221314989484,
					11.506635055800379
				],
				[
					10.809221314989484,
					11.506635055800379
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.1943359375,
				0.2373046875,
				0.30078125,
				0.3740234375,
				0.404296875,
				0.4248046875,
				0.4248046875,
				0.443359375,
				0.4462890625,
				0.431640625,
				0.4345703125,
				0.453125,
				0.5166015625,
				0.5224609375,
				0.53125,
				0.5361328125,
				0.5322265625,
				0.486328125,
				0.365234375,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 568,
			"versionNonce": 39803182,
			"isDeleted": false,
			"id": "0bJcq9nT3VFGlOCYlNc69",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1271.5808366307147,
			"y": 1008.2225748078708,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 15.342144604268228,
			"height": 13.250036394831579,
			"seed": 743435364,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862519,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					3.835562753666264
				],
				[
					0.6973605356124806,
					7.671098904733321
				],
				[
					0.6973605356124806,
					8.717139708152041
				],
				[
					1.7434279416304084,
					10.11188738197621
				],
				[
					2.0921348120358556,
					10.460567649782451
				],
				[
					2.7894953476483364,
					9.41452684636373
				],
				[
					3.1381490128553695,
					7.671098904733321
				],
				[
					3.835562753666264,
					3.1381756154545766
				],
				[
					4.532923289278744,
					0.3487068704054473
				],
				[
					5.578990695296673,
					-1.3947210712249611
				],
				[
					7.322418636927081,
					-2.4407884772428887
				],
				[
					10.460567649782451,
					-2.7894687450491293
				],
				[
					12.552702461818306,
					-2.4407884772428887
				],
				[
					14.296130403448714,
					-2.0921082094366485
				],
				[
					15.342144604268228,
					-1.7434279416304084
				],
				[
					15.342144604268228,
					-1.7434279416304084
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2998046875,
				0.357421875,
				0.4267578125,
				0.4423828125,
				0.45703125,
				0.4755859375,
				0.4990234375,
				0.51953125,
				0.5390625,
				0.5458984375,
				0.5478515625,
				0.5498046875,
				0.55078125,
				0.5283203125,
				0.41796875,
				0.015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 569,
			"versionNonce": 1489017010,
			"isDeleted": false,
			"id": "k5n9_I0KTMT8ZMvOnlryf",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1290.0611834530366,
			"y": 1004.0383583889975,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 14.644837273854161,
			"height": 12.552675859219098,
			"seed": 552836068,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862519,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.6973605356124806,
					1.0460674060179278
				],
				[
					-1.0460674060179278,
					2.4407884772428887
				],
				[
					-1.394774276423375,
					4.8816035570849845
				],
				[
					-1.394774276423375,
					8.019779172539561
				],
				[
					-0.6973605356124806,
					11.506635055800379
				],
				[
					-0.3487068704054473,
					12.552675859219098
				],
				[
					0.3486536652070333,
					12.552675859219098
				],
				[
					1.0460674060179278,
					11.506635055800379
				],
				[
					2.0920816068374415,
					9.414500243764522
				],
				[
					3.1381490128553695,
					4.8816035570849845
				],
				[
					3.83550954846785,
					2.4407884772428887
				],
				[
					5.230283824891226,
					0.6973605356124806
				],
				[
					7.322365431728667,
					0
				],
				[
					10.460567649782451,
					0
				],
				[
					11.855288721007412,
					0.6973605356124806
				],
				[
					13.250062997430787,
					1.7434279416304084
				],
				[
					13.250062997430787,
					1.7434279416304084
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2021484375,
				0.2939453125,
				0.365234375,
				0.4013671875,
				0.41796875,
				0.4521484375,
				0.4736328125,
				0.4921875,
				0.5078125,
				0.5224609375,
				0.5419921875,
				0.5478515625,
				0.5478515625,
				0.5537109375,
				0.5537109375,
				0.552734375,
				0.5048828125,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 560,
			"versionNonce": 62391150,
			"isDeleted": false,
			"id": "QqudcIJ2b1mimj9tMI9cr",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1308.192823404953,
			"y": 1010.663389887713,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 14.993490939061195,
			"height": 1.7434279416304084,
			"seed": 516619484,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862519,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					5.230283824891226,
					-0.6973871382116875
				],
				[
					6.276351230909153,
					-0.6973871382116875
				],
				[
					11.157928185394931,
					-1.7434279416304084
				],
				[
					13.250062997430787,
					-1.7434279416304084
				],
				[
					14.644784068655747,
					-1.0460674060179278
				],
				[
					14.993490939061195,
					-1.0460674060179278
				],
				[
					13.59871666263782,
					-1.7434279416304084
				],
				[
					13.59871666263782,
					-1.7434279416304084
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.3994140625,
				0.509765625,
				0.5205078125,
				0.5615234375,
				0.564453125,
				0.537109375,
				0.5263671875,
				0.0146484375,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 560,
			"versionNonce": 911127154,
			"isDeleted": false,
			"id": "vOEE7pLdD20hU4F9nQpCp",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1312.3770398238264,
			"y": 1000.2028222379306,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 15.342197809466741,
			"height": 2.0921082094366485,
			"seed": 1099264860,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862519,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.6973605356124806,
					-0.3486802678062403
				],
				[
					2.7894953476483364,
					-0.6973871382116875
				],
				[
					5.927644360503706,
					-1.3947476738241682
				],
				[
					8.368486042945008,
					-1.3947476738241682
				],
				[
					10.809274520187898,
					-1.0460674060179278
				],
				[
					11.506635055800476,
					-1.0460674060179278
				],
				[
					15.342197809466741,
					0.6973605356124806
				],
				[
					15.342197809466741,
					0.6973605356124806
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.234375,
				0.4013671875,
				0.498046875,
				0.53125,
				0.5400390625,
				0.533203125,
				0.5302734375,
				0.015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 560,
			"versionNonce": 553739694,
			"isDeleted": false,
			"id": "7fFoIn7SSDwh45yei6_Th",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1345.85087758521,
			"y": 1009.2686422138888,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 5.578937490098259,
			"height": 20.57245503175866,
			"seed": 543545820,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862519,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.6973605356124806,
					-1.7434279416304084
				],
				[
					1.0460674060179278,
					-4.184216418873297
				],
				[
					1.3947210712249611,
					-5.578964092697466
				],
				[
					2.0920816068374415,
					-10.11188738197621
				],
				[
					1.7434279416304084,
					-11.855315323606618
				],
				[
					1.7434279416304084,
					-12.90135612702534
				],
				[
					-3.4868558832608167,
					-20.57245503175866
				],
				[
					-3.4868558832608167,
					-20.57245503175866
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.294921875,
				0.359375,
				0.498046875,
				0.5244140625,
				0.564453125,
				0.5615234375,
				0.5615234375,
				0.0166015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 562,
			"versionNonce": 1987286066,
			"isDeleted": false,
			"id": "y3xKQnzD6_7iA5p7xSG65",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1333.2981751233913,
			"y": 989.0448674499364,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 26.151419124456126,
			"height": 2.7894953476483364,
			"seed": 901132380,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862519,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1.0460674060179278,
					0.6973871382116876
				],
				[
					1.7434279416304084,
					1.046067406017928
				],
				[
					4.532923289278744,
					1.046067406017928
				],
				[
					9.763207114169969,
					0.6973871382116876
				],
				[
					14.296130403448714,
					1.046067406017928
				],
				[
					16.388212010286157,
					1.046067406017928
				],
				[
					19.526414228339938,
					2.092134812035856
				],
				[
					21.967202705582828,
					2.7894953476483364
				],
				[
					26.151419124456126,
					2.7894953476483364
				],
				[
					26.151419124456126,
					2.7894953476483364
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.212890625,
				0.3564453125,
				0.42578125,
				0.5009765625,
				0.5224609375,
				0.525390625,
				0.525390625,
				0.466796875,
				0.2138671875,
				0.0126953125,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 566,
			"versionNonce": 191135726,
			"isDeleted": false,
			"id": "TIQ9PdT9Fw5CeAj9sDpYm",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1353.8706567577494,
			"y": 996.7159663546697,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 14.644784068655747,
			"height": 11.157928185394931,
			"seed": 1283799900,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862519,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1.3947210712249611,
					5.927644360503706
				],
				[
					2.0920816068374415,
					8.368459440345802
				],
				[
					2.7894421424499223,
					10.460567649782451
				],
				[
					3.4868558832608167,
					11.157928185394931
				],
				[
					3.83550954846785,
					10.80924791758869
				],
				[
					5.578937490098259,
					8.019752569940355
				],
				[
					6.9737117665216335,
					5.578964092697466
				],
				[
					8.717139708152041,
					2.7894687450491293
				],
				[
					10.111860779377002,
					1.3947476738241682
				],
				[
					10.809221314989484,
					1.3947476738241682
				],
				[
					11.855288721007412,
					1.7434279416304084
				],
				[
					12.90135612702534,
					2.4407884772428887
				],
				[
					14.644784068655747,
					3.4868558832608167
				],
				[
					14.644784068655747,
					3.4868558832608167
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2509765625,
				0.3310546875,
				0.369140625,
				0.376953125,
				0.4287109375,
				0.4794921875,
				0.5234375,
				0.5283203125,
				0.5390625,
				0.5390625,
				0.537109375,
				0.5244140625,
				0.4326171875,
				0.015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 578,
			"versionNonce": 722877938,
			"isDeleted": false,
			"id": "D4x_92Yns00Z_YHDEIs4Y",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1369.212801362017,
			"y": 1001.2488630413493,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 36.611986774238574,
			"height": 10.80924791758869,
			"seed": 1833901916,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862519,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					3.835562753666264
				],
				[
					1.3947210712249611,
					4.8816035570849845
				],
				[
					3.835562753666264,
					4.8816035570849845
				],
				[
					7.322418636927081,
					2.7894953476483364
				],
				[
					8.368432837746594,
					0.3487068704054473
				],
				[
					8.717139708152041,
					-2.0921082094366485
				],
				[
					9.065846578557489,
					-3.835536151067057
				],
				[
					9.763207114169969,
					-3.4868558832608167
				],
				[
					10.809274520187898,
					-1.7434279416304084
				],
				[
					12.203995591412859,
					0
				],
				[
					14.644784068655747,
					1.0460674060179278
				],
				[
					17.085572545898636,
					0.3487068704054473
				],
				[
					19.526414228339938,
					-1.0460408034187207
				],
				[
					21.26984216997035,
					-2.7894687450491293
				],
				[
					20.57242842915945,
					-4.881576954485777
				],
				[
					18.480346822322012,
					-4.184216418873297
				],
				[
					16.388212010286157,
					-2.4407884772428887
				],
				[
					15.690851474673675,
					-0.3486802678062403
				],
				[
					16.388212010286157,
					1.0460674060179278
				],
				[
					19.526414228339938,
					2.440815079842096
				],
				[
					24.756698053231165,
					3.1381756154545766
				],
				[
					28.24355393649198,
					3.4868558832608167
				],
				[
					31.38170294934735,
					4.184243021472504
				],
				[
					34.51985196220272,
					5.230283824891226
				],
				[
					36.611986774238574,
					5.927670963102913
				],
				[
					36.611986774238574,
					5.927670963102913
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2548828125,
				0.3818359375,
				0.4462890625,
				0.4814453125,
				0.4970703125,
				0.517578125,
				0.546875,
				0.564453125,
				0.5458984375,
				0.46875,
				0.275390625,
				0.013671875,
				0.2177734375,
				0.3994140625,
				0.45703125,
				0.4794921875,
				0.4794921875,
				0.4853515625,
				0.517578125,
				0.5478515625,
				0.5810546875,
				0.5947265625,
				0.5966796875,
				0.5556640625,
				0.4306640625,
				0.015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 560,
			"versionNonce": 1726632494,
			"isDeleted": false,
			"id": "ZGxnf31Tc0SIOUKpW5yYH",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1300.521751102819,
			"y": 1003.6896781211913,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 6.276351230909153,
			"height": 11.50660845320117,
			"seed": 1732890204,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862519,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.6973605356124806,
					2.0921082094366485
				],
				[
					1.0460674060179278,
					2.7894687450491293
				],
				[
					1.3947210712249611,
					4.532896686679537
				],
				[
					3.4868558832608167,
					8.368459440345802
				],
				[
					4.532923289278744,
					10.460567649782451
				],
				[
					5.927644360503706,
					11.50660845320117
				],
				[
					6.276351230909153,
					10.11188738197621
				],
				[
					6.276351230909153,
					10.11188738197621
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.353515625,
				0.478515625,
				0.4892578125,
				0.5166015625,
				0.5380859375,
				0.5400390625,
				0.470703125,
				0.0166015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 560,
			"versionNonce": 289255346,
			"isDeleted": false,
			"id": "17Ow56NhzDmr5ndh0k3LM",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1305.054674392098,
			"y": 1005.0844257950155,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 11.506635055800379,
			"height": 34.51985196220272,
			"seed": 957437148,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862519,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.3487068704054473,
					1.7434279416304084
				],
				[
					-1.394774276423375,
					5.578964092697466
				],
				[
					-2.7894953476483364,
					9.414500243764522
				],
				[
					-5.230283824891226,
					15.690851474673675
				],
				[
					-7.322418636927081,
					21.967176102983622
				],
				[
					-9.065846578557489,
					27.197459927874846
				],
				[
					-11.506635055800379,
					34.51985196220272
				],
				[
					-11.506635055800379,
					34.51985196220272
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.4052734375,
				0.494140625,
				0.541015625,
				0.5615234375,
				0.580078125,
				0.5732421875,
				0.4970703125,
				0.0166015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 569,
			"versionNonce": 1853611118,
			"isDeleted": false,
			"id": "oCLRt05gihr1PwVtAHPmI",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1252.0544224023747,
			"y": 1068.8938724971292,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 18.480293617123596,
			"height": 22.315909575988275,
			"seed": 1825885020,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862519,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-8.019725967341147,
					2.7894953476483364
				],
				[
					-11.15792818539493,
					4.184243021472504
				],
				[
					-13.25000979223237,
					5.578964092697466
				],
				[
					-13.25000979223237,
					8.019779172539561
				],
				[
					-11.506581850601963,
					9.763207114169969
				],
				[
					-9.065793373359075,
					10.80924791758869
				],
				[
					-6.276298025710738,
					11.855315323606618
				],
				[
					-4.184216418873297,
					12.901382729624546
				],
				[
					-2.4407884772428887,
					14.644810671254955
				],
				[
					-3.4868558832608163,
					16.388238612885363
				],
				[
					-5.927644360503705,
					18.480346822322012
				],
				[
					-8.717139708152041,
					20.22377476395242
				],
				[
					-13.947423533043265,
					21.967202705582828
				],
				[
					-17.085572545898636,
					22.315909575988275
				],
				[
					-18.480293617123596,
					22.315909575988275
				],
				[
					-12.901356127025338,
					22.315909575988275
				],
				[
					-12.901356127025338,
					22.315909575988275
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.1494140625,
				0.267578125,
				0.3564453125,
				0.451171875,
				0.4931640625,
				0.4951171875,
				0.4951171875,
				0.4951171875,
				0.4951171875,
				0.4951171875,
				0.5029296875,
				0.5283203125,
				0.552734375,
				0.57421875,
				0.5791015625,
				0.572265625,
				0.0166015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 565,
			"versionNonce": 756083058,
			"isDeleted": false,
			"id": "-ntdtE5-S2UnCqYqLS-cD",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1255.889985156041,
			"y": 1079.7031204147181,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 9.065846578557489,
			"height": 10.111860779377002,
			"seed": 106256356,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862519,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.3487068704054473,
					3.138175615454576
				],
				[
					0.6973605356124806,
					5.578990695296672
				],
				[
					1.3947210712249611,
					6.973711766521633
				],
				[
					2.0921348120358556,
					6.973711766521633
				],
				[
					3.1381490128553695,
					5.230283824891225
				],
				[
					4.184216418873297,
					2.789495347648336
				],
				[
					4.881576954485777,
					0.34870687040544723
				],
				[
					5.578990695296673,
					-2.0921082094366485
				],
				[
					5.578990695296673,
					-2.789468745049129
				],
				[
					5.578990695296673,
					-3.138149012855369
				],
				[
					6.625004896116186,
					-3.138149012855369
				],
				[
					9.065846578557489,
					-1.7434279416304082
				],
				[
					9.065846578557489,
					-1.7434279416304082
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2705078125,
				0.33203125,
				0.380859375,
				0.4345703125,
				0.4716796875,
				0.5029296875,
				0.51953125,
				0.5244140625,
				0.5361328125,
				0.5380859375,
				0.5380859375,
				0.4169921875,
				0.015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 568,
			"versionNonce": 400694958,
			"isDeleted": false,
			"id": "RZbEf78GID4l4SMFxWaC2",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1269.1400481534718,
			"y": 1081.7952552267536,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 11.157928185394931,
			"height": 13.947423533043267,
			"seed": 1064421340,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862519,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.3487068704054473,
					-1.7434279416304084
				],
				[
					0.3486536652070333,
					-3.835562753666264
				],
				[
					1.3947210712249611,
					-5.578990695296673
				],
				[
					2.4407884772428887,
					-6.625031498715393
				],
				[
					3.1381490128553695,
					-6.625031498715393
				],
				[
					3.83550954846785,
					-6.276351230909153
				],
				[
					4.881576954485777,
					-5.578990695296673
				],
				[
					6.625004896116186,
					-5.230283824891226
				],
				[
					8.368432837746594,
					-5.578990695296673
				],
				[
					8.717139708152041,
					-5.230283824891226
				],
				[
					8.717139708152041,
					-3.1381756154545766
				],
				[
					7.671072302134114,
					-0.3487068704054473
				],
				[
					7.671072302134114,
					2.4407884772428887
				],
				[
					8.717139708152041,
					5.230283824891226
				],
				[
					10.809221314989484,
					7.322392034327874
				],
				[
					10.809221314989484,
					7.322392034327874
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.318359375,
				0.4345703125,
				0.4970703125,
				0.5166015625,
				0.513671875,
				0.51171875,
				0.51171875,
				0.5205078125,
				0.5234375,
				0.53515625,
				0.5400390625,
				0.5400390625,
				0.54296875,
				0.5400390625,
				0.4228515625,
				0.015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 566,
			"versionNonce": 1708583730,
			"isDeleted": false,
			"id": "ZE-7O_x7ozoxhNlhnR4My",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1289.3638229174242,
			"y": 1076.9136516696688,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 17.78298628670953,
			"height": 1.0460674060179278,
			"seed": 267210844,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862519,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-1.7434279416304084,
					-0.3486802678062403
				],
				[
					-2.440841682441303,
					-0.6973871382116875
				],
				[
					-2.0921348120358556,
					-0.6973871382116875
				],
				[
					-1.394774276423375,
					-1.0460674060179278
				],
				[
					0.6973605356124806,
					-1.0460674060179278
				],
				[
					3.1381490128553695,
					-0.6973871382116875
				],
				[
					6.625004896116186,
					-0.6973871382116875
				],
				[
					10.111860779377002,
					-0.6973871382116875
				],
				[
					13.250009792232373,
					-1.0460674060179278
				],
				[
					13.947423533043267,
					-0.6973871382116875
				],
				[
					14.644784068655747,
					-0.6973871382116875
				],
				[
					14.99343773386278,
					-0.6973871382116875
				],
				[
					15.342144604268228,
					-0.6973871382116875
				],
				[
					15.342144604268228,
					-0.6973871382116875
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2060546875,
				0.3037109375,
				0.4375,
				0.5078125,
				0.5234375,
				0.537109375,
				0.5517578125,
				0.564453125,
				0.5703125,
				0.572265625,
				0.572265625,
				0.529296875,
				0.513671875,
				0.3076171875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 562,
			"versionNonce": 935729390,
			"isDeleted": false,
			"id": "PxFKrI_lGXtfFvPstbip1",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1301.567818508837,
			"y": 1080.0518272851234,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 16.73686567549319,
			"height": 3.4868558832608167,
			"seed": 1737634908,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862519,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.3486536652070333,
					0
				],
				[
					2.4407884772428887,
					0
				],
				[
					6.276298025710739,
					-0.6973871382116875
				],
				[
					9.763153908971555,
					-1.7434279416304084
				],
				[
					13.59871666263782,
					-2.440815079842096
				],
				[
					14.99343773386278,
					-2.7894953476483364
				],
				[
					15.690851474673675,
					-2.7894953476483364
				],
				[
					16.388212010286157,
					-3.1381756154545766
				],
				[
					16.73686567549319,
					-3.4868558832608167
				],
				[
					16.73686567549319,
					-3.4868558832608167
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.171875,
				0.48046875,
				0.5126953125,
				0.5224609375,
				0.52734375,
				0.529296875,
				0.5185546875,
				0.513671875,
				0.4052734375,
				0.0126953125,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 560,
			"versionNonce": 569816306,
			"isDeleted": false,
			"id": "IF51cWU1hGdH5zkOUaoSf",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1302.2651790444495,
			"y": 1068.545192229323,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 15.690851474673675,
			"height": 1.0460674060179278,
			"seed": 311312220,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862519,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.6973605356124806,
					0
				],
				[
					1.7434279416304084,
					-0.3486802678062403
				],
				[
					4.184216418873297,
					-0.6973605356124806
				],
				[
					7.322365431728667,
					-1.0460674060179278
				],
				[
					11.157928185394931,
					-1.0460674060179278
				],
				[
					13.947423533043267,
					-1.0460674060179278
				],
				[
					15.690851474673675,
					-1.0460674060179278
				],
				[
					15.690851474673675,
					-1.0460674060179278
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.3876953125,
				0.505859375,
				0.51953125,
				0.5419921875,
				0.546875,
				0.546875,
				0.4833984375,
				0.0166015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 561,
			"versionNonce": 632343342,
			"isDeleted": false,
			"id": "lT2U6YIDS8Oq7G1OtpQIy",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1334.6929493998148,
			"y": 1077.262331937475,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 2.0920816068374415,
			"height": 16.039531742479916,
			"seed": 913253852,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862519,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					-2.7894953476483364
				],
				[
					0,
					-6.9737117665216335
				],
				[
					-0.34870687040544723,
					-10.11188738197621
				],
				[
					-0.6974137408108945,
					-12.203995591412859
				],
				[
					-1.0460674060179278,
					-14.296103800849508
				],
				[
					-1.0460674060179278,
					-15.342171206867436
				],
				[
					-0.6974137408108945,
					-16.039531742479916
				],
				[
					1.0460142008195137,
					-15.690851474673675
				],
				[
					1.0460142008195137,
					-15.690851474673675
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2431640625,
				0.431640625,
				0.5361328125,
				0.5517578125,
				0.5537109375,
				0.544921875,
				0.4990234375,
				0.234375,
				0.0126953125,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 569,
			"versionNonce": 1660372658,
			"isDeleted": false,
			"id": "-BsudM_GD8qOqob48DeYb",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1315.4180050401023,
			"y": 1057.826447015326,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 19.17770735793449,
			"height": 13.947423533043267,
			"seed": 467765092,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862519,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					3.1381756154545766
				],
				[
					0.34870687040544723,
					4.184243021472504
				],
				[
					2.0921348120358556,
					5.927670963102913
				],
				[
					5.230283824891225,
					6.276351230909153
				],
				[
					8.717139708152041,
					5.230283824891226
				],
				[
					12.552702461818305,
					2.7894953476483364
				],
				[
					16.7369188806916,
					0
				],
				[
					19.17770735793449,
					-3.1381756154545766
				],
				[
					17.434279416304083,
					-5.230283824891226
				],
				[
					13.598716662637818,
					-6.9737117665216335
				],
				[
					10.111860779377002,
					-7.671072302134114
				],
				[
					7.32241863692708,
					-6.9737117665216335
				],
				[
					6.973711766521633,
					-5.927644360503706
				],
				[
					9.763207114169969,
					-4.184216418873297
				],
				[
					9.763207114169969,
					-4.184216418873297
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2626953125,
				0.3134765625,
				0.3662109375,
				0.4443359375,
				0.4873046875,
				0.4970703125,
				0.4990234375,
				0.5087890625,
				0.52734375,
				0.5458984375,
				0.5732421875,
				0.587890625,
				0.59765625,
				0.55859375,
				0.0126953125,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 752,
			"versionNonce": 1611347310,
			"isDeleted": false,
			"id": "J4v0hwHZ2MB1d__7XoPnW",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1234.968849856476,
			"y": 1119.1045892353056,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 14.296130403448714,
			"height": 24.059310915019477,
			"seed": 340359268,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862519,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					0.6973605356124806
				],
				[
					0,
					2.0921082094366485
				],
				[
					0,
					5.578964092697466
				],
				[
					-0.3487068704054473,
					7.671072302134114
				],
				[
					0,
					13.250036394831579
				],
				[
					0.3486536652070333,
					16.388212010286157
				],
				[
					0.3486536652070333,
					19.17770735793449
				],
				[
					0.3486536652070333,
					21.26981556737114
				],
				[
					0,
					21.967176102983622
				],
				[
					-0.3487068704054473,
					22.31588297338907
				],
				[
					1.7434279416304084,
					21.61849583517738
				],
				[
					5.230283824891226,
					21.61849583517738
				],
				[
					9.763207114169969,
					21.967176102983622
				],
				[
					11.855288721007412,
					22.31588297338907
				],
				[
					12.90135612702534,
					22.66456324119531
				],
				[
					13.59871666263782,
					23.013243509001548
				],
				[
					13.947423533043267,
					24.059310915019477
				],
				[
					13.947423533043267,
					24.059310915019477
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2158203125,
				0.283203125,
				0.306640625,
				0.3359375,
				0.357421875,
				0.384765625,
				0.392578125,
				0.40234375,
				0.43359375,
				0.4619140625,
				0.4833984375,
				0.5,
				0.5,
				0.5,
				0.5,
				0.501953125,
				0.48046875,
				0.03125,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 753,
			"versionNonce": 1635754098,
			"isDeleted": false,
			"id": "2miSho-5Qoa2f0WKsrR46",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1251.0083549963567,
			"y": 1118.4072020970941,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 9.763207114169969,
			"height": 23.361950379406995,
			"seed": 2093272036,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862519,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.34870687040544723,
					2.440815079842096
				],
				[
					0.34870687040544723,
					6.276351230909153
				],
				[
					0.34870687040544723,
					10.11188738197621
				],
				[
					0,
					14.993490939061195
				],
				[
					-0.3486536652070332,
					17.78298628670953
				],
				[
					-0.3486536652070332,
					19.87509449614618
				],
				[
					-0.6973605356124805,
					21.26984216997035
				],
				[
					-0.6973605356124805,
					21.967202705582828
				],
				[
					-0.3486536652070332,
					23.013270111600757
				],
				[
					1.0460674060179278,
					23.361950379406995
				],
				[
					3.4868558832608163,
					23.013270111600757
				],
				[
					5.927697565702119,
					22.31588297338907
				],
				[
					7.671125507332527,
					21.967202705582828
				],
				[
					8.717139708152041,
					21.618522437776587
				],
				[
					9.065846578557489,
					21.618522437776587
				],
				[
					9.065846578557489,
					21.967202705582828
				],
				[
					9.065846578557489,
					22.66456324119531
				],
				[
					9.065846578557489,
					23.361950379406995
				],
				[
					9.065846578557489,
					23.361950379406995
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2880859375,
				0.39453125,
				0.416015625,
				0.4248046875,
				0.4345703125,
				0.458984375,
				0.4794921875,
				0.4921875,
				0.4970703125,
				0.5048828125,
				0.51171875,
				0.5185546875,
				0.521484375,
				0.521484375,
				0.525390625,
				0.5224609375,
				0.5224609375,
				0.2333984375,
				0.0556640625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 752,
			"versionNonce": 807294894,
			"isDeleted": false,
			"id": "J-luqsODgvU52ilRi7MZd",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1276.1137599199933,
			"y": 1127.124341805246,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 14.296130403448714,
			"height": 14.644810671254955,
			"seed": 1904848740,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862519,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-5.230283824891226,
					0.3487068704054473
				],
				[
					-8.019779172539561,
					1.3947476738241682
				],
				[
					-9.763207114169969,
					3.1381756154545766
				],
				[
					-10.111913984575416,
					4.184243021472504
				],
				[
					-8.368486042945008,
					5.927670963102913
				],
				[
					-4.532923289278744,
					7.322418636927081
				],
				[
					-1.394774276423375,
					8.717139708152041
				],
				[
					1.046014200819514,
					9.763207114169969
				],
				[
					2.4407884772428887,
					10.809274520187898
				],
				[
					2.4407884772428887,
					11.506635055800379
				],
				[
					1.046014200819514,
					12.901382729624546
				],
				[
					-2.0921348120358556,
					13.598743265237026
				],
				[
					-5.92769756570212,
					13.947423533043267
				],
				[
					-9.065846578557489,
					13.947423533043267
				],
				[
					-10.809274520187898,
					14.296130403448714
				],
				[
					-11.855341926205826,
					14.644810671254955
				],
				[
					-8.368486042945008,
					14.296130403448714
				],
				[
					-8.368486042945008,
					14.296130403448714
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.1923828125,
				0.302734375,
				0.408203125,
				0.4794921875,
				0.4921875,
				0.494140625,
				0.494140625,
				0.4921875,
				0.486328125,
				0.4912109375,
				0.4931640625,
				0.4990234375,
				0.5166015625,
				0.53515625,
				0.5576171875,
				0.55859375,
				0.466796875,
				0.0166015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 752,
			"versionNonce": 693551666,
			"isDeleted": false,
			"id": "MveoHEgS1YpQ3gGLKUunK",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1284.1334858873345,
			"y": 1135.1441209777856,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 9.065846578557489,
			"height": 8.717139708152041,
			"seed": 1390813924,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862519,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-2.7894421424499223,
					2.4407884772428887
				],
				[
					-3.1381490128553695,
					3.1381756154545766
				],
				[
					-3.1381490128553695,
					3.835536151067057
				],
				[
					-0.6973605356124806,
					4.8816035570849845
				],
				[
					1.7434279416304084,
					4.184216418873297
				],
				[
					4.184269624071711,
					3.4868558832608167
				],
				[
					5.578990695296673,
					1.7434279416304084
				],
				[
					5.92769756570212,
					0.3486802678062403
				],
				[
					4.881630159684192,
					-1.3947476738241682
				],
				[
					3.4868558832608167,
					-2.7894953476483364
				],
				[
					1.394774276423375,
					-3.4868558832608167
				],
				[
					-0.3486536652070333,
					-3.835536151067057
				],
				[
					-1.3947210712249611,
					-3.835536151067057
				],
				[
					-1.7434279416304084,
					-3.1381756154545766
				],
				[
					-1.3947210712249611,
					-2.4407884772428887
				],
				[
					1.394774276423375,
					-1.0460674060179278
				],
				[
					0,
					0
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2900390625,
				0.3955078125,
				0.4365234375,
				0.4775390625,
				0.482421875,
				0.482421875,
				0.4658203125,
				0.447265625,
				0.4501953125,
				0.4716796875,
				0.4873046875,
				0.4990234375,
				0.5078125,
				0.5078125,
				0.4990234375,
				0.40625,
				0.015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 743,
			"versionNonce": 1309880814,
			"isDeleted": false,
			"id": "2wFcWsOn0RykN9geoVY3q",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1294.9427604075224,
			"y": 1140.0257245348705,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 3.1381490128553695,
			"height": 23.361950379406995,
			"seed": 1198007908,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862519,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.3487068704054473,
					-5.927670963102913
				],
				[
					-0.3487068704054473,
					-7.671098904733321
				],
				[
					-0.3487068704054473,
					-9.763207114169969
				],
				[
					-0.6973605356124806,
					-13.947423533043267
				],
				[
					-0.6973605356124806,
					-16.388238612885363
				],
				[
					-1.3947210712249611,
					-20.921135299564902
				],
				[
					-2.4407884772428887,
					-22.66456324119531
				],
				[
					-3.1381490128553695,
					-23.361950379406995
				],
				[
					-3.1381490128553695,
					-23.361950379406995
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.30859375,
				0.4970703125,
				0.5302734375,
				0.5537109375,
				0.5712890625,
				0.5712890625,
				0.5263671875,
				0.3544921875,
				0.0146484375,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 739,
			"versionNonce": 895724530,
			"isDeleted": false,
			"id": "smkHn84Laetk4_YxKKnWW",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1305.0546211868993,
			"y": 1131.3085848267185,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 2.0921348120358556,
			"height": 0.6973871382116875,
			"seed": 1943910884,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862519,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-1.046014200819514,
					-0.3486802678062403
				],
				[
					-1.3947210712249611,
					-0.3486802678062403
				],
				[
					0.6974137408108946,
					-0.6973871382116875
				],
				[
					0,
					0
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.421875,
				0.4970703125,
				0.4970703125,
				0.0166015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 749,
			"versionNonce": 83018798,
			"isDeleted": false,
			"id": "Jq3IQmVwyAGgGsrGMlqQB",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1309.9362513465835,
			"y": 1131.3085848267185,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 11.506635055800379,
			"height": 11.157928185394931,
			"seed": 861199716,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862519,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					3.835536151067057
				],
				[
					0,
					4.184216418873297
				],
				[
					0,
					4.532896686679537
				],
				[
					0.6973605356124806,
					2.7894687450491293
				],
				[
					1.7434279416304084,
					0
				],
				[
					2.7894953476483364,
					-2.7894953476483364
				],
				[
					4.184216418873297,
					-4.8816035570849845
				],
				[
					5.927644360503706,
					-6.625031498715393
				],
				[
					8.019779172539561,
					-6.625031498715393
				],
				[
					10.809221314989484,
					-3.835536151067057
				],
				[
					11.157928185394931,
					-3.1381756154545766
				],
				[
					10.809221314989484,
					0
				],
				[
					10.111860779377002,
					1.7434279416304084
				],
				[
					11.506635055800379,
					2.4407884772428887
				],
				[
					11.506635055800379,
					2.4407884772428887
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.1611328125,
				0.2314453125,
				0.279296875,
				0.294921875,
				0.4287109375,
				0.46484375,
				0.4775390625,
				0.482421875,
				0.490234375,
				0.49609375,
				0.5146484375,
				0.517578125,
				0.5234375,
				0.525390625,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 750,
			"versionNonce": 195911090,
			"isDeleted": false,
			"id": "aX9JILEe3hBrgn3uy6bt5",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1331.2060403113553,
			"y": 1128.8677697468763,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 10.809221314989484,
			"height": 8.717139708152041,
			"seed": 1327206628,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862519,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					3.138202218053784,
					-1.7434279416304084
				],
				[
					3.8355627536662644,
					-2.4407884772428887
				],
				[
					3.486855883260817,
					-3.4868558832608167
				],
				[
					2.092134812035856,
					-4.184216418873297
				],
				[
					-1.3947210712249614,
					-3.835536151067057
				],
				[
					-3.486855883260817,
					-2.4407884772428887
				],
				[
					-4.881576954485778,
					-0.3486802678062403
				],
				[
					-5.578937490098259,
					1.3947476738241682
				],
				[
					-5.578937490098259,
					3.1381756154545766
				],
				[
					-4.881576954485778,
					3.835562753666264
				],
				[
					-3.486855883260817,
					4.184243021472504
				],
				[
					-1.3947210712249614,
					4.184243021472504
				],
				[
					2.7894953476483364,
					4.184243021472504
				],
				[
					5.230283824891226,
					4.532923289278744
				],
				[
					0,
					0
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2509765625,
				0.3134765625,
				0.34765625,
				0.3896484375,
				0.396484375,
				0.4326171875,
				0.482421875,
				0.50390625,
				0.525390625,
				0.5498046875,
				0.552734375,
				0.560546875,
				0.55859375,
				0.4111328125,
				0.015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 739,
			"versionNonce": 1453723246,
			"isDeleted": false,
			"id": "QbDWsnq5a0Oh5BIxWkZlj",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1338.8771658186881,
			"y": 1134.4467604421732,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 5.927644360503706,
			"height": 17.085599148497842,
			"seed": 918541412,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862519,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					2.4407884772428887,
					-5.230283824891225
				],
				[
					4.53287008408033,
					-8.019779172539561
				],
				[
					5.927644360503706,
					-11.855315323606616
				],
				[
					4.53287008408033,
					-17.085599148497842
				],
				[
					4.53287008408033,
					-17.085599148497842
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.302734375,
				0.4833984375,
				0.4970703125,
				0.412109375,
				0.015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 742,
			"versionNonce": 1499125618,
			"isDeleted": false,
			"id": "aGDx0mwXhYTsDGDQ8dPaf",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1340.6205937603183,
			"y": 1118.4072020970941,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 9.065793373359075,
			"height": 12.552702461818306,
			"seed": 940550116,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862519,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					4.532923289278744
				],
				[
					0.3486536652070332,
					6.276351230909153
				],
				[
					1.0460142008195137,
					7.671098904733321
				],
				[
					2.0920816068374415,
					9.41452684636373
				],
				[
					3.138149012855369,
					10.11188738197621
				],
				[
					5.230283824891225,
					11.506635055800379
				],
				[
					9.065793373359075,
					12.552702461818306
				],
				[
					9.065793373359075,
					12.552702461818306
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2509765625,
				0.37109375,
				0.4501953125,
				0.501953125,
				0.52734375,
				0.52734375,
				0.4853515625,
				0.0166015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 746,
			"versionNonce": 536219822,
			"isDeleted": false,
			"id": "J0MNkhIdQHr5JiCIEK7xR",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1355.2653778289744,
			"y": 1131.3085848267185,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 18.829000487529044,
			"height": 18.480346822322012,
			"seed": 924388196,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862519,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.6973605356124805,
					-3.1381756154545766
				],
				[
					-2.0921348120358556,
					-6.276351230909153
				],
				[
					-3.8355627536662635,
					-10.460567649782451
				],
				[
					-6.973711766521633,
					-16.388238612885363
				],
				[
					-6.6250581013145995,
					-17.434279416304083
				],
				[
					-5.578990695296672,
					-18.13166655451577
				],
				[
					-3.138202218053783,
					-18.480346822322012
				],
				[
					1.394721071224961,
					-18.13166655451577
				],
				[
					3.138149012855369,
					-17.782959684110324
				],
				[
					7.322365431728666,
					-17.085599148497842
				],
				[
					11.85528872100741,
					-16.039531742479916
				],
				[
					11.85528872100741,
					-16.039531742479916
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.4111328125,
				0.486328125,
				0.4970703125,
				0.4482421875,
				0.3251953125,
				0.4384765625,
				0.509765625,
				0.5361328125,
				0.53515625,
				0.5302734375,
				0.42578125,
				0.015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 744,
			"versionNonce": 246618418,
			"isDeleted": false,
			"id": "9vRDXdED-Uxa9smtPqMMi",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1369.5614550272242,
			"y": 1128.1704092112639,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 16.039558345079122,
			"height": 3.1381756154545766,
			"seed": 1714028260,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862519,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.3487068704054473,
					0
				],
				[
					1.0460674060179278,
					0
				],
				[
					3.1382022180537836,
					-0.3486802678062403
				],
				[
					4.532923289278744,
					-0.3486802678062403
				],
				[
					8.368486042945008,
					-0.6973605356124806
				],
				[
					12.552702461818306,
					-1.3947476738241682
				],
				[
					13.598769867836234,
					-1.7434279416304084
				],
				[
					15.342197809466642,
					-2.0921082094366485
				],
				[
					16.039558345079122,
					-3.1381756154545766
				],
				[
					16.039558345079122,
					-3.1381756154545766
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.25,
				0.35546875,
				0.4033203125,
				0.46484375,
				0.482421875,
				0.49609375,
				0.4921875,
				0.4853515625,
				0.3359375,
				0.0146484375,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 739,
			"versionNonce": 1015794414,
			"isDeleted": false,
			"id": "-b6mjIz2KiX17x8c2C9Mp",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1373.3970177808908,
			"y": 1114.571665946027,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 13.947423533043267,
			"height": 1.3947476738241682,
			"seed": 2110816868,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862519,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					8.717139708152041,
					-1.046040803418721
				],
				[
					10.111860779377002,
					-1.3947476738241682
				],
				[
					12.203995591412859,
					-1.046040803418721
				],
				[
					13.947423533043267,
					-0.6973605356124807
				],
				[
					13.947423533043267,
					-0.6973605356124807
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.41015625,
				0.47265625,
				0.4775390625,
				0.48046875,
				0.3818359375,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 792,
			"versionNonce": 2065507058,
			"isDeleted": false,
			"id": "YZjmfhh8quHBWDFOYalMj",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1401.6405185121841,
			"y": 1104.1111248988439,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 9.414500243764522,
			"height": 27.894847066086534,
			"seed": 1960482276,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862519,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					0.3486802678062403
				],
				[
					0,
					1.7434279416304084
				],
				[
					0,
					9.065819975958282
				],
				[
					-0.3486536652070332,
					13.947423533043267
				],
				[
					-0.3486536652070332,
					20.22377476395242
				],
				[
					-0.3486536652070332,
					23.013243509001548
				],
				[
					0,
					24.75667145063196
				],
				[
					0,
					25.802738856649885
				],
				[
					0.34870687040544723,
					26.151419124456126
				],
				[
					1.394774276423375,
					26.151419124456126
				],
				[
					3.138202218053783,
					25.802738856649885
				],
				[
					6.6250581013145995,
					25.802738856649885
				],
				[
					8.368486042945008,
					26.151419124456126
				],
				[
					8.717139708152041,
					26.151419124456126
				],
				[
					9.065846578557489,
					27.197486530474052
				],
				[
					9.065846578557489,
					27.894847066086534
				],
				[
					8.717139708152041,
					27.894847066086534
				],
				[
					8.717139708152041,
					27.894847066086534
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2509765625,
				0.3271484375,
				0.341796875,
				0.3671875,
				0.37890625,
				0.38671875,
				0.4033203125,
				0.4306640625,
				0.4423828125,
				0.4716796875,
				0.521484375,
				0.5244140625,
				0.5263671875,
				0.5263671875,
				0.5263671875,
				0.48828125,
				0.30078125,
				0.23828125,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 794,
			"versionNonce": 720387374,
			"isDeleted": false,
			"id": "m7YKVg8dSfxFwH_rhtm_0",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1418.0287305224704,
			"y": 1099.92690847997,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 7.671072302134114,
			"height": 33.12513089097776,
			"seed": 945174884,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862519,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					-0.3487068704054473
				],
				[
					-0.3486536652070333,
					1.3947210712249611
				],
				[
					-0.6973605356124806,
					5.230283824891226
				],
				[
					-1.046014200819514,
					11.855288721007412
				],
				[
					-1.3947210712249611,
					20.57242842915945
				],
				[
					-1.3947210712249611,
					24.407991182825718
				],
				[
					-1.046014200819514,
					28.940887869505254
				],
				[
					-1.046014200819514,
					29.986955275523183
				],
				[
					-1.046014200819514,
					31.032996078941903
				],
				[
					-1.046014200819514,
					32.07906348495983
				],
				[
					-1.046014200819514,
					32.42774375276607
				],
				[
					-0.6973605356124806,
					32.776424020572314
				],
				[
					0.3487068704054473,
					32.42774375276607
				],
				[
					1.7434279416304084,
					32.07906348495983
				],
				[
					2.440841682441303,
					32.07906348495983
				],
				[
					3.835562753666264,
					31.73038321715359
				],
				[
					4.184269624071711,
					31.73038321715359
				],
				[
					4.532923289278744,
					32.07906348495983
				],
				[
					6.276351230909153,
					32.42774375276607
				],
				[
					6.276351230909153,
					32.42774375276607
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2900390625,
				0.3759765625,
				0.41796875,
				0.44921875,
				0.47265625,
				0.4873046875,
				0.5,
				0.521484375,
				0.52734375,
				0.53515625,
				0.548828125,
				0.5556640625,
				0.5556640625,
				0.578125,
				0.5810546875,
				0.5810546875,
				0.583984375,
				0.5224609375,
				0.501953125,
				0.0146484375,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 786,
			"versionNonce": 1763701938,
			"isDeleted": false,
			"id": "-ZoZGMRZ5J6JiJeZSWj2p",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1443.134135446107,
			"y": 1103.4137643632314,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 13.947423533043267,
			"height": 27.546140195681087,
			"seed": 1670474980,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862519,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-5.578990695296673,
					2.7894687450491293
				],
				[
					-10.460567649782451,
					9.763180511570763
				],
				[
					-12.203995591412859,
					14.644784068655747
				],
				[
					-12.901409332223754,
					19.17770735793449
				],
				[
					-11.855341926205826,
					23.71060404461403
				],
				[
					-9.065846578557489,
					25.80271225405068
				],
				[
					-6.9737117665216335,
					26.848779660068605
				],
				[
					-3.4868558832608167,
					27.197459927874846
				],
				[
					-1.394774276423375,
					27.546140195681087
				],
				[
					0,
					27.197459927874846
				],
				[
					1.046014200819514,
					27.546140195681087
				],
				[
					1.046014200819514,
					27.546140195681087
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2041015625,
				0.248046875,
				0.380859375,
				0.462890625,
				0.4873046875,
				0.513671875,
				0.52734375,
				0.5361328125,
				0.5302734375,
				0.46875,
				0.2919921875,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 795,
			"versionNonce": 814507886,
			"isDeleted": false,
			"id": "3m3DUyuYVGeFX8gLUyZl7",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1460.5684148624114,
			"y": 1113.5256251426083,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 10.111860779377002,
			"height": 16.039558345079122,
			"seed": 2014982244,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862520,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-3.138202218053783,
					0
				],
				[
					-6.276351230909152,
					0.3487068704054473
				],
				[
					-9.065846578557489,
					1.3947476738241682
				],
				[
					-8.717139708152041,
					1.7434279416304084
				],
				[
					-7.32241863692708,
					3.4868558832608167
				],
				[
					-4.532923289278744,
					4.8816035570849845
				],
				[
					-2.0921348120358556,
					6.625031498715393
				],
				[
					-0.34870687040544723,
					8.368459440345802
				],
				[
					0.6973605356124805,
					10.460567649782451
				],
				[
					1.0460142008195137,
					12.203995591412859
				],
				[
					0.6973605356124805,
					12.901382729624546
				],
				[
					-0.6974137408108945,
					13.947423533043267
				],
				[
					-2.0921348120358556,
					14.296130403448714
				],
				[
					-4.184269624071711,
					14.644810671254955
				],
				[
					-6.6250581013145995,
					14.993490939061195
				],
				[
					-8.019779172539561,
					15.342171206867436
				],
				[
					-8.368486042945008,
					15.690851474673675
				],
				[
					-8.019779172539561,
					15.690851474673675
				],
				[
					-7.671125507332527,
					16.039558345079122
				],
				[
					-3.8355627536662635,
					15.690851474673675
				],
				[
					-3.8355627536662635,
					15.690851474673675
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2431640625,
				0.2890625,
				0.380859375,
				0.470703125,
				0.4833984375,
				0.48046875,
				0.48046875,
				0.4736328125,
				0.4716796875,
				0.4736328125,
				0.482421875,
				0.501953125,
				0.5400390625,
				0.5625,
				0.5791015625,
				0.58984375,
				0.58984375,
				0.5869140625,
				0.4228515625,
				0.3720703125,
				0.0146484375,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 791,
			"versionNonce": 979537522,
			"isDeleted": false,
			"id": "KR4riVe2IKVSN_lbxPKwH",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1467.8907802941403,
			"y": 1115.9664402224505,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 10.809221314989484,
			"height": 9.763180511570763,
			"seed": 364807140,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862520,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-1.046067406017928,
					1.3947476738241682
				],
				[
					-1.3947210712249614,
					2.0921082094366485
				],
				[
					-1.3947210712249614,
					3.4868558832608167
				],
				[
					-1.046067406017928,
					4.8816035570849845
				],
				[
					0,
					6.625031498715393
				],
				[
					1.7434279416304086,
					8.368459440345802
				],
				[
					3.486855883260817,
					9.414500243764522
				],
				[
					4.8816301596841924,
					9.763180511570763
				],
				[
					6.276351230909154,
					9.763180511570763
				],
				[
					6.973711766521634,
					8.717139708152041
				],
				[
					7.671072302134115,
					6.9737117665216335
				],
				[
					8.717139708152043,
					4.532896686679537
				],
				[
					9.414500243764524,
					2.4407884772428887
				],
				[
					9.414500243764524,
					2.0921082094366485
				],
				[
					9.414500243764524,
					3.1381756154545766
				],
				[
					9.414500243764524,
					3.4868558832608167
				],
				[
					9.414500243764524,
					3.4868558832608167
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2109375,
				0.265625,
				0.2939453125,
				0.36328125,
				0.3974609375,
				0.404296875,
				0.4296875,
				0.4482421875,
				0.470703125,
				0.4833984375,
				0.498046875,
				0.517578125,
				0.5498046875,
				0.5634765625,
				0.5654296875,
				0.244140625,
				0.05859375,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 797,
			"versionNonce": 2108246446,
			"isDeleted": false,
			"id": "7ORi1rYgpI7zTnE3eqBs0",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1481.1408432915714,
			"y": 1116.663800758063,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 15.690851474673675,
			"height": 11.506635055800379,
			"seed": 848062308,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862520,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.3487068704054473,
					1.3947476738241682
				],
				[
					-0.3487068704054473,
					1.7434279416304084
				],
				[
					-0.3487068704054473,
					3.4868558832608167
				],
				[
					-0.3487068704054473,
					4.8816035570849845
				],
				[
					-0.3487068704054473,
					6.625031498715393
				],
				[
					0.3487068704054473,
					6.625031498715393
				],
				[
					2.7894953476483364,
					4.532923289278744
				],
				[
					4.881576954485777,
					2.7894953476483364
				],
				[
					7.322418636927081,
					0.6973871382116875
				],
				[
					7.671072302134114,
					0.3486802678062403
				],
				[
					8.019779172539561,
					0.6973871382116875
				],
				[
					8.368432837746594,
					1.3947476738241682
				],
				[
					9.414500243764522,
					1.7434279416304084
				],
				[
					11.157928185394931,
					1.7434279416304084
				],
				[
					12.90135612702534,
					2.0921082094366485
				],
				[
					13.59871666263782,
					3.835536151067057
				],
				[
					13.59871666263782,
					5.927670963102913
				],
				[
					13.59871666263782,
					8.368459440345802
				],
				[
					13.947423533043267,
					9.41452684636373
				],
				[
					14.296130403448714,
					10.460567649782451
				],
				[
					14.993490939061195,
					11.157954787994138
				],
				[
					15.342144604268228,
					11.506635055800379
				],
				[
					15.342144604268228,
					11.506635055800379
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2255859375,
				0.2685546875,
				0.3037109375,
				0.376953125,
				0.4130859375,
				0.4443359375,
				0.4990234375,
				0.5224609375,
				0.52734375,
				0.5244140625,
				0.5244140625,
				0.5244140625,
				0.52734375,
				0.537109375,
				0.5458984375,
				0.5537109375,
				0.5537109375,
				0.55859375,
				0.5791015625,
				0.58203125,
				0.5634765625,
				0.4248046875,
				0.015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 600,
			"versionNonce": 61599794,
			"isDeleted": false,
			"id": "1reIGJwlTxsyYcNChnMEV",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1501.0159643903162,
			"y": 1100.9729492833887,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 12.552649256619892,
			"height": 39.052775251481464,
			"seed": 1389484772,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862520,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					-1.0460408034187207
				],
				[
					0,
					-2.4407884772428887
				],
				[
					0.6973605356124806,
					-3.1381490128553695
				],
				[
					3.4868558832608167,
					-2.4407884772428887
				],
				[
					5.578937490098259,
					0.6973871382116875
				],
				[
					7.671072302134114,
					4.8816035570849845
				],
				[
					9.763153908971555,
					9.41452684636373
				],
				[
					11.157928185394931,
					16.388238612885363
				],
				[
					12.203995591412859,
					19.87509449614618
				],
				[
					12.552649256619892,
					23.013270111600757
				],
				[
					12.552649256619892,
					25.454058588843644
				],
				[
					11.506581850601965,
					29.98698187812239
				],
				[
					10.460567649782451,
					32.427770355365276
				],
				[
					9.763153908971555,
					33.822518029189446
				],
				[
					9.763153908971555,
					34.51987856480193
				],
				[
					9.763153908971555,
					34.868558832608166
				],
				[
					9.763153908971555,
					35.565945970819854
				],
				[
					10.111860779377002,
					35.9146262386261
				],
				[
					10.111860779377002,
					35.9146262386261
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.1923828125,
				0.2431640625,
				0.3017578125,
				0.3466796875,
				0.37890625,
				0.3740234375,
				0.369140625,
				0.37109375,
				0.3798828125,
				0.39453125,
				0.41796875,
				0.44921875,
				0.4873046875,
				0.5029296875,
				0.513671875,
				0.5185546875,
				0.521484375,
				0.4853515625,
				0.47265625,
				0
			]
		},
		{
			"type": "text",
			"version": 118,
			"versionNonce": 1366287342,
			"isDeleted": false,
			"id": "pym91Zhn",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 517.8725214013716,
			"y": 628.5053173730639,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 108,
			"height": 25,
			"seed": 1088388704,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862520,
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
			"version": 508,
			"versionNonce": 685971954,
			"isDeleted": false,
			"id": "KGwjUGcJ",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 658.091811141281,
			"y": 858.880152639462,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 158,
			"height": 25,
			"seed": 2130725472,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862520,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "largestSize += 1",
			"rawText": "largestSize += 1",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "largestSize += 1",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 921,
			"versionNonce": 501823022,
			"isDeleted": false,
			"id": "Ur-knG0bKpgbBhHGcZXgM",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 566.6973079139211,
			"y": 793.5879378985294,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 462,
			"height": 35,
			"seed": 2140623456,
			"groupIds": [],
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "ZQt3LQf8"
				}
			],
			"updated": 1685655862520,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 501,
			"versionNonce": 2031029170,
			"isDeleted": false,
			"id": "ZQt3LQf8",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 580.1973079139211,
			"y": 798.5879378985294,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 435,
			"height": 25,
			"seed": 1429116832,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862520,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "while either l1_temp or l2_temp are not null",
			"rawText": "while either l1_temp or l2_temp are not null",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "Ur-knG0bKpgbBhHGcZXgM",
			"originalText": "while either l1_temp or l2_temp are not null",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 362,
			"versionNonce": 738082926,
			"isDeleted": false,
			"id": "AFZ3ZRWc",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 583.8382071451581,
			"y": 751.9801482494361,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 154,
			"height": 25,
			"seed": 43714144,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862520,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "largestSize = 0",
			"rawText": "largestSize = 0",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "largestSize = 0",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "line",
			"version": 333,
			"versionNonce": 1247200626,
			"isDeleted": false,
			"id": "OK1sm5XeV3JhMQgqJvgwu",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1033.2020520993754,
			"y": 812.7914730138161,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 39.047131090970424,
			"height": 1.280292651131731,
			"seed": 1645033056,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1685655862520,
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
					39.047131090970424,
					-1.280292651131731
				]
			]
		},
		{
			"type": "line",
			"version": 465,
			"versionNonce": 1064829614,
			"isDeleted": false,
			"id": "TlnJmBchXFJmL0gXlieSA",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1070.3288052601984,
			"y": 812.7914974324356,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 0.6400608603969431,
			"height": 97.93834653001898,
			"seed": 1434124192,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1685655862520,
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
					-0.6400608603969431,
					97.93834653001898
				]
			]
		},
		{
			"type": "line",
			"version": 396,
			"versionNonce": 369182514,
			"isDeleted": false,
			"id": "E-dZzVvbJFS_ihV92YMx9",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1062.0073303536867,
			"y": 912.6500997995045,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 434.00101686198855,
			"height": 2.5604876277848234,
			"seed": 1670980192,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1685655862520,
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
					-434.00101686198855,
					2.5604876277848234
				]
			]
		},
		{
			"type": "line",
			"version": 285,
			"versionNonce": 989822190,
			"isDeleted": false,
			"id": "bJag2NLX11gewNR4h8sKh",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 627.366252631301,
			"y": 915.210587427289,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 2.5605364650242564,
			"height": 80.01493313552595,
			"seed": 186288736,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1685655862520,
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
					2.5605364650242564,
					-80.01493313552595
				]
			]
		},
		{
			"type": "rectangle",
			"version": 397,
			"versionNonce": 343249138,
			"isDeleted": false,
			"id": "65e1pMbn3eCtMUBSdj5Lw",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 602.2173640119872,
			"y": 951.9407235524059,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 170,
			"height": 36,
			"seed": 874462816,
			"groupIds": [],
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "f1S00YO4"
				}
			],
			"updated": 1685655862520,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 166,
			"versionNonce": 1142796078,
			"isDeleted": false,
			"id": "f1S00YO4",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 613.2173640119872,
			"y": 957.4407235524059,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 148,
			"height": 25,
			"seed": 914081376,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862520,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "for largestSize",
			"rawText": "for largestSize",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "65e1pMbn3eCtMUBSdj5Lw",
			"originalText": "for largestSize",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "line",
			"version": 277,
			"versionNonce": 1497014962,
			"isDeleted": false,
			"id": "8RK__71PeYMqiMS0AuXNU",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 775.8739489959414,
			"y": 970.90091251748,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 318.13935461195535,
			"height": 5.7610849532057955,
			"seed": 1877922720,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1685655862520,
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
					318.13935461195535,
					-5.7610849532057955
				]
			]
		},
		{
			"type": "line",
			"version": 357,
			"versionNonce": 1731959150,
			"isDeleted": false,
			"id": "ysA78j8moqWYCZd_Ei-gG",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 615.8440827248896,
			"y": 991.3847402838985,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 17.283206022377726,
			"height": 798.8690631227474,
			"seed": 328407968,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1685655862520,
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
					17.283206022377726,
					798.8690631227474
				]
			]
		},
		{
			"type": "text",
			"version": 201,
			"versionNonce": 1861713010,
			"isDeleted": false,
			"id": "378lKNzK",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 584.2467962440666,
			"y": 711.7096448933212,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 89,
			"height": 25,
			"seed": 114413152,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862520,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "llSolution;",
			"rawText": "llSolution;",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "llSolution;",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 188,
			"versionNonce": 1000487854,
			"isDeleted": false,
			"id": "SIm5WW90",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 679.8557362098727,
			"y": 1032.9924810957523,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 106,
			"height": 25,
			"seed": 1772065376,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862520,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "valuel1 = 0",
			"rawText": "valuel1 = 0",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "valuel1 = 0",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 219,
			"versionNonce": 1936924210,
			"isDeleted": false,
			"id": "24AzcU4z",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 685.6169676747967,
			"y": 1064.9983566754838,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 115,
			"height": 25,
			"seed": 1241389664,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862520,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "valuel2 = 0",
			"rawText": "valuel2 = 0",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "valuel2 = 0",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 329,
			"versionNonce": 125474286,
			"isDeleted": false,
			"id": "LmPnKYKmZIeX8ZfWbO0Ir",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 685.6168700003178,
			"y": 1095.72425704614,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 252,
			"height": 38,
			"seed": 1459558304,
			"groupIds": [],
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"id": "iq995rDEaZrZ-n0xsauKL",
					"type": "arrow"
				},
				{
					"type": "text",
					"id": "xQxY3kzC"
				}
			],
			"updated": 1685655862520,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 231,
			"versionNonce": 865372146,
			"isDeleted": false,
			"id": "xQxY3kzC",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 702.6168700003178,
			"y": 1102.22425704614,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 218,
			"height": 25,
			"seed": 1471859616,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862520,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "if both values not null",
			"rawText": "if both values not null",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "LmPnKYKmZIeX8ZfWbO0Ir",
			"originalText": "if both values not null",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "arrow",
			"version": 1386,
			"versionNonce": 1674422318,
			"isDeleted": false,
			"id": "iq995rDEaZrZ-n0xsauKL",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 771.9492031946093,
			"y": 1141.8995313972466,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 134.22949759529774,
			"height": 32.236112725546604,
			"seed": 1512178592,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "8hlovFyI"
				}
			],
			"updated": 1685655862520,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "LmPnKYKmZIeX8ZfWbO0Ir",
				"focus": 0.7450653893870717,
				"gap": 8.17527435110651
			},
			"endBinding": {
				"elementId": "ljKeKlyW",
				"focus": 0.27923643355088673,
				"gap": 14.406081872275081
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
					134.22949759529774,
					32.236112725546604
				]
			]
		},
		{
			"type": "text",
			"version": 134,
			"versionNonce": 1197652402,
			"isDeleted": false,
			"id": "8hlovFyI",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 842.1276506665424,
			"y": 1166.4397142512275,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 16,
			"height": 25,
			"seed": 1199288224,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862520,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "T",
			"rawText": "T",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "iq995rDEaZrZ-n0xsauKL",
			"originalText": "T",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 329,
			"versionNonce": 1619292782,
			"isDeleted": false,
			"id": "ljKeKlyW",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 906.4581831288494,
			"y": 1188.5417259950682,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 152,
			"height": 25,
			"seed": 1709928032,
			"groupIds": [],
			"roundness": null,
			"boundElements": [
				{
					"id": "iq995rDEaZrZ-n0xsauKL",
					"type": "arrow"
				}
			],
			"updated": 1685655862520,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "value1 = l1.value",
			"rawText": "value1 = l1.value",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "value1 = l1.value",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 363,
			"versionNonce": 772060018,
			"isDeleted": false,
			"id": "eTV2buH5",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 912.8591824307335,
			"y": 1228.2290156209142,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 170,
			"height": 25,
			"seed": 1161991776,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862520,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "value2 = l2.value",
			"rawText": "value2 = l2.value",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "value2 = l2.value",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 563,
			"versionNonce": 677901486,
			"isDeleted": false,
			"id": "u71ND3sHIMPnZs-Y22QGH",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 690.9228175866624,
			"y": 1248.8574086070075,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 155,
			"height": 37,
			"seed": 205936224,
			"groupIds": [],
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "yoIAIXuZ"
				},
				{
					"id": "faYJtzqdCbcchlFSR0NpZ",
					"type": "arrow"
				}
			],
			"updated": 1685655862520,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 545,
			"versionNonce": 1774286130,
			"isDeleted": false,
			"id": "yoIAIXuZ",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 716.9228175866624,
			"y": 1254.8574086070075,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 103,
			"height": 25,
			"seed": 1553131424,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862520,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "if sum < 9",
			"rawText": "if sum < 9",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "u71ND3sHIMPnZs-Y22QGH",
			"originalText": "if sum < 9",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 744,
			"versionNonce": 622931694,
			"isDeleted": false,
			"id": "D2N_3paL6vP3_T4LXuC1W",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 780.7694001894498,
			"y": 1338.2350233230445,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 188,
			"height": 35,
			"seed": 1989816928,
			"groupIds": [],
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "cUn8HeKJ"
				},
				{
					"id": "faYJtzqdCbcchlFSR0NpZ",
					"type": "arrow"
				},
				{
					"id": "ZjW3Z--Ot0gZRdAVkZmvW",
					"type": "arrow"
				}
			],
			"updated": 1685655862520,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 753,
			"versionNonce": 469761778,
			"isDeleted": false,
			"id": "cUn8HeKJ",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 794.7694001894498,
			"y": 1343.2350233230445,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 160,
			"height": 25,
			"seed": 1193956960,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862520,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "if carry == true",
			"rawText": "if carry == true",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "D2N_3paL6vP3_T4LXuC1W",
			"originalText": "if carry == true",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "arrow",
			"version": 1464,
			"versionNonce": 590946606,
			"isDeleted": false,
			"id": "faYJtzqdCbcchlFSR0NpZ",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 727.1100114861629,
			"y": 1290.9606938968236,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 94.75922534746269,
			"height": 35.20657057963115,
			"seed": 1858288224,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "j208RnMj"
				}
			],
			"updated": 1685655862520,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "u71ND3sHIMPnZs-Y22QGH",
				"focus": 0.8236229043455013,
				"gap": 5.103285289816085
			},
			"endBinding": {
				"elementId": "D2N_3paL6vP3_T4LXuC1W",
				"focus": 0.18909833877792098,
				"gap": 12.06775884658964
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
					94.75922534746269,
					35.20657057963115
				]
			]
		},
		{
			"type": "text",
			"version": 236,
			"versionNonce": 558321842,
			"isDeleted": false,
			"id": "j208RnMj",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 836.6869380042114,
			"y": 1322.6289955923212,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 16,
			"height": 25,
			"seed": 1952049760,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862520,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "T",
			"rawText": "T",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "faYJtzqdCbcchlFSR0NpZ",
			"originalText": "T",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 488,
			"versionNonce": 1981336430,
			"isDeleted": false,
			"id": "YitmxPR5",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 898.7769644316915,
			"y": 1424.105513331996,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 85,
			"height": 25,
			"seed": 1266051680,
			"groupIds": [],
			"roundness": null,
			"boundElements": [
				{
					"id": "ZjW3Z--Ot0gZRdAVkZmvW",
					"type": "arrow"
				}
			],
			"updated": 1685655862520,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "sum += 1",
			"rawText": "sum += 1",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "sum += 1",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "arrow",
			"version": 1218,
			"versionNonce": 759065202,
			"isDeleted": false,
			"id": "ZjW3Z--Ot0gZRdAVkZmvW",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 827.5077197397413,
			"y": 1378.6570899157045,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 65.23296097980597,
			"height": 39.50930354052639,
			"seed": 486272928,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "wslASSB1"
				}
			],
			"updated": 1685655862520,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "D2N_3paL6vP3_T4LXuC1W",
				"focus": 0.692530953763714,
				"gap": 5.42206659266003
			},
			"endBinding": {
				"elementId": "YitmxPR5",
				"focus": -0.28654236415231776,
				"gap": 6.036283712144154
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
					65.23296097980597,
					39.50930354052639
				]
			]
		},
		{
			"type": "text",
			"version": 134,
			"versionNonce": 470363566,
			"isDeleted": false,
			"id": "wslASSB1",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 909.3405363610602,
			"y": 1431.7693595054557,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 16,
			"height": 25,
			"seed": 893947488,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862520,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "T",
			"rawText": "T",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "ZjW3Z--Ot0gZRdAVkZmvW",
			"originalText": "T",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 248,
			"versionNonce": 1722567730,
			"isDeleted": false,
			"id": "XWCHqCBa",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 787.3964119257888,
			"y": 1503.4803367698855,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 206,
			"height": 25,
			"seed": 96862816,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862520,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "llSolution.value = sum",
			"rawText": "llSolution.value = sum",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "llSolution.value = sum",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 239,
			"versionNonce": 1647527918,
			"isDeleted": false,
			"id": "KTztRTlCMFO_hGrdywcmE",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 688.8180533726119,
			"y": 1583.4953675798902,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 80,
			"height": 35,
			"seed": 1458283424,
			"groupIds": [],
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "CN2nYge6"
				}
			],
			"updated": 1685655862520,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 221,
			"versionNonce": 58193394,
			"isDeleted": false,
			"id": "CN2nYge6",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 709.8180533726119,
			"y": 1588.4953675798902,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 38,
			"height": 25,
			"seed": 1476378528,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862520,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "else",
			"rawText": "else",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "KTztRTlCMFO_hGrdywcmE",
			"originalText": "else",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 211,
			"versionNonce": 144710190,
			"isDeleted": false,
			"id": "xElYFQwW",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 759.8711577177929,
			"y": 1619.3419990199181,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 124,
			"height": 25,
			"seed": 1734354848,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862520,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "carry = true",
			"rawText": "carry = true",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "carry = true",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 196,
			"versionNonce": 1688758194,
			"isDeleted": false,
			"id": "WKOQFTNw",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 763.071755043214,
			"y": 1651.988081971765,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 94,
			"height": 25,
			"seed": 1437138848,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862520,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "sum -= 10",
			"rawText": "sum -= 10",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "sum -= 10",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 182,
			"versionNonce": 1714988142,
			"isDeleted": false,
			"id": "ASXx62SK",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 903.2579765013429,
			"y": 1454.8312183536937,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 132,
			"height": 25,
			"seed": 2143669856,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862520,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "carry = false",
			"rawText": "carry = false",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "carry = false",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 330,
			"versionNonce": 845455730,
			"isDeleted": false,
			"id": "bXM31pbp",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 763.131027991563,
			"y": 1691.977858573774,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 206,
			"height": 25,
			"seed": 1568888416,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862520,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "llSolution.value = sum",
			"rawText": "llSolution.value = sum",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "llSolution.value = sum",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 353,
			"versionNonce": 214296238,
			"isDeleted": false,
			"id": "UvoTTpgF",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 775.9334172932471,
			"y": 1729.7449167811897,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 158,
			"height": 25,
			"seed": 454747744,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862520,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "llSolution = next",
			"rawText": "llSolution = next",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "llSolution = next",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 423,
			"versionNonce": 2012455730,
			"isDeleted": false,
			"id": "hPdW1Xdk",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 786.4908694566873,
			"y": 1533.8683702328703,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 158,
			"height": 25,
			"seed": 436298336,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862520,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "llSolution = next",
			"rawText": "llSolution = next",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "llSolution = next",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "line",
			"version": 283,
			"versionNonce": 1827725550,
			"isDeleted": false,
			"id": "OcMvy3AToK6hvTtMV_nWI",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 631.5350722192002,
			"y": 1774.4549025054948,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 462.2555258256855,
			"height": 0,
			"seed": 360187808,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1685655862520,
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
					462.2555258256855,
					0
				]
			]
		},
		{
			"type": "line",
			"version": 292,
			"versionNonce": 1069313266,
			"isDeleted": false,
			"id": "SbBnqpb4QErPPXF316lqk",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1093.3290931788501,
			"y": 977.3203275691537,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 0,
			"height": 787.5561706495356,
			"seed": 1949787744,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1685655862521,
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
					787.5561706495356
				]
			]
		},
		{
			"id": "exilHY7MVp5lul_mthCmu",
			"type": "ellipse",
			"x": 1096.8429949016831,
			"y": 31.425093169575277,
			"width": 46,
			"height": 49,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [
				"9hX1u_x2ljBZy_eVTNM85"
			],
			"roundness": {
				"type": 2
			},
			"seed": 1954994802,
			"version": 230,
			"versionNonce": 249755310,
			"isDeleted": false,
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
			"updated": 1685657264459,
			"link": null,
			"locked": false
		},
		{
			"id": "bQ9Kjc4G",
			"type": "text",
			"x": 1113.0795389343925,
			"y": 43.600977030504865,
			"width": 14,
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
				"9hX1u_x2ljBZy_eVTNM85"
			],
			"roundness": null,
			"seed": 1307528622,
			"version": 72,
			"versionNonce": 2112852786,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1685657264459,
			"link": null,
			"locked": false,
			"text": "2",
			"rawText": "2",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "center",
			"verticalAlign": "middle",
			"baseline": 17,
			"containerId": "exilHY7MVp5lul_mthCmu",
			"originalText": "2",
			"lineHeight": 1.25
		},
		{
			"id": "qD1dnyM8cY5Fi9I6jbduK",
			"type": "ellipse",
			"x": 1195.0767122168188,
			"y": 26.100352074470436,
			"width": 46,
			"height": 49,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [
				"9hX1u_x2ljBZy_eVTNM85"
			],
			"roundness": {
				"type": 2
			},
			"seed": 266420722,
			"version": 168,
			"versionNonce": 1663521266,
			"isDeleted": false,
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
			"updated": 1685657262601,
			"link": null,
			"locked": false
		},
		{
			"id": "LrJzMGg3",
			"type": "text",
			"x": 1211.8132562495282,
			"y": 38.276235935400024,
			"width": 13,
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
				"9hX1u_x2ljBZy_eVTNM85"
			],
			"roundness": null,
			"seed": 6240370,
			"version": 57,
			"versionNonce": 445679726,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1685657262601,
			"link": null,
			"locked": false,
			"text": "4",
			"rawText": "4",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "center",
			"verticalAlign": "middle",
			"baseline": 17,
			"containerId": "qD1dnyM8cY5Fi9I6jbduK",
			"originalText": "4",
			"lineHeight": 1.25
		},
		{
			"id": "IJJojCOaSu6BXOfooL_LH",
			"type": "ellipse",
			"x": 1294.7705204620147,
			"y": 33.801548714504264,
			"width": 47,
			"height": 49,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [
				"9hX1u_x2ljBZy_eVTNM85"
			],
			"roundness": {
				"type": 2
			},
			"seed": 1311385202,
			"version": 120,
			"versionNonce": 2062351730,
			"isDeleted": false,
			"boundElements": [
				{
					"type": "text",
					"id": "BY3tMLOh"
				}
			],
			"updated": 1685657262601,
			"link": null,
			"locked": false
		},
		{
			"id": "BY3tMLOh",
			"type": "text",
			"x": 1311.1535111041308,
			"y": 45.97743257543385,
			"width": 14,
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
				"9hX1u_x2ljBZy_eVTNM85"
			],
			"roundness": null,
			"seed": 1126797358,
			"version": 32,
			"versionNonce": 880888494,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1685657262601,
			"link": null,
			"locked": false,
			"text": "3",
			"rawText": "3",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "center",
			"verticalAlign": "middle",
			"baseline": 17,
			"containerId": "IJJojCOaSu6BXOfooL_LH",
			"originalText": "3",
			"lineHeight": 1.25
		},
		{
			"id": "0b4tR5q7vjmysYkD2HHcQ",
			"type": "arrow",
			"x": 1145.1656589413928,
			"y": 53.034949972234266,
			"width": 45.46930966006994,
			"height": 1.4111187177396403,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [
				"9hX1u_x2ljBZy_eVTNM85"
			],
			"roundness": {
				"type": 2
			},
			"seed": 876922990,
			"version": 91,
			"versionNonce": 12213490,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1685657264460,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					45.46930966006994,
					1.4111187177396403
				]
			],
			"lastCommittedPoint": null,
			"startBinding": {
				"elementId": "exilHY7MVp5lul_mthCmu",
				"focus": -0.14657606810296117,
				"gap": 2.469332983882069
			},
			"endBinding": {
				"elementId": "qD1dnyM8cY5Fi9I6jbduK",
				"focus": -0.19164758936026538,
				"gap": 4.6831636924216085
			},
			"startArrowhead": null,
			"endArrowhead": "arrow"
		},
		{
			"id": "krEjcblc8Oo_g-wRpnRTJ",
			"type": "arrow",
			"x": 1242.5844030829219,
			"y": 51.83355635313265,
			"width": 54.54897317488167,
			"height": 4.545756022032634,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [
				"9hX1u_x2ljBZy_eVTNM85"
			],
			"roundness": {
				"type": 2
			},
			"seed": 2062249646,
			"version": 31,
			"versionNonce": 165403314,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1685657262602,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					54.54897317488167,
					4.545756022032634
				]
			],
			"lastCommittedPoint": null,
			"startBinding": {
				"elementId": "qD1dnyM8cY5Fi9I6jbduK",
				"focus": -0.032924178754430225,
				"gap": 1.5352239703298736
			},
			"endBinding": null,
			"startArrowhead": null,
			"endArrowhead": "arrow"
		},
		{
			"id": "4ktnhSsKOpNCwK4cOKRVh",
			"type": "ellipse",
			"x": 1110.9605066118306,
			"y": 106.38260384514672,
			"width": 47,
			"height": 49,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [
				"rfh2hC-4_wjn4UI5_wHT5"
			],
			"roundness": {
				"type": 2
			},
			"seed": 1131699566,
			"version": 309,
			"versionNonce": 674952238,
			"isDeleted": false,
			"boundElements": [
				{
					"type": "text",
					"id": "q7xmGnTH"
				}
			],
			"updated": 1685657266409,
			"link": null,
			"locked": false
		},
		{
			"id": "q7xmGnTH",
			"type": "text",
			"x": 1128.3434972539467,
			"y": 118.5584877060763,
			"width": 12,
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
				"rfh2hC-4_wjn4UI5_wHT5"
			],
			"roundness": null,
			"seed": 338239858,
			"version": 254,
			"versionNonce": 1145056690,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1685657266409,
			"link": null,
			"locked": false,
			"text": "5",
			"rawText": "5",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "center",
			"verticalAlign": "middle",
			"baseline": 17,
			"containerId": "4ktnhSsKOpNCwK4cOKRVh",
			"originalText": "5",
			"lineHeight": 1.25
		},
		{
			"id": "Y1xH8USbSnljmuMKGFIcC",
			"type": "ellipse",
			"x": 1197.680413612618,
			"y": 101.18743995003666,
			"width": 45,
			"height": 49,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [
				"rfh2hC-4_wjn4UI5_wHT5"
			],
			"roundness": {
				"type": 2
			},
			"seed": 1643053106,
			"version": 241,
			"versionNonce": 1097350766,
			"isDeleted": false,
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
			"updated": 1685657266409,
			"link": null,
			"locked": false
		},
		{
			"id": "y3MQq29Y",
			"type": "text",
			"x": 1213.7705110359207,
			"y": 113.36332381096625,
			"width": 13,
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
				"rfh2hC-4_wjn4UI5_wHT5"
			],
			"roundness": null,
			"seed": 582260146,
			"version": 214,
			"versionNonce": 1391607982,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1685657266409,
			"link": null,
			"locked": false,
			"text": "6",
			"rawText": "6",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "center",
			"verticalAlign": "middle",
			"baseline": 17,
			"containerId": "Y1xH8USbSnljmuMKGFIcC",
			"originalText": "6",
			"lineHeight": 1.25
		},
		{
			"id": "y1g7qtk355waWdqEx29nd",
			"type": "ellipse",
			"x": 1289.660996886499,
			"y": 100.3385183304822,
			"width": 51,
			"height": 49,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [
				"rfh2hC-4_wjn4UI5_wHT5"
			],
			"roundness": {
				"type": 2
			},
			"seed": 1776940334,
			"version": 311,
			"versionNonce": 1020389682,
			"isDeleted": false,
			"boundElements": [
				{
					"type": "text",
					"id": "RqHOIK5i"
				}
			],
			"updated": 1685657266409,
			"link": null,
			"locked": false
		},
		{
			"id": "RqHOIK5i",
			"type": "text",
			"x": 1308.629773966242,
			"y": 112.51440219141179,
			"width": 13,
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
				"rfh2hC-4_wjn4UI5_wHT5"
			],
			"roundness": null,
			"seed": 1935575150,
			"version": 265,
			"versionNonce": 545389294,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1685657266409,
			"link": null,
			"locked": false,
			"text": "4",
			"rawText": "4",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "center",
			"verticalAlign": "middle",
			"baseline": 17,
			"containerId": "y1g7qtk355waWdqEx29nd",
			"originalText": "4",
			"lineHeight": 1.25
		},
		{
			"id": "4BpZhqcvHudFxTghtgYue",
			"type": "arrow",
			"x": 1156.2152120709436,
			"y": 121.96799644096745,
			"width": 48.70447572382659,
			"height": 1.2987662014001558,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [
				"rfh2hC-4_wjn4UI5_wHT5"
			],
			"roundness": {
				"type": 2
			},
			"seed": 2030321266,
			"version": 195,
			"versionNonce": 484569842,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1685657266409,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					48.70447572382659,
					-1.2987662014001558
				]
			],
			"lastCommittedPoint": null,
			"startBinding": null,
			"endBinding": null,
			"startArrowhead": null,
			"endArrowhead": "arrow"
		},
		{
			"id": "Zf8jKqqcGJBrzgJsSwvVm",
			"type": "arrow",
			"x": 1245.1999699154867,
			"y": 128.49852093274916,
			"width": 48.68644129406188,
			"height": 4.582276100171992,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [
				"rfh2hC-4_wjn4UI5_wHT5"
			],
			"roundness": {
				"type": 2
			},
			"seed": 753478770,
			"version": 411,
			"versionNonce": 432719026,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1685657266421,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					48.68644129406188,
					-4.582276100171992
				]
			],
			"lastCommittedPoint": null,
			"startBinding": {
				"elementId": "Y1xH8USbSnljmuMKGFIcC",
				"focus": 0.21006876647029482,
				"gap": 2.654620251194789
			},
			"endBinding": null,
			"startArrowhead": null,
			"endArrowhead": "arrow"
		},
		{
			"id": "NEjY1Xn_YKnNmMlzzZv5o",
			"type": "ellipse",
			"x": 1111.1753030010043,
			"y": 182.31133642112775,
			"width": 57,
			"height": 49,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [
				"Ajld6Asjms0H9O_g9IwNA"
			],
			"roundness": {
				"type": 2
			},
			"seed": 1539496238,
			"version": 192,
			"versionNonce": 1318965230,
			"isDeleted": false,
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
			"updated": 1685657267744,
			"link": null,
			"locked": false
		},
		{
			"id": "RzKJ3NZ7",
			"type": "text",
			"x": 1134.0227597371877,
			"y": 194.48722028205736,
			"width": 11,
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
				"Ajld6Asjms0H9O_g9IwNA"
			],
			"roundness": null,
			"seed": 1976927150,
			"version": 148,
			"versionNonce": 377070126,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1685657267744,
			"link": null,
			"locked": false,
			"text": "7",
			"rawText": "7",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "center",
			"verticalAlign": "middle",
			"baseline": 17,
			"containerId": "NEjY1Xn_YKnNmMlzzZv5o",
			"originalText": "7",
			"lineHeight": 1.25
		},
		{
			"id": "vxvUoabl2P81si07C7P1B",
			"type": "ellipse",
			"x": 1202.6680756266192,
			"y": 176.992739546645,
			"width": 58,
			"height": 50,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [
				"Ajld6Asjms0H9O_g9IwNA"
			],
			"roundness": {
				"type": 2
			},
			"seed": 1564053678,
			"version": 209,
			"versionNonce": 1628135346,
			"isDeleted": false,
			"boundElements": [
				{
					"type": "text",
					"id": "W1G5e9CW"
				}
			],
			"updated": 1685657267744,
			"link": null,
			"locked": false
		},
		{
			"id": "W1G5e9CW",
			"type": "text",
			"x": 1224.6619789722092,
			"y": 189.31507001698128,
			"width": 14,
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
				"Ajld6Asjms0H9O_g9IwNA"
			],
			"roundness": null,
			"seed": 776435438,
			"version": 186,
			"versionNonce": 262220910,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1685657267744,
			"link": null,
			"locked": false,
			"text": "0",
			"rawText": "0",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "center",
			"verticalAlign": "middle",
			"baseline": 17,
			"containerId": "vxvUoabl2P81si07C7P1B",
			"originalText": "0",
			"lineHeight": 1.25
		},
		{
			"id": "H-a6zWexNz3TrcXhni8xB",
			"type": "ellipse",
			"x": 1303.4734743127372,
			"y": 177.5384707963001,
			"width": 50,
			"height": 49,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [
				"Ajld6Asjms0H9O_g9IwNA"
			],
			"roundness": {
				"type": 2
			},
			"seed": 1705974126,
			"version": 196,
			"versionNonce": 396925298,
			"isDeleted": false,
			"boundElements": [
				{
					"type": "text",
					"id": "ebTfCNkg"
				}
			],
			"updated": 1685657267744,
			"link": null,
			"locked": false
		},
		{
			"id": "ebTfCNkg",
			"type": "text",
			"x": 1320.7958047830734,
			"y": 189.7143546572297,
			"width": 15,
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
				"Ajld6Asjms0H9O_g9IwNA"
			],
			"roundness": null,
			"seed": 1306406386,
			"version": 173,
			"versionNonce": 131952302,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1685657267744,
			"link": null,
			"locked": false,
			"text": "8",
			"rawText": "8",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "center",
			"verticalAlign": "middle",
			"baseline": 17,
			"containerId": "H-a6zWexNz3TrcXhni8xB",
			"originalText": "8",
			"lineHeight": 1.25
		},
		{
			"id": "-y-piyUZ_HAiYpXFSxj5t",
			"type": "arrow",
			"x": 1169.2028740849448,
			"y": 197.94700829698968,
			"width": 35.71661553080639,
			"height": 3.8963976937099574,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [
				"Ajld6Asjms0H9O_g9IwNA"
			],
			"roundness": {
				"type": 2
			},
			"seed": 16711858,
			"version": 275,
			"versionNonce": 778200306,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1685657267828,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					35.71661553080639,
					-3.8963976937099574
				]
			],
			"lastCommittedPoint": null,
			"startBinding": {
				"elementId": "NEjY1Xn_YKnNmMlzzZv5o",
				"focus": -0.22849828739977093,
				"gap": 2.7258043173164097
			},
			"endBinding": null,
			"startArrowhead": null,
			"endArrowhead": "arrow"
		},
		{
			"id": "Z62sIMhULBsARu8kHIw_b",
			"type": "arrow",
			"x": 1254.2733979850325,
			"y": 201.84335644594483,
			"width": 57.795938223137,
			"height": 1.2987662014001558,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [
				"Ajld6Asjms0H9O_g9IwNA"
			],
			"roundness": {
				"type": 2
			},
			"seed": 1720661678,
			"version": 146,
			"versionNonce": 735537390,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1685657267744,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					57.795938223137,
					1.2987662014001558
				]
			],
			"lastCommittedPoint": null,
			"startBinding": null,
			"endBinding": null,
			"startArrowhead": null,
			"endArrowhead": "arrow"
		},
		{
			"type": "freedraw",
			"version": 410,
			"versionNonce": 71936306,
			"isDeleted": true,
			"id": "s3owtlrDw_Sg7kSXGiR92",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 20,
			"angle": 0,
			"x": 1070.223793659009,
			"y": 34.94548194461555,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 39.51767340769008,
			"height": 33.12511315591161,
			"seed": 293263460,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862517,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-4.649158912747194,
					3.777436074398954
				],
				[
					-9.298273487829109,
					9.007706597990575
				],
				[
					-12.203986723879723,
					15.109722128763151
				],
				[
					-13.65684334190513,
					19.758858872677706
				],
				[
					-12.78512050355679,
					23.826861836915192
				],
				[
					-9.879407267506176,
					26.151419124456126
				],
				[
					-1.1622675593541343,
					26.44198601429466
				],
				[
					5.811426472101427,
					24.989129396269327
				],
				[
					18.88713603432949,
					17.724846306142616
				],
				[
					23.826839668082577,
					12.204008892712462
				],
				[
					25.860830065784953,
					4.068002964237487
				],
				[
					24.698562506430818,
					-0.8717006695156007
				],
				[
					21.792849270380106,
					-4.939703633753088
				],
				[
					14.237977121582198,
					-6.6831271416169535
				],
				[
					9.007728766823314,
					-6.39256025177842
				],
				[
					3.486847015727781,
					-4.939703633753088
				],
				[
					0.5811337796770671,
					-2.6151463462121307
				],
				[
					0.8717228383483393,
					3.1962801258892224
				],
				[
					0,
					0
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.212890625,
				0.2431640625,
				0.2841796875,
				0.3544921875,
				0.3994140625,
				0.4013671875,
				0.4033203125,
				0.3857421875,
				0.365234375,
				0.326171875,
				0.33984375,
				0.3740234375,
				0.4052734375,
				0.4384765625,
				0.48828125,
				0.4970703125,
				0.4970703125,
				0.4404296875,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 399,
			"versionNonce": 2103851758,
			"isDeleted": true,
			"id": "1ypE94xCFXdPXrW8ER53C",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 20,
			"angle": 0,
			"x": 1072.5483731153827,
			"y": 48.31175839668214,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 1.1622675593541343,
			"height": 12.78512050355684,
			"seed": 1895259876,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862517,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					-2.324557287540933
				],
				[
					0.29054472100589407,
					-3.486847015727731
				],
				[
					0.29054472100589407,
					-7.554849979965218
				],
				[
					0.29054472100589407,
					-9.879407267506176
				],
				[
					0.29054472100589407,
					-11.913419834041239
				],
				[
					0.29054472100589407,
					-12.78512050355684
				],
				[
					-0.5811337796770671,
					-10.460563216015908
				],
				[
					-0.8717228383482402,
					-8.717139708152041
				],
				[
					-0.8717228383482402,
					-8.717139708152041
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2109375,
				0.294921875,
				0.345703125,
				0.4814453125,
				0.5068359375,
				0.509765625,
				0.498046875,
				0.1767578125,
				0.01171875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 406,
			"versionNonce": 526496498,
			"isDeleted": true,
			"id": "UrHAibTv347Tebna7p6E5",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 20,
			"angle": 0,
			"x": 1093.4694995474147,
			"y": 41.91919814490376,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 23.24570588840551,
			"height": 0.8717006695156007,
			"seed": 1979652060,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862517,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-1.1622675593541343,
					-0.29056688983853357
				],
				[
					-1.7434456766965793,
					-0.29056688983853357
				],
				[
					-2.0339903977024734,
					-0.29056688983853357
				],
				[
					-1.1622675593541343,
					-0.29056688983853357
				],
				[
					0.8717228383482402,
					-0.29056688983853357
				],
				[
					3.486847015727682,
					0.29056688983853357
				],
				[
					10.16999632617735,
					0.5811337796770671
				],
				[
					13.947432400576304,
					0.5811337796770671
				],
				[
					16.562556577955746,
					0.5811337796770671
				],
				[
					18.88713603432939,
					0.5811337796770671
				],
				[
					19.75885887267763,
					0.29056688983853357
				],
				[
					20.921126432031766,
					0.29056688983853357
				],
				[
					21.21171549070304,
					0.29056688983853357
				],
				[
					20.63058171102597,
					0.29056688983853357
				],
				[
					20.049403593683525,
					0.29056688983853357
				],
				[
					20.049403593683525,
					0.29056688983853357
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2001953125,
				0.2607421875,
				0.2919921875,
				0.3095703125,
				0.4033203125,
				0.400390625,
				0.388671875,
				0.3828125,
				0.3828125,
				0.380859375,
				0.37109375,
				0.3662109375,
				0.3349609375,
				0.2744140625,
				0.04296875,
				0.0126953125,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 407,
			"versionNonce": 1190964526,
			"isDeleted": true,
			"id": "uCcglhpEcxT23emLL0_wR",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 20,
			"angle": 0,
			"x": 1110.6131899050474,
			"y": 49.764615014707545,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 15.981422798278777,
			"height": 15.40026684976902,
			"seed": 335585372,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862517,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					2.3245794563736464,
					-0.8717006695156007
				],
				[
					4.0680251330702255,
					-1.4528566180253568
				],
				[
					8.426594987146247,
					-3.486847015727756
				],
				[
					11.332308223196861,
					-4.939703633753088
				],
				[
					13.947432400576401,
					-6.392560251778445
				],
				[
					15.981422798278777,
					-7.2642830901267095
				],
				[
					15.40028901860171,
					-8.717139708152041
				],
				[
					13.366298620899334,
					-10.1699963261774
				],
				[
					11.332308223196861,
					-11.62285294420273
				],
				[
					9.007728766823314,
					-13.366276452066597
				],
				[
					6.102015530772601,
					-15.109699959930486
				],
				[
					4.939747971418466,
					-15.40026684976902
				],
				[
					3.4868913533931587,
					-15.40026684976902
				],
				[
					2.3245794563736464,
					-15.109699959930486
				],
				[
					2.0340347353677526,
					-14.528566180253419
				],
				[
					4.358569854076021,
					-13.65684334190513
				],
				[
					4.358569854076021,
					-13.65684334190513
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2568359375,
				0.2880859375,
				0.294921875,
				0.30859375,
				0.330078125,
				0.3349609375,
				0.3388671875,
				0.3642578125,
				0.419921875,
				0.470703125,
				0.4931640625,
				0.49609375,
				0.49609375,
				0.4775390625,
				0.3837890625,
				0.2333984375,
				0.0126953125,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 404,
			"versionNonce": 911377586,
			"isDeleted": true,
			"id": "aq8shratpsg--4XLFxfxo",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 20,
			"angle": 0,
			"x": 1149.2591848120546,
			"y": 50.055204073378775,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 7.5548278111325295,
			"height": 14.23799929041486,
			"seed": 1358623460,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862517,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-2.3245794563735473,
					-0.8717228383482649
				],
				[
					-4.067980795404749,
					-2.324579456373622
				],
				[
					-4.649114575081816,
					-2.9057132360506888
				],
				[
					-4.939703633753088,
					-4.358569854076021
				],
				[
					-3.486847015727682,
					-6.973716200288176
				],
				[
					-2.0339903977023743,
					-8.426572818313508
				],
				[
					-1.4528566180253073,
					-9.588862546500307
				],
				[
					-2.0339903977023743,
					-11.332286054364197
				],
				[
					-2.9057132360506146,
					-12.494575782550996
				],
				[
					-4.939703633753088,
					-13.656865510737795
				],
				[
					-6.392560251778395,
					-13.947432400576329
				],
				[
					-7.5548278111325295,
					-14.23799929041486
				],
				[
					-6.973694031455462,
					-13.656865510737795
				],
				[
					-6.973694031455462,
					-13.656865510737795
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2705078125,
				0.3203125,
				0.4111328125,
				0.4443359375,
				0.478515625,
				0.4677734375,
				0.4501953125,
				0.439453125,
				0.4619140625,
				0.48046875,
				0.49609375,
				0.49609375,
				0.49609375,
				0.015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 411,
			"versionNonce": 1904924526,
			"isDeleted": true,
			"id": "gCTaCByx_UYGGnS9zc8nv",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 20,
			"angle": 0,
			"x": 1133.2777620137758,
			"y": 27.39063196465034,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 40.97053002571539,
			"height": 31.381711816880436,
			"seed": 1718537956,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862517,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-6.973694031455562,
					6.101993361939886
				],
				[
					-9.007684429157935,
					8.717139708152041
				],
				[
					-11.332263885531583,
					15.40028901860166
				],
				[
					-10.169996326177449,
					20.33999265235475
				],
				[
					-5.811426472101427,
					23.826839668082503
				],
				[
					-0.8717228383483393,
					25.57028534477906
				],
				[
					12.494575782550996,
					26.151419124456126
				],
				[
					22.373983050057173,
					22.955138998566902
				],
				[
					26.732552904133193,
					19.17770292416795
				],
				[
					29.638266140183806,
					13.947432400576329
				],
				[
					29.34772141917801,
					4.939703633753088
				],
				[
					26.732552904133193,
					0
				],
				[
					23.536294947076584,
					-3.486847015727756
				],
				[
					17.434279416304083,
					-5.23029269242431
				],
				[
					11.622852944202656,
					-5.23029269242431
				],
				[
					1.7434456766964803,
					-2.615146346212155
				],
				[
					-0.29054472100589407,
					-1.4528566180253568
				],
				[
					-2.0339903977024734,
					0.8717228383482649
				],
				[
					-0.5811337796770671,
					4.939703633753088
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
				0.4287109375,
				0.4560546875,
				0.4931640625,
				0.49609375,
				0.4892578125,
				0.474609375,
				0.423828125,
				0.38671875,
				0.4013671875,
				0.4228515625,
				0.46484375,
				0.4873046875,
				0.505859375,
				0.5166015625,
				0.525390625,
				0.53515625,
				0.5283203125,
				0.439453125,
				0.015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 403,
			"versionNonce": 1656954482,
			"isDeleted": true,
			"id": "stVrtTbN3nDVNXqp3h9DB",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 20,
			"angle": 0,
			"x": 1162.3348943742826,
			"y": 36.10777167280236,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 32.25343465522872,
			"height": 0.8717228383482897,
			"seed": 1168904924,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862517,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.581133779677067,
					0
				],
				[
					1.162311897019512,
					0
				],
				[
					2.3245794563736464,
					-0.29056688983853357
				],
				[
					6.1020155307726,
					0
				],
				[
					9.298273487829109,
					-0.29056688983853357
				],
				[
					14.238021459247573,
					-0.29056688983853357
				],
				[
					19.758858872677727,
					-0.29056688983853357
				],
				[
					23.826839668082574,
					-0.5811337796770671
				],
				[
					28.76658763950094,
					-0.5811337796770671
				],
				[
					31.381711816880483,
					-0.8717228383482897
				],
				[
					32.25343465522872,
					-0.8717228383482897
				],
				[
					31.96284559655755,
					-0.5811337796770671
				],
				[
					31.96284559655755,
					-0.5811337796770671
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.193359375,
				0.2255859375,
				0.2529296875,
				0.2822265625,
				0.3603515625,
				0.3876953125,
				0.404296875,
				0.4169921875,
				0.4228515625,
				0.427734375,
				0.41796875,
				0.365234375,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 405,
			"versionNonce": 1968814510,
			"isDeleted": true,
			"id": "LcpO9XR6m8coWa2KlOLrU",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 20,
			"angle": 0,
			"x": 1191.1014820137834,
			"y": 42.20976503474236,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 20.049403593683625,
			"height": 17.14371252646555,
			"seed": 1226555748,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862517,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					3.7773917367336747,
					-1.1622897281867985
				],
				[
					7.845416869803802,
					-2.615146346212155
				],
				[
					10.169996326177449,
					-3.1962801258892224
				],
				[
					14.819110901259265,
					-4.649136743914554
				],
				[
					18.01541319598115,
					-6.101993361939886
				],
				[
					20.049403593683625,
					-8.717139708152041
				],
				[
					19.468269814006558,
					-11.332286054364197
				],
				[
					18.01541319598115,
					-13.366276452066597
				],
				[
					15.109699959930536,
					-14.528566180253394
				],
				[
					9.007684429157935,
					-15.981422798278752
				],
				[
					6.68310497278429,
					-16.562556577955817
				],
				[
					6.1019711931072225,
					-16.85312346779435
				],
				[
					5.811426472101427,
					-17.14371252646555
				],
				[
					7.845416869803802,
					-17.14371252646555
				],
				[
					7.845416869803802,
					-17.14371252646555
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2822265625,
				0.3046875,
				0.27734375,
				0.271484375,
				0.2763671875,
				0.2763671875,
				0.2802734375,
				0.2841796875,
				0.3349609375,
				0.4169921875,
				0.486328125,
				0.4931640625,
				0.4873046875,
				0.4345703125,
				0.0126953125,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 412,
			"versionNonce": 1903853618,
			"isDeleted": true,
			"id": "Dg8hAzaDvuBI3WGYzcwh0",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 20,
			"angle": 0,
			"x": 1212.8943312841634,
			"y": 40.466341526878466,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 11.332263885531583,
			"height": 20.92112643203184,
			"seed": 532470492,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862517,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.2905447210058941,
					0.29056688983853357
				],
				[
					1.7434013390312015,
					0.29056688983853357
				],
				[
					4.358569854076022,
					0.29056688983853357
				],
				[
					6.973694031455563,
					-0.29056688983853357
				],
				[
					10.460541047183245,
					-1.4528566180253568
				],
				[
					11.041674826860312,
					-2.324579456373622
				],
				[
					10.460541047183245,
					-3.486847015727756
				],
				[
					9.007684429157937,
					-4.649136743914554
				],
				[
					7.8454168698038025,
					-5.8114264721013775
				],
				[
					8.42655064948087,
					-7.554849979965243
				],
				[
					9.879407267506178,
					-9.298273487829109
				],
				[
					11.332263885531583,
					-11.041719164525663
				],
				[
					11.332263885531583,
					-13.65684334190513
				],
				[
					10.751130105854516,
					-15.981422798278752
				],
				[
					9.879407267506178,
					-18.306002254652373
				],
				[
					9.007684429157937,
					-20.04942576251624
				],
				[
					8.42655064948087,
					-20.630559542193307
				],
				[
					7.264283090126735,
					-20.04942576251624
				],
				[
					6.392560251778495,
					-18.88713603432944
				],
				[
					6.101971193107223,
					-16.853145636627016
				],
				[
					7.264283090126735,
					-15.400289018601685
				],
				[
					7.264283090126735,
					-15.400289018601685
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.1923828125,
				0.212890625,
				0.2666015625,
				0.3232421875,
				0.375,
				0.3916015625,
				0.3955078125,
				0.41796875,
				0.4267578125,
				0.447265625,
				0.482421875,
				0.4775390625,
				0.4716796875,
				0.4873046875,
				0.51171875,
				0.5234375,
				0.5234375,
				0.5234375,
				0.478515625,
				0.376953125,
				0.1806640625,
				0.0126953125,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 413,
			"versionNonce": 1502761966,
			"isDeleted": true,
			"id": "V_iIOBcBSAOOHBwIxYe5U",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 20,
			"angle": 0,
			"x": 1218.1245796389226,
			"y": 14.024355512583753,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 31.091122758209213,
			"height": 34.868558832608166,
			"seed": 259715292,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862517,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-3.196257957056509,
					0.8717006695156007
				],
				[
					-4.649114575081915,
					1.7434235078638656
				],
				[
					-5.811426472101328,
					3.1962801258891975
				],
				[
					-8.426550649480868,
					9.588840377667642
				],
				[
					-10.751130105854417,
					17.14371252646555
				],
				[
					-11.04167482686031,
					23.245705888405436
				],
				[
					-10.460541047183243,
					27.60427574248146
				],
				[
					-8.426550649480868,
					31.381689648047747
				],
				[
					-1.4528566180253073,
					33.996835994259875
				],
				[
					4.068025133070127,
					33.12513532474428
				],
				[
					10.16999632617735,
					30.80055586837068
				],
				[
					15.40028901860171,
					27.313708852642925
				],
				[
					18.01545753364653,
					23.245705888405436
				],
				[
					20.049447931348904,
					13.65684334190513
				],
				[
					19.468314151671837,
					6.973716200288152
				],
				[
					18.306002254652324,
					2.324557287540933
				],
				[
					15.981422798278777,
					-0.29056688983853357
				],
				[
					8.717139708152041,
					-0.8717228383482897
				],
				[
					4.939747971418466,
					0.29056688983853357
				],
				[
					3.777436074398954,
					1.1622897281867985
				],
				[
					1.7434456766965793,
					3.486847015727731
				],
				[
					0.5811781173424452,
					9.007706597990575
				],
				[
					0.5811781173424452,
					9.007706597990575
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.1611328125,
				0.2001953125,
				0.25390625,
				0.3017578125,
				0.37890625,
				0.408203125,
				0.412109375,
				0.4140625,
				0.4033203125,
				0.4013671875,
				0.416015625,
				0.4296875,
				0.4482421875,
				0.474609375,
				0.5146484375,
				0.515625,
				0.513671875,
				0.51953125,
				0.5341796875,
				0.5234375,
				0.5166015625,
				0.3916015625,
				0.0146484375,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 371,
			"versionNonce": 2120198642,
			"isDeleted": true,
			"id": "DKilvaHIkEsoUCZW6-Kp1",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 20,
			"angle": 0,
			"x": 1067.3180804229582,
			"y": 92.47861288595215,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 17.434279416304083,
			"height": 20.049425762516215,
			"seed": 704996580,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862517,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					0.29056688983853357
				],
				[
					-0.29058905867127216,
					0.29056688983853357
				],
				[
					-0.5811337796770671,
					0.29056688983853357
				],
				[
					-0.5811337796770671,
					0
				],
				[
					-0.29058905867127216,
					-1.1622897281868232
				],
				[
					0.8717228383482402,
					-2.905713236050664
				],
				[
					2.6151241773794416,
					-5.8114264721013775
				],
				[
					4.939703633753088,
					-10.1699963261774
				],
				[
					5.811426472101328,
					-13.075709562228063
				],
				[
					6.973694031455462,
					-14.819133070091953
				],
				[
					7.845416869803703,
					-15.981422798278727
				],
				[
					6.973694031455462,
					-17.14371252646555
				],
				[
					4.939703633753088,
					-18.01543536481384
				],
				[
					2.0339903977023743,
					-18.596569144490907
				],
				[
					-1.7434456766965793,
					-18.88713603432944
				],
				[
					-5.811426472101427,
					-19.468291982839148
				],
				[
					-9.007728766823314,
					-19.75885887267768
				],
				[
					-9.588862546500382,
					-19.75885887267768
				],
				[
					-9.588862546500382,
					-19.468291982839148
				],
				[
					-9.298273487829109,
					-18.596569144490907
				],
				[
					-7.554872148797908,
					-17.14371252646555
				],
				[
					-7.554872148797908,
					-17.14371252646555
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.1474609375,
				0.3408203125,
				0.380859375,
				0.4921875,
				0.5244140625,
				0.556640625,
				0.5576171875,
				0.5556640625,
				0.55078125,
				0.5439453125,
				0.5361328125,
				0.5302734375,
				0.5263671875,
				0.5263671875,
				0.537109375,
				0.5556640625,
				0.5693359375,
				0.576171875,
				0.5693359375,
				0.5185546875,
				0.3525390625,
				0.0146484375,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 408,
			"versionNonce": 1480435246,
			"isDeleted": true,
			"id": "ScPbeiY8wwQmfgzI4isV5",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 20,
			"angle": 0,
			"x": 1092.016642929389,
			"y": 82.30861655977475,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 28.47599858082977,
			"height": 5.230292692424261,
			"seed": 337489636,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862517,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.8717228383482402,
					0
				],
				[
					-1.4528566180253073,
					0
				],
				[
					-1.4528566180253073,
					-0.29056688983853357
				],
				[
					-1.1622675593541343,
					-0.29056688983853357
				],
				[
					0.29058905867127216,
					-1.162289728186774
				],
				[
					1.7434456766965793,
					-1.7434235078638411
				],
				[
					4.067980795404848,
					-2.0340125665350635
				],
				[
					6.973694031455562,
					-2.324579456373597
				],
				[
					11.332263885531583,
					-2.6151463462121307
				],
				[
					16.853145636627016,
					-3.4868691845604207
				],
				[
					20.3399926523548,
					-3.7774360743989543
				],
				[
					24.11742872675375,
					-4.358569854076022
				],
				[
					25.860830065784953,
					-4.358569854076022
				],
				[
					26.4420081831274,
					-4.649136743914555
				],
				[
					26.732552904133193,
					-4.649136743914555
				],
				[
					26.732552904133193,
					-4.939725802585728
				],
				[
					27.023141962804466,
					-5.230292692424261
				],
				[
					27.023141962804466,
					-5.230292692424261
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.173828125,
				0.234375,
				0.2890625,
				0.34765625,
				0.41796875,
				0.439453125,
				0.44921875,
				0.453125,
				0.4609375,
				0.466796875,
				0.466796875,
				0.46875,
				0.470703125,
				0.4736328125,
				0.4765625,
				0.470703125,
				0.0263671875,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 363,
			"versionNonce": 276405170,
			"isDeleted": true,
			"id": "BfQILAaaD7MTvt9g_S8nc",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 20,
			"angle": 0,
			"x": 1117.296339215497,
			"y": 84.63317384731573,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 13.366254283233857,
			"height": 15.109699959930486,
			"seed": 1750278628,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862517,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					-0.29056688983853357
				],
				[
					0.5811337796770671,
					-0.8717006695156007
				],
				[
					2.3245794563736464,
					-2.3245572875409577
				],
				[
					4.939703633753088,
					-3.7774139055662648
				],
				[
					10.46058538484862,
					-6.683127141616978
				],
				[
					10.751130105854417,
					-7.845416869803752
				],
				[
					9.298273487829109,
					-9.007706597990575
				],
				[
					6.683149310449667,
					-10.751130105854466
				],
				[
					4.068025133070127,
					-12.494553613718306
				],
				[
					0.8717228383482402,
					-14.528566180253419
				],
				[
					-1.1622675593541343,
					-14.819133070091953
				],
				[
					-2.6151241773794416,
					-14.819133070091953
				],
				[
					-0.8717228383482402,
					-15.109699959930486
				],
				[
					-0.8717228383482402,
					-15.109699959930486
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.3056640625,
				0.3388671875,
				0.3388671875,
				0.3310546875,
				0.318359375,
				0.2587890625,
				0.26953125,
				0.3076171875,
				0.4140625,
				0.48828125,
				0.515625,
				0.513671875,
				0.44140625,
				0.015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 413,
			"versionNonce": 38056046,
			"isDeleted": true,
			"id": "DxFmx8hXtZu_UJ9hXurvb",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 20,
			"angle": 0,
			"x": 1146.644060634675,
			"y": 82.30861655977475,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 13.366298620899236,
			"height": 21.502282380541573,
			"seed": 258473444,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862517,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.290589058671173,
					-0.5811559485097066
				],
				[
					-0.5811337796770671,
					-1.162289728186774
				],
				[
					-0.8717228383482402,
					-2.0340125665350635
				],
				[
					-0.5811337796770671,
					-4.068002964237488
				],
				[
					0.5811337796770671,
					-8.42657281831351
				],
				[
					1.1622675593541343,
					-11.622852944202707
				],
				[
					1.4528566180253073,
					-13.366276452066598
				],
				[
					1.4528566180253073,
					-13.947432400576306
				],
				[
					0.8717228383482402,
					-13.656865510737772
				],
				[
					-0.8717228383482402,
					-12.494575782550998
				],
				[
					-3.486847015727781,
					-11.91341983404124
				],
				[
					-7.264283090126734,
					-12.204008892712464
				],
				[
					-10.16999632617735,
					-13.656865510737772
				],
				[
					-11.913442002873929,
					-16.271989688117262
				],
				[
					-11.913442002873929,
					-18.01543536481382
				],
				[
					-11.622852944202755,
					-19.758858872677685
				],
				[
					-10.46058538484862,
					-20.921148600864505
				],
				[
					-8.717139708152041,
					-21.502282380541573
				],
				[
					-4.649158912747194,
					-21.502282380541573
				],
				[
					-2.6151685150448194,
					-21.21171549070304
				],
				[
					-0.290589058671173,
					-19.758858872677685
				],
				[
					0.5811337796770671,
					-18.596569144490886
				],
				[
					0.5811337796770671,
					-18.596569144490886
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.1904296875,
				0.412109375,
				0.4658203125,
				0.5009765625,
				0.5341796875,
				0.5478515625,
				0.5439453125,
				0.53125,
				0.5205078125,
				0.4833984375,
				0.4599609375,
				0.4638671875,
				0.490234375,
				0.517578125,
				0.546875,
				0.5517578125,
				0.5517578125,
				0.544921875,
				0.5380859375,
				0.5283203125,
				0.5263671875,
				0.3125,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 370,
			"versionNonce": 904877426,
			"isDeleted": true,
			"id": "7OCF_LxeTzar7fk_8yB04",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 20,
			"angle": 0,
			"x": 1131.2437716160734,
			"y": 56.44776432515715,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 35.44969261228523,
			"height": 38.064861127330055,
			"seed": 1272518748,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862517,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-4.939703633753088,
					7.2642830901267095
				],
				[
					-6.973694031455462,
					12.78514267238953
				],
				[
					-7.264283090126636,
					15.690855908440243
				],
				[
					-6.392560251778395,
					20.921126432031866
				],
				[
					-2.6151241773794416,
					25.57028534477906
				],
				[
					2.6151241773795406,
					29.638266140183905
				],
				[
					10.169996326177449,
					31.381711816880436
				],
				[
					15.40028901860171,
					30.509988978532146
				],
				[
					21.21171549070304,
					28.47599858082977
				],
				[
					25.57028534477906,
					24.407995616592284
				],
				[
					28.1854095221586,
					20.630559542193332
				],
				[
					27.604275742481533,
					11.622852944202755
				],
				[
					24.98915156510199,
					5.23029269242431
				],
				[
					20.63058171102597,
					-0.8717228383482649
				],
				[
					16.562556577955842,
					-4.358569854076021
				],
				[
					10.751130105854516,
					-6.683149310449618
				],
				[
					6.102015530772601,
					-6.101993361939886
				],
				[
					3.486847015727781,
					-4.358569854076021
				],
				[
					2.0339903977024734,
					2.324579456373622
				],
				[
					2.6151241773795406,
					6.683149310449643
				],
				[
					2.6151241773795406,
					6.683149310449643
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2880859375,
				0.3447265625,
				0.384765625,
				0.40625,
				0.44140625,
				0.44140625,
				0.4326171875,
				0.43359375,
				0.4365234375,
				0.4384765625,
				0.44921875,
				0.470703125,
				0.501953125,
				0.5205078125,
				0.5283203125,
				0.54296875,
				0.5595703125,
				0.5546875,
				0.5322265625,
				0.2373046875,
				0.0126953125,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 401,
			"versionNonce": 1668313774,
			"isDeleted": true,
			"id": "mt16E1B84ftjHat15TBFB",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 20,
			"angle": 0,
			"x": 1162.0443496532766,
			"y": 71.55746428508763,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 37.77427206865878,
			"height": 3.486847015727781,
			"seed": 1191088612,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862517,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.290544721005795,
					0.2905890586712226
				],
				[
					2.6151241773794416,
					0.5811559485097562
				],
				[
					6.392560251778395,
					0.8717228383482897
				],
				[
					10.751130105854417,
					0.8717228383482897
				],
				[
					17.14369035763281,
					0.8717228383482897
				],
				[
					25.860830065784853,
					0.2905890586712226
				],
				[
					31.67225653788628,
					-0.29056688983853357
				],
				[
					35.15910355361396,
					-1.1622675593541343
				],
				[
					37.77427206865878,
					-2.033990397702424
				],
				[
					37.77427206865878,
					-2.615124177379491
				],
				[
					37.77427206865878,
					-2.615124177379491
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.234375,
				0.2900390625,
				0.318359375,
				0.3486328125,
				0.365234375,
				0.3671875,
				0.380859375,
				0.3935546875,
				0.3984375,
				0.314453125,
				0.07421875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 408,
			"versionNonce": 537384754,
			"isDeleted": true,
			"id": "vzEjjtv1JTBVRNfMuxNi1",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 20,
			"angle": 0,
			"x": 1192.8448833528146,
			"y": 76.20662319783497,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 19.177725093000664,
			"height": 18.596569144490907,
			"seed": 1577023836,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862517,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-1.1622675593541343,
					0
				],
				[
					0.29058905867127216,
					-1.1622897281868232
				],
				[
					3.777436074398954,
					-3.1963022947218866
				],
				[
					5.23029269242436,
					-4.358569854076021
				],
				[
					10.169996326177449,
					-7.264283090126734
				],
				[
					13.075709562228063,
					-9.007728766823265
				],
				[
					14.238021459247575,
					-9.879429436338866
				],
				[
					14.238021459247575,
					-11.332286054364221
				],
				[
					12.785164841222267,
					-12.204008892712487
				],
				[
					9.298273487829109,
					-13.656865510737818
				],
				[
					5.811426472101427,
					-15.109722128763176
				],
				[
					3.1963022947218866,
					-16.562578746788507
				],
				[
					0,
					-18.01543536481384
				],
				[
					-1.7434013390312013,
					-18.596569144490907
				],
				[
					-3.777436074398954,
					-18.596569144490907
				],
				[
					-4.939703633753088,
					-18.01543536481384
				],
				[
					-4.358569854076021,
					-17.724868474975306
				],
				[
					-4.358569854076021,
					-17.724868474975306
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.212890625,
				0.30078125,
				0.4658203125,
				0.4775390625,
				0.4716796875,
				0.4599609375,
				0.4580078125,
				0.453125,
				0.455078125,
				0.4736328125,
				0.501953125,
				0.5283203125,
				0.54296875,
				0.5478515625,
				0.54296875,
				0.5029296875,
				0.3173828125,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 375,
			"versionNonce": 644476142,
			"isDeleted": true,
			"id": "yIRzLM8SySAMW-B-KXaPS",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 20,
			"angle": 0,
			"x": 1057.4386731554523,
			"y": 65.16490403330926,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 39.22712868668419,
			"height": 34.577991942769636,
			"seed": 377534044,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862517,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-1.7434456766965793,
					0.5811337796770671
				],
				[
					-2.9057132360507136,
					1.7434235078638904
				],
				[
					-3.777436074398954,
					2.61514634621218
				],
				[
					-5.811426472101427,
					5.8114264721013775
				],
				[
					-9.007728766823314,
					13.366276452066597
				],
				[
					-10.169996326177449,
					20.630559542193332
				],
				[
					-10.46058538484862,
					26.732552904133193
				],
				[
					-9.007728766823314,
					31.67227870671897
				],
				[
					-2.3245794563736464,
					34.577991942769636
				],
				[
					3.486847015727682,
					33.706269104421395
				],
				[
					10.460541047183243,
					30.80055586837068
				],
				[
					17.14369035763281,
					26.44198601429466
				],
				[
					23.24570588840541,
					22.955138998566927
				],
				[
					28.1854095221585,
					15.981422798278777
				],
				[
					28.76654330183557,
					11.332286054364221
				],
				[
					26.732552904133193,
					6.683149310449667
				],
				[
					23.536250609411304,
					2.61514634621218
				],
				[
					14.52856618025337,
					0.8717228383482897
				],
				[
					8.135961590809597,
					1.4528566180253568
				],
				[
					2.3245351187082686,
					4.068002964237487
				],
				[
					-1.1623118970195123,
					7.554849979965268
				],
				[
					-0.29058905867127216,
					12.494575782550996
				],
				[
					-0.29058905867127216,
					12.494575782550996
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2109375,
				0.240234375,
				0.27734375,
				0.30859375,
				0.376953125,
				0.4296875,
				0.4423828125,
				0.4443359375,
				0.44921875,
				0.4462890625,
				0.4521484375,
				0.45703125,
				0.443359375,
				0.4404296875,
				0.45703125,
				0.4736328125,
				0.486328125,
				0.50390625,
				0.5341796875,
				0.5458984375,
				0.54296875,
				0.5107421875,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 414,
			"versionNonce": 1059725554,
			"isDeleted": true,
			"id": "7_fekEmbIpWyhg8ShvZ-r",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 20,
			"angle": 0,
			"x": 1215.2188664028718,
			"y": 71.26689739524915,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 12.204031061545201,
			"height": 19.75883670384504,
			"seed": 45152100,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862517,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.5811781173424452,
					0.29056688983853357
				],
				[
					1.4528566180254063,
					0.29056688983853357
				],
				[
					2.9057132360507136,
					0.8717228383482897
				],
				[
					4.358569854076021,
					1.4528566180253568
				],
				[
					6.392604589443773,
					1.4528566180253568
				],
				[
					9.007728766823314,
					0.29056688983853357
				],
				[
					9.298317825494488,
					-1.4528566180253568
				],
				[
					8.426594987146247,
					-3.486847015727731
				],
				[
					6.9737383691208406,
					-5.230270523591622
				],
				[
					4.649158912747293,
					-6.973716200288176
				],
				[
					2.9057132360507136,
					-8.135983759642311
				],
				[
					1.4528566180254063,
					-9.298273487829109
				],
				[
					1.1623118970195123,
					-11.332286054364197
				],
				[
					1.1623118970195123,
					-14.237999290414885
				],
				[
					2.3245794563736464,
					-17.724846306142616
				],
				[
					2.6151685150448194,
					-18.305980085819684
				],
				[
					3.1963022947218866,
					-18.305980085819684
				],
				[
					4.358569854076021,
					-18.01541319598115
				],
				[
					6.9737383691208406,
					-17.434279416304083
				],
				[
					7.554872148797908,
					-17.14371252646555
				],
				[
					9.007728766823314,
					-16.562556577955817
				],
				[
					10.46058538484862,
					-15.690855908440218
				],
				[
					12.204031061545201,
					-14.237999290414885
				],
				[
					12.204031061545201,
					-14.237999290414885
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.185546875,
				0.232421875,
				0.263671875,
				0.3037109375,
				0.341796875,
				0.3671875,
				0.3720703125,
				0.3857421875,
				0.416015625,
				0.4658203125,
				0.5029296875,
				0.513671875,
				0.51953125,
				0.5234375,
				0.5234375,
				0.5234375,
				0.5322265625,
				0.55078125,
				0.5537109375,
				0.5517578125,
				0.544921875,
				0.501953125,
				0.341796875,
				0.0146484375,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 412,
			"versionNonce": 951721774,
			"isDeleted": true,
			"id": "KSLIaTGMJ5H7xzkY7i4j8",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 20,
			"angle": 0,
			"x": 1213.1848760051694,
			"y": 47.44005772716656,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 43.004564761083145,
			"height": 30.800555868370704,
			"seed": 1986245860,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862517,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-3.196257957056509,
					1.4528566180253568
				],
				[
					-8.42655064948087,
					5.8114264721013775
				],
				[
					-10.460541047183245,
					8.426572818313508
				],
				[
					-13.366254283233959,
					13.947410231743664
				],
				[
					-13.947432400576306,
					18.88713603432944
				],
				[
					-13.075709562228065,
					23.536272778243994
				],
				[
					-10.169996326177351,
					27.023119793971727
				],
				[
					-4.358569854076022,
					29.34769925034537
				],
				[
					0.8717228383482403,
					29.34769925034537
				],
				[
					7.264283090126735,
					28.475976411997085
				],
				[
					13.656843341905132,
					25.860852234617592
				],
				[
					20.049447931348904,
					21.502282380541573
				],
				[
					26.442008183127303,
					14.819133070091953
				],
				[
					29.05713236050684,
					9.298273487829109
				],
				[
					28.476042918495054,
					4.649136743914554
				],
				[
					25.860874403450236,
					1.1622897281868232
				],
				[
					19.758858872677735,
					-1.452856618025332
				],
				[
					13.366298620899238,
					-0.8717228383482649
				],
				[
					9.007728766823217,
					0.8717006695156007
				],
				[
					6.102015530772601,
					2.9057132360506888
				],
				[
					4.649158912747194,
					5.520859582262844
				],
				[
					4.649158912747194,
					5.520859582262844
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2548828125,
				0.2978515625,
				0.380859375,
				0.404296875,
				0.4580078125,
				0.4794921875,
				0.482421875,
				0.478515625,
				0.4697265625,
				0.4697265625,
				0.4677734375,
				0.4560546875,
				0.453125,
				0.47265625,
				0.482421875,
				0.494140625,
				0.501953125,
				0.5390625,
				0.5517578125,
				0.5537109375,
				0.53125,
				0.0146484375,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 407,
			"versionNonce": 1591554738,
			"isDeleted": true,
			"id": "NVtu9GVy7IpeOGJKHuazy",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 20,
			"angle": 0,
			"x": 1238.7551613499486,
			"y": 27.390654133483196,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 34.57796977393709,
			"height": 3.1962801258892224,
			"seed": 1348122460,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862517,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.5811337796770671,
					0
				],
				[
					-0.5811337796770671,
					-0.29056688983853357
				],
				[
					0,
					0
				],
				[
					1.7434456766966786,
					0.29056688983853357
				],
				[
					4.0680251330702255,
					0.5811337796770671
				],
				[
					7.264283090126834,
					1.1622897281868232
				],
				[
					12.785164841222267,
					1.7434235078638904
				],
				[
					16.27201185694995,
					1.7434235078638904
				],
				[
					20.339992652354898,
					1.7434235078638904
				],
				[
					24.698562506430918,
					1.7434235078638904
				],
				[
					27.604275742481533,
					1.7434235078638904
				],
				[
					30.80057803720342,
					2.033990397702424
				],
				[
					32.25343465522882,
					2.615146346212155
				],
				[
					32.54397937623462,
					2.615146346212155
				],
				[
					33.41570221458296,
					2.9057132360506888
				],
				[
					33.996835994260024,
					2.9057132360506888
				],
				[
					33.996835994260024,
					2.9057132360506888
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.1220703125,
				0.1796875,
				0.2470703125,
				0.37890625,
				0.3740234375,
				0.3740234375,
				0.3720703125,
				0.3720703125,
				0.38671875,
				0.3955078125,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.384765625,
				0.2822265625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 403,
			"versionNonce": 1858734446,
			"isDeleted": true,
			"id": "KIegBf3hNsJ9pH8zBHCfU",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 20,
			"angle": 0,
			"x": 1268.684016548803,
			"y": 34.0737812751002,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 13.075709562228063,
			"height": 14.819133070091953,
			"seed": 736472036,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862517,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					3.1963022947218866,
					-1.7434235078638904
				],
				[
					6.3925602517784945,
					-2.9057132360506888
				],
				[
					9.298273487829109,
					-4.067980795404823
				],
				[
					11.622852944202855,
					-5.520837413430155
				],
				[
					13.075709562228063,
					-6.973694031455512
				],
				[
					11.913442002873929,
					-8.426550649480845
				],
				[
					9.879407267506176,
					-9.588840377667642
				],
				[
					6.683149310449767,
					-11.332263885531534
				],
				[
					1.7434456766966786,
					-13.366276452066597
				],
				[
					0.29058905867127216,
					-14.237977121582198
				],
				[
					1.1622675593541343,
					-14.528566180253419
				],
				[
					4.067980795404947,
					-14.819133070091953
				],
				[
					4.067980795404947,
					-14.819133070091953
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.244140625,
				0.28125,
				0.3154296875,
				0.353515625,
				0.3701171875,
				0.3857421875,
				0.4052734375,
				0.462890625,
				0.498046875,
				0.5185546875,
				0.5166015625,
				0.2900390625,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 414,
			"versionNonce": 1103629426,
			"isDeleted": true,
			"id": "EJJUukaZKfHk2zd49MR5X",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 20,
			"angle": 0,
			"x": 1290.1862767605126,
			"y": 30.877501149210985,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 13.656887679570408,
			"height": 15.981422798278752,
			"seed": 2130850780,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862517,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.5811337796770671,
					0
				],
				[
					-0.5811337796770671,
					-0.29056688983853357
				],
				[
					-0.2905447210059932,
					0
				],
				[
					0.871722838348141,
					0.29056688983853357
				],
				[
					2.0340347353677526,
					0.29056688983853357
				],
				[
					3.777436074398954,
					0
				],
				[
					6.102015530772501,
					-1.1622897281867985
				],
				[
					6.392604589443773,
					-2.615146346212155
				],
				[
					5.230292692424162,
					-3.7774139055662896
				],
				[
					3.4868913533929606,
					-4.939703633753088
				],
				[
					0.871722838348141,
					-6.39256025177842
				],
				[
					-0.2905447210059932,
					-7.554849979965243
				],
				[
					-1.1622675593541343,
					-9.588840377667642
				],
				[
					-1.4528566180254063,
					-11.332286054364197
				],
				[
					-1.4528566180254063,
					-12.494553613718331
				],
				[
					-1.1622675593541343,
					-13.65684334190513
				],
				[
					-0.5811337796770671,
					-14.23799929041486
				],
				[
					0.871722838348141,
					-14.819133070091928
				],
				[
					2.9057132360506146,
					-15.400266849768995
				],
				[
					6.9737383691208406,
					-15.690855908440218
				],
				[
					9.588862546500183,
					-15.400266849768995
				],
				[
					11.04171916452559,
					-15.109699959930461
				],
				[
					12.204031061545003,
					-14.528566180253394
				],
				[
					12.204031061545003,
					-14.528566180253394
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.173828125,
				0.2177734375,
				0.2802734375,
				0.4140625,
				0.427734375,
				0.4384765625,
				0.4521484375,
				0.47265625,
				0.48046875,
				0.48828125,
				0.4970703125,
				0.4970703125,
				0.5078125,
				0.521484375,
				0.5244140625,
				0.5244140625,
				0.5302734375,
				0.5439453125,
				0.552734375,
				0.5546875,
				0.5546875,
				0.5146484375,
				0.3857421875,
				0.0146484375,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 410,
			"versionNonce": 669166510,
			"isDeleted": true,
			"id": "lOsXAVKPoM7h363TEt7RB",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 20,
			"angle": 0,
			"x": 1292.5108562168862,
			"y": 5.016648914593388,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 31.091122758209213,
			"height": 27.02314196280439,
			"seed": 618999388,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1685655862517,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-4.067980795404749,
					1.7434456766965547
				],
				[
					-7.554827811132629,
					5.520859582262819
				],
				[
					-9.007684429157838,
					8.136005928474974
				],
				[
					-10.751130105854516,
					13.656865510737795
				],
				[
					-10.460541047183243,
					19.17772509300064
				],
				[
					-7.554827811132629,
					22.955138998566902
				],
				[
					-0.8717228383483393,
					25.279718454940525
				],
				[
					4.649158912747293,
					24.98915156510199
				],
				[
					10.460585384848523,
					23.53629494707666
				],
				[
					14.528566180253469,
					20.339992652354773
				],
				[
					18.306002254652423,
					15.981422798278752
				],
				[
					20.3399926523547,
					8.717139708152041
				],
				[
					17.724868474975356,
					2.9057132360506888
				],
				[
					14.238021459247475,
					-0.29056688983853357
				],
				[
					10.751130105854516,
					-1.7434235078638656
				],
				[
					2.6151685150448194,
					-0.5811337796770671
				],
				[
					-0.8717228383483393,
					1.1622897281867985
				],
				[
					-2.6151241773795406,
					3.777436074398954
				],
				[
					-2.0339903977024734,
					9.00772876682324
				],
				[
					-2.0339903977024734,
					9.00772876682324
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2509765625,
				0.33203125,
				0.3916015625,
				0.4140625,
				0.439453125,
				0.4453125,
				0.4521484375,
				0.4443359375,
				0.4541015625,
				0.4658203125,
				0.4775390625,
				0.4912109375,
				0.501953125,
				0.5107421875,
				0.513671875,
				0.51953125,
				0.51953125,
				0.513671875,
				0.423828125,
				0.015625,
				0
			]
		},
		{
			"id": "pjEuQZpf",
			"type": "text",
			"x": 583.8319406981773,
			"y": 305.16846701770385,
			"width": 10,
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
			"seed": 1118550254,
			"version": 3,
			"versionNonce": 2051183406,
			"isDeleted": true,
			"boundElements": null,
			"updated": 1685655862521,
			"link": null,
			"locked": false,
			"text": "",
			"rawText": "",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "left",
			"verticalAlign": "top",
			"baseline": 17,
			"containerId": null,
			"originalText": "",
			"lineHeight": 1.25
		},
		{
			"id": "fmAanhMXCXyV-vLD2Z3Zf",
			"type": "line",
			"x": 842.5581704125798,
			"y": 361.59402691114457,
			"width": 54.548973174881894,
			"height": 5.195163895110113,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 20,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"seed": 50124846,
			"version": 24,
			"versionNonce": 89799922,
			"isDeleted": true,
			"boundElements": null,
			"updated": 1685656252266,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					54.548973174881894,
					5.195163895110113
				]
			],
			"lastCommittedPoint": null,
			"startBinding": null,
			"endBinding": null,
			"startArrowhead": null,
			"endArrowhead": null
		},
		{
			"id": "MQZfDI1-g936wgVkPQLyk",
			"type": "freedraw",
			"x": 830.2196437755047,
			"y": 418.74063157833643,
			"width": 116.2413090917288,
			"height": 75.32957921056732,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 20,
			"groupIds": [],
			"roundness": null,
			"seed": 1110033198,
			"version": 28,
			"versionNonce": 1668042098,
			"isDeleted": true,
			"boundElements": null,
			"updated": 1685656262256,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-1.2987662014002126,
					0.6493831006999926
				],
				[
					-2.5975324028003115,
					0.6493831006999926
				],
				[
					1.9481988468548934,
					-1.948198846855007
				],
				[
					9.09146249931041,
					-7.143313197210318
				],
				[
					18.183024088130423,
					-17.53364098743043
				],
				[
					38.96358057906116,
					-31.17088428115096
				],
				[
					51.95144077208158,
					-41.56116252661627
				],
				[
					66.2380671665021,
					-50.652674570681484
				],
				[
					77.92716115812232,
					-57.146604667191696
				],
				[
					89.61625514974264,
					-62.34171901754701
				],
				[
					100.65591649590806,
					-68.83564911405722
				],
				[
					105.85108039101817,
					-71.43323106161222
				],
				[
					109.74737899521858,
					-73.38142990846723
				],
				[
					112.99434404347369,
					-74.03081300916733
				],
				[
					113.64377668892848,
					-74.68019610986732
				],
				[
					112.99434404347369,
					-74.03081300916733
				],
				[
					112.34501048752838,
					-73.38142990846723
				],
				[
					112.34501048752838,
					-72.73204680776712
				],
				[
					111.69557784207359,
					-72.08261416231232
				],
				[
					111.69557784207359,
					-70.78384796091223
				],
				[
					111.04624428612829,
					-68.83564911405722
				],
				[
					111.04624428612829,
					-68.18626601335711
				],
				[
					109.09804543927328,
					-65.58868406580211
				],
				[
					109.09804543927328,
					-65.58868406580211
				]
			],
			"pressures": [
				0.17578125,
				0.1943359375,
				0.1943359375,
				0.2294921875,
				0.259765625,
				0.2685546875,
				0.255859375,
				0.25390625,
				0.25390625,
				0.25390625,
				0.255859375,
				0.2744140625,
				0.298828125,
				0.3232421875,
				0.337890625,
				0.341796875,
				0.396484375,
				0.396484375,
				0.39453125,
				0.3818359375,
				0.3720703125,
				0.345703125,
				0.3193359375,
				0.013671875,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				109.09804543927328,
				-65.58868406580211
			]
		},
		{
			"id": "5lI9mIFEbikusVfh9Vxlo",
			"type": "freedraw",
			"x": 937.3694903679232,
			"y": 374.58193664891985,
			"width": 71.43323106161233,
			"height": 62.9911516630018,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 20,
			"groupIds": [],
			"roundness": null,
			"seed": 308214446,
			"version": 25,
			"versionNonce": 1742588014,
			"isDeleted": true,
			"boundElements": null,
			"updated": 1685656293920,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.6494326454549082,
					0
				],
				[
					-3.246965048255106,
					0.6494326454549082
				],
				[
					-6.493930096510212,
					3.8963976937099005
				],
				[
					-11.689093991620211,
					11.689093991620325
				],
				[
					-16.23482524127553,
					22.079372237085636
				],
				[
					-24.02752153918584,
					36.36604817626096
				],
				[
					-28.57335187835065,
					50.652674570681484
				],
				[
					-27.92391923289574,
					58.445420413346596
				],
				[
					-23.378187983240537,
					62.9911516630018
				],
				[
					-11.03966134616553,
					62.34171901754701
				],
				[
					-2.5976314923098016,
					57.146604667191696
				],
				[
					9.09146249931041,
					48.055092623126484
				],
				[
					18.183024088130423,
					39.61301322451607
				],
				[
					25.32628774058594,
					33.119083128005855
				],
				[
					29.87201899024126,
					29.87211807975075
				],
				[
					33.118984038496365,
					27.92391923289574
				],
				[
					35.06718288535126,
					27.27453613219575
				],
				[
					37.66481437766106,
					27.27453613219575
				],
				[
					39.61291413500658,
					27.92391923289574
				],
				[
					42.85987918326168,
					29.222685434295954
				],
				[
					42.85987918326168,
					29.222685434295954
				]
			],
			"pressures": [
				0.232421875,
				0.2568359375,
				0.265625,
				0.2900390625,
				0.3154296875,
				0.3544921875,
				0.4033203125,
				0.4326171875,
				0.451171875,
				0.4560546875,
				0.4541015625,
				0.4560546875,
				0.470703125,
				0.4833984375,
				0.486328125,
				0.486328125,
				0.4833984375,
				0.455078125,
				0.3955078125,
				0.291015625,
				0.013671875,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				42.85987918326168,
				29.222685434295954
			]
		},
		{
			"id": "ggPRwZOqZbLTX7vmO_ApO",
			"type": "freedraw",
			"x": 1017.8941839288459,
			"y": 379.12771744332986,
			"width": 34.41784932940595,
			"height": 54.549022719636696,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 20,
			"groupIds": [],
			"roundness": null,
			"seed": 457699954,
			"version": 26,
			"versionNonce": 1679015282,
			"isDeleted": true,
			"boundElements": null,
			"updated": 1685656293920,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-1.2987662014002126,
					-0.6493831007001063
				],
				[
					-4.545731249655319,
					1.298766201400099
				],
				[
					-9.091462499310524,
					5.844546995810106
				],
				[
					-21.429989136385643,
					18.83240718883053
				],
				[
					-27.923919232895855,
					29.222685434295954
				],
				[
					-32.46965048255106,
					37.66476483290637
				],
				[
					-34.41784932940595,
					43.50931182871648
				],
				[
					-33.118984038496365,
					47.40565997767169
				],
				[
					-28.57325278884116,
					48.055092623126484
				],
				[
					-23.378088893731046,
					44.15869492941658
				],
				[
					-12.987860193020424,
					35.716615530806166
				],
				[
					-10.390228700710622,
					32.46965048255106
				],
				[
					-6.493930096510212,
					26.62510348674084
				],
				[
					-5.195163895110113,
					19.481790289530636
				],
				[
					-6.493930096510212,
					18.83240718883053
				],
				[
					-11.03966134616553,
					22.728755337785742
				],
				[
					-19.481790289530636,
					29.222685434295954
				],
				[
					-25.326287740586054,
					35.06723243010606
				],
				[
					-28.57325278884116,
					40.91172988116148
				],
				[
					-29.87201899024126,
					47.40565997767169
				],
				[
					-29.222685434295954,
					53.89963961893659
				],
				[
					-29.222685434295954,
					53.89963961893659
				]
			],
			"pressures": [
				0.2109375,
				0.2431640625,
				0.287109375,
				0.3427734375,
				0.4541015625,
				0.4912109375,
				0.49609375,
				0.49609375,
				0.4990234375,
				0.4931640625,
				0.4853515625,
				0.4814453125,
				0.4765625,
				0.4697265625,
				0.4599609375,
				0.455078125,
				0.46484375,
				0.4580078125,
				0.4453125,
				0.4111328125,
				0.2958984375,
				0.013671875,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				-29.222685434295954,
				53.89963961893659
			]
		},
		{
			"id": "Y8ErEb1VAbK7DuBQB8vBI",
			"type": "freedraw",
			"x": 995.814861236515,
			"y": 407.7010197769257,
			"width": 30.521550725205543,
			"height": 18.183024088130423,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 20,
			"groupIds": [],
			"roundness": null,
			"seed": 2054428530,
			"version": 24,
			"versionNonce": 1713801902,
			"isDeleted": true,
			"boundElements": null,
			"updated": 1685656293920,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-1.948198846855007,
					1.298766201400099
				],
				[
					-3.246965048255106,
					2.5975324028003115
				],
				[
					-5.195163895110113,
					3.246965048255106
				],
				[
					-0.6494326454547945,
					1.9481493021002052
				],
				[
					11.039661346165417,
					-3.8963976937099005
				],
				[
					16.884158797220834,
					-8.442128943365105
				],
				[
					20.780556490930735,
					-12.338477092320318
				],
				[
					24.02752153918584,
					-14.936059039875317
				],
				[
					24.676954184640636,
					-14.936059039875317
				],
				[
					22.079322692330948,
					-14.286675939175325
				],
				[
					18.183024088130537,
					-12.338477092320318
				],
				[
					12.33842754756563,
					-8.442128943365105
				],
				[
					0.6493335559453044,
					-3.246965048255106
				],
				[
					-4.545731249655205,
					-0.6494326454547945
				],
				[
					-5.844596540564908,
					0.6493831007001063
				],
				[
					-5.195163895110113,
					0.6493831007001063
				],
				[
					2.5975324028003115,
					-1.948198846855007
				],
				[
					7.143263652455516,
					-3.246965048255106
				],
				[
					13.637193748965728,
					-4.545780794410007
				],
				[
					13.637193748965728,
					-4.545780794410007
				]
			],
			"pressures": [
				0.2880859375,
				0.3193359375,
				0.3251953125,
				0.3466796875,
				0.3271484375,
				0.3076171875,
				0.291015625,
				0.287109375,
				0.287109375,
				0.287109375,
				0.28125,
				0.3076171875,
				0.34765625,
				0.3857421875,
				0.416015625,
				0.423828125,
				0.3603515625,
				0.2509765625,
				0.1904296875,
				0.0126953125,
				0
			],
			"simulatePressure": false,
			"lastCommittedPoint": [
				13.637193748965728,
				-4.545780794410007
			]
		},
		{
			"id": "dMNHvrsSNAUo2Kw0Tf2-Y",
			"type": "rectangle",
			"x": 1094.5225788855682,
			"y": 356.3989621055441,
			"width": 63.64053476370191,
			"height": 55.1984058203368,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 20,
			"groupIds": [],
			"roundness": {
				"type": 3
			},
			"seed": 77324978,
			"version": 22,
			"versionNonce": 1566523186,
			"isDeleted": true,
			"boundElements": null,
			"updated": 1685656293920,
			"link": null,
			"locked": false
		},
		{
			"id": "-HYxKWc0QHARpDaAqX32F",
			"type": "rectangle",
			"x": 1155.5654821569601,
			"y": 392.1155776363503,
			"width": 27.92391923289597,
			"height": 88.96682250428785,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 20,
			"groupIds": [],
			"roundness": {
				"type": 3
			},
			"seed": 92113970,
			"version": 12,
			"versionNonce": 446498030,
			"isDeleted": true,
			"boundElements": null,
			"updated": 1685656293920,
			"link": null,
			"locked": false
		},
		{
			"id": "_9gmWvhE_Mduqa9dcxCrg",
			"type": "rectangle",
			"x": 1075.0407885960376,
			"y": 418.09129802239113,
			"width": 120.7871394308936,
			"height": 44.808078030116576,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 20,
			"groupIds": [],
			"roundness": {
				"type": 3
			},
			"seed": 868592882,
			"version": 12,
			"versionNonce": 760514802,
			"isDeleted": true,
			"boundElements": null,
			"updated": 1685656293920,
			"link": null,
			"locked": false
		},
		{
			"id": "Z4PxENQOjrvMvyTsKUk_4",
			"type": "rectangle",
			"x": 1078.2877536442925,
			"y": 419.3900642237912,
			"width": 87.01862365743318,
			"height": 77.27782760217713,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 20,
			"groupIds": [],
			"roundness": {
				"type": 3
			},
			"seed": 1159812530,
			"version": 12,
			"versionNonce": 1724528430,
			"isDeleted": true,
			"boundElements": null,
			"updated": 1685656293920,
			"link": null,
			"locked": false
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
		"scrollX": -472.2112771811997,
		"scrollY": 170.0963634925524,
		"zoom": {
			"value": 0.6159598179459269
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