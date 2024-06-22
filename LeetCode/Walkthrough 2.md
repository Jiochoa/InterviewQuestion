---

excalidraw-plugin: parsed
tags: [excalidraw]

---
==⚠  Switch to EXCALIDRAW VIEW in the MORE OPTIONS menu of this document. ⚠==


# Text Elements
IMPLEMENTATION ^txKTVQEb

[[LeetCode/Questions#Solution 10]] ^qFvkk2O0

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

## 13. Roman to integer
 ^spAe4fUE

IMPLEMENTATION ^9ZsQSZiN

[[LeetCode/Questions#Solution 13]] ^vIIJuhXv

INFO ^YOFe7PZX

Convert the given S: string (Roman numerals) 
to an answer: Int.
- S.len => 1 to 15 (I V X L C D M)
- answer just an int

> int romanToInt(String s) < ^kHg1rOYI

EXAMLES ^OWEbgxFz

Input: s = "LVIII"
Output: 58
Explanation: L = 50, V= 5, III = 3. ^xROFJMiH

Input: s = "MCMXCIV"
Output: 1994
Explanation: M = 1000, CM = 900, XC = 90 and IV = 4. ^rr5oev45

WALKTHROUGH ^s65aHWDz

- specialCase: map
- numeral: map
- answer: int
- iterate sChars
    - if 2 or more chars remain
        - if next 2 are specialCase
            - answer += specialCase
            - i + 2
            - continue
    - if is numeral
        - answer += numeral.get(s[i])
        - i + 1
    - else return null
- retrun answer ^brFQf6wz

## 17. Letter Combination of a Phone Number
 ^uBlrd7yo

INFO ^61AXDvGo

Retrutn all possible letter combination that the given number could represent

digits beween 0 and 4

> public List<String> letterCombination (String digits) < ^pXQgceEH

EXAMPLE ^bVUePlAd

digits = "23"
output = [ "ab", "ae", "af", "bd", "be", "cd", "ce", "cf" ] ^ok86lQOx

WALKTHROUGH ^RPb75Unv

- make hashmap of all digits
- if  ^5WlIRxAq

## 20. Valid Parentheses
 ^Z5okNo6b

IMPLEMENTATION ^9KNdFl5M

[[LeetCode/Questions#Solution 20]] ^RodWzksg

INFO ^p7xeRQ3m

determine if the string is valid
valid if:
- same closing an open brackets
- correct order
- corresponding brackets
cons: s.len is from 1 to 10^4

> boolean isValid(Srting s) < ^gqCaUXKC

EXAMPLE ^arsWtfvc

Input: s = "()[]{}"
Output: true ^gD0Spuvj

WALKTHROUGH ^yPZGGe5u

- if (s[0] is opener) 
    - currOpener = s[0]
- else 
    - return false
- iterate s
    - if s[i] is opener
        - currOpener = next
    - if s[i] is correspondingCloser(curropener)
        - delete currentOpener and s[i]
        - start over 
    - else
        - return false
- return true ^XKzBRoaq

%%
# Drawing
```json
{
	"type": "excalidraw",
	"version": 2,
	"source": "https://github.com/zsviczian/obsidian-excalidraw-plugin/releases/tag/2.0.23",
	"elements": [
		{
			"type": "text",
			"version": 595,
			"versionNonce": 1094230137,
			"isDeleted": false,
			"id": "txKTVQEb",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1805.7992422992102,
			"y": -800.7021016768164,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 189,
			"height": 25,
			"seed": 1835354865,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955739214,
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
			"baseline": 18
		},
		{
			"type": "text",
			"version": 666,
			"versionNonce": 1981819225,
			"isDeleted": false,
			"id": "qFvkk2O0",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1830.429224552232,
			"y": -759.9985161025539,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 380,
			"height": 25,
			"seed": 625001681,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955739214,
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
			"baseline": 18
		},
		{
			"type": "line",
			"version": 337,
			"versionNonce": 987993657,
			"isDeleted": false,
			"id": "hhZnwOSQtTqhUSlXC3vdk",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1296.6017712556559,
			"y": -856.297760335354,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 0,
			"height": 2065.5999145507812,
			"seed": 1783089111,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1718955739214,
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
			"version": 105,
			"versionNonce": 1919313689,
			"isDeleted": false,
			"id": "FC6Kc4U1",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1381.0050548546733,
			"y": -804.0294060689876,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 351,
			"height": 50,
			"seed": 1040924217,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955739214,
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
			"baseline": 43
		},
		{
			"type": "text",
			"version": 140,
			"versionNonce": 1461459961,
			"isDeleted": false,
			"id": "EaF72K9B",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1325.2547801964702,
			"y": -697.7739649785703,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 50,
			"height": 25,
			"seed": 1457119321,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955739214,
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
			"baseline": 18
		},
		{
			"type": "text",
			"version": 448,
			"versionNonce": 151532761,
			"isDeleted": false,
			"id": "QS6xixLZ",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1388.504806899351,
			"y": -656.0239535344786,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 424,
			"height": 250,
			"seed": 749339543,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955739214,
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
			"baseline": 243
		},
		{
			"type": "text",
			"version": 128,
			"versionNonce": 1539191225,
			"isDeleted": false,
			"id": "iC30sz9z",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1322.7547611229838,
			"y": -381.02401075493765,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 91,
			"height": 25,
			"seed": 259953625,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955739214,
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
			"baseline": 18
		},
		{
			"type": "text",
			"version": 183,
			"versionNonce": 1684116121,
			"isDeleted": false,
			"id": "bv4ytyYR",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1380.504776381773,
			"y": -319.5239764226622,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 539,
			"height": 75,
			"seed": 465097559,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955739214,
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
			"baseline": 68
		},
		{
			"type": "text",
			"version": 104,
			"versionNonce": 1202050937,
			"isDeleted": false,
			"id": "VuknZj0n",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1379.254776381773,
			"y": -184.5239764226622,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 611,
			"height": 100,
			"seed": 12733655,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955739214,
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
			"baseline": 93
		},
		{
			"type": "text",
			"version": 128,
			"versionNonce": 1204715609,
			"isDeleted": false,
			"id": "3ErbVFPg",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1384.5067590352364,
			"y": -49.156230312351624,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 618,
			"height": 75,
			"seed": 769943159,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955739214,
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
			"baseline": 68
		},
		{
			"type": "text",
			"version": 113,
			"versionNonce": 313462073,
			"isDeleted": false,
			"id": "DQp9SlhM",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1336.5067637302436,
			"y": 86.22829117202303,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 149,
			"height": 25,
			"seed": 34518777,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955739214,
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
			"baseline": 18
		},
		{
			"type": "text",
			"version": 113,
			"versionNonce": 1336606233,
			"isDeleted": false,
			"id": "OKLnofNr",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1842.6606098840894,
			"y": 103.1513680951,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 151,
			"height": 25,
			"seed": 1034549529,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955739214,
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
			"baseline": 18
		},
		{
			"type": "line",
			"version": 448,
			"versionNonce": 1840632569,
			"isDeleted": false,
			"id": "gPEmd2mqkbrFzy3jB7CWK",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2274.800234180323,
			"y": -817.445490605526,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 0,
			"height": 2065.5999145507812,
			"seed": 1664362724,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1718955739214,
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
			"version": 103,
			"versionNonce": 827526105,
			"isDeleted": false,
			"id": "7E6maRv2",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2354.198237091314,
			"y": -758.3625893575628,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 334,
			"height": 50,
			"seed": 1479951332,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955739214,
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
			"baseline": 43
		},
		{
			"type": "text",
			"version": 647,
			"versionNonce": 43395257,
			"isDeleted": false,
			"id": "TsBS2I7U",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2820.38330699996,
			"y": -754.7144050328776,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 189,
			"height": 25,
			"seed": 1993477476,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955739214,
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
			"baseline": 18
		},
		{
			"type": "text",
			"version": 724,
			"versionNonce": 2065869209,
			"isDeleted": false,
			"id": "xcIGUIFU",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2845.01328925298,
			"y": -714.0108194586152,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 371,
			"height": 25,
			"seed": 192069860,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955739214,
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
			"baseline": 18
		},
		{
			"type": "text",
			"version": 177,
			"versionNonce": 875302521,
			"isDeleted": false,
			"id": "1wV7KCko",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2321.298134203479,
			"y": -656.4126033084556,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 50,
			"height": 25,
			"seed": 1524031460,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955739214,
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
			"baseline": 18
		},
		{
			"type": "text",
			"version": 367,
			"versionNonce": 1417008985,
			"isDeleted": false,
			"id": "BC6F8C7t",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2379.7684691053937,
			"y": -589.2653130681783,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 458,
			"height": 200,
			"seed": 1176142564,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955739214,
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
			"baseline": 193
		},
		{
			"type": "text",
			"version": 118,
			"versionNonce": 1582531641,
			"isDeleted": false,
			"id": "lMxKPcvf",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2322.054170312146,
			"y": -340.4081963689595,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 91,
			"height": 25,
			"seed": 626437340,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955739214,
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
			"baseline": 18
		},
		{
			"type": "text",
			"version": 161,
			"versionNonce": 1034458393,
			"isDeleted": false,
			"id": "zEW3vNBp",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2387.4827461003742,
			"y": -269.83673292029863,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 560,
			"height": 125,
			"seed": 239320028,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955739214,
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
			"baseline": 118
		},
		{
			"type": "text",
			"version": 145,
			"versionNonce": 367561209,
			"isDeleted": false,
			"id": "JFj5GE8o",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2330.3711113463705,
			"y": 234.44117758472407,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 149,
			"height": 25,
			"seed": 756031332,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955739214,
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
			"baseline": 18
		},
		{
			"type": "text",
			"version": 235,
			"versionNonce": 1343677145,
			"isDeleted": false,
			"id": "DNPxkTHc",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2350.371242135994,
			"y": 597.6794123317477,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 151,
			"height": 25,
			"seed": 2075437412,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955739214,
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
			"baseline": 18
		},
		{
			"type": "text",
			"version": 391,
			"versionNonce": 1757880249,
			"isDeleted": false,
			"id": "M0prJgM1",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2360.5468152043077,
			"y": 339.9911856109585,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 502,
			"height": 200,
			"seed": 11511709,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955739214,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "// iterate heights (start at the ends)\n- maxArea = 0\n- while startIndex < endIndex \n    - currArea = endIndex - startIndex \n      * min(heights[startIndex], heights[endIndex])\n    - if currArea > currMaxArea\n        - maxAea = currArea\n- return MaxArea",
			"rawText": "// iterate heights (start at the ends)\n- maxArea = 0\n- while startIndex < endIndex \n    - currArea = endIndex - startIndex \n      * min(heights[startIndex], heights[endIndex])\n    - if currArea > currMaxArea\n        - maxAea = currArea\n- return MaxArea",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "// iterate heights (start at the ends)\n- maxArea = 0\n- while startIndex < endIndex \n    - currArea = endIndex - startIndex \n      * min(heights[startIndex], heights[endIndex])\n    - if currArea > currMaxArea\n        - maxAea = currArea\n- return MaxArea",
			"lineHeight": 1.25,
			"baseline": 193
		},
		{
			"type": "text",
			"version": 280,
			"versionNonce": 2115813529,
			"isDeleted": false,
			"id": "FvKJ5cc8",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2437.657614357964,
			"y": 669.5469174902983,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 235,
			"height": 75,
			"seed": 1009336083,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955739214,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "maxArea = 0\nstartIndex = 0\nendIndex = height.len - 1",
			"rawText": "maxArea = 0\nstartIndex = 0\nendIndex = height.len - 1",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "maxArea = 0\nstartIndex = 0\nendIndex = height.len - 1",
			"lineHeight": 1.25,
			"baseline": 68
		},
		{
			"type": "rectangle",
			"version": 496,
			"versionNonce": 499860857,
			"isDeleted": false,
			"id": "SNcSW2i5ZSYGKZwrOqK0q",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2429.6020452390403,
			"y": 761.7691193674682,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 306,
			"height": 35,
			"seed": 1313911677,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "ri3wmAZC"
				}
			],
			"updated": 1718955739214,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 467,
			"versionNonce": 1393962585,
			"isDeleted": false,
			"id": "ri3wmAZC",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2439.6020452390403,
			"y": 766.7691193674682,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 286,
			"height": 25,
			"seed": 997919581,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955739214,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "while startIndex < endIndex ",
			"rawText": "while startIndex < endIndex ",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "SNcSW2i5ZSYGKZwrOqK0q",
			"originalText": "while startIndex < endIndex ",
			"lineHeight": 1.25,
			"baseline": 18
		},
		{
			"type": "line",
			"version": 299,
			"versionNonce": 1959852857,
			"isDeleted": false,
			"id": "DsyZAFioMJYqauwhsYhSf",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2455.213241121196,
			"y": 798.4358063791869,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 0,
			"height": 221.99996948242267,
			"seed": 23788339,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1718955739214,
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
					221.99996948242267
				]
			]
		},
		{
			"type": "line",
			"version": 348,
			"versionNonce": 861875225,
			"isDeleted": false,
			"id": "1m6wc7V3HziW_P5l-2bk2",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2736.5465541094773,
			"y": 775.0072364038338,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 253.14307803199245,
			"height": 0,
			"seed": 397046685,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1718955739214,
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
					253.14307803199245,
					0
				]
			]
		},
		{
			"type": "text",
			"version": 314,
			"versionNonce": 1723089145,
			"isDeleted": false,
			"id": "knDqSQjd",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2520.5465947995826,
			"y": 832.4357962066615,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 430,
			"height": 50,
			"seed": 691864787,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955739214,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "curArea = (endIndex - startIndex) \n* min (height[startIndex], height[endIndex])",
			"rawText": "curArea = (endIndex - startIndex) \n* min (height[startIndex], height[endIndex])",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "curArea = (endIndex - startIndex) \n* min (height[startIndex], height[endIndex])",
			"lineHeight": 1.25,
			"baseline": 43
		},
		{
			"type": "rectangle",
			"version": 292,
			"versionNonce": 475249113,
			"isDeleted": false,
			"id": "BmBBitO2LhhlJJMoPcNyt",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2528.8799789955465,
			"y": 908.9358012929245,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 260,
			"height": 35,
			"seed": 1577029053,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "lnfT11Nh"
				}
			],
			"updated": 1718955739214,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 309,
			"versionNonce": 1699813049,
			"isDeleted": false,
			"id": "lnfT11Nh",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2552.3799789955465,
			"y": 913.9358012929245,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 213,
			"height": 25,
			"seed": 28472349,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955739214,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "if curArea > maxArea",
			"rawText": "if curArea > maxArea",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "BmBBitO2LhhlJJMoPcNyt",
			"originalText": "if curArea > maxArea",
			"lineHeight": 1.25,
			"baseline": 18
		},
		{
			"type": "arrow",
			"version": 781,
			"versionNonce": 1595743383,
			"isDeleted": false,
			"id": "ICvtQYaCdaGax5EUXcANu",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2557.8446112266265,
			"y": 943.8881720727793,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 90.81473782986723,
			"height": 36.52220574021226,
			"seed": 1449810269,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "Qpaygbid"
				}
			],
			"updated": 1718955739439,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": {
				"elementId": "eTlcueKy",
				"focus": -0.8351715477706242,
				"gap": 10.648973212398232
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
					90.81473782986723,
					36.52220574021226
				]
			]
		},
		{
			"type": "text",
			"version": 162,
			"versionNonce": 1137797303,
			"isDeleted": false,
			"id": "Qpaygbid",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 7335.18319369636,
			"y": 1364.100604621229,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 16,
			"height": 25,
			"seed": 165862803,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955723341,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "T",
			"rawText": "T",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "ICvtQYaCdaGax5EUXcANu",
			"originalText": "T",
			"lineHeight": 1.25,
			"baseline": 18
		},
		{
			"type": "text",
			"version": 469,
			"versionNonce": 461601913,
			"isDeleted": false,
			"id": "eTlcueKy",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2659.308322268892,
			"y": 968.1501037192174,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 193,
			"height": 25,
			"seed": 80307965,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [
				{
					"id": "ICvtQYaCdaGax5EUXcANu",
					"type": "arrow"
				}
			],
			"updated": 1718955739214,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "maxArea = cueArea",
			"rawText": "maxArea = cueArea",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "maxArea = cueArea",
			"lineHeight": 1.25,
			"baseline": 18
		},
		{
			"type": "line",
			"version": 377,
			"versionNonce": 757559865,
			"isDeleted": false,
			"id": "8Sz-pHCDh7qYxIwlJFu4q",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2457.2134140541393,
			"y": 1018.4357555165577,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 530.7619149344282,
			"height": 0,
			"seed": 1098097149,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1718955739214,
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
					530.7619149344282,
					0
				]
			]
		},
		{
			"type": "line",
			"version": 334,
			"versionNonce": 667861785,
			"isDeleted": false,
			"id": "1Khb0gkam4sW4OO4PCXSK",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2992.261072338644,
			"y": 1020.2452880453898,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 0,
			"height": 248.66666158040368,
			"seed": 907181459,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1718955739214,
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
					-248.66666158040368
				]
			]
		},
		{
			"type": "rectangle",
			"version": 353,
			"versionNonce": 1998125049,
			"isDeleted": false,
			"id": "ReYgHt40JfzsQymkbVMRg",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2470.7133123288795,
			"y": 1062.1024577870658,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 182,
			"height": 35,
			"seed": 1082216797,
			"groupIds": [
				"egYVYmNrpBaM5TJqKh5By"
			],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "IGDlEbPR"
				}
			],
			"updated": 1718955739214,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 363,
			"versionNonce": 1292472537,
			"isDeleted": false,
			"id": "IGDlEbPR",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2485.2133123288795,
			"y": 1067.1024577870658,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 153,
			"height": 25,
			"seed": 1709325107,
			"groupIds": [
				"egYVYmNrpBaM5TJqKh5By"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955739214,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "return maxArea",
			"rawText": "return maxArea",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "ReYgHt40JfzsQymkbVMRg",
			"originalText": "return maxArea",
			"lineHeight": 1.25,
			"baseline": 18
		},
		{
			"type": "rectangle",
			"version": 301,
			"versionNonce": 1328811449,
			"isDeleted": false,
			"id": "EX_0b3-orrBJf_XqSHloh",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2464.546686352317,
			"y": 1053.7691091949432,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 195.33340454101562,
			"height": 53.33333333333326,
			"seed": 140661043,
			"groupIds": [
				"egYVYmNrpBaM5TJqKh5By"
			],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1718955739214,
			"link": null,
			"locked": false
		},
		{
			"type": "line",
			"version": 480,
			"versionNonce": 616296089,
			"isDeleted": false,
			"id": "rRa7yQsNrz1bDOyxh2m5z",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3282.2528096731867,
			"y": -840.7526858378556,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 0,
			"height": 2065.5999145507812,
			"seed": 1905218035,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1718955739214,
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
			"type": "line",
			"version": 505,
			"versionNonce": 457900569,
			"isDeleted": false,
			"id": "zVdLsq3qf0zwJiZ6H_tRp",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3438.7479122921777,
			"y": -882.8801217636676,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 881.4284722369223,
			"height": 0,
			"seed": 1734513050,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1718955787975,
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
					881.4284722369223,
					0
				]
			]
		},
		{
			"type": "text",
			"version": 101,
			"versionNonce": 1320507129,
			"isDeleted": false,
			"id": "spAe4fUE",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3437.8904822938566,
			"y": -755.869020709519,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 243,
			"height": 50,
			"seed": 1365347034,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787975,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "## 13. Roman to integer\n",
			"rawText": "## 13. Roman to integer\n",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "## 13. Roman to integer\n",
			"lineHeight": 1.25,
			"baseline": 43
		},
		{
			"type": "text",
			"version": 274,
			"versionNonce": 1338118105,
			"isDeleted": false,
			"id": "9ZsQSZiN",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3895.5203874130684,
			"y": -782.7361108249122,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 189,
			"height": 25,
			"seed": 1064135046,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787975,
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
			"baseline": 18
		},
		{
			"type": "text",
			"version": 339,
			"versionNonce": 75803833,
			"isDeleted": false,
			"id": "vIIJuhXv",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3878.89044790103,
			"y": -736.4786306654303,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 380,
			"height": 25,
			"seed": 1381124294,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787975,
			"link": "[[LeetCode/Questions#Solution 13]]",
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "📍[[LeetCode/Questions#Solution 13]]",
			"rawText": "[[LeetCode/Questions#Solution 13]]",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "📍[[LeetCode/Questions#Solution 13]]",
			"lineHeight": 1.25,
			"baseline": 18
		},
		{
			"type": "text",
			"version": 123,
			"versionNonce": 1151380889,
			"isDeleted": false,
			"id": "YOFe7PZX",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3431.3189335897387,
			"y": -663.9327578824482,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 50,
			"height": 25,
			"seed": 1914993754,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787975,
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
			"baseline": 18
		},
		{
			"type": "text",
			"version": 239,
			"versionNonce": 659133049,
			"isDeleted": false,
			"id": "kHg1rOYI",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3469.3188962904765,
			"y": -615.2660708707294,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 448,
			"height": 150,
			"seed": 1890359194,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787975,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Convert the given S: string (Roman numerals) \nto an answer: Int.\n- S.len => 1 to 15 (I V X L C D M)\n- answer just an int\n\n> int romanToInt(String s) <",
			"rawText": "Convert the given S: string (Roman numerals) \nto an answer: Int.\n- S.len => 1 to 15 (I V X L C D M)\n- answer just an int\n\n> int romanToInt(String s) <",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Convert the given S: string (Roman numerals) \nto an answer: Int.\n- S.len => 1 to 15 (I V X L C D M)\n- answer just an int\n\n> int romanToInt(String s) <",
			"lineHeight": 1.25,
			"baseline": 143
		},
		{
			"type": "text",
			"version": 127,
			"versionNonce": 289594201,
			"isDeleted": false,
			"id": "OWEbgxFz",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3433.763340734921,
			"y": -412.599410985747,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 90,
			"height": 25,
			"seed": 1496226202,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787975,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "EXAMLES",
			"rawText": "EXAMLES",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "EXAMLES",
			"lineHeight": 1.25,
			"baseline": 18
		},
		{
			"type": "text",
			"version": 68,
			"versionNonce": 48236601,
			"isDeleted": false,
			"id": "xROFJMiH",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3493.5411388577504,
			"y": -298.15496654130266,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 352,
			"height": 75,
			"seed": 1522618310,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787975,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Input: s = \"LVIII\"\nOutput: 58\nExplanation: L = 50, V= 5, III = 3.",
			"rawText": "Input: s = \"LVIII\"\nOutput: 58\nExplanation: L = 50, V= 5, III = 3.",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Input: s = \"LVIII\"\nOutput: 58\nExplanation: L = 50, V= 5, III = 3.",
			"lineHeight": 1.25,
			"baseline": 68
		},
		{
			"type": "freedraw",
			"version": 206,
			"versionNonce": 637835545,
			"isDeleted": false,
			"id": "Uyk-Ax_gDUit1GMB8HSjY",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3790.7189438244704,
			"y": -34.54991160697682,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 16.42720597204479,
			"height": 23.870757363837384,
			"seed": 843098566,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787975,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.5133416191831324,
					3.5934500824643307
				],
				[
					0.256690392319067,
					8.983615414796864
				],
				[
					-0.5133416191831324,
					15.657154377814924
				],
				[
					-1.0266832383661992,
					18.73726284109632
				],
				[
					-1.5400248575493316,
					20.790648900556253
				],
				[
					-2.0534056421874656,
					22.330693340832987
				],
				[
					-2.310056869051531,
					23.357396161926783
				],
				[
					-2.310056869051531,
					23.614066971518252
				],
				[
					-2.566747261370598,
					23.870757363837384
				],
				[
					-2.310056869051531,
					23.870757363837384
				],
				[
					-0.25665122686406544,
					23.100725352335317
				],
				[
					4.363462511238996,
					22.330693340832987
				],
				[
					6.6735585457455295,
					22.074022531241518
				],
				[
					8.21358340329486,
					22.074022531241518
				],
				[
					8.726964187932994,
					22.074022531241518
				],
				[
					10.010337818618327,
					22.074022531241518
				],
				[
					11.293711449303593,
					21.817351721649786
				],
				[
					12.320394687669857,
					21.56068091205832
				],
				[
					13.860458710674191,
					21.04731971014772
				],
				[
					13.860458710674191,
					21.04731971014772
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.3203125,
				0.46875,
				0.5263671875,
				0.5537109375,
				0.5625,
				0.5703125,
				0.5810546875,
				0.5859375,
				0.5859375,
				0.6005859375,
				0.6220703125,
				0.61328125,
				0.611328125,
				0.609375,
				0.609375,
				0.609375,
				0.5703125,
				0.4833984375,
				0.283203125,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 192,
			"versionNonce": 472124921,
			"isDeleted": false,
			"id": "LoUeY4nB1br7xRH3Uay-x",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3812.0229539269376,
			"y": -24.796264180677554,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 12.577045914533857,
			"height": 1.283373630685266,
			"seed": 1389040006,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787975,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1.5400640230043332,
					-0.7700320115023307
				],
				[
					4.620152903558064,
					-1.283373630685266
				],
				[
					10.523679437801393,
					-1.283373630685266
				],
				[
					11.293672283848592,
					-1.0267028210937985
				],
				[
					12.577045914533857,
					-0.25669039231913265
				],
				[
					12.577045914533857,
					-0.25669039231913265
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.296875,
				0.4853515625,
				0.55859375,
				0.5791015625,
				0.5712890625,
				0.3681640625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 194,
			"versionNonce": 205645529,
			"isDeleted": false,
			"id": "68H5XtKadvIqiTM-vFQcd",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3818.953163699547,
			"y": -34.03656998779388,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 2.0534056421874656,
			"height": 17.453889210411052,
			"seed": 2120949382,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787975,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					6.160197343834863
				],
				[
					0.256690392319067,
					9.753647426299194
				],
				[
					1.0267224038212006,
					12.320394687669989
				],
				[
					1.0267224038212006,
					13.603768318355256
				],
				[
					1.5400640230043332,
					15.65717396054259
				],
				[
					1.7967152498683985,
					17.197218400819587
				],
				[
					2.0534056421874656,
					17.453889210411052
				],
				[
					2.0534056421874656,
					17.453889210411052
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.3740234375,
				0.498046875,
				0.5419921875,
				0.55078125,
				0.55078125,
				0.5048828125,
				0.283203125,
				0.0673828125,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 208,
			"versionNonce": 1894884281,
			"isDeleted": false,
			"id": "7HEmWGHX-RrejNIa_v_fG",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3833.070273637085,
			"y": -36.85998805875579,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 13.60376831835519,
			"height": 20.020616889054182,
			"seed": 1473787398,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787975,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					0.7700320115020681
				],
				[
					0.5133416191831324,
					3.5934500824643307
				],
				[
					1.5400640230043987,
					7.1869001649286615
				],
				[
					2.0534056421875313,
					8.726944605205395
				],
				[
					3.85012089205593,
					13.603768318354993
				],
				[
					4.876843295877197,
					15.913844770134057
				],
				[
					5.646836141924329,
					17.71056002000252
				],
				[
					6.1602169265624624,
					18.73726284109632
				],
				[
					6.4168681534265275,
					18.993933650687786
				],
				[
					6.673558545745594,
					19.250604460279256
				],
				[
					6.930209772609595,
					19.507275269870984
				],
				[
					6.930209772609595,
					19.250604460279256
				],
				[
					7.700241784111794,
					18.22390163918572
				],
				[
					8.98361541479706,
					15.657154377814924
				],
				[
					10.266989045482392,
					11.807033485759126
				],
				[
					11.293711449303657,
					7.443570974520129
				],
				[
					13.090426699172056,
					0.2566708095914677
				],
				[
					13.347077926036057,
					-0.5133416191831981
				],
				[
					13.60376831835519,
					-0.5133416191831981
				],
				[
					13.347077926036057,
					-0.25667080959173033
				],
				[
					12.320394687669857,
					0.5133612019106003
				],
				[
					12.320394687669857,
					0.5133612019106003
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.333984375,
				0.4853515625,
				0.517578125,
				0.5361328125,
				0.541015625,
				0.5517578125,
				0.560546875,
				0.568359375,
				0.5771484375,
				0.580078125,
				0.583984375,
				0.5908203125,
				0.5947265625,
				0.5966796875,
				0.6025390625,
				0.599609375,
				0.595703125,
				0.544921875,
				0.541015625,
				0.537109375,
				0.2490234375,
				0.0126953125,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 196,
			"versionNonce": 643220633,
			"isDeleted": false,
			"id": "-13RYgn1ELiDcDm49c91x",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3853.3476005011853,
			"y": -27.876372643959257,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 12.833736306852924,
			"height": 0.2566708095914677,
			"seed": 1823087878,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787975,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.513380784638134,
					0
				],
				[
					0.7699928460471323,
					-0.2566708095914677
				],
				[
					3.8501208920558643,
					-0.2566708095914677
				],
				[
					8.21358340329486,
					0
				],
				[
					10.01029865316326,
					0
				],
				[
					11.036981891529525,
					0
				],
				[
					11.807013903031658,
					-0.2566708095914677
				],
				[
					12.06370429535079,
					-0.2566708095914677
				],
				[
					12.32035552221479,
					-0.2566708095914677
				],
				[
					12.32035552221479,
					-0.2566708095914677
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.3662109375,
				0.4970703125,
				0.5361328125,
				0.5546875,
				0.5546875,
				0.5595703125,
				0.55859375,
				0.5361328125,
				0.4609375,
				0.34765625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 195,
			"versionNonce": 941934969,
			"isDeleted": false,
			"id": "xjL7GeEk6h9gSuHDVTFa9",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3857.7110630124243,
			"y": -36.08995604725396,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 3.336779272872797,
			"height": 13.347077926036123,
			"seed": 28188806,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787975,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1.283373630685266,
					5.903506951515993
				],
				[
					1.5400248575493316,
					6.930209772609529
				],
				[
					2.310056869051531,
					8.470254212886525
				],
				[
					2.566747261370598,
					10.010318235890924
				],
				[
					2.8233984882345977,
					11.037001474257059
				],
				[
					3.0800888805536646,
					12.320375104942324
				],
				[
					3.336779272872797,
					13.090407116444654
				],
				[
					3.336779272872797,
					13.347077926036123
				],
				[
					3.336779272872797,
					13.347077926036123
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.4189453125,
				0.52734375,
				0.5439453125,
				0.5615234375,
				0.56640625,
				0.56640625,
				0.5185546875,
				0.345703125,
				0.2900390625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 196,
			"versionNonce": 1872704089,
			"isDeleted": false,
			"id": "UVl_eReBg75444_A3aaZl",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3885.431941268318,
			"y": -19.406098848344755,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 1.7967152498683985,
			"height": 27.464207446301977,
			"seed": 732793498,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-1.5400640230043987,
					-7.956912593703327
				],
				[
					-1.0267224038212663,
					-13.603768318355256
				],
				[
					-0.513380784638134,
					-16.42718638931752
				],
				[
					-0.256690392319067,
					-23.870757363837647
				],
				[
					-0.256690392319067,
					-26.694175434799646
				],
				[
					0,
					-27.464207446301977
				],
				[
					0,
					-27.207517053982844
				],
				[
					0,
					-24.640769792612314
				],
				[
					0.25665122686399977,
					-20.02063647178185
				],
				[
					0.25665122686399977,
					-20.02063647178185
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.3662109375,
				0.55078125,
				0.5634765625,
				0.5654296875,
				0.5654296875,
				0.5546875,
				0.5400390625,
				0.494140625,
				0.375,
				0.0146484375,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 192,
			"versionNonce": 563707705,
			"isDeleted": false,
			"id": "QOE34-OZjW_8LOtW04tE1",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3876.961667472704,
			"y": -47.38364791382992,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 7.956893010975859,
			"height": 5.390165332332795,
			"seed": 1257197338,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1.7967152498684642,
					-0.2566708095914677
				],
				[
					3.0800888805537303,
					-0.5133416191829354
				],
				[
					4.876804130422129,
					-0.2566708095914677
				],
				[
					6.673519380290528,
					0
				],
				[
					7.956893010975859,
					4.87682371314986
				],
				[
					7.956893010975859,
					4.87682371314986
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.3359375,
				0.5029296875,
				0.5263671875,
				0.5263671875,
				0.4951171875,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 193,
			"versionNonce": 1014444057,
			"isDeleted": false,
			"id": "nowsKclRAAcNCl7EVvS-w",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3876.704977080385,
			"y": -14.78596552751469,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 13.090426699172056,
			"height": 2.566747261370532,
			"seed": 189395482,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					5.903526534243396,
					-1.0266832383661335
				],
				[
					7.443590557247728,
					-1.5400444402769966
				],
				[
					10.010337818618327,
					-2.3100568690516625
				],
				[
					11.807053068486725,
					-2.566747261370532
				],
				[
					12.83373630685299,
					-2.3100568690516625
				],
				[
					13.090426699172056,
					-1.7967152498684642
				],
				[
					13.090426699172056,
					-1.7967152498684642
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.4111328125,
				0.5078125,
				0.51171875,
				0.5205078125,
				0.5234375,
				0.4365234375,
				0.015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 192,
			"versionNonce": 371967225,
			"isDeleted": false,
			"id": "qaIjzz5FHUOvTkl-6Iarf",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3899.549051205856,
			"y": -30.956461524512633,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 12.32035552221479,
			"height": 3.080108463281395,
			"seed": 1224728966,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					3.593430499736797,
					-0.513361201910863
				],
				[
					6.930209772609595,
					-1.0267028210937985
				],
				[
					10.523640272346391,
					-1.7967348325961292
				],
				[
					11.550362676167659,
					-2.053405642187597
				],
				[
					12.32035552221479,
					-3.080108463281395
				],
				[
					12.32035552221479,
					-3.080108463281395
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.345703125,
				0.5,
				0.517578125,
				0.517578125,
				0.5078125,
				0.0146484375,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 193,
			"versionNonce": 2050670041,
			"isDeleted": false,
			"id": "qjuuIg-LPQAXBvIEWyOzf",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3906.2225705861465,
			"y": -39.68340612971815,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 0.7700320115021337,
			"height": 13.603768318355256,
			"seed": 196603526,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.7700320115021337,
					4.363462511238996
				],
				[
					-0.7700320115021337,
					5.390165332332795
				],
				[
					-0.5133416191830668,
					8.213583403294795
				],
				[
					-0.5133416191830668,
					10.52365985507386
				],
				[
					-0.7700320115021337,
					12.320394687669989
				],
				[
					-0.7700320115021337,
					13.603768318355256
				],
				[
					-0.7700320115021337,
					13.603768318355256
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.4072265625,
				0.5146484375,
				0.5224609375,
				0.5361328125,
				0.537109375,
				0.45703125,
				0.015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 196,
			"versionNonce": 2008521401,
			"isDeleted": false,
			"id": "XiSr-iIgzYHW-o8aJwl4_",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3929.579986330801,
			"y": -18.892757229161816,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 3.0800888805536646,
			"height": 33.36771439781771,
			"seed": 537552858,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.5133416191831324,
					-4.6201333208304645
				],
				[
					0.25665122686406544,
					-7.443570974520129
				],
				[
					0.25665122686406544,
					-14.887122366312857
				],
				[
					0,
					-17.71056002000252
				],
				[
					-0.256690392319067,
					-23.87073778110998
				],
				[
					-0.5133416191830668,
					-28.74756149425958
				],
				[
					-0.5133416191830668,
					-31.82766995754071
				],
				[
					-0.5133416191830668,
					-33.36771439781771
				],
				[
					-2.566747261370532,
					-32.34101157672391
				],
				[
					-2.566747261370532,
					-32.34101157672391
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2509765625,
				0.4580078125,
				0.5322265625,
				0.5859375,
				0.5986328125,
				0.607421875,
				0.59765625,
				0.5537109375,
				0.453125,
				0.015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 191,
			"versionNonce": 1866849177,
			"isDeleted": false,
			"id": "ZehGI1k3B64PLVitkvYLP",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3922.9064277850557,
			"y": -51.4904396154775,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 12.83373630685299,
			"height": 3.850120892056061,
			"seed": 936721498,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					6.930209772609595,
					-1.5400444402769966
				],
				[
					10.780330664665458,
					-2.053405642187597
				],
				[
					11.807053068486725,
					-2.053405642187597
				],
				[
					12.83373630685299,
					1.7967152498684642
				],
				[
					12.83373630685299,
					1.7967152498684642
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.447265625,
				0.54296875,
				0.54296875,
				0.53125,
				0.0146484375,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 190,
			"versionNonce": 1629028473,
			"isDeleted": false,
			"id": "mQ544b_zHkAt8aaTXU9Vh",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3927.0132390694307,
			"y": -17.35271278888513,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 6.930209772609529,
			"height": 2.3100568690516625,
			"seed": 431614982,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					5.390145749605196,
					-1.7967152498684642
				],
				[
					6.416868153426462,
					-2.3100568690516625
				],
				[
					6.930209772609529,
					-1.5400444402769966
				],
				[
					6.930209772609529,
					-1.5400444402769966
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.4306640625,
				0.51953125,
				0.47265625,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 192,
			"versionNonce": 2062846297,
			"isDeleted": false,
			"id": "645rTzmFTeiwL2-Rmg36m",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3942.927064256837,
			"y": -36.60331724916432,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 6.930209772609529,
			"height": 1.540044440276734,
			"seed": 1661788614,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					3.0800888805536646,
					0
				],
				[
					4.363462511238996,
					0
				],
				[
					5.90352653424333,
					-0.5133416191831981
				],
				[
					6.930209772609529,
					-0.7700124287746658
				],
				[
					6.416868153426462,
					-1.540044440276734
				],
				[
					6.416868153426462,
					-1.540044440276734
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.3974609375,
				0.494140625,
				0.5078125,
				0.4873046875,
				0.2353515625,
				0.0126953125,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 191,
			"versionNonce": 1714157113,
			"isDeleted": false,
			"id": "2I5Va-iGmWvo_qVYppmS-",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3945.2371211258887,
			"y": -41.73681177190565,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 1.2833736306853318,
			"height": 13.603768318354993,
			"seed": 1008914118,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.5133807846381996,
					4.876823713149597
				],
				[
					1.0267224038212663,
					8.470273795613927
				],
				[
					1.2833736306853318,
					11.550362676167659
				],
				[
					1.2833736306853318,
					13.603768318354993
				],
				[
					1.2833736306853318,
					13.603768318354993
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.3818359375,
				0.5224609375,
				0.525390625,
				0.419921875,
				0.015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 198,
			"versionNonce": 1436731161,
			"isDeleted": false,
			"id": "-NXestAciW5Y7jlK6B6HP",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3958.070857432742,
			"y": -22.742878121217927,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 3.593430499736797,
			"height": 29.26092269617018,
			"seed": 831829722,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.513380784638134,
					-0.7700124287746658
				],
				[
					1.0267224038212663,
					-3.0800888805537303
				],
				[
					1.5400640230043332,
					-5.903506951515993
				],
				[
					1.5400640230043332,
					-11.807033485759126
				],
				[
					1.283373630685266,
					-16.427186389317256
				],
				[
					1.0267224038212663,
					-22.33069334083325
				],
				[
					0.7700320115021337,
					-26.437485042480514
				],
				[
					0.513380784638134,
					-29.00423230385131
				],
				[
					0.513380784638134,
					-29.26092269617018
				],
				[
					-0.5133416191831324,
					-27.97754906548491
				],
				[
					-2.053366476732464,
					-26.437485042480514
				],
				[
					-2.053366476732464,
					-26.437485042480514
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2255859375,
				0.4365234375,
				0.5068359375,
				0.544921875,
				0.5830078125,
				0.5966796875,
				0.609375,
				0.609375,
				0.599609375,
				0.5380859375,
				0.349609375,
				0.0146484375,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 193,
			"versionNonce": 1405910009,
			"isDeleted": false,
			"id": "RhSvLVcdR0lcj3nQxSMaU",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3948.317249171898,
			"y": -50.720427186702636,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 12.320355522214856,
			"height": 2.3100764517790644,
			"seed": 661245978,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					4.876804130422129,
					-0.25667080959173033
				],
				[
					7.18686099947366,
					-0.25667080959173033
				],
				[
					10.010298653163325,
					0
				],
				[
					11.807013903031724,
					0.5133612019106003
				],
				[
					12.320355522214856,
					1.0267028210937985
				],
				[
					11.807013903031724,
					2.053405642187334
				],
				[
					11.807013903031724,
					2.053405642187334
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.4365234375,
				0.5390625,
				0.5458984375,
				0.5498046875,
				0.5126953125,
				0.36328125,
				0.0146484375,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 194,
			"versionNonce": 1353487577,
			"isDeleted": false,
			"id": "lVO3cmS6NsgclzT3_QtPd",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3952.937362910001,
			"y": -21.45950449053271,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 13.603768318355124,
			"height": 1.283373630685266,
			"seed": 2051269510,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					4.876843295877131,
					-1.0267028210937985
				],
				[
					6.416868153426462,
					-1.283373630685266
				],
				[
					10.266989045482326,
					-1.283373630685266
				],
				[
					11.807053068486725,
					-1.0267028210937985
				],
				[
					12.833736306852924,
					-0.7700124287746658
				],
				[
					13.347117091491123,
					-0.5133416191831981
				],
				[
					13.603768318355124,
					0
				],
				[
					13.603768318355124,
					0
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.3203125,
				0.4765625,
				0.498046875,
				0.5107421875,
				0.5126953125,
				0.453125,
				0.275390625,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 191,
			"versionNonce": 1876332985,
			"isDeleted": false,
			"id": "iYfXdP0QdP6wN8_7TCU3b",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3953.707394921503,
			"y": -50.46373679438375,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 11.807053068486725,
			"height": 0.7700124287746658,
			"seed": 965144518,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					4.876843295877131,
					0.5133416191829354
				],
				[
					8.98361541479706,
					0.7700124287746658
				],
				[
					10.780330664665458,
					0.7700124287746658
				],
				[
					11.807053068486725,
					0.7700124287746658
				],
				[
					11.807053068486725,
					0.7700124287746658
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.4072265625,
				0.5029296875,
				0.51171875,
				0.416015625,
				0.015625,
				0
			]
		},
		{
			"type": "text",
			"version": 75,
			"versionNonce": 376304281,
			"isDeleted": false,
			"id": "rr5oev45",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3487.763381425025,
			"y": -173.26606747988717,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 555,
			"height": 75,
			"seed": 1084305670,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Input: s = \"MCMXCIV\"\nOutput: 1994\nExplanation: M = 1000, CM = 900, XC = 90 and IV = 4.",
			"rawText": "Input: s = \"MCMXCIV\"\nOutput: 1994\nExplanation: M = 1000, CM = 900, XC = 90 and IV = 4.",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Input: s = \"MCMXCIV\"\nOutput: 1994\nExplanation: M = 1000, CM = 900, XC = 90 and IV = 4.",
			"lineHeight": 1.25,
			"baseline": 68
		},
		{
			"type": "freedraw",
			"version": 235,
			"versionNonce": 958805881,
			"isDeleted": false,
			"id": "pMreTdTXwOm0z4OrH1uEP",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3963.3870726363,
			"y": 80.44573699704233,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 19.66452963065294,
			"height": 22.94194081712569,
			"seed": 1192736522,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.27313496326618275,
					0.27311412599403856
				],
				[
					0.5462490892602213,
					0
				],
				[
					1.0924773412482984,
					-2.184954682496597
				],
				[
					2.4580688084906352,
					-4.9161376169812705
				],
				[
					4.096774401727011,
					-10.378503485950619
				],
				[
					4.9161376169812705,
					-14.47527788767763
				],
				[
					5.189251742975309,
					-17.206460822162303
				],
				[
					5.462365868969348,
					-18.2989381634106
				],
				[
					6.008614958229569,
					-18.02580320014442
				],
				[
					6.554843210217646,
					-15.840869354919967
				],
				[
					7.101092299477868,
					-9.559140270696359
				],
				[
					7.101092299477868,
					-5.462365868969348
				],
				[
					7.374206425471906,
					-3.277432023744895
				],
				[
					8.466683766720204,
					-4.096774401727011
				],
				[
					9.832275233962541,
					-6.827957336211685
				],
				[
					12.017209079186994,
					-10.924731737938696
				],
				[
					13.382800546429332,
					-15.294620265659745
				],
				[
					15.29464110293189,
					-21.030121097895275
				],
				[
					16.387097606908043,
					-22.668826691131652
				],
				[
					17.206460822162303,
					-20.483872008635053
				],
				[
					17.47957494815634,
					-16.66021173290208
				],
				[
					17.206460822162303,
					-11.744094953192956
				],
				[
					17.47957494815634,
					-6.008614958229569
				],
				[
					17.75268907415038,
					-4.643023490987232
				],
				[
					18.57205228940464,
					-2.4580688084906352
				],
				[
					19.118280541392718,
					-1.0924773412482984
				],
				[
					19.66452963065294,
					-2.184954682496597
				],
				[
					19.66452963065294,
					-2.184954682496597
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.234375,
				0.2587890625,
				0.3955078125,
				0.4521484375,
				0.494140625,
				0.51953125,
				0.5244140625,
				0.5263671875,
				0.5263671875,
				0.5263671875,
				0.5234375,
				0.5234375,
				0.5234375,
				0.5234375,
				0.5234375,
				0.533203125,
				0.5361328125,
				0.5380859375,
				0.5478515625,
				0.5380859375,
				0.5263671875,
				0.533203125,
				0.55859375,
				0.5703125,
				0.5703125,
				0.5302734375,
				0.2978515625,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 216,
			"versionNonce": 1782767705,
			"isDeleted": false,
			"id": "X-81zCRxeYEQF-FwJ7pFZ",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3996.980631065371,
			"y": 68.97475616984366,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 12.290344042453176,
			"height": 2.184954682496597,
			"seed": 1592097866,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1.911819719230414,
					0
				],
				[
					3.8236602757329723,
					0.27313496326618275
				],
				[
					6.008594120957425,
					0.5462490892602213
				],
				[
					9.012912018708281,
					1.365591467242337
				],
				[
					10.651617611944657,
					1.9118405565025582
				],
				[
					12.017209079186994,
					2.184954682496597
				],
				[
					12.290344042453176,
					2.184954682496597
				],
				[
					12.017209079186994,
					1.9118405565025582
				],
				[
					12.017209079186994,
					1.9118405565025582
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.26953125,
				0.474609375,
				0.5029296875,
				0.515625,
				0.521484375,
				0.521484375,
				0.515625,
				0.4228515625,
				0.015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 214,
			"versionNonce": 664235321,
			"isDeleted": false,
			"id": "2MTUCkcYM4kPLLUL9skGl",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4004.627951616837,
			"y": 62.96616204888596,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 1.6387055932363754,
			"height": 11.470959989926772,
			"seed": 94547862,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.27311412599403856,
					5.735479994963386
				],
				[
					0.8193423779821156,
					7.3741855881997616
				],
				[
					1.0924565039761542,
					9.559140270696359
				],
				[
					1.365591467242337,
					10.105368522684435
				],
				[
					1.6387055932363754,
					10.924731737938696
				],
				[
					1.6387055932363754,
					11.470959989926772
				],
				[
					1.6387055932363754,
					11.470959989926772
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.359375,
				0.50390625,
				0.5341796875,
				0.53515625,
				0.529296875,
				0.4208984375,
				0.015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 222,
			"versionNonce": 1753701913,
			"isDeleted": false,
			"id": "QZH1AfmdfIo-I3BnFJcM0",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4039.8602156391435,
			"y": 57.23068205392292,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 14.47527788767763,
			"height": 18.02580320014442,
			"seed": 288393162,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-5.73550083223553,
					3.8236602757329723
				],
				[
					-7.101092299477868,
					5.189251742975309
				],
				[
					-9.012912018708281,
					8.193548803454021
				],
				[
					-10.924731737938696,
					13.929028798417407
				],
				[
					-10.6516384492168,
					15.840848517647823
				],
				[
					-9.832275233962541,
					16.93332585889612
				],
				[
					-8.466683766720204,
					17.75268907415038
				],
				[
					-6.281729084223608,
					18.02580320014442
				],
				[
					-3.550546149738934,
					18.02580320014442
				],
				[
					-1.365591467242337,
					17.75268907415038
				],
				[
					0.27309328872189437,
					17.47957494815634
				],
				[
					1.6386847559642312,
					17.47957494815634
				],
				[
					2.731182934484674,
					17.47957494815634
				],
				[
					3.550546149738934,
					17.75268907415038
				],
				[
					3.550546149738934,
					17.75268907415038
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2431640625,
				0.396484375,
				0.4287109375,
				0.4892578125,
				0.5224609375,
				0.546875,
				0.564453125,
				0.576171875,
				0.5791015625,
				0.5810546875,
				0.583984375,
				0.552734375,
				0.4970703125,
				0.37109375,
				0.0146484375,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 215,
			"versionNonce": 1812345593,
			"isDeleted": false,
			"id": "N2zSGc0i2DPDbpGnUTGSu",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4053.2429953483006,
			"y": 68.97475616984366,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 10.6516384492168,
			"height": 1.0924773412482984,
			"seed": 432307158,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1.365591467242337,
					0
				],
				[
					2.184954682496597,
					0
				],
				[
					3.8236811130051165,
					0.27313496326618275
				],
				[
					6.827957336211685,
					0.8193632152542598
				],
				[
					8.739777055442099,
					1.0924773412482984
				],
				[
					10.105368522684435,
					1.0924773412482984
				],
				[
					10.6516384492168,
					0.8193632152542598
				],
				[
					10.6516384492168,
					0.8193632152542598
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.30859375,
				0.443359375,
				0.4658203125,
				0.4990234375,
				0.5068359375,
				0.5068359375,
				0.4912109375,
				0.3369140625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 214,
			"versionNonce": 1184328665,
			"isDeleted": false,
			"id": "n3xdi1PqxZeeo5tpFHHIz",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4057.3397697500277,
			"y": 63.51239030087436,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 7.101092299477868,
			"height": 13.65591467242337,
			"seed": 772691478,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.5462282519880771,
					7.374206425471906
				],
				[
					-0.27309328872189437,
					8.466683766720204
				],
				[
					0.5462282519880771,
					11.744094953192956
				],
				[
					1.911819719230414,
					13.109686420435292
				],
				[
					3.8236811130051165,
					13.65591467242337
				],
				[
					6.55486404748979,
					12.563458168447216
				],
				[
					6.55486404748979,
					12.563458168447216
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.357421875,
				0.5009765625,
				0.5126953125,
				0.521484375,
				0.4853515625,
				0.244140625,
				0.0126953125,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 228,
			"versionNonce": 810453177,
			"isDeleted": false,
			"id": "Ged9Efxet3Ne_UzoJ9dFq",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4076.184957002699,
			"y": 74.16400791281876,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 24.85373969908396,
			"height": 19.93762291937483,
			"seed": 1556859210,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					6.554822372945502,
					-13.382800546429332
				],
				[
					8.466642092175915,
					-17.47957494815634
				],
				[
					9.832233559418253,
					-19.93762291937483
				],
				[
					10.105368522684435,
					-19.118280541392718
				],
				[
					10.37846181140633,
					-13.65591467242337
				],
				[
					10.37846181140633,
					-9.559140270696359
				],
				[
					10.651596774672512,
					-6.554843210217646
				],
				[
					12.563416493902928,
					-5.735479994963386
				],
				[
					13.65591467242337,
					-6.827957336211685
				],
				[
					17.75268907415038,
					-10.651617611944657
				],
				[
					20.483872008635053,
					-13.109665583163148
				],
				[
					23.21505494311973,
					-17.20643998489016
				],
				[
					24.307511447095884,
					-17.75268907415038
				],
				[
					24.85373969908396,
					-16.387097606908043
				],
				[
					24.85373969908396,
					-13.65591467242337
				],
				[
					24.307511447095884,
					-10.924731737938696
				],
				[
					24.0343764838297,
					-6.281708246951464
				],
				[
					24.0343764838297,
					-4.916116779709126
				],
				[
					24.307511447095884,
					-2.1849338452244527
				],
				[
					24.85373969908396,
					-0.27311412599403856
				],
				[
					24.85373969908396,
					-0.27311412599403856
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.3203125,
				0.46875,
				0.46875,
				0.46875,
				0.4736328125,
				0.4931640625,
				0.5078125,
				0.5107421875,
				0.51953125,
				0.5224609375,
				0.529296875,
				0.5263671875,
				0.5263671875,
				0.5263671875,
				0.533203125,
				0.5458984375,
				0.5712890625,
				0.5830078125,
				0.572265625,
				0.47265625,
				0.0166015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 216,
			"versionNonce": 315558297,
			"isDeleted": false,
			"id": "sZvAloQlYbmoOW1wlcg2n",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4108.13978900126,
			"y": 67.33605057660725,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 12.83655145716911,
			"height": 1.911819719230414,
			"seed": 1855220246,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1.6386847559642312,
					0
				],
				[
					3.823639438460828,
					-0.27311412599403856
				],
				[
					4.9161376169812705,
					-0.27311412599403856
				],
				[
					7.101050624933579,
					-0.5462282519880771
				],
				[
					9.559140270696359,
					-0.5462282519880771
				],
				[
					11.744094953192956,
					-0.5462282519880771
				],
				[
					12.83655145716911,
					-0.8193423779821156
				],
				[
					12.290323205181032,
					-1.911819719230414
				],
				[
					12.290323205181032,
					-1.911819719230414
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2490234375,
				0.4482421875,
				0.498046875,
				0.50390625,
				0.517578125,
				0.5224609375,
				0.5224609375,
				0.4306640625,
				0.015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 214,
			"versionNonce": 1464626809,
			"isDeleted": false,
			"id": "ltRu_XX93oUUiZXh9gKXX",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4113.329019906963,
			"y": 61.87368470763795,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 1.0924981785204426,
			"height": 14.202163761683591,
			"seed": 1790032906,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.5462282519880771,
					4.643023490987232
				],
				[
					-0.8193632152542598,
					8.739797892714243
				],
				[
					-0.8193632152542598,
					11.470980827198916
				],
				[
					-0.5462282519880771,
					13.382800546429332
				],
				[
					-0.27309328872189437,
					14.202163761683591
				],
				[
					0.27313496326618275,
					14.202163761683591
				],
				[
					0.27313496326618275,
					14.202163761683591
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.357421875,
				0.4404296875,
				0.49609375,
				0.5185546875,
				0.521484375,
				0.4423828125,
				0.015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 212,
			"versionNonce": 1955215193,
			"isDeleted": false,
			"id": "XDKiRlfvAJyIBetJCwypj",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4128.350526046629,
			"y": 72.52530231958235,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 17.206460822162303,
			"height": 19.937643756646978,
			"seed": 1468982934,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					8.739777055442099,
					-9.012912018708281
				],
				[
					10.378503485950619,
					-10.378503485950619
				],
				[
					14.202142924411447,
					-13.382800546429332
				],
				[
					17.206460822162303,
					-19.937643756646978
				],
				[
					17.206460822162303,
					-19.937643756646978
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.4072265625,
				0.548828125,
				0.548828125,
				0.5322265625,
				0.015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 218,
			"versionNonce": 1021043769,
			"isDeleted": false,
			"id": "hTtThyoaACrIgcRPXxUVj",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4136.817209813349,
			"y": 52.31454443694156,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 16.387097606908043,
			"height": 18.84516641539868,
			"seed": 965579274,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.27313496326618275,
					3.8236602757329723
				],
				[
					0,
					6.554843210217646
				],
				[
					0.27309328872189437,
					7.101071462205724
				],
				[
					2.184954682496597,
					9.559140270696359
				],
				[
					4.6430026537150875,
					11.197845863932734
				],
				[
					9.012912018708281,
					13.382800546429332
				],
				[
					10.924731737938696,
					14.748392013671667
				],
				[
					12.563416493902928,
					16.113983480914005
				],
				[
					13.929007961145263,
					17.206460822162303
				],
				[
					16.11396264364186,
					18.84516641539868
				],
				[
					16.11396264364186,
					18.84516641539868
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.423828125,
				0.490234375,
				0.53515625,
				0.548828125,
				0.58984375,
				0.603515625,
				0.60546875,
				0.580078125,
				0.5302734375,
				0.4287109375,
				0.015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 213,
			"versionNonce": 1814361369,
			"isDeleted": false,
			"id": "2tay-KawdQ02HzoBZ44cy",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4164.402132446918,
			"y": 65.42423085737664,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 15.294641102931827,
			"height": 3.277411186472751,
			"seed": 401589014,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					6.281729084223546,
					1.911819719230414
				],
				[
					8.466683766720143,
					2.4580688084906352
				],
				[
					10.651638449216739,
					3.277411186472751
				],
				[
					13.382821383701414,
					2.731182934484674
				],
				[
					15.294641102931827,
					0.8193423779821156
				],
				[
					15.294641102931827,
					0.8193423779821156
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.423828125,
				0.5068359375,
				0.51171875,
				0.513671875,
				0.416015625,
				0.015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 214,
			"versionNonce": 1977149945,
			"isDeleted": false,
			"id": "1HB44kfZ5h1_YwCVfwMhh",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4172.868816213639,
			"y": 61.05434232965581,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 1.365591467242337,
			"height": 13.382779709157187,
			"seed": 1914865686,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.5462282519880771,
					6.281708246951464
				],
				[
					-0.8193632152542598,
					9.012891181436137
				],
				[
					-0.5462282519880771,
					11.197845863932734
				],
				[
					0,
					12.83655145716911
				],
				[
					0.27313496326618275,
					13.382779709157187
				],
				[
					0.5462282519880771,
					13.382779709157187
				],
				[
					0.5462282519880771,
					13.382779709157187
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.392578125,
				0.5009765625,
				0.5244140625,
				0.53515625,
				0.509765625,
				0.3525390625,
				0.0283203125,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 218,
			"versionNonce": 318456537,
			"isDeleted": false,
			"id": "eR0CEpJ5SnQBI53DaHb_k",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4202.092465277716,
			"y": 48.21777003521447,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 25.67310291433822,
			"height": 23.76130403237995,
			"seed": 1516549962,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-6.827957336211685,
					9.832254396690397
				],
				[
					-9.832233559418253,
					15.021506139665707
				],
				[
					-11.470959989926772,
					19.118280541392718
				],
				[
					-10.651596774672512,
					22.12257760187143
				],
				[
					-6.554822372945502,
					23.76130403237995
				],
				[
					-2.184954682496597,
					23.488169069113766
				],
				[
					0.5462282519880771,
					23.21505494311973
				],
				[
					5.1892725802474535,
					22.12257760187143
				],
				[
					9.012912018708281,
					21.030121097895275
				],
				[
					14.202142924411447,
					19.937643756646978
				],
				[
					14.202142924411447,
					19.937643756646978
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.30859375,
				0.478515625,
				0.5390625,
				0.580078125,
				0.603515625,
				0.615234375,
				0.6181640625,
				0.6181640625,
				0.576171875,
				0.4736328125,
				0.0166015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 213,
			"versionNonce": 270499769,
			"isDeleted": false,
			"id": "UxO8zuL31LdldjpRinTfa",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4218.479562884623,
			"y": 62.14679883363169,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 13.109686420435292,
			"height": 1.0924565039761542,
			"seed": 1908310486,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					3.8236811130051165,
					-0.8193423779821156
				],
				[
					7.101092299477868,
					-1.0924565039761542
				],
				[
					11.197866701204878,
					-1.0924565039761542
				],
				[
					12.563458168447216,
					-0.8193423779821156
				],
				[
					13.109686420435292,
					-0.5462282519880771
				],
				[
					13.109686420435292,
					-0.5462282519880771
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.3818359375,
				0.51953125,
				0.5244140625,
				0.5263671875,
				0.5234375,
				0.44140625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 216,
			"versionNonce": 1533616281,
			"isDeleted": false,
			"id": "029da7QEUv4cLr2b28yos",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4227.219339940066,
			"y": 53.40702177818957,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 3.8236811130051165,
			"height": 20.210757882641015,
			"seed": 1983637206,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-1.365591467242337,
					4.9161376169812705
				],
				[
					-1.365591467242337,
					8.193548803454021
				],
				[
					-0.8193215407099714,
					11.197845863932734
				],
				[
					0.27313496326618275,
					13.929028798417407
				],
				[
					1.365591467242337,
					16.66021173290208
				],
				[
					1.9118613937747024,
					18.57205228940464
				],
				[
					2.184954682496597,
					19.664508793380794
				],
				[
					2.4580896457627794,
					20.210757882641015
				],
				[
					2.4580896457627794,
					20.210757882641015
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.419921875,
				0.5029296875,
				0.541015625,
				0.5625,
				0.5693359375,
				0.5498046875,
				0.484375,
				0.3095703125,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 215,
			"versionNonce": 1384883577,
			"isDeleted": false,
			"id": "Y-SaJ_V1p6U8nlyECyT5R",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4251.799986350427,
			"y": 71.15971085234014,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 2.1849130079523085,
			"height": 29.223649064077154,
			"seed": 2070405962,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.5462699265323655,
					-5.735479994963386
				],
				[
					1.0924981785204426,
					-12.563437331175072
				],
				[
					1.365591467242337,
					-18.02580320014442
				],
				[
					1.365591467242337,
					-20.483872008635053
				],
				[
					1.0924981785204426,
					-25.946237877604403
				],
				[
					0.8193632152542598,
					-29.223649064077154
				],
				[
					-0.8193215407099714,
					-26.21935200359844
				],
				[
					-0.8193215407099714,
					-26.21935200359844
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.4580078125,
				0.541015625,
				0.5712890625,
				0.5673828125,
				0.5576171875,
				0.5341796875,
				0.431640625,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 214,
			"versionNonce": 1355451993,
			"isDeleted": false,
			"id": "H4UCnEPRVX3RCCBiTQVH7",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4279.658085621807,
			"y": 58.59627352116513,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 11.470959989926772,
			"height": 2.4580688084906352,
			"seed": 2011075850,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					2.458047971218491,
					0
				],
				[
					4.6430026537150875,
					0.27311412599403856
				],
				[
					8.193548803454021,
					0
				],
				[
					9.559140270696359,
					-0.27311412599403856
				],
				[
					11.19782502666059,
					-0.5462490892602213
				],
				[
					11.470959989926772,
					-2.184954682496597
				],
				[
					11.470959989926772,
					-2.184954682496597
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.4453125,
				0.5068359375,
				0.53125,
				0.5439453125,
				0.5439453125,
				0.4638671875,
				0.0166015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 215,
			"versionNonce": 2096716601,
			"isDeleted": false,
			"id": "ct20703J1sQwp5CDf3PRS",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4284.574181564243,
			"y": 49.85647562845088,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 6.554822372945502,
			"height": 14.748392013671667,
			"seed": 1428462998,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.8193215407099714,
					3.8236602757329723
				],
				[
					-0.5462282519880771,
					6.554843210217646
				],
				[
					1.0924981785204426,
					10.651617611944657
				],
				[
					1.9118613937747024,
					12.017209079186994
				],
				[
					3.2774528610170393,
					13.929049635689552
				],
				[
					4.369909364993194,
					14.748392013671667
				],
				[
					5.73550083223553,
					14.47527788767763
				],
				[
					5.73550083223553,
					14.47527788767763
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.4443359375,
				0.505859375,
				0.53125,
				0.552734375,
				0.5546875,
				0.5322265625,
				0.3544921875,
				0.02734375,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 220,
			"versionNonce": 1467714585,
			"isDeleted": false,
			"id": "eNPJZ23jXwgrIds60J1_4",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4308.335506433896,
			"y": 43.301653255505244,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 24.034418158373988,
			"height": 32.501060250549905,
			"seed": 945905622,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-1.0924981785204426,
					13.65591467242337
				],
				[
					0,
					19.118280541392718
				],
				[
					1.911819719230414,
					21.03010026062313
				],
				[
					3.823639438460828,
					21.57632851261121
				],
				[
					7.647278876921656,
					18.845145578126534
				],
				[
					14.202142924411447,
					11.197845863932734
				],
				[
					17.479554110884198,
					5.462365868969348
				],
				[
					19.664508793380794,
					-1.0924773412482984
				],
				[
					21.303193549345025,
					-6.281729084223608
				],
				[
					22.122556764599285,
					-9.832275233962541
				],
				[
					22.941919979853544,
					-10.924731737938696
				],
				[
					22.122556764599285,
					-7.647320551465945
				],
				[
					22.122556764599285,
					-7.647320551465945
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.4111328125,
				0.4736328125,
				0.4912109375,
				0.4951171875,
				0.5087890625,
				0.552734375,
				0.56640625,
				0.568359375,
				0.55859375,
				0.513671875,
				0.4560546875,
				0.3115234375,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 215,
			"versionNonce": 138715385,
			"isDeleted": false,
			"id": "VLqpcEo9AQbQUxTRZRDar",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4254.804304248179,
			"y": 40.843584447014564,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 6.008594120957425,
			"height": 2.4580688084906352,
			"seed": 1039503306,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1.6387264305085196,
					-0.8193632152542598
				],
				[
					1.911819719230414,
					-1.0924773412482984
				],
				[
					2.458047971218491,
					-1.365591467242337
				],
				[
					3.277411186472751,
					-1.9118405565025582
				],
				[
					4.6430026537150875,
					-2.4580688084906352
				],
				[
					5.462365868969348,
					-2.4580688084906352
				],
				[
					6.008594120957425,
					-1.9118405565025582
				],
				[
					6.008594120957425,
					-1.9118405565025582
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.3837890625,
				0.4921875,
				0.5380859375,
				0.546875,
				0.5302734375,
				0.4375,
				0.2392578125,
				0.0126953125,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 214,
			"versionNonce": 1826101721,
			"isDeleted": false,
			"id": "4jwv9iQo32eoCpoWNPXna",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4245.79139222947,
			"y": 41.93606178826303,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 12.017229916459138,
			"height": 2.731182934484674,
			"seed": 1573941642,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					3.8236811130051165,
					0.8193423779821156
				],
				[
					5.1892725802474535,
					1.0924565039761542
				],
				[
					7.647320551465945,
					1.0924565039761542
				],
				[
					10.6516384492168,
					0.8193423779821156
				],
				[
					12.017229916459138,
					1.0924565039761542
				],
				[
					10.924731737938696,
					2.731182934484674
				],
				[
					10.924731737938696,
					2.731182934484674
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2666015625,
				0.4814453125,
				0.5166015625,
				0.54296875,
				0.5546875,
				0.5166015625,
				0.015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 216,
			"versionNonce": 1716090553,
			"isDeleted": false,
			"id": "p940d_RcD8lOUMgHP5n3j",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4244.4258007622275,
			"y": 73.89089378682502,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 12.83655145716911,
			"height": 0.8193632152542598,
			"seed": 1878722838,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					5.462365868969348,
					-0.8193632152542598
				],
				[
					7.920455514732128,
					-0.8193632152542598
				],
				[
					9.286046981974463,
					-0.8193632152542598
				],
				[
					10.6516384492168,
					-0.8193632152542598
				],
				[
					11.744094953192956,
					-0.5462282519880771
				],
				[
					12.83655145716911,
					-0.5462282519880771
				],
				[
					12.83655145716911,
					0
				],
				[
					12.563458168447216,
					0
				],
				[
					12.563458168447216,
					0
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.29296875,
				0.568359375,
				0.603515625,
				0.6103515625,
				0.6103515625,
				0.5908203125,
				0.5224609375,
				0.02734375,
				0.0146484375,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 217,
			"versionNonce": 1731999641,
			"isDeleted": false,
			"id": "KcJxWKSsVmxQorZMg-iWD",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3952.1891850978236,
			"y": 160.7425611128906,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 5.189251742975309,
			"height": 34.68603577031865,
			"seed": 1152787146,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1.9118405565025582,
					-8.739797892714243
				],
				[
					2.184954682496597,
					-11.470980827198916
				],
				[
					2.4580688084906352,
					-17.47957494815634
				],
				[
					2.4580688084906352,
					-23.21505494311973
				],
				[
					2.731182934484674,
					-31.135489620579712
				],
				[
					3.0042970604787125,
					-33.86667255506438
				],
				[
					3.277432023744895,
					-34.68603577031865
				],
				[
					3.8236602757329723,
					-34.139786681058425
				],
				[
					5.189251742975309,
					-24.034418158373988
				],
				[
					5.189251742975309,
					-24.034418158373988
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2021484375,
				0.4521484375,
				0.5068359375,
				0.5595703125,
				0.583984375,
				0.58984375,
				0.587890625,
				0.576171875,
				0.48046875,
				0.0166015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 223,
			"versionNonce": 1105452153,
			"isDeleted": false,
			"id": "4BB7_0jja-RVjSI-sj_oZ",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3963.387030961756,
			"y": 134.5232091092921,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 12.56343733117504,
			"height": 26.49248696686462,
			"seed": 714343242,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-2.731182934484674,
					6.008594120957425
				],
				[
					-3.5505253124667897,
					12.290323205181032
				],
				[
					-3.823639438460828,
					18.845145578126534
				],
				[
					-3.5505253124667897,
					23.21505494311973
				],
				[
					-2.1849338452244527,
					24.580646410362064
				],
				[
					1.0924773412482984,
					23.488169069113766
				],
				[
					4.369909364993163,
					19.664508793380794
				],
				[
					6.827957336211654,
					14.748371176399523
				],
				[
					8.739797892714211,
					8.193548803454021
				],
				[
					8.739797892714211,
					4.3698885277210495
				],
				[
					3.0043178977508256,
					-1.9118405565025582
				],
				[
					-1.365591467242337,
					1.365591467242337
				],
				[
					-1.6387055932363754,
					2.458047971218491
				],
				[
					-1.365591467242337,
					5.189230905703165
				],
				[
					4.916137616981239,
					8.739777055442099
				],
				[
					4.916137616981239,
					8.739777055442099
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.185546875,
				0.3115234375,
				0.375,
				0.4228515625,
				0.439453125,
				0.439453125,
				0.44140625,
				0.44140625,
				0.431640625,
				0.4296875,
				0.44921875,
				0.513671875,
				0.521484375,
				0.5166015625,
				0.453125,
				0.0126953125,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 224,
			"versionNonce": 906224985,
			"isDeleted": false,
			"id": "APWXHe_SnrCCKUdXGY08A",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3973.765534447707,
			"y": 140.80491735624355,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 11.744074115920812,
			"height": 23.488189906385912,
			"seed": 750182410,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-1.365591467242337,
					11.197845863932734
				],
				[
					1.0924773412482984,
					11.470980827198916
				],
				[
					5.462365868969348,
					8.739797892714243
				],
				[
					9.012912018708281,
					3.0042970604787125
				],
				[
					10.105368522684435,
					-1.0924773412482984
				],
				[
					10.105368522684435,
					-2.731182934484674
				],
				[
					9.012912018708281,
					-6.008594120957425
				],
				[
					6.827957336211685,
					-9.28602614470232
				],
				[
					3.8236602757329723,
					-11.470959989926772
				],
				[
					1.0924773412482984,
					-12.017209079186994
				],
				[
					-0.8193632152542598,
					-10.105368522684435
				],
				[
					-1.365591467242337,
					-8.46666292944806
				],
				[
					-1.6387055932363754,
					-5.189251742975309
				],
				[
					-0.8193632152542598,
					-1.6387055932363754
				],
				[
					2.731182934484674,
					3.550546149738934
				],
				[
					0,
					0
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.3359375,
				0.44921875,
				0.458984375,
				0.453125,
				0.462890625,
				0.4677734375,
				0.474609375,
				0.5029296875,
				0.53125,
				0.548828125,
				0.5517578125,
				0.5517578125,
				0.544921875,
				0.5205078125,
				0.4169921875,
				0.015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 224,
			"versionNonce": 1055904313,
			"isDeleted": false,
			"id": "SSifXxp_lx-G5DDfNMyd1",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3986.0558576528874,
			"y": 128.24148002506854,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 9.559140270696359,
			"height": 27.31182934484674,
			"seed": 250455254,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-3.277411186472751,
					17.75268907415038
				],
				[
					-3.8236602757329723,
					23.488169069113766
				],
				[
					-3.0042970604787125,
					27.31182934484674
				],
				[
					-1.365591467242337,
					26.765601092858663
				],
				[
					1.0924773412482984,
					23.21505494311973
				],
				[
					4.096774401727011,
					18.84516641539868
				],
				[
					5.735479994963386,
					11.197845863932734
				],
				[
					5.735479994963386,
					7.920434677459983
				],
				[
					4.096774401727011,
					3.277411186472751
				],
				[
					2.184954682496597,
					1.6387055932363754
				],
				[
					0.27311412599403856,
					2.731182934484674
				],
				[
					-1.365591467242337,
					6.008594120957425
				],
				[
					-1.911819719230414,
					7.647320551465945
				],
				[
					-2.184954682496597,
					11.197845863932734
				],
				[
					-1.6387055932363754,
					15.021506139665707
				],
				[
					0.5462282519880771,
					18.84516641539868
				],
				[
					0.5462282519880771,
					18.84516641539868
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2529296875,
				0.4501953125,
				0.482421875,
				0.4921875,
				0.4873046875,
				0.4892578125,
				0.4892578125,
				0.4873046875,
				0.4931640625,
				0.4970703125,
				0.50390625,
				0.5224609375,
				0.5244140625,
				0.5166015625,
				0.4892578125,
				0.3212890625,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 214,
			"versionNonce": 562766617,
			"isDeleted": false,
			"id": "SFlrn0O0MkYf0enFv_Mrp",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3994.5225205823363,
			"y": 143.53610029072843,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 16.387097606908043,
			"height": 0.8193632152542598,
			"seed": 274321482,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					2.184954682496597,
					0.8193632152542598
				],
				[
					7.374206425471906,
					0.5462490892602213
				],
				[
					10.924731737938696,
					0.27311412599403856
				],
				[
					13.65591467242337,
					0.27311412599403856
				],
				[
					16.113983480914005,
					0.27311412599403856
				],
				[
					16.387097606908043,
					0.27311412599403856
				],
				[
					16.387097606908043,
					0.27311412599403856
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.3349609375,
				0.5,
				0.5322265625,
				0.5380859375,
				0.5400390625,
				0.4931640625,
				0.0126953125,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 212,
			"versionNonce": 977885177,
			"isDeleted": false,
			"id": "vzKBYa_nCYz4nl1aHdI31",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4004.081660853032,
			"y": 136.98125708051066,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 1.6387055932363754,
			"height": 20.757006971901237,
			"seed": 1858819670,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					9.559140270696359
				],
				[
					0.27311412599403856,
					13.65591467242337
				],
				[
					1.0924773412482984,
					19.118280541392718
				],
				[
					1.6387055932363754,
					20.757006971901237
				],
				[
					1.6387055932363754,
					20.757006971901237
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.357421875,
				0.5185546875,
				0.5478515625,
				0.38671875,
				0.1103515625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 214,
			"versionNonce": 187560153,
			"isDeleted": false,
			"id": "tTpq0wUwurghOWKllVuuQ",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4030.8472619458908,
			"y": 151.1834208421942,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 1.365591467242337,
			"height": 21.303235223889313,
			"seed": 581789258,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.5462490892602213,
					-8.739797892714243
				],
				[
					-0.5462490892602213,
					-11.744094953192956
				],
				[
					-1.0924773412482984,
					-15.840869354919967
				],
				[
					-1.365591467242337,
					-17.75268907415038
				],
				[
					-1.365591467242337,
					-20.483872008635053
				],
				[
					-1.0924773412482984,
					-21.303235223889313
				],
				[
					-1.0924773412482984,
					-21.303235223889313
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.333984375,
				0.53515625,
				0.5498046875,
				0.552734375,
				0.544921875,
				0.4921875,
				0.154296875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 223,
			"versionNonce": 164392377,
			"isDeleted": false,
			"id": "eq174eoQY54klEhMPlAry",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4040.4064022165876,
			"y": 136.98125708051066,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 11.197845863932734,
			"height": 15.021506139665707,
			"seed": 1039081558,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-2.4580688084906352,
					12.017209079186994
				],
				[
					-1.365591467242337,
					13.929049635689552
				],
				[
					2.1849338452244527,
					12.836572294441254
				],
				[
					4.9161376169812705,
					10.105389359956579
				],
				[
					7.647320551465945,
					6.827957336211685
				],
				[
					8.739777055442099,
					3.550546149738934
				],
				[
					8.193548803454021,
					1.0924773412482984
				],
				[
					6.281729084223608,
					-0.5462282519880771
				],
				[
					4.369909364993194,
					-1.0924565039761542
				],
				[
					2.4580688084906352,
					0
				],
				[
					0.8193423779821156,
					1.9118405565025582
				],
				[
					0.27311412599403856,
					4.096774401727011
				],
				[
					1.0924773412482984,
					5.462365868969348
				],
				[
					3.550546149738934,
					3.550546149738934
				],
				[
					0,
					0
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2802734375,
				0.4931640625,
				0.4951171875,
				0.4951171875,
				0.50390625,
				0.5,
				0.498046875,
				0.5087890625,
				0.5234375,
				0.54296875,
				0.552734375,
				0.552734375,
				0.5361328125,
				0.3974609375,
				0.0146484375,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 219,
			"versionNonce": 759713433,
			"isDeleted": false,
			"id": "j_jiLQyv2I-w2hx3oO3sJ",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4052.696725421768,
			"y": 147.90598881844926,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 7.647320551465945,
			"height": 15.294620265659745,
			"seed": 1552232342,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					3.823639438460828,
					-2.1849338452244527
				],
				[
					4.369909364993194,
					-2.731182934484674
				],
				[
					6.008594120957425,
					-10.378482648678474
				],
				[
					4.6430026537150875,
					-12.563437331175072
				],
				[
					3.823639438460828,
					-13.65591467242337
				],
				[
					1.365591467242337,
					-15.294620265659745
				],
				[
					0,
					-14.475257050405485
				],
				[
					-1.0924565039761542,
					-12.290323205181032
				],
				[
					-1.6387264305085196,
					-11.470959989926772
				],
				[
					-1.365591467242337,
					-9.012891181436137
				],
				[
					0.27313496326618275,
					-7.3741855881997616
				],
				[
					0.27313496326618275,
					-7.3741855881997616
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.302734375,
				0.4873046875,
				0.494140625,
				0.5283203125,
				0.556640625,
				0.564453125,
				0.5859375,
				0.603515625,
				0.5927734375,
				0.587890625,
				0.5146484375,
				0.0166015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 222,
			"versionNonce": 1012208505,
			"isDeleted": false,
			"id": "lccoF2TCI-3EG3G7Hb5xj",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4063.6214571597075,
			"y": 135.61566561326845,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 7.647320551465945,
			"height": 14.202163761683591,
			"seed": 1584968790,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-3.277411186472751,
					12.017209079186994
				],
				[
					-1.365591467242337,
					12.836572294441254
				],
				[
					0.5462282519880771,
					12.017209079186994
				],
				[
					2.458047971218491,
					9.832275233962541
				],
				[
					3.823639438460828,
					6.827957336211685
				],
				[
					4.369909364993194,
					3.8236602757329723
				],
				[
					4.096774401727011,
					1.9118405565025582
				],
				[
					2.458047971218491,
					-0.5462282519880771
				],
				[
					1.365591467242337,
					-1.365591467242337
				],
				[
					0,
					-1.0924565039761542
				],
				[
					-0.5462282519880771,
					-0.5462282519880771
				],
				[
					-1.0924565039761542,
					1.0924773412482984
				],
				[
					0,
					2.731182934484674
				],
				[
					0,
					0
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.1923828125,
				0.4833984375,
				0.5078125,
				0.51171875,
				0.517578125,
				0.51953125,
				0.521484375,
				0.533203125,
				0.5576171875,
				0.5673828125,
				0.572265625,
				0.572265625,
				0.5185546875,
				0.0166015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 213,
			"versionNonce": 1530281049,
			"isDeleted": false,
			"id": "TYRypqfU1qZD5X8IaWBqx",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4069.9031862439306,
			"y": 140.5318032302498,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 8.193548803454021,
			"height": 1.911819719230414,
			"seed": 1309653514,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					3.277411186472751,
					-0.8193632152542598
				],
				[
					6.281729084223608,
					-1.6387055932363754
				],
				[
					6.827957336211685,
					-1.911819719230414
				],
				[
					7.647320551465945,
					-1.911819719230414
				],
				[
					8.193548803454021,
					-1.6387055932363754
				],
				[
					8.193548803454021,
					-1.6387055932363754
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.4453125,
				0.5380859375,
				0.5498046875,
				0.541015625,
				0.4892578125,
				0.33203125,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 208,
			"versionNonce": 1505708345,
			"isDeleted": false,
			"id": "RXESluPqBSCIPVGiGBk46",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4084.6515574203304,
			"y": 148.1791237817156,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 0.00005462365868969348,
			"height": 0.00005462365868969348,
			"seed": 1076192522,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.00005462365868969348,
					0.00005462365868969348
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.318359375,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 219,
			"versionNonce": 1096006169,
			"isDeleted": false,
			"id": "axj80bWopCPYnvAjVJqO3",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4084.6515574203304,
			"y": 148.72535203370353,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 3.0043178977508567,
			"height": 21.57634934988335,
			"seed": 765281750,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					-0.5462282519880771
				],
				[
					0.27313496326618275,
					-3.0042970604787125
				],
				[
					1.0924981785204426,
					-7.3741855881997616
				],
				[
					1.6387264305085196,
					-10.651617611944657
				],
				[
					1.365591467242337,
					-16.113983480914005
				],
				[
					0.8193632152542598,
					-19.664508793380794
				],
				[
					0.27313496326618275,
					-21.03010026062313
				],
				[
					0.27313496326618275,
					-21.57634934988335
				],
				[
					0,
					-21.303235223889313
				],
				[
					0.5462282519880771,
					-19.391394667386756
				],
				[
					3.0043178977508567,
					-16.66021173290208
				],
				[
					3.0043178977508567,
					-16.66021173290208
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.1796875,
				0.390625,
				0.4873046875,
				0.5234375,
				0.537109375,
				0.552734375,
				0.556640625,
				0.5595703125,
				0.556640625,
				0.521484375,
				0.3056640625,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 221,
			"versionNonce": 585567993,
			"isDeleted": false,
			"id": "lkUWO9HxJQmgSff9x9_d9",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4091.479514756542,
			"y": 139.71244001499554,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 7.647320551465945,
			"height": 11.744074115920812,
			"seed": 502551190,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.8193632152542598,
					5.462365868969348
				],
				[
					2.184954682496597,
					5.462365868969348
				],
				[
					3.277411186472751,
					4.9161376169812705
				],
				[
					5.462365868969348,
					2.731182934484674
				],
				[
					6.55486404748979,
					0
				],
				[
					6.008594120957425,
					-1.911819719230414
				],
				[
					4.6430026537150875,
					-3.5505253124667897
				],
				[
					1.365591467242337,
					-6.008594120957425
				],
				[
					0,
					-6.281708246951464
				],
				[
					-1.0924565039761542,
					-5.462365868969348
				],
				[
					-0.8193632152542598,
					-3.277411186472751
				],
				[
					0.5462282519880771,
					-2.458047971218491
				],
				[
					4.9161376169812705,
					-2.458047971218491
				],
				[
					4.9161376169812705,
					-2.458047971218491
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.330078125,
				0.4814453125,
				0.5068359375,
				0.5166015625,
				0.5361328125,
				0.5361328125,
				0.5458984375,
				0.5732421875,
				0.591796875,
				0.60546875,
				0.609375,
				0.5029296875,
				0.2314453125,
				0.0126953125,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 223,
			"versionNonce": 620546009,
			"isDeleted": false,
			"id": "d56kbzpwxxTWkEvhDKBBD",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4099.399970271274,
			"y": 139.9855749782614,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 11.197866701204878,
			"height": 13.65591467242337,
			"seed": 1931992214,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.8193215407099714,
					2.731182934484674
				],
				[
					2.458047971218491,
					1.0924565039761542
				],
				[
					4.369867690448905,
					-1.365591467242337
				],
				[
					6.008594120957425,
					-3.550546149738934
				],
				[
					6.554822372945502,
					-5.73550083223553
				],
				[
					5.189230905703165,
					-7.647320551465945
				],
				[
					4.369867690448905,
					-8.739797892714243
				],
				[
					2.1849130079523085,
					-10.378503485950619
				],
				[
					0.27309328872189437,
					-10.924731737938696
				],
				[
					-2.184954682496597,
					-10.378503485950619
				],
				[
					-4.096774401727011,
					-9.012912018708281
				],
				[
					-4.643044328259376,
					-7.374206425471906
				],
				[
					-3.550546149738934,
					-6.008614958229569
				],
				[
					-0.5462699265323655,
					-4.096774401727011
				],
				[
					0,
					0
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.419921875,
				0.533203125,
				0.5498046875,
				0.5595703125,
				0.5595703125,
				0.568359375,
				0.587890625,
				0.6015625,
				0.62109375,
				0.6259765625,
				0.6328125,
				0.634765625,
				0.5732421875,
				0.275390625,
				0.0126953125,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 215,
			"versionNonce": 1369990329,
			"isDeleted": false,
			"id": "pgJNcS3k9Cq8QAf_5_tPH",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4019.103166992698,
			"y": 121.95975094084497,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 27.31182934484674,
			"height": 39.875287513293955,
			"seed": 1714693078,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-8.193548803454021,
					19.391415504658898
				],
				[
					-9.28602614470232,
					28.95055577535526
				],
				[
					-6.554843210217646,
					35.50537814830076
				],
				[
					-1.365591467242337,
					38.78281017204566
				],
				[
					-0.27311412599403856,
					39.05592429803969
				],
				[
					9.28602614470232,
					39.875287513293955
				],
				[
					18.02580320014442,
					39.32903842403373
				],
				[
					18.02580320014442,
					39.32903842403373
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.345703125,
				0.501953125,
				0.544921875,
				0.5693359375,
				0.560546875,
				0.556640625,
				0.23828125,
				0.0126953125,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 217,
			"versionNonce": 613246361,
			"isDeleted": false,
			"id": "ADkvwh8yQGwlFwPQV_J1f",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4100.219291811984,
			"y": 110.21567682492423,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 15.567776066198071,
			"height": 49.16129282072413,
			"seed": 2008350230,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					7.101092299477868,
					7.920434677459983
				],
				[
					12.563458168447216,
					16.93332585889612
				],
				[
					13.65591467242337,
					20.210757882641015
				],
				[
					15.567776066198071,
					28.404306686095037
				],
				[
					15.021506139665707,
					36.05160640028884
				],
				[
					13.65591467242337,
					40.14838080201585
				],
				[
					12.017229916459138,
					44.518269329736896
				],
				[
					9.832275233962541,
					47.522587227487755
				],
				[
					4.9161376169812705,
					49.16129282072413
				],
				[
					4.9161376169812705,
					49.16129282072413
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.3515625,
				0.4599609375,
				0.5146484375,
				0.5244140625,
				0.537109375,
				0.5458984375,
				0.5498046875,
				0.5244140625,
				0.4345703125,
				0.015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 215,
			"versionNonce": 1491028601,
			"isDeleted": false,
			"id": "dJHSRQF5d5dr5L-_fkQV1",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4120.703163820619,
			"y": 137.80062029576493,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 9.012912018708281,
			"height": 1.0924773412482984,
			"seed": 1140913558,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					2.4580896457627794,
					0
				],
				[
					3.0043178977508567,
					-0.27311412599403856
				],
				[
					4.643044328259376,
					-0.5462282519880771
				],
				[
					5.73550083223553,
					-0.5462282519880771
				],
				[
					7.101092299477868,
					-0.8193632152542598
				],
				[
					7.920455514732128,
					-0.8193632152542598
				],
				[
					9.012912018708281,
					-1.0924773412482984
				],
				[
					9.012912018708281,
					-1.0924773412482984
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.4326171875,
				0.46875,
				0.4794921875,
				0.4931640625,
				0.49609375,
				0.4599609375,
				0.3720703125,
				0.0146484375,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 215,
			"versionNonce": 2002883417,
			"isDeleted": false,
			"id": "ok3Ke_SfWcw-GyWWZLteY",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4125.892436400866,
			"y": 127.42211680981427,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 2.1849130079523085,
			"height": 21.849463475877393,
			"seed": 445036502,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.27309328872189437,
					7.101092299477868
				],
				[
					0,
					10.924731737938696
				],
				[
					-0.5462282519880771,
					15.567755228925927
				],
				[
					-0.27313496326618275,
					18.84516641539868
				],
				[
					0.27309328872189437,
					21.030121097895275
				],
				[
					0.8193632152542598,
					21.849463475877393
				],
				[
					1.6386847559642312,
					21.57634934988335
				],
				[
					1.6386847559642312,
					21.57634934988335
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.333984375,
				0.4580078125,
				0.5087890625,
				0.52734375,
				0.5322265625,
				0.5087890625,
				0.3505859375,
				0.0146484375,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 216,
			"versionNonce": 610779193,
			"isDeleted": false,
			"id": "JzqVDxPP-Us46FkgCcK40",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4142.006399044509,
			"y": 109.6694277356637,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 11.470959989926772,
			"height": 42.060221358518405,
			"seed": 1105924630,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-4.6430026537150875,
					12.836572294441254
				],
				[
					-6.554822372945502,
					26.219372840870584
				],
				[
					-5.735459157691242,
					33.047330177082266
				],
				[
					-2.458047971218491,
					38.78281017204566
				],
				[
					-1.0924565039761542,
					40.14840163928799
				],
				[
					0.8193632152542598,
					41.24087898053629
				],
				[
					2.4580896457627794,
					42.060221358518405
				],
				[
					4.9161376169812705,
					41.78710723252437
				],
				[
					4.9161376169812705,
					41.78710723252437
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.30859375,
				0.474609375,
				0.5615234375,
				0.5869140625,
				0.583984375,
				0.5400390625,
				0.4677734375,
				0.3056640625,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 215,
			"versionNonce": 768954649,
			"isDeleted": false,
			"id": "Gd_JTgMxEYzL5_qf25Fd9",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4152.384902530459,
			"y": 137.80062029576493,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 7.647320551465945,
			"height": 19.937643756646978,
			"seed": 1804768266,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					2.184954682496597,
					-9.559140270696359
				],
				[
					3.0043178977508567,
					-16.66021173290208
				],
				[
					2.731182934484674,
					-19.118280541392718
				],
				[
					3.0043178977508567,
					-19.937643756646978
				],
				[
					3.823639438460828,
					-19.937643756646978
				],
				[
					4.369909364993194,
					-19.664508793380794
				],
				[
					7.647320551465945,
					-15.840869354919967
				],
				[
					7.647320551465945,
					-15.840869354919967
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.357421875,
				0.5322265625,
				0.548828125,
				0.548828125,
				0.5234375,
				0.4169921875,
				0.3818359375,
				0.01171875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 222,
			"versionNonce": 1495123449,
			"isDeleted": false,
			"id": "_qjYSn3JBuuQEJXFvgN2g",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4161.944042801155,
			"y": 133.97696002003204,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 9.286005307430175,
			"height": 18.298917326138458,
			"seed": 2072169930,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1.0924565039761542,
					1.365591467242337
				],
				[
					2.731182934484674,
					0.5462490892602213
				],
				[
					6.554822372945502,
					-2.731182934484674
				],
				[
					8.193548803454021,
					-5.735479994963386
				],
				[
					9.286005307430175,
					-8.193548803454021
				],
				[
					9.286005307430175,
					-10.651617611944657
				],
				[
					8.466683766720204,
					-13.382800546429332
				],
				[
					5.73550083223553,
					-16.387097606908043
				],
				[
					3.277411186472751,
					-16.93332585889612
				],
				[
					1.6387264305085196,
					-16.387097606908043
				],
				[
					0,
					-13.382800546429332
				],
				[
					0,
					-11.197845863932734
				],
				[
					0.5462282519880771,
					-9.832254396690397
				],
				[
					3.277411186472751,
					-9.28602614470232
				],
				[
					3.277411186472751,
					-9.28602614470232
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.30859375,
				0.416015625,
				0.4658203125,
				0.4931640625,
				0.4951171875,
				0.5,
				0.5087890625,
				0.521484375,
				0.5439453125,
				0.560546875,
				0.5791015625,
				0.5703125,
				0.5185546875,
				0.23828125,
				0.0126953125,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 218,
			"versionNonce": 1900322521,
			"isDeleted": false,
			"id": "zEieje95x6GufZ4jDDjjG",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4172.595639575828,
			"y": 131.51889121154136,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 10.105410197228723,
			"height": 11.470959989926772,
			"seed": 1189582294,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					3.550546149738934,
					1.0924773412482984
				],
				[
					8.193548803454021,
					-2.1849338452244527
				],
				[
					10.105410197228723,
					-8.193548803454021
				],
				[
					7.920455514732128,
					-10.105368522684435
				],
				[
					5.73550083223553,
					-10.378482648678474
				],
				[
					4.096774401727011,
					-9.832254396690397
				],
				[
					3.550546149738934,
					-8.739777055442099
				],
				[
					3.2774528610170393,
					-7.3741855881997616
				],
				[
					3.8236811130051165,
					-6.554822372945502
				],
				[
					6.281729084223608,
					-6.008594120957425
				],
				[
					6.281729084223608,
					-6.008594120957425
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.3837890625,
				0.4560546875,
				0.478515625,
				0.5185546875,
				0.556640625,
				0.583984375,
				0.5927734375,
				0.5859375,
				0.5224609375,
				0.27734375,
				0.0126953125,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 213,
			"versionNonce": 350051257,
			"isDeleted": false,
			"id": "zAI2ytCdUOLp0muLzeY9q",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4185.705325996263,
			"y": 126.05652534257206,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 12.017229916459138,
			"height": 0.8193632152542598,
			"seed": 2139548426,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					5.1892725802474535,
					0.27313496326618275
				],
				[
					9.012912018708281,
					0.27313496326618275
				],
				[
					11.197866701204878,
					0.8193632152542598
				],
				[
					11.744094953192956,
					0.8193632152542598
				],
				[
					12.017229916459138,
					0
				],
				[
					12.017229916459138,
					0
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.328125,
				0.55078125,
				0.55859375,
				0.5654296875,
				0.515625,
				0.017578125,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 215,
			"versionNonce": 1141603481,
			"isDeleted": false,
			"id": "XleJiyIpWdkSBnBZp8S0a",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4205.096741500922,
			"y": 133.43073176804364,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 3.277411186472751,
			"height": 18.2989381634106,
			"seed": 939267594,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1.365591467242337,
					-7.101071462205724
				],
				[
					1.365591467242337,
					-8.46666292944806
				],
				[
					1.6386847559642312,
					-13.65591467242337
				],
				[
					1.6386847559642312,
					-15.021506139665707
				],
				[
					1.911819719230414,
					-17.206460822162303
				],
				[
					2.184954682496597,
					-18.02580320014442
				],
				[
					3.277411186472751,
					-18.2989381634106
				],
				[
					3.277411186472751,
					-18.2989381634106
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.4052734375,
				0.5712890625,
				0.5888671875,
				0.6083984375,
				0.6015625,
				0.5654296875,
				0.4228515625,
				0.017578125,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 221,
			"versionNonce": 780304761,
			"isDeleted": false,
			"id": "GI1VqErIaBdN3ETJpQHcp",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4214.10965351963,
			"y": 124.96406883859572,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 10.378503485950619,
			"height": 13.382779709157187,
			"seed": 196808650,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-1.0924981785204426,
					5.189230905703165
				],
				[
					-0.5462699265323655,
					6.008594120957425
				],
				[
					1.365591467242337,
					6.554822372945502
				],
				[
					4.096774401727011,
					5.735479994963386
				],
				[
					6.28168740967932,
					3.277411186472751
				],
				[
					9.012870344163993,
					0
				],
				[
					9.286005307430175,
					-1.9118405565025582
				],
				[
					7.647278876921656,
					-5.462365868969348
				],
				[
					6.28168740967932,
					-6.827957336211685
				],
				[
					4.916095942436982,
					-6.827957336211685
				],
				[
					3.823639438460828,
					-5.462365868969348
				],
				[
					3.277411186472751,
					-3.550546149738934
				],
				[
					4.916095942436982,
					-2.4580688084906352
				],
				[
					4.916095942436982,
					-2.4580688084906352
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.3974609375,
				0.5048828125,
				0.5263671875,
				0.5595703125,
				0.578125,
				0.5830078125,
				0.5927734375,
				0.599609375,
				0.623046875,
				0.6259765625,
				0.6328125,
				0.626953125,
				0.5478515625,
				0.017578125,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 218,
			"versionNonce": 1099295321,
			"isDeleted": false,
			"id": "bblt9Gk1BUyehm_SOxBye",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4219.845112677322,
			"y": 109.39631360966996,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 9.559140270696359,
			"height": 27.85807843410696,
			"seed": 1094133194,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					2.184954682496597,
					0.8193632152542598
				],
				[
					4.6430026537150875,
					3.277432023744895
				],
				[
					7.647320551465945,
					6.554843210217646
				],
				[
					9.559140270696359,
					12.290323205181032
				],
				[
					9.012912018708281,
					15.567755228925927
				],
				[
					6.55486404748979,
					20.210757882641015
				],
				[
					4.6430026537150875,
					23.21505494311973
				],
				[
					3.8236811130051165,
					24.580646410362064
				],
				[
					2.4580896457627794,
					26.49248696686462
				],
				[
					0.8193632152542598,
					27.85807843410696
				],
				[
					0.8193632152542598,
					27.85807843410696
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.4716796875,
				0.5146484375,
				0.509765625,
				0.513671875,
				0.5234375,
				0.5517578125,
				0.5791015625,
				0.5810546875,
				0.5751953125,
				0.4892578125,
				0.0166015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 216,
			"versionNonce": 1978218297,
			"isDeleted": false,
			"id": "RJhEk7sWiBVvxIRRqUx_S",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3950.2773653785935,
			"y": 94.92105655926434,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 43.69892695175475,
			"height": 41.51399310653033,
			"seed": 1463229270,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					9.012891181436137,
					-10.651617611944657
				],
				[
					20.48387200863502,
					-22.668826691131652
				],
				[
					28.404306686095005,
					-29.223669901349297
				],
				[
					35.77849227429477,
					-36.870969615543096
				],
				[
					37.690311993525185,
					-38.236561082785435
				],
				[
					40.69462989127604,
					-40.14840163928799
				],
				[
					42.60644961050645,
					-41.24087898053629
				],
				[
					43.69892695175475,
					-41.51399310653033
				],
				[
					43.69892695175475,
					-41.51399310653033
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.3740234375,
				0.486328125,
				0.51171875,
				0.5205078125,
				0.5224609375,
				0.5166015625,
				0.43359375,
				0.2431640625,
				0.0126953125,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 223,
			"versionNonce": 1578100761,
			"isDeleted": false,
			"id": "QjN-0AFJXoG7vIF2wakmc",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4011.4558672785042,
			"y": 90.55114719427138,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 89.58278774873402,
			"height": 40.14838080201585,
			"seed": 691916694,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					5.189230905703165,
					-3.5505253124667897
				],
				[
					10.924731737938696,
					-6.827957336211685
				],
				[
					13.929028798417407,
					-8.46666292944806
				],
				[
					20.21073704536887,
					-11.470959989926772
				],
				[
					28.404285848822894,
					-15.294620265659745
				],
				[
					42.060221358518405,
					-21.57632851261121
				],
				[
					51.346226665948585,
					-24.853760536356102
				],
				[
					63.36345658240772,
					-29.76987731606523
				],
				[
					69.91827895535322,
					-32.774195213816085
				],
				[
					75.92687307631064,
					-35.23224318503458
				],
				[
					80.29678244130385,
					-37.14408374153714
				],
				[
					84.66665013175275,
					-38.78278933477351
				],
				[
					87.6709680295036,
					-39.60215255002777
				],
				[
					89.03655949674594,
					-40.14838080201585
				],
				[
					89.58278774873402,
					-39.60215255002777
				],
				[
					89.58278774873402,
					-39.60215255002777
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.328125,
				0.4716796875,
				0.4921875,
				0.494140625,
				0.5029296875,
				0.5087890625,
				0.513671875,
				0.5224609375,
				0.52734375,
				0.5380859375,
				0.541015625,
				0.541015625,
				0.541015625,
				0.517578125,
				0.4150390625,
				0.015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 222,
			"versionNonce": 1944943865,
			"isDeleted": false,
			"id": "0QxaHxU_S2bd_35Fer9mr",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4128.350484372085,
			"y": 85.36191628856795,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 78.38494188480122,
			"height": 41.78710723252437,
			"seed": 873510614,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.5462282519880771,
					-0.27313496326618275
				],
				[
					2.184954682496597,
					-0.8193632152542598
				],
				[
					6.55486404748979,
					-3.550546149738934
				],
				[
					10.378503485950619,
					-6.281729084223608
				],
				[
					16.93332585889612,
					-9.832275233962541
				],
				[
					28.404327523367183,
					-17.206460822162303
				],
				[
					40.96774401727011,
					-24.307532284368026
				],
				[
					48.88819953200223,
					-28.677420812089075
				],
				[
					63.09034245641368,
					-34.95914989631268
				],
				[
					70.46452804461344,
					-39.05592429803969
				],
				[
					74.56130244634045,
					-40.69462989127607
				],
				[
					77.29248538082507,
					-41.51399310653033
				],
				[
					78.38494188480122,
					-41.78710723252437
				],
				[
					77.56562034409124,
					-40.96774401727011
				],
				[
					77.56562034409124,
					-40.96774401727011
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2021484375,
				0.38671875,
				0.4345703125,
				0.486328125,
				0.5,
				0.51171875,
				0.521484375,
				0.55078125,
				0.5654296875,
				0.58203125,
				0.583984375,
				0.583984375,
				0.572265625,
				0.529296875,
				0.0146484375,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 214,
			"versionNonce": 654669273,
			"isDeleted": false,
			"id": "YaFCSNCH6zOGF4ftRptcy",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4232.135435882503,
			"y": 126.60277443183213,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 19.118280541392718,
			"height": 2.184954682496597,
			"seed": 636592010,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.5462282519880771,
					0.27311412599403856
				],
				[
					4.369909364993194,
					0
				],
				[
					10.6516384492168,
					-0.8193632152542598
				],
				[
					16.93332585889612,
					-1.0924773412482984
				],
				[
					19.118280541392718,
					-1.365591467242337
				],
				[
					17.479595785428486,
					-1.9118405565025582
				],
				[
					17.479595785428486,
					-1.9118405565025582
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.423828125,
				0.474609375,
				0.5107421875,
				0.5234375,
				0.5263671875,
				0.4599609375,
				0.0166015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 213,
			"versionNonce": 711676601,
			"isDeleted": false,
			"id": "Z02xYc_eh4Bhq5J7cPiM2",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4240.0558913972345,
			"y": 118.13611150238421,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 3.5505044751946455,
			"height": 24.307511447095884,
			"seed": 2036513558,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					2.1849130079523085,
					6.008594120957425
				],
				[
					3.0042762232065683,
					8.739777055442099
				],
				[
					3.5505044751946455,
					14.475257050405485
				],
				[
					3.277411186472751,
					18.02580320014442
				],
				[
					2.458047971218491,
					24.307511447095884
				],
				[
					2.458047971218491,
					24.307511447095884
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.384765625,
				0.5009765625,
				0.53125,
				0.546875,
				0.494140625,
				0.0126953125,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 217,
			"versionNonce": 46306201,
			"isDeleted": false,
			"id": "pOF6o67jnstmD87krLL2b",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4260.266628442603,
			"y": 110.76190507691217,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 12.290323205181032,
			"height": 30.316126405325452,
			"seed": 1717141526,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-4.6430026537150875,
					11.744094953192956
				],
				[
					-5.189230905703165,
					14.47527788767763
				],
				[
					-4.9161376169812705,
					19.66452963065294
				],
				[
					-2.458047971218491,
					24.853760536356102
				],
				[
					-1.365591467242337,
					25.946237877604403
				],
				[
					1.365591467242337,
					27.85807843410696
				],
				[
					4.096774401727011,
					29.223669901349297
				],
				[
					6.008594120957425,
					30.316126405325452
				],
				[
					7.101092299477868,
					30.316126405325452
				],
				[
					7.101092299477868,
					30.316126405325452
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2958984375,
				0.4384765625,
				0.466796875,
				0.5,
				0.5185546875,
				0.5146484375,
				0.4755859375,
				0.3701171875,
				0.1708984375,
				0.01171875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 220,
			"versionNonce": 1413396601,
			"isDeleted": false,
			"id": "b7UVbnVAfoJqHYYInj1fe",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4268.1870422827915,
			"y": 132.06514030080143,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 14.47527788767763,
			"height": 18.298917326138458,
			"seed": 1641805718,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					6.008635795501713,
					0.5462282519880771
				],
				[
					9.012912018708281,
					-0.5462490892602213
				],
				[
					10.378503485950619,
					-2.4580688084906352
				],
				[
					10.105410197228723,
					-4.3698885277210495
				],
				[
					4.643044328259376,
					-7.920434677459983
				],
				[
					1.9118613937747024,
					-10.924731737938696
				],
				[
					2.4580896457627794,
					-13.65591467242337
				],
				[
					4.643044328259376,
					-15.294620265659745
				],
				[
					8.193548803454021,
					-16.66021173290208
				],
				[
					10.924731737938696,
					-17.47957494815634
				],
				[
					12.836593131713398,
					-17.75268907415038
				],
				[
					14.47527788767763,
					-17.47957494815634
				],
				[
					14.47527788767763,
					-17.47957494815634
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.35546875,
				0.453125,
				0.4765625,
				0.478515625,
				0.4541015625,
				0.4501953125,
				0.5556640625,
				0.6142578125,
				0.62109375,
				0.6142578125,
				0.5703125,
				0.4228515625,
				0.015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 212,
			"versionNonce": 1889747289,
			"isDeleted": false,
			"id": "8mHMo56f9roVz397rt8hB",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4283.754818348989,
			"y": 125.51029709058366,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 13.65591467242337,
			"height": 1.6387055932363754,
			"seed": 1356110858,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					3.823639438460828,
					-0.27311412599403856
				],
				[
					9.012870344163993,
					-1.0924773412482984
				],
				[
					11.470959989926772,
					-1.6387055932363754
				],
				[
					13.65591467242337,
					-1.6387055932363754
				],
				[
					13.65591467242337,
					-1.6387055932363754
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.4697265625,
				0.5146484375,
				0.5126953125,
				0.4697265625,
				0.2939453125,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 213,
			"versionNonce": 625192505,
			"isDeleted": false,
			"id": "dGcOH7PtchCYtBSWq3sAE",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4306.969873292109,
			"y": 129.333957366317,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 7.101050624933579,
			"height": 18.84516641539868,
			"seed": 1596760406,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					3.0042762232065683,
					-7.920434677459983
				],
				[
					3.823639438460828,
					-10.651617611944657
				],
				[
					6.28168740967932,
					-17.75268907415038
				],
				[
					6.827957336211685,
					-18.84516641539868
				],
				[
					7.101050624933579,
					-18.02580320014442
				],
				[
					7.101050624933579,
					-18.02580320014442
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.4560546875,
				0.6064453125,
				0.609375,
				0.513671875,
				0.330078125,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 214,
			"versionNonce": 1224965913,
			"isDeleted": false,
			"id": "JR4WGSTa4t2ayBSblu5PP",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4306.969873292109,
			"y": 115.13179360463346,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 3.2774528610170393,
			"height": 10.924731737938696,
			"seed": 568215126,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-3.2774528610170393,
					-2.458047971218491
				],
				[
					-3.2774528610170393,
					-4.3698885277210495
				],
				[
					-2.731182934484674,
					-6.281708246951464
				],
				[
					-2.184954682496597,
					-8.193548803454021
				],
				[
					-1.9118613937747024,
					-10.651596774672512
				],
				[
					-1.9118613937747024,
					-10.924731737938696
				],
				[
					-1.9118613937747024,
					-10.924731737938696
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.4873046875,
				0.5712890625,
				0.58203125,
				0.5751953125,
				0.5185546875,
				0.08203125,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 219,
			"versionNonce": 173421561,
			"isDeleted": false,
			"id": "t2NOgcLpUheAfyRsjE29h",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4315.982743636273,
			"y": 100.92965068022158,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 15.021506139665707,
			"height": 35.7784922742948,
			"seed": 919215370,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					7.101092299477868,
					4.3698885277210495
				],
				[
					10.6516384492168,
					7.647320551465945
				],
				[
					14.202184598955736,
					12.017209079186994
				],
				[
					15.021506139665707,
					15.567734391653783
				],
				[
					12.017229916459138,
					27.858057596834815
				],
				[
					11.197866701204878,
					29.496784027343335
				],
				[
					9.286046981974463,
					32.774195213816085
				],
				[
					6.55486404748979,
					34.6860149330465
				],
				[
					3.8236811130051165,
					35.7784922742948
				],
				[
					2.184954682496597,
					35.7784922742948
				],
				[
					0.8193632152542598,
					34.95914989631268
				],
				[
					0.8193632152542598,
					34.95914989631268
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.212890625,
				0.2802734375,
				0.3671875,
				0.4892578125,
				0.5146484375,
				0.5673828125,
				0.576171875,
				0.59765625,
				0.607421875,
				0.5712890625,
				0.44140625,
				0.015625,
				0
			]
		},
		{
			"type": "text",
			"version": 77,
			"versionNonce": 2101300441,
			"isDeleted": false,
			"id": "s65aHWDz",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3446.277324688489,
			"y": 0.12699399681469004,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 149,
			"height": 25,
			"seed": 236773194,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
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
			"baseline": 18
		},
		{
			"type": "text",
			"version": 553,
			"versionNonce": 1767000505,
			"isDeleted": false,
			"id": "brFQf6wz",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3481.0273094297,
			"y": 66.37695584984203,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 366,
			"height": 350,
			"seed": 121604310,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "- specialCase: map\n- numeral: map\n- answer: int\n- iterate sChars\n    - if 2 or more chars remain\n        - if next 2 are specialCase\n            - answer += specialCase\n            - i + 2\n            - continue\n    - if is numeral\n        - answer += numeral.get(s[i])\n        - i + 1\n    - else return null\n- retrun answer",
			"rawText": "- specialCase: map\n- numeral: map\n- answer: int\n- iterate sChars\n    - if 2 or more chars remain\n        - if next 2 are specialCase\n            - answer += specialCase\n            - i + 2\n            - continue\n    - if is numeral\n        - answer += numeral.get(s[i])\n        - i + 1\n    - else return null\n- retrun answer",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "- specialCase: map\n- numeral: map\n- answer: int\n- iterate sChars\n    - if 2 or more chars remain\n        - if next 2 are specialCase\n            - answer += specialCase\n            - i + 2\n            - continue\n    - if is numeral\n        - answer += numeral.get(s[i])\n        - i + 1\n    - else return null\n- retrun answer",
			"lineHeight": 1.25,
			"baseline": 343
		},
		{
			"type": "line",
			"version": 386,
			"versionNonce": 1471326873,
			"isDeleted": false,
			"id": "clDckbb0R7fsujNns4A97",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4359.092277003395,
			"y": 1255.5128421670702,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 0,
			"height": 2090.6667073567705,
			"seed": 85917520,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1718955787976,
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
			"version": 118,
			"versionNonce": 1628696441,
			"isDeleted": false,
			"id": "uBlrd7yo",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4468.711269996145,
			"y": -748.9678480346731,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 451,
			"height": 50,
			"seed": 1066918832,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "## 17. Letter Combination of a Phone Number\n",
			"rawText": "## 17. Letter Combination of a Phone Number\n",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "## 17. Letter Combination of a Phone Number\n",
			"lineHeight": 1.25,
			"baseline": 43
		},
		{
			"type": "text",
			"version": 70,
			"versionNonce": 1002018905,
			"isDeleted": false,
			"id": "61AXDvGo",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4453.15571444059,
			"y": -677.856736923562,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 50,
			"height": 25,
			"seed": 1320834896,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
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
			"baseline": 18
		},
		{
			"type": "text",
			"version": 229,
			"versionNonce": 158803257,
			"isDeleted": false,
			"id": "pXQgceEH",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4514.933465091632,
			"y": -599.1900838202644,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 759,
			"height": 125,
			"seed": 1512910256,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Retrutn all possible letter combination that the given number could represent\n\ndigits beween 0 and 4\n\n> public List<String> letterCombination (String digits) <",
			"rawText": "Retrutn all possible letter combination that the given number could represent\n\ndigits beween 0 and 4\n\n> public List<String> letterCombination (String digits) <",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Retrutn all possible letter combination that the given number could represent\n\ndigits beween 0 and 4\n\n> public List<String> letterCombination (String digits) <",
			"lineHeight": 1.25,
			"baseline": 118
		},
		{
			"type": "text",
			"version": 73,
			"versionNonce": 1706038809,
			"isDeleted": false,
			"id": "bVUePlAd",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4451.989051164765,
			"y": -380.88456386854887,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 91,
			"height": 25,
			"seed": 537378736,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
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
			"baseline": 18
		},
		{
			"type": "text",
			"version": 159,
			"versionNonce": 861399801,
			"isDeleted": false,
			"id": "ok86lQOx",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4510.6557178314315,
			"y": -310.21789720188235,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 528,
			"height": 50,
			"seed": 206258512,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "digits = \"23\"\noutput = [ \"ab\", \"ae\", \"af\", \"bd\", \"be\", \"cd\", \"ce\", \"cf\" ]",
			"rawText": "digits = \"23\"\noutput = [ \"ab\", \"ae\", \"af\", \"bd\", \"be\", \"cd\", \"ce\", \"cf\" ]",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "digits = \"23\"\noutput = [ \"ab\", \"ae\", \"af\", \"bd\", \"be\", \"cd\", \"ce\", \"cf\" ]",
			"lineHeight": 1.25,
			"baseline": 43
		},
		{
			"type": "text",
			"version": 77,
			"versionNonce": 720511961,
			"isDeleted": false,
			"id": "RPb75Unv",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4455.18900233664,
			"y": -160.08451504042296,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 149,
			"height": 25,
			"seed": 864111952,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
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
			"baseline": 18
		},
		{
			"type": "text",
			"version": 179,
			"versionNonce": 680673465,
			"isDeleted": false,
			"id": "5WlIRxAq",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4483.988888404348,
			"y": -101.68453131646493,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 280,
			"height": 50,
			"seed": 427635024,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "- make hashmap of all digits\n- if ",
			"rawText": "- make hashmap of all digits\n- if ",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "- make hashmap of all digits\n- if ",
			"lineHeight": 1.25,
			"baseline": 43
		},
		{
			"type": "line",
			"version": 452,
			"versionNonce": 970703257,
			"isDeleted": false,
			"id": "d69JUkhHksBzmfmEst6YY",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 5300.509123199182,
			"y": 1201.909825974597,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 0,
			"height": 2090.6667073567705,
			"seed": 2038042274,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1718955787976,
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
			"version": 98,
			"versionNonce": 1812080249,
			"isDeleted": false,
			"id": "Z5okNo6b",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 5394.153335302529,
			"y": -877.397994845669,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 258,
			"height": 50,
			"seed": 1239260002,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "## 20. Valid Parentheses\n",
			"rawText": "## 20. Valid Parentheses\n",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "## 20. Valid Parentheses\n",
			"lineHeight": 1.25,
			"baseline": 43
		},
		{
			"type": "text",
			"version": 291,
			"versionNonce": 1506340697,
			"isDeleted": false,
			"id": "9KNdFl5M",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 5829.429678425875,
			"y": -873.4509274117972,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 189,
			"height": 25,
			"seed": 220935714,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
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
			"baseline": 18
		},
		{
			"type": "text",
			"version": 362,
			"versionNonce": 2038668345,
			"isDeleted": false,
			"id": "RodWzksg",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 5812.799738913837,
			"y": -827.1934472523153,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 389,
			"height": 25,
			"seed": 1617175010,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": "[[LeetCode/Questions#Solution 20]]",
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "📍[[LeetCode/Questions#Solution 20]]",
			"rawText": "[[LeetCode/Questions#Solution 20]]",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "📍[[LeetCode/Questions#Solution 20]]",
			"lineHeight": 1.25,
			"baseline": 18
		},
		{
			"type": "text",
			"version": 70,
			"versionNonce": 722840857,
			"isDeleted": false,
			"id": "p7xeRQ3m",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 5376.981534901053,
			"y": -772.3676418775108,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 50,
			"height": 25,
			"seed": 1306183458,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
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
			"baseline": 18
		},
		{
			"type": "text",
			"version": 244,
			"versionNonce": 99787257,
			"isDeleted": false,
			"id": "gqCaUXKC",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 5416.981534901053,
			"y": -730.549460059329,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 314,
			"height": 200,
			"seed": 1364534818,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "determine if the string is valid\nvalid if:\n- same closing an open brackets\n- correct order\n- corresponding brackets\ncons: s.len is from 1 to 10^4\n\n> boolean isValid(Srting s) <",
			"rawText": "determine if the string is valid\nvalid if:\n- same closing an open brackets\n- correct order\n- corresponding brackets\ncons: s.len is from 1 to 10^4\n\n> boolean isValid(Srting s) <",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "determine if the string is valid\nvalid if:\n- same closing an open brackets\n- correct order\n- corresponding brackets\ncons: s.len is from 1 to 10^4\n\n> boolean isValid(Srting s) <",
			"lineHeight": 1.25,
			"baseline": 193
		},
		{
			"type": "text",
			"version": 86,
			"versionNonce": 1730018009,
			"isDeleted": false,
			"id": "arsWtfvc",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 5369.708807628325,
			"y": -496.0040055138743,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 91,
			"height": 25,
			"seed": 1075393314,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
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
			"baseline": 18
		},
		{
			"type": "text",
			"version": 106,
			"versionNonce": 1059796921,
			"isDeleted": false,
			"id": "gD0Spuvj",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 5423.890603615541,
			"y": -426.9130964229648,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 180,
			"height": 50,
			"seed": 1097542562,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Input: s = \"()[]{}\"\nOutput: true",
			"rawText": "Input: s = \"()[]{}\"\nOutput: true",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Input: s = \"()[]{}\"\nOutput: true",
			"lineHeight": 1.25,
			"baseline": 43
		},
		{
			"type": "freedraw",
			"version": 80,
			"versionNonce": 540924057,
			"isDeleted": false,
			"id": "z3HLkzo3lwKqeFU2O3wfE",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 5843.973563593596,
			"y": -472.1016566037856,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 21.17647058823536,
			"height": 40.94119801240822,
			"seed": 2038731902,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-4.705882352941444,
					0.941198012408222
				],
				[
					-6.117625517003944,
					1.411779067095722
				],
				[
					-9.882345760569933,
					5.176499310661711
				],
				[
					-14.11764705882365,
					10.823543772978155
				],
				[
					-18.352912454044144,
					16.941205193014866
				],
				[
					-21.17647058823536,
					23.05883071001881
				],
				[
					-21.17647058823536,
					30.58823529411802
				],
				[
					-18.352912454044144,
					34.82353659237151
				],
				[
					-15.99997127757365,
					37.64705882352973
				],
				[
					-14.11764705882365,
					39.5294189453125
				],
				[
					-13.647030101103155,
					40
				],
				[
					-12.705867991728155,
					40.94119801240822
				],
				[
					-12.705867991728155,
					40.94119801240822
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.1923828125,
				0.2744140625,
				0.3125,
				0.37890625,
				0.4404296875,
				0.484375,
				0.505859375,
				0.51171875,
				0.51171875,
				0.51953125,
				0.5126953125,
				0.5126953125,
				0.443359375,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 83,
			"versionNonce": 201940345,
			"isDeleted": false,
			"id": "xOO2QRlW_fl18oj8G1xJm",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 5880.208879253063,
			"y": -470.2192964820024,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 22.117632697610134,
			"height": 45.17646340762849,
			"seed": 610360482,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					5.176499310661711,
					-0.4705810546875
				],
				[
					7.058823529411711,
					-0.4705810546875
				],
				[
					8.941147748161711,
					0.4705810546875
				],
				[
					11.764705882352928,
					3.294139188878489
				],
				[
					15.529426125919144,
					9.882345760569933
				],
				[
					18.352912454044144,
					14.588228113510922
				],
				[
					20.235308478860134,
					18.823529411764866
				],
				[
					22.117632697610134,
					24.470609777114078
				],
				[
					21.647087545955856,
					31.52943330652579
				],
				[
					19.76469152113964,
					35.29411764705901
				],
				[
					17.411750344669144,
					38.11763987821678
				],
				[
					15.529426125919144,
					40.4705810546875
				],
				[
					14.117647058823422,
					42.82352223115822
				],
				[
					13.176484949448422,
					44.70588235294099
				],
				[
					14.117647058823422,
					44.70588235294099
				],
				[
					14.117647058823422,
					44.70588235294099
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2568359375,
				0.314453125,
				0.3330078125,
				0.3466796875,
				0.384765625,
				0.4228515625,
				0.4365234375,
				0.4638671875,
				0.4853515625,
				0.4990234375,
				0.515625,
				0.5244140625,
				0.5244140625,
				0.505859375,
				0.4189453125,
				0.015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 90,
			"versionNonce": 30492249,
			"isDeleted": false,
			"id": "N68z-fg1mi56Llw5J1JTT",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 5955.032379942401,
			"y": -465.5134141290614,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 21.647015739889866,
			"height": 36.705860811121056,
			"seed": 1672050274,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-11.764705882353155,
					1.882360121783222
				],
				[
					-15.999971277573422,
					0.941198012408222
				],
				[
					-17.411750344669144,
					-0.4705810546875
				],
				[
					-18.352912454044144,
					-1.8823601217827672
				],
				[
					-18.823529411764866,
					-2.8235222311577672
				],
				[
					-18.823529411764866,
					-3.2941032858452672
				],
				[
					-18.352912454044144,
					-2.8235222311577672
				],
				[
					-17.882295496323422,
					0.941198012408222
				],
				[
					-18.352912454044144,
					6.117661420037166
				],
				[
					-18.823529411764866,
					11.294124827665655
				],
				[
					-20.705853630514866,
					20.23530847886059
				],
				[
					-21.176470588235134,
					25.411771886489078
				],
				[
					-21.647015739889866,
					29.17649213005552
				],
				[
					-21.176470588235134,
					31.52943330652579
				],
				[
					-19.294074563419144,
					33.41175752527579
				],
				[
					-16.470588235294144,
					33.41175752527579
				],
				[
					-13.647030101103155,
					32.94117647058829
				],
				[
					-10.823471966911711,
					32.47059541590079
				],
				[
					-9.882309857536711,
					32.47059541590079
				],
				[
					-9.411764705882433,
					32.47059541590079
				],
				[
					-8.941147748161711,
					32.47059541590079
				],
				[
					-8.941147748161711,
					32.94117647058829
				],
				[
					-8.941147748161711,
					32.94117647058829
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2822265625,
				0.4599609375,
				0.5126953125,
				0.51953125,
				0.513671875,
				0.513671875,
				0.513671875,
				0.482421875,
				0.4619140625,
				0.447265625,
				0.44140625,
				0.4267578125,
				0.4296875,
				0.43359375,
				0.4482421875,
				0.4794921875,
				0.4921875,
				0.50390625,
				0.5068359375,
				0.5068359375,
				0.47265625,
				0.380859375,
				0.0126953125,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 91,
			"versionNonce": 1281954617,
			"isDeleted": false,
			"id": "qu5YqsYLBZOoigCOANfiG",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 5972.4442020931365,
			"y": -463.6310540072782,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 20.705853630514866,
			"height": 43.76468434053322,
			"seed": 2116791230,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					3.7646484375,
					-0.941162109375
				],
				[
					7.058823529411711,
					-2.352941176470722
				],
				[
					10.352926815257433,
					-2.823522231158222
				],
				[
					16.470588235294144,
					-3.294103285845722
				],
				[
					18.823529411764866,
					-3.294103285845722
				],
				[
					19.294074563419144,
					-2.823522231158222
				],
				[
					19.764691521139866,
					0.4705810546875
				],
				[
					19.764691521139866,
					6.588242474724211
				],
				[
					20.235236672794144,
					11.294124827665655
				],
				[
					20.705853630514866,
					16.000007180606644
				],
				[
					20.705853630514866,
					21.17647058823559
				],
				[
					19.764691521139866,
					28.2352941176473
				],
				[
					17.882295496323422,
					32.47059541590079
				],
				[
					15.529354319853155,
					36.70589671415428
				],
				[
					13.647030101103155,
					39.5294189453125
				],
				[
					12.235251034007433,
					40.4705810546875
				],
				[
					9.411764705882433,
					40
				],
				[
					7.058823529411711,
					39.058837890625
				],
				[
					5.647044462316444,
					38.11763987821678
				],
				[
					5.647044462316444,
					37.64705882352928
				],
				[
					4.705882352941444,
					36.70589671415428
				],
				[
					4.235265395220722,
					35.76469870174651
				],
				[
					5.176427504595722,
					33.41175752527579
				],
				[
					5.176427504595722,
					33.41175752527579
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2578125,
				0.3525390625,
				0.396484375,
				0.4169921875,
				0.42578125,
				0.427734375,
				0.4599609375,
				0.4736328125,
				0.494140625,
				0.484375,
				0.484375,
				0.484375,
				0.484375,
				0.4912109375,
				0.5078125,
				0.5205078125,
				0.5400390625,
				0.5830078125,
				0.599609375,
				0.609375,
				0.6123046875,
				0.591796875,
				0.513671875,
				0.0166015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 105,
			"versionNonce": 271860761,
			"isDeleted": false,
			"id": "siueqOrTpGDwxY6OXqsPS",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 6038.797100185967,
			"y": -473.0428187131606,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 20.235308478860134,
			"height": 54.58822811351138,
			"seed": 1609512702,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-7.529368681065989,
					1.411779067095722
				],
				[
					-10.352926815257433,
					3.764720243566444
				],
				[
					-10.8235437729777,
					7.529404584099211
				],
				[
					-8.470602596507433,
					11.294124827665655
				],
				[
					-5.176427504595722,
					14.588228113511377
				],
				[
					-1.88232421875,
					19.294110466452366
				],
				[
					-0.941162109375,
					21.64705164292309
				],
				[
					-1.411779067095722,
					23.99999281939381
				],
				[
					-2.352941176470722,
					25.882352941176578
				],
				[
					-5.176427504595722,
					28.2352941176473
				],
				[
					-11.294088924632433,
					29.64707318474302
				],
				[
					-15.058809168198422,
					30.11765423943052
				],
				[
					-17.411750344669144,
					30.11765423943052
				],
				[
					-18.82352941176441,
					29.64707318474302
				],
				[
					-19.294074563419144,
					29.1764562270223
				],
				[
					-20.235308478860134,
					28.7058751723348
				],
				[
					-20.235308478860134,
					28.2352941176473
				],
				[
					-19.76469152113941,
					28.2352941176473
				],
				[
					-18.82352941176441,
					28.2352941176473
				],
				[
					-17.88236730238941,
					27.7647130629598
				],
				[
					-15.529426125919144,
					27.7647130629598
				],
				[
					-12.235251034007433,
					28.7058751723348
				],
				[
					-8.941147748161711,
					29.64707318474302
				],
				[
					-5.176427504595722,
					32.47059541590079
				],
				[
					-4.705882352940989,
					34.35295553768401
				],
				[
					-5.647044462315989,
					36.23527975643401
				],
				[
					-8.941147748161711,
					38.58822093290473
				],
				[
					-14.5881922104777,
					41.88236012178322
				],
				[
					-16.470588235294144,
					44.705882352941444
				],
				[
					-17.411750344669144,
					47.99998563878671
				],
				[
					-16.470588235294144,
					50.35292681525743
				],
				[
					-15.058809168198422,
					52.235286937040655
				],
				[
					-9.411764705882433,
					53.64706600413638
				],
				[
					-7.529368681065989,
					53.64706600413638
				],
				[
					-5.176427504595722,
					54.11764705882388
				],
				[
					-3.294103285845722,
					54.58822811351138
				],
				[
					-0.470545151654278,
					54.58822811351138
				],
				[
					-0.470545151654278,
					54.58822811351138
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2509765625,
				0.4072265625,
				0.474609375,
				0.4921875,
				0.4853515625,
				0.4765625,
				0.4697265625,
				0.4697265625,
				0.4697265625,
				0.4765625,
				0.5068359375,
				0.54296875,
				0.55859375,
				0.5703125,
				0.5791015625,
				0.58203125,
				0.583984375,
				0.5712890625,
				0.5576171875,
				0.5576171875,
				0.552734375,
				0.533203125,
				0.5166015625,
				0.513671875,
				0.51171875,
				0.509765625,
				0.509765625,
				0.51171875,
				0.5185546875,
				0.5341796875,
				0.5390625,
				0.5439453125,
				0.5419921875,
				0.5380859375,
				0.5302734375,
				0.486328125,
				0.3427734375,
				0.0146484375,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 120,
			"versionNonce": 421943545,
			"isDeleted": false,
			"id": "GtHvN5KUQWqHXa4fhDcIS",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 6063.267674060048,
			"y": -473.9839808225356,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 32.94117647058829,
			"height": 61.17647058823559,
			"seed": 703720226,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.941233915441444,
					0
				],
				[
					1.882396024816444,
					0
				],
				[
					5.647116268382433,
					0
				],
				[
					10.823543772978155,
					0.4705810546875
				],
				[
					15.058880974264866,
					1.4117431640625
				],
				[
					18.823529411764866,
					2.823522231158222
				],
				[
					21.647087545955856,
					4.705882352941444
				],
				[
					24.4706456801473,
					8.470566693474211
				],
				[
					24.4706456801473,
					10.823507869944933
				],
				[
					23.058866613051578,
					13.176449046415655
				],
				[
					20.705925436580856,
					15.999971277573877
				],
				[
					16.470588235294144,
					20.235272575827366
				],
				[
					13.176484949448422,
					22.11763269761059
				],
				[
					10.352998621323422,
					23.52941176470631
				],
				[
					8.000057444853155,
					24.94115492876881
				],
				[
					6.117661420036711,
					25.882352941176578
				],
				[
					8.000057444853155,
					26.352933995864078
				],
				[
					11.764705882353155,
					26.823515050551578
				],
				[
					15.058880974264866,
					27.294096105239078
				],
				[
					17.882367302389866,
					27.764677159926578
				],
				[
					22.117704503676578,
					29.6470372817098
				],
				[
					24.4706456801473,
					30.58823529411802
				],
				[
					26.3529698988973,
					31.52939740349302
				],
				[
					28.2352941176473,
					31.99997845818052
				],
				[
					28.705911075367567,
					31.99997845818052
				],
				[
					29.17652803308829,
					31.99997845818052
				],
				[
					28.705911075367567,
					31.99997845818052
				],
				[
					28.2352941176473,
					31.99997845818052
				],
				[
					27.764748965992567,
					32.47055951286802
				],
				[
					24.941190831801578,
					33.41175752527579
				],
				[
					22.588249655330856,
					34.35291963465079
				],
				[
					18.823529411764866,
					36.23527975643401
				],
				[
					15.058880974264866,
					38.58822093290473
				],
				[
					10.823543772978155,
					40.941162109375
				],
				[
					8.000057444853155,
					41.88232421875
				],
				[
					6.117661420036711,
					42.35294117647072
				],
				[
					6.117661420036711,
					42.82352223115822
				],
				[
					8.000057444853155,
					44.705882352941444
				],
				[
					10.823543772978155,
					46.588206571691444
				],
				[
					13.647101907169144,
					47.99998563878671
				],
				[
					16.470588235294144,
					49.41176470588243
				],
				[
					18.352984260110134,
					50.35292681525743
				],
				[
					19.294146369485134,
					51.764705882353155
				],
				[
					19.294146369485134,
					53.176449046415655
				],
				[
					17.882367302389866,
					54.58822811351138
				],
				[
					16.000043083639866,
					55.99997127757388
				],
				[
					12.705939797794144,
					57.411750344669144
				],
				[
					5.176499310661711,
					59.294110466452366
				],
				[
					0.941233915441444,
					60.235272575827366
				],
				[
					-0.470545151654278,
					60.705853630514866
				],
				[
					-2.823486328125,
					61.17647058823559
				],
				[
					-3.7646484375,
					59.294110466452366
				],
				[
					-3.7646484375,
					59.294110466452366
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.3662109375,
				0.48828125,
				0.501953125,
				0.5166015625,
				0.5166015625,
				0.5146484375,
				0.5185546875,
				0.521484375,
				0.5185546875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.5224609375,
				0.541015625,
				0.5576171875,
				0.564453125,
				0.5673828125,
				0.5654296875,
				0.5546875,
				0.5546875,
				0.556640625,
				0.5537109375,
				0.5517578125,
				0.5517578125,
				0.5517578125,
				0.5517578125,
				0.5517578125,
				0.5693359375,
				0.5693359375,
				0.5693359375,
				0.5771484375,
				0.56640625,
				0.560546875,
				0.5546875,
				0.548828125,
				0.552734375,
				0.552734375,
				0.552734375,
				0.5234375,
				0.5087890625,
				0.4951171875,
				0.484375,
				0.484375,
				0.4912109375,
				0.49609375,
				0.5068359375,
				0.5166015625,
				0.5224609375,
				0.537109375,
				0.5390625,
				0.5390625,
				0.4794921875,
				0.0166015625,
				0
			]
		},
		{
			"type": "rectangle",
			"version": 119,
			"versionNonce": 1757598169,
			"isDeleted": false,
			"id": "UMwG1mUIifGKhTYVvPozT",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 5822.326511950673,
			"y": -516.3369219990059,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 280.9411621093748,
			"height": 21.176470588235134,
			"seed": 1235998334,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 131,
			"versionNonce": 69021369,
			"isDeleted": false,
			"id": "LKUBsmSLhQhkcJcdsszGD",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 5816.208886433669,
			"y": -404.3369435408258,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 299.76472742417263,
			"height": 16.941169289981644,
			"seed": 254371134,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false
		},
		{
			"type": "freedraw",
			"version": 203,
			"versionNonce": 30994329,
			"isDeleted": false,
			"id": "vacvSrxndqR_LQWJPT_3N",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 6340.914679029028,
			"y": -431.86638402795825,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 21.17647058823536,
			"height": 40.94119801240822,
			"seed": 1322777186,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-4.705882352941444,
					0.941198012408222
				],
				[
					-6.117625517003944,
					1.411779067095722
				],
				[
					-9.882345760569933,
					5.176499310661711
				],
				[
					-14.11764705882365,
					10.823543772978155
				],
				[
					-18.352912454044144,
					16.941205193014866
				],
				[
					-21.17647058823536,
					23.05883071001881
				],
				[
					-21.17647058823536,
					30.58823529411802
				],
				[
					-18.352912454044144,
					34.82353659237151
				],
				[
					-15.99997127757365,
					37.64705882352973
				],
				[
					-14.11764705882365,
					39.5294189453125
				],
				[
					-13.647030101103155,
					40
				],
				[
					-12.705867991728155,
					40.94119801240822
				],
				[
					-12.705867991728155,
					40.94119801240822
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.1923828125,
				0.2744140625,
				0.3125,
				0.37890625,
				0.4404296875,
				0.484375,
				0.505859375,
				0.51171875,
				0.51171875,
				0.51953125,
				0.5126953125,
				0.5126953125,
				0.443359375,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 206,
			"versionNonce": 1479119993,
			"isDeleted": false,
			"id": "DErtmfsySdZUO4bQEQuqO",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 6377.149994688495,
			"y": -429.9840239061755,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 22.117632697610134,
			"height": 45.17646340762849,
			"seed": 275668514,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					5.176499310661711,
					-0.4705810546875
				],
				[
					7.058823529411711,
					-0.4705810546875
				],
				[
					8.941147748161711,
					0.4705810546875
				],
				[
					11.764705882352928,
					3.294139188878489
				],
				[
					15.529426125919144,
					9.882345760569933
				],
				[
					18.352912454044144,
					14.588228113510922
				],
				[
					20.235308478860134,
					18.823529411764866
				],
				[
					22.117632697610134,
					24.470609777114078
				],
				[
					21.647087545955856,
					31.52943330652579
				],
				[
					19.76469152113964,
					35.29411764705901
				],
				[
					17.411750344669144,
					38.11763987821678
				],
				[
					15.529426125919144,
					40.4705810546875
				],
				[
					14.117647058823422,
					42.82352223115822
				],
				[
					13.176484949448422,
					44.70588235294099
				],
				[
					14.117647058823422,
					44.70588235294099
				],
				[
					14.117647058823422,
					44.70588235294099
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2568359375,
				0.314453125,
				0.3330078125,
				0.3466796875,
				0.384765625,
				0.4228515625,
				0.4365234375,
				0.4638671875,
				0.4853515625,
				0.4990234375,
				0.515625,
				0.5244140625,
				0.5244140625,
				0.505859375,
				0.4189453125,
				0.015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 213,
			"versionNonce": 1792187737,
			"isDeleted": false,
			"id": "HPrsQPZYvHoJZb1LgnGSu",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 6451.9734953778325,
			"y": -425.27814155323404,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 21.647015739889866,
			"height": 36.705860811121056,
			"seed": 1627539938,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-11.764705882353155,
					1.882360121783222
				],
				[
					-15.999971277573422,
					0.941198012408222
				],
				[
					-17.411750344669144,
					-0.4705810546875
				],
				[
					-18.352912454044144,
					-1.8823601217827672
				],
				[
					-18.823529411764866,
					-2.8235222311577672
				],
				[
					-18.823529411764866,
					-3.2941032858452672
				],
				[
					-18.352912454044144,
					-2.8235222311577672
				],
				[
					-17.882295496323422,
					0.941198012408222
				],
				[
					-18.352912454044144,
					6.117661420037166
				],
				[
					-18.823529411764866,
					11.294124827665655
				],
				[
					-20.705853630514866,
					20.23530847886059
				],
				[
					-21.176470588235134,
					25.411771886489078
				],
				[
					-21.647015739889866,
					29.17649213005552
				],
				[
					-21.176470588235134,
					31.52943330652579
				],
				[
					-19.294074563419144,
					33.41175752527579
				],
				[
					-16.470588235294144,
					33.41175752527579
				],
				[
					-13.647030101103155,
					32.94117647058829
				],
				[
					-10.823471966911711,
					32.47059541590079
				],
				[
					-9.882309857536711,
					32.47059541590079
				],
				[
					-9.411764705882433,
					32.47059541590079
				],
				[
					-8.941147748161711,
					32.47059541590079
				],
				[
					-8.941147748161711,
					32.94117647058829
				],
				[
					-8.941147748161711,
					32.94117647058829
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2822265625,
				0.4599609375,
				0.5126953125,
				0.51953125,
				0.513671875,
				0.513671875,
				0.513671875,
				0.482421875,
				0.4619140625,
				0.447265625,
				0.44140625,
				0.4267578125,
				0.4296875,
				0.43359375,
				0.4482421875,
				0.4794921875,
				0.4921875,
				0.50390625,
				0.5068359375,
				0.5068359375,
				0.47265625,
				0.380859375,
				0.0126953125,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 214,
			"versionNonce": 1495763513,
			"isDeleted": false,
			"id": "AT_ovaOJJ24j338qrTeb5",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 6469.3853175285685,
			"y": -423.39578143145036,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 20.705853630514866,
			"height": 43.76468434053322,
			"seed": 396541346,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					3.7646484375,
					-0.941162109375
				],
				[
					7.058823529411711,
					-2.352941176470722
				],
				[
					10.352926815257433,
					-2.823522231158222
				],
				[
					16.470588235294144,
					-3.294103285845722
				],
				[
					18.823529411764866,
					-3.294103285845722
				],
				[
					19.294074563419144,
					-2.823522231158222
				],
				[
					19.764691521139866,
					0.4705810546875
				],
				[
					19.764691521139866,
					6.588242474724211
				],
				[
					20.235236672794144,
					11.294124827665655
				],
				[
					20.705853630514866,
					16.000007180606644
				],
				[
					20.705853630514866,
					21.17647058823559
				],
				[
					19.764691521139866,
					28.2352941176473
				],
				[
					17.882295496323422,
					32.47059541590079
				],
				[
					15.529354319853155,
					36.70589671415428
				],
				[
					13.647030101103155,
					39.5294189453125
				],
				[
					12.235251034007433,
					40.4705810546875
				],
				[
					9.411764705882433,
					40
				],
				[
					7.058823529411711,
					39.058837890625
				],
				[
					5.647044462316444,
					38.11763987821678
				],
				[
					5.647044462316444,
					37.64705882352928
				],
				[
					4.705882352941444,
					36.70589671415428
				],
				[
					4.235265395220722,
					35.76469870174651
				],
				[
					5.176427504595722,
					33.41175752527579
				],
				[
					5.176427504595722,
					33.41175752527579
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2578125,
				0.3525390625,
				0.396484375,
				0.4169921875,
				0.42578125,
				0.427734375,
				0.4599609375,
				0.4736328125,
				0.494140625,
				0.484375,
				0.484375,
				0.484375,
				0.484375,
				0.4912109375,
				0.5078125,
				0.5205078125,
				0.5400390625,
				0.5830078125,
				0.599609375,
				0.609375,
				0.6123046875,
				0.591796875,
				0.513671875,
				0.0166015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 228,
			"versionNonce": 202103577,
			"isDeleted": false,
			"id": "8brrtEEdCZTSThNKXqDVI",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 6535.738215621398,
			"y": -432.80754613733325,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 20.235308478860134,
			"height": 54.58822811351138,
			"seed": 1367259490,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-7.529368681065989,
					1.411779067095722
				],
				[
					-10.352926815257433,
					3.764720243566444
				],
				[
					-10.8235437729777,
					7.529404584099211
				],
				[
					-8.470602596507433,
					11.294124827665655
				],
				[
					-5.176427504595722,
					14.588228113511377
				],
				[
					-1.88232421875,
					19.294110466452366
				],
				[
					-0.941162109375,
					21.64705164292309
				],
				[
					-1.411779067095722,
					23.99999281939381
				],
				[
					-2.352941176470722,
					25.882352941176578
				],
				[
					-5.176427504595722,
					28.2352941176473
				],
				[
					-11.294088924632433,
					29.64707318474302
				],
				[
					-15.058809168198422,
					30.11765423943052
				],
				[
					-17.411750344669144,
					30.11765423943052
				],
				[
					-18.82352941176441,
					29.64707318474302
				],
				[
					-19.294074563419144,
					29.1764562270223
				],
				[
					-20.235308478860134,
					28.7058751723348
				],
				[
					-20.235308478860134,
					28.2352941176473
				],
				[
					-19.76469152113941,
					28.2352941176473
				],
				[
					-18.82352941176441,
					28.2352941176473
				],
				[
					-17.88236730238941,
					27.7647130629598
				],
				[
					-15.529426125919144,
					27.7647130629598
				],
				[
					-12.235251034007433,
					28.7058751723348
				],
				[
					-8.941147748161711,
					29.64707318474302
				],
				[
					-5.176427504595722,
					32.47059541590079
				],
				[
					-4.705882352940989,
					34.35295553768401
				],
				[
					-5.647044462315989,
					36.23527975643401
				],
				[
					-8.941147748161711,
					38.58822093290473
				],
				[
					-14.5881922104777,
					41.88236012178322
				],
				[
					-16.470588235294144,
					44.705882352941444
				],
				[
					-17.411750344669144,
					47.99998563878671
				],
				[
					-16.470588235294144,
					50.35292681525743
				],
				[
					-15.058809168198422,
					52.235286937040655
				],
				[
					-9.411764705882433,
					53.64706600413638
				],
				[
					-7.529368681065989,
					53.64706600413638
				],
				[
					-5.176427504595722,
					54.11764705882388
				],
				[
					-3.294103285845722,
					54.58822811351138
				],
				[
					-0.470545151654278,
					54.58822811351138
				],
				[
					-0.470545151654278,
					54.58822811351138
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.2509765625,
				0.4072265625,
				0.474609375,
				0.4921875,
				0.4853515625,
				0.4765625,
				0.4697265625,
				0.4697265625,
				0.4697265625,
				0.4765625,
				0.5068359375,
				0.54296875,
				0.55859375,
				0.5703125,
				0.5791015625,
				0.58203125,
				0.583984375,
				0.5712890625,
				0.5576171875,
				0.5576171875,
				0.552734375,
				0.533203125,
				0.5166015625,
				0.513671875,
				0.51171875,
				0.509765625,
				0.509765625,
				0.51171875,
				0.5185546875,
				0.5341796875,
				0.5390625,
				0.5439453125,
				0.5419921875,
				0.5380859375,
				0.5302734375,
				0.486328125,
				0.3427734375,
				0.0146484375,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 243,
			"versionNonce": 66260985,
			"isDeleted": false,
			"id": "v6aKY-NIDgDKjvYZpE5jY",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 6560.208789495479,
			"y": -433.74870824670825,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 32.94117647058829,
			"height": 61.17647058823559,
			"seed": 769998114,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.941233915441444,
					0
				],
				[
					1.882396024816444,
					0
				],
				[
					5.647116268382433,
					0
				],
				[
					10.823543772978155,
					0.4705810546875
				],
				[
					15.058880974264866,
					1.4117431640625
				],
				[
					18.823529411764866,
					2.823522231158222
				],
				[
					21.647087545955856,
					4.705882352941444
				],
				[
					24.4706456801473,
					8.470566693474211
				],
				[
					24.4706456801473,
					10.823507869944933
				],
				[
					23.058866613051578,
					13.176449046415655
				],
				[
					20.705925436580856,
					15.999971277573877
				],
				[
					16.470588235294144,
					20.235272575827366
				],
				[
					13.176484949448422,
					22.11763269761059
				],
				[
					10.352998621323422,
					23.52941176470631
				],
				[
					8.000057444853155,
					24.94115492876881
				],
				[
					6.117661420036711,
					25.882352941176578
				],
				[
					8.000057444853155,
					26.352933995864078
				],
				[
					11.764705882353155,
					26.823515050551578
				],
				[
					15.058880974264866,
					27.294096105239078
				],
				[
					17.882367302389866,
					27.764677159926578
				],
				[
					22.117704503676578,
					29.6470372817098
				],
				[
					24.4706456801473,
					30.58823529411802
				],
				[
					26.3529698988973,
					31.52939740349302
				],
				[
					28.2352941176473,
					31.99997845818052
				],
				[
					28.705911075367567,
					31.99997845818052
				],
				[
					29.17652803308829,
					31.99997845818052
				],
				[
					28.705911075367567,
					31.99997845818052
				],
				[
					28.2352941176473,
					31.99997845818052
				],
				[
					27.764748965992567,
					32.47055951286802
				],
				[
					24.941190831801578,
					33.41175752527579
				],
				[
					22.588249655330856,
					34.35291963465079
				],
				[
					18.823529411764866,
					36.23527975643401
				],
				[
					15.058880974264866,
					38.58822093290473
				],
				[
					10.823543772978155,
					40.941162109375
				],
				[
					8.000057444853155,
					41.88232421875
				],
				[
					6.117661420036711,
					42.35294117647072
				],
				[
					6.117661420036711,
					42.82352223115822
				],
				[
					8.000057444853155,
					44.705882352941444
				],
				[
					10.823543772978155,
					46.588206571691444
				],
				[
					13.647101907169144,
					47.99998563878671
				],
				[
					16.470588235294144,
					49.41176470588243
				],
				[
					18.352984260110134,
					50.35292681525743
				],
				[
					19.294146369485134,
					51.764705882353155
				],
				[
					19.294146369485134,
					53.176449046415655
				],
				[
					17.882367302389866,
					54.58822811351138
				],
				[
					16.000043083639866,
					55.99997127757388
				],
				[
					12.705939797794144,
					57.411750344669144
				],
				[
					5.176499310661711,
					59.294110466452366
				],
				[
					0.941233915441444,
					60.235272575827366
				],
				[
					-0.470545151654278,
					60.705853630514866
				],
				[
					-2.823486328125,
					61.17647058823559
				],
				[
					-3.7646484375,
					59.294110466452366
				],
				[
					-3.7646484375,
					59.294110466452366
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.3662109375,
				0.48828125,
				0.501953125,
				0.5166015625,
				0.5166015625,
				0.5146484375,
				0.5185546875,
				0.521484375,
				0.5185546875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.5224609375,
				0.541015625,
				0.5576171875,
				0.564453125,
				0.5673828125,
				0.5654296875,
				0.5546875,
				0.5546875,
				0.556640625,
				0.5537109375,
				0.5517578125,
				0.5517578125,
				0.5517578125,
				0.5517578125,
				0.5517578125,
				0.5693359375,
				0.5693359375,
				0.5693359375,
				0.5771484375,
				0.56640625,
				0.560546875,
				0.5546875,
				0.548828125,
				0.552734375,
				0.552734375,
				0.552734375,
				0.5234375,
				0.5087890625,
				0.4951171875,
				0.484375,
				0.484375,
				0.4912109375,
				0.49609375,
				0.5068359375,
				0.5166015625,
				0.5224609375,
				0.537109375,
				0.5390625,
				0.5390625,
				0.4794921875,
				0.0166015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 150,
			"versionNonce": 1725999321,
			"isDeleted": false,
			"id": "MG5-mcelZJqJ-lEhCRi7R",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 6290.56169835922,
			"y": -451.86631222189135,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 34.35295553768401,
			"height": 88.47056669347421,
			"seed": 1086912738,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-4.235265395220267,
					2.352941176470722
				],
				[
					-7.999985638786711,
					4.235301298253944
				],
				[
					-15.529390222885922,
					8.470566693474211
				],
				[
					-21.647051642922634,
					12.235286937040655
				],
				[
					-27.764677159926578,
					15.529390222885922
				],
				[
					-31.529397403492567,
					18.823529411764866
				],
				[
					-30.588235294117567,
					21.17647058823559
				],
				[
					-27.294096105239078,
					23.999992819393356
				],
				[
					-22.588213752297634,
					27.294096105239078
				],
				[
					-16.470588235294144,
					30.11765423943052
				],
				[
					-13.6470301011027,
					31.52939740349302
				],
				[
					-11.294088924631978,
					33.41175752527579
				],
				[
					-10.823507869944478,
					34.82353659237151
				],
				[
					-13.6470301011027,
					38.11763987821723
				],
				[
					-15.999971277573422,
					40
				],
				[
					-19.29411046645191,
					41.4117431640625
				],
				[
					-22.117632697610134,
					41.4117431640625
				],
				[
					-25.411735983455856,
					41.4117431640625
				],
				[
					-30.117618336396845,
					40.941162109375
				],
				[
					-31.999978458180067,
					40.941162109375
				],
				[
					-32.94117647058829,
					40.941162109375
				],
				[
					-32.94117647058829,
					40.4705810546875
				],
				[
					-32.47055951286757,
					40.4705810546875
				],
				[
					-31.529397403492567,
					40.4705810546875
				],
				[
					-31.058816348805067,
					40.4705810546875
				],
				[
					-30.117618336396845,
					40.4705810546875
				],
				[
					-28.705875172334345,
					40.941162109375
				],
				[
					-24.941154928768356,
					40.941162109375
				],
				[
					-22.117632697610134,
					40.941162109375
				],
				[
					-18.352912454044144,
					40.941162109375
				],
				[
					-14.588228113510922,
					43.29410328584572
				],
				[
					-13.6470301011027,
					46.117625517003944
				],
				[
					-13.6470301011027,
					49.41176470588243
				],
				[
					-15.529390222885922,
					53.176449046415655
				],
				[
					-17.411750344669144,
					56.470588235294144
				],
				[
					-19.29411046645191,
					60.70588953354809
				],
				[
					-18.82352941176441,
					63.529411764705856
				],
				[
					-16.941169289981644,
					66.35293399586408
				],
				[
					-13.6470301011027,
					69.6470372817098
				],
				[
					-12.7058679917277,
					70.58823529411757
				],
				[
					-8.470566693474211,
					72.94117647058829
				],
				[
					-4.705882352940989,
					76.23527975643401
				],
				[
					-1.88232421875,
					80.4705810546875
				],
				[
					1.411779067095722,
					88.47056669347421
				],
				[
					1.411779067095722,
					88.47056669347421
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.234375,
				0.326171875,
				0.375,
				0.4638671875,
				0.501953125,
				0.5224609375,
				0.525390625,
				0.525390625,
				0.515625,
				0.5048828125,
				0.48046875,
				0.48046875,
				0.48046875,
				0.48046875,
				0.5185546875,
				0.546875,
				0.57421875,
				0.58984375,
				0.6025390625,
				0.6103515625,
				0.6103515625,
				0.607421875,
				0.607421875,
				0.5810546875,
				0.5791015625,
				0.5791015625,
				0.576171875,
				0.5732421875,
				0.5732421875,
				0.5693359375,
				0.560546875,
				0.552734375,
				0.55078125,
				0.55078125,
				0.5615234375,
				0.568359375,
				0.5830078125,
				0.5830078125,
				0.5810546875,
				0.5712890625,
				0.5712890625,
				0.5546875,
				0.509765625,
				0.41796875,
				0.015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 146,
			"versionNonce": 1315448249,
			"isDeleted": false,
			"id": "fFBi_ewZNgohIVb4VMzLA",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 6600.208807446995,
			"y": -453.2780912889866,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 42.35294117647072,
			"height": 93.64706600413592,
			"seed": 1755337726,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					4.235265395220722,
					0
				],
				[
					7.999985638786711,
					0.4705810546875
				],
				[
					12.705867991728155,
					1.4117790670952672
				],
				[
					17.411750344669144,
					3.294139188878489
				],
				[
					23.058794806985134,
					7.058823529411711
				],
				[
					25.411735983455856,
					10.8235437729777
				],
				[
					25.411735983455856,
					15.05884507123119
				],
				[
					23.529411764705856,
					19.764727424172634
				],
				[
					20.235236672794144,
					24.470609777113623
				],
				[
					17.411750344669144,
					29.647073184742567
				],
				[
					13.176413143382433,
					34.823536592371056
				],
				[
					12.705867991728155,
					36.23531565946678
				],
				[
					14.117647058823422,
					37.17647776884178
				],
				[
					18.823529411764866,
					37.17647776884178
				],
				[
					22.117632697610134,
					36.70589671415428
				],
				[
					25.882352941176578,
					37.17647776884178
				],
				[
					28.235294117646845,
					38.11763987821678
				],
				[
					29.647001378676578,
					39.058837890625
				],
				[
					30.117618336396845,
					39.5294189453125
				],
				[
					28.705839269301578,
					41.88236012178277
				],
				[
					26.352898092830856,
					43.29413918887849
				],
				[
					23.999956916360134,
					45.64708036534921
				],
				[
					20.235236672794144,
					49.41176470588198
				],
				[
					18.352912454044144,
					52.2352869370402
				],
				[
					17.411750344669144,
					54.11764705882342
				],
				[
					17.411750344669144,
					55.52942612591869
				],
				[
					18.352912454044144,
					56.47058823529369
				],
				[
					21.176470588235134,
					57.41178624770191
				],
				[
					26.823515050551578,
					58.35294835707691
				],
				[
					31.999942555146845,
					59.29411046645191
				],
				[
					40,
					62.117668600643356
				],
				[
					40.941162109375,
					63.058830710018356
				],
				[
					42.35294117647072,
					66.35293399586362
				],
				[
					40,
					72.47059541590033
				],
				[
					36.235279756433556,
					76.23531565946678
				],
				[
					20.705853630514866,
					84.23530129825349
				],
				[
					17.882295496323422,
					85.64708036534921
				],
				[
					14.588192210478155,
					87.52940458409921
				],
				[
					7.999985638786711,
					90.8235437729777
				],
				[
					3.294103285845722,
					93.64706600413592
				],
				[
					3.294103285845722,
					93.64706600413592
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.333984375,
				0.328125,
				0.3310546875,
				0.373046875,
				0.4169921875,
				0.43359375,
				0.4384765625,
				0.44140625,
				0.443359375,
				0.4501953125,
				0.4794921875,
				0.5205078125,
				0.5224609375,
				0.5244140625,
				0.5126953125,
				0.5166015625,
				0.5166015625,
				0.513671875,
				0.513671875,
				0.51171875,
				0.515625,
				0.52734375,
				0.53515625,
				0.541015625,
				0.5458984375,
				0.5478515625,
				0.5517578125,
				0.5537109375,
				0.55078125,
				0.548828125,
				0.546875,
				0.55078125,
				0.5537109375,
				0.5615234375,
				0.5751953125,
				0.58984375,
				0.6220703125,
				0.6162109375,
				0.6025390625,
				0.44921875,
				0.015625,
				0
			]
		},
		{
			"type": "text",
			"version": 89,
			"versionNonce": 1437402777,
			"isDeleted": false,
			"id": "yPZGGe5u",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 5361.855841138404,
			"y": -300.10160633953683,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 149,
			"height": 25,
			"seed": 2112660414,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
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
			"baseline": 18
		},
		{
			"type": "text",
			"version": 486,
			"versionNonce": 1734527865,
			"isDeleted": false,
			"id": "XKzBRoaq",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 5436.080603574208,
			"y": -175.45398608617552,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 452,
			"height": 325,
			"seed": 1336919358,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955787976,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "- if (s[0] is opener) \n    - currOpener = s[0]\n- else \n    - return false\n- iterate s\n    - if s[i] is opener\n        - currOpener = next\n    - if s[i] is correspondingCloser(curropener)\n        - delete currentOpener and s[i]\n        - start over \n    - else\n        - return false\n- return true",
			"rawText": "- if (s[0] is opener) \n    - currOpener = s[0]\n- else \n    - return false\n- iterate s\n    - if s[i] is opener\n        - currOpener = next\n    - if s[i] is correspondingCloser(curropener)\n        - delete currentOpener and s[i]\n        - start over \n    - else\n        - return false\n- return true",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "- if (s[0] is opener) \n    - currOpener = s[0]\n- else \n    - return false\n- iterate s\n    - if s[i] is opener\n        - currOpener = next\n    - if s[i] is correspondingCloser(curropener)\n        - delete currentOpener and s[i]\n        - start over \n    - else\n        - return false\n- return true",
			"lineHeight": 1.25,
			"baseline": 318
		},
		{
			"type": "freedraw",
			"version": 402,
			"versionNonce": 1152674711,
			"isDeleted": false,
			"id": "1DkcQeCD0tfr1SnhtFrUq",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2395.5579003210423,
			"y": -73.67417475751063,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 12.004568800389206,
			"height": 22.917828302845244,
			"seed": 28253668,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955778334,
			"link": null,
			"locked": false,
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
			"version": 400,
			"versionNonce": 342941879,
			"isDeleted": false,
			"id": "qL2qOP6t0VfdSKCKyjm4w",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2394.466570207718,
			"y": -41.48005089910896,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 9.8219293891321,
			"height": 17.461198551617255,
			"seed": 1893419876,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955778334,
			"link": null,
			"locked": false,
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
			"version": 399,
			"versionNonce": 1528934871,
			"isDeleted": false,
			"id": "g4WcCiIUGq5bAEEczV7LD",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2392.283909981071,
			"y": -37.114730445814075,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 7.639289977874991,
			"height": 22.917828302845297,
			"seed": 295556452,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955778334,
			"link": null,
			"locked": false,
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
			"version": 391,
			"versionNonce": 1910202103,
			"isDeleted": false,
			"id": "ZVUtzZzCOES0vhOyr3CM4",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2390.64692521878,
			"y": 9.812277088590747,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 3.8196241735464076,
			"height": 8.184944626842093,
			"seed": 1657709660,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955778334,
			"link": null,
			"locked": false,
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
			"version": 407,
			"versionNonce": 455239703,
			"isDeleted": false,
			"id": "wWaNjF2LOj3D5Dgci2ixG",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2387.9186103431666,
			"y": 15.81456148878533,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 10.9132595024562,
			"height": 22.372173653878683,
			"seed": 81758300,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955778334,
			"link": null,
			"locked": false,
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
			"version": 401,
			"versionNonce": 1424706871,
			"isDeleted": false,
			"id": "Yae8gClQPsRhtgApektVf",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2391.1925798677466,
			"y": 39.82374072034497,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 11.458934966813358,
			"height": 17.4612401823984,
			"seed": 244666460,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955778334,
			"link": null,
			"locked": false,
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
			"version": 401,
			"versionNonce": 1788513879,
			"isDeleted": false,
			"id": "WDJwtPxOUlzKjpvNKZ6uq",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2384.6446408185857,
			"y": 64.37857460087116,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 8.73062009119909,
			"height": 18.552549480331514,
			"seed": 1862400732,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955778334,
			"link": null,
			"locked": false,
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
			"version": 399,
			"versionNonce": 1191488375,
			"isDeleted": false,
			"id": "VQCMsrfTiiPoDrpnMNAVD",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2392.283909981071,
			"y": 89.47906313036384,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 10.9132595024562,
			"height": 13.095919729103525,
			"seed": 571577692,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955778334,
			"link": null,
			"locked": false,
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
			"version": 385,
			"versionNonce": 107881623,
			"isDeleted": false,
			"id": "elFx3phLJBMhzuUL1I1ZD",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2386.8272802298434,
			"y": 120.58183606005127,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 1.6369847622901685,
			"height": 18.006853200583866,
			"seed": 478299364,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955778334,
			"link": null,
			"locked": false,
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
			"version": 395,
			"versionNonce": 1217100215,
			"isDeleted": false,
			"id": "CXubDOUDlLikJEqih4rfl",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2380.279320365291,
			"y": 147.31933016722496,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 10.36760485348926,
			"height": 17.4612401823984,
			"seed": 277263972,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955778334,
			"link": null,
			"locked": false,
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
			"version": 439,
			"versionNonce": 1115761367,
			"isDeleted": false,
			"id": "O_yNuEUA1LQVpXBMRneme",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2374.8226906140626,
			"y": 156.04997107381473,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 548.3913108138083,
			"height": 25.10053016027382,
			"seed": 1199622500,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955778334,
			"link": null,
			"locked": false,
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
			"version": 432,
			"versionNonce": 283359223,
			"isDeleted": false,
			"id": "3xQbE4d5ogHNdjrh8xAxy",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2424.478033839472,
			"y": 135.86041601580234,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 6.547939049161543,
			"height": 37.65075360962959,
			"seed": 1009662308,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955778334,
			"link": null,
			"locked": false,
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
			"version": 425,
			"versionNonce": 1236771095,
			"isDeleted": false,
			"id": "-fVB2RQtKx73ZwQaKfMfj",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2470.3137112605527,
			"y": -83.49608333125241,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 6.002305215584823,
			"height": 235.1807755825534,
			"seed": 1059871964,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955778334,
			"link": null,
			"locked": false,
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
			"version": 426,
			"versionNonce": 1316054583,
			"isDeleted": false,
			"id": "k4Nk0VBIMYB2CEYgHDHEY",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2467.5853963849404,
			"y": -74.76548405544378,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 2.1826602266473274,
			"height": 217.17388075118834,
			"seed": 1624048356,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955778334,
			"link": null,
			"locked": false,
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
			"version": 417,
			"versionNonce": 1576372055,
			"isDeleted": false,
			"id": "wCPURhtYGwsNY_g_061Qa",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2514.5124247347358,
			"y": -30.0211367476864,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 2.1826602266473274,
			"height": 160.4249230122606,
			"seed": 1488460388,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955778334,
			"link": null,
			"locked": false,
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
			"version": 417,
			"versionNonce": 1721271415,
			"isDeleted": false,
			"id": "TzBskays86CLJsdsA1oIM",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2513.966770085768,
			"y": -16.379562369616224,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 2.728314875614267,
			"height": 165.8815111327074,
			"seed": 390124516,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955778334,
			"link": null,
			"locked": false,
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
			"version": 405,
			"versionNonce": 404675991,
			"isDeleted": false,
			"id": "K4bMImxqNMlPtvNQAP58f",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2562.5307831978553,
			"y": 78.56580362790777,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 3.2740111553625133,
			"height": 75.84716186822595,
			"seed": 1914871140,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955778334,
			"link": null,
			"locked": false,
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
			"version": 396,
			"versionNonce": 901583543,
			"isDeleted": false,
			"id": "gc_0qmj9kvewxcrxC4ZH5",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2561.9850869181064,
			"y": 85.11374267706896,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 3.273969524580337,
			"height": 60.02292726350837,
			"seed": 406925796,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955778334,
			"link": null,
			"locked": false,
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
			"version": 411,
			"versionNonce": 672637911,
			"isDeleted": false,
			"id": "5vHTD-HlibR5uidfXoSMT",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2616.00572978142,
			"y": -0.00967311593217346,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 4.365278822514216,
			"height": 134.23308355405345,
			"seed": 410969316,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955778334,
			"link": null,
			"locked": false,
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
			"version": 419,
			"versionNonce": 1329795319,
			"isDeleted": false,
			"id": "f-hRZXoeWABoY9ziH6kyJ",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2613.277414905806,
			"y": 5.992611284262466,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 4.365278822514216,
			"height": 143.50937910960988,
			"seed": 541570020,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955778334,
			"link": null,
			"locked": false,
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
			"version": 409,
			"versionNonce": 348379671,
			"isDeleted": false,
			"id": "D1s0VFjEnicBEfYFdginh",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2660.7501187199587,
			"y": 21.271191240013422,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 4.365278822514216,
			"height": 120.04585452701681,
			"seed": 1871608540,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955778334,
			"link": null,
			"locked": false,
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
			"version": 406,
			"versionNonce": 1032748855,
			"isDeleted": false,
			"id": "aXRL8wJmNfn05Qds5Wu_W",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2658.0218038443445,
			"y": 30.547445164788655,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 5.456629751227665,
			"height": 112.95221919810795,
			"seed": 1729791836,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955778334,
			"link": null,
			"locked": false,
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
			"version": 425,
			"versionNonce": 2080866391,
			"isDeleted": false,
			"id": "kDUI3J6KIW4rszWt3aN1u",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2706.040120676683,
			"y": -82.9504286822858,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 4.910975102261594,
			"height": 217.71949376937368,
			"seed": 620071260,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955778334,
			"link": null,
			"locked": false,
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
			"version": 407,
			"versionNonce": 1107516791,
			"isDeleted": false,
			"id": "SVtIHXZSlj8YpPIJjwMzR",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2756.7867940154165,
			"y": 37.095425844730926,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 2.18261859586602,
			"height": 91.12570019319571,
			"seed": 1321609692,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955778334,
			"link": null,
			"locked": false,
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
			"version": 396,
			"versionNonce": 1388746391,
			"isDeleted": false,
			"id": "HZQ5J_px-ee0KOkn09uSm",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2754.0584791398014,
			"y": 40.36939536931152,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 3.273969524580337,
			"height": 84.57776114403461,
			"seed": 642314716,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955778334,
			"link": null,
			"locked": false,
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
			"version": 380,
			"versionNonce": 352693175,
			"isDeleted": false,
			"id": "kh7_xJ9LXzMyUgGgoVKI0",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2797.1658625006603,
			"y": -60.57825502840711,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 0.5456546489660709,
			"height": 0.5456546489666135,
			"seed": 1059347684,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955778334,
			"link": null,
			"locked": false,
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
			"version": 414,
			"versionNonce": 618994903,
			"isDeleted": false,
			"id": "RcZmvPikcr5pMrtBRTG22",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2798.8028264475597,
			"y": -62.76091525505461,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 1.09130929793301,
			"height": 199.16698591982342,
			"seed": 1138175068,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955778334,
			"link": null,
			"locked": false,
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
			"version": 388,
			"versionNonce": 637102583,
			"isDeleted": false,
			"id": "LTH65pp7sdcRyFINgzkRZ",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2452.852512708936,
			"y": -81.31342310460496,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 21.280843540555235,
			"height": 2.728314875613995,
			"seed": 1659378148,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955778334,
			"link": null,
			"locked": false,
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
			"version": 385,
			"versionNonce": 1430721303,
			"isDeleted": false,
			"id": "447YGBr1oqM-DYH0nz6Rt",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2452.3068372445796,
			"y": -80.22211380667187,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 24.55483388052579,
			"height": 3.2739695245805542,
			"seed": 1642880740,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955778334,
			"link": null,
			"locked": false,
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
			"version": 384,
			"versionNonce": 1531090999,
			"isDeleted": false,
			"id": "MAiRkdh2CAQL5-xr12Twv",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2693.4898972273268,
			"y": -82.40477403331926,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 19.6438587782642,
			"height": 2.1826185958662916,
			"seed": 1851822180,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955778334,
			"link": null,
			"locked": false,
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
			"version": 386,
			"versionNonce": 1573943639,
			"isDeleted": false,
			"id": "bKuTonufW3GuYNcM_aCrk",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2692.944200947579,
			"y": -82.9504286822858,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 18.006894831365116,
			"height": 1.6369639468997321,
			"seed": 493963740,
			"groupIds": [
				"UfUMjzjtELzKDi-gv7ArM"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1718955778334,
			"link": null,
			"locked": false,
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
		"scrollX": 1292.2774589927324,
		"scrollY": 2118.302916877536,
		"zoom": {
			"value": 0.1420337802730137
		},
		"currentItemRoundness": "round",
		"gridSize": null,
		"gridColor": {
			"Bold": "#C9C9C9FF",
			"Regular": "#EDEDEDFF"
		},
		"currentStrokeOptions": null,
		"previousGridSize": null,
		"frameRendering": {
			"enabled": true,
			"clip": true,
			"name": true,
			"outline": true
		}
	},
	"files": {}
}
```
%%