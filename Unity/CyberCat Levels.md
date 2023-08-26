---

excalidraw-plugin: parsed
tags: [excalidraw]

---
==⚠  Switch to EXCALIDRAW VIEW in the MORE OPTIONS menu of this document. ⚠==


# Text Elements
start ^KOmb3hNR

Push / Pull ^DLyswqdy

Long Jump ^1dPpCltE

Crouch ^2NrlQHM3

Climb ^GJioXrEd

Elevator switch ^wRrxYeIM

TUTORIAL ^Y7fJsHIE

INTO CINEMATIC ^XnebrG71

1. While waiting for the elevator to reach floor, 
move the camera to the other side of the 
building and focus on the gray cat ^58qwBuPV

3. Cat get on elevator 
and clicks the inside switch ^pJILEGOk

2. While waiting for the elevator to reach floor, 
move the camera to the other side of the 
building and focus on the gray cat ^QZ8r8jyF

4. title of the game and
roll the intro credits as the 
elevator goes down ^d882DXuB

PUZZLE ^3Zjzee5i

Elevator switch ^jsWk1e1G

5. Get to the end of the level
and click the elevator button to 
start the level ending animation, which
cat jump on platform and clicks to go up
as level ends with more credits and screen
darkens ^wBp8WhoR

push trash
can to climb ^bYLndyoR

wall jump 
to get up ^TH8nHuZN

can go down or wait 
to go up for treat ^znUFCY96

another small view before exit ^WuLo0oNq

Death pit ^aTqZLtwX

Level 1 ^8AmIuv51

Level 3 ^xbzj1fqc

window entrance ^1W89ZfLC

living room ^1xAcZOHy

kitchen ^HM41WlYg

pet door ^VNBXdAFo

Level 1 ^mIzoYf2G

Level 2 ^ANQHjpkg

Level 3 ^hsmRdwOT

parking lot ^NyonXevM

building puzzle ^qL98QAo1

Factory space 1 ^XFxnWaUJ

Level 6 ^RhZtrxjb

apartment floor 1 ^VzRCZTgr

Crowded street ^OBxeOJcW

Level 5 ^01i6Y166

apartment floor 2 ^sMkOQ8YJ

Level 4 ^LmD2A6AP

Factory space 2 ^RZzEna0D

Level 7 ^AfdVGiEy

Factory space 3 ^9iaSVHGq

Level 8 ^7KiHeXge

Factory roof 1 ^kyuLcY9D

Level 9 ^eNsn9j25

Factory roof 2 ^v3ivSRJL

Level 10 ^Be4UxvXF

Level 2 ^BC7X5gmz

Cinematic 2 ^K9zb3C8G

Cinematic 1 ^CCzK6JWe

Level 1 ^RrDHGcxz

Level 2 ^B6D0cq9k

Cinematic 1 ^9ZWnqF35

Cinematic Title ^eU2e0gUt

Main Menu ^Yo1XFulB

START ^FlNNEoYi

QUIT ^D2d1xSMr

Cutscene to go to the Main Menu screen ^jqAvLTlE

PLAYER
-----------------------
* movement
    + run / infinite runner
    + sprint
    + crouch
    + jump
    + climb ledge
    + climb ladder / net
    + wall jump
    + zipline top / bottom
    + swim
    + press trigger
    + jetpack
    - push / pull
    - charge jump
    - dash
    - double jump ^XTNuy0YH

LEVEL STRUCTURES
----------------------------
+ floor
+ death zone
+ ziplines top / bottom
+ water
+ push areas
+ trigger areas
+ moving platforms
+ moving ladders
+ rotating platforms
+ path mover
- elevator
 ^1WhKaQif

CutScene 1 ^GyIFFF5J

Main Menu ^UlGhBpfj

Cutscene Title ^nYOl2Kmq

Cutscene 2 ^3rV4nASB

      Credits

Creddits ...... Credits
Creddits ...... Credits
Creddits ...... Credits
Creddits ...... Credits



Creddits ...... Credits
Creddits ...... Credits
Creddits ...... Credits ^uo6I2VYy

LevelLoader ^Ag0HUSoO

Crossfade ^x2LqxMHA

public class LevelLoarer: MonoBehavior
{
	public Animator transition;
	public float transitionTime = 1f;
	void Update()
	{
		if(Input.GetMouseButtonDown(0))
		{
			LoadNextLevel();
		}
	}
	
	public void LoadNextLevel()
	{
		StartCoroutine(
			LoadLevel(
				SceneManager.LoadScene(SceneManager.GetActiveScene().buildIndex + 1))
		);
		
	}

	IEnumerator LoadLevel(int levelIndex)
	{
		// Play animation
		transition.setTrigger("Start");
		// wait for animation
		yield return waitForSeconds(transitionTime);
		// load scene
		SceneManager.LoadScene(levelIndex)
	}
} ^ybRvbzcX

This is for testing purposes for now ^pMOfPeGA

This is how you start a coroutine ^EpxldSKq

This is to go the ne next scene ^RuemmRxY

The coroutine is needed because we need to make the game wait for the transition to finish ^MmUauxRW

%%
# Drawing
```json
{
	"type": "excalidraw",
	"version": 2,
	"source": "https://github.com/zsviczian/obsidian-excalidraw-plugin/releases/tag/1.9.16",
	"elements": [
		{
			"type": "rectangle",
			"version": 1936,
			"versionNonce": 1232324382,
			"isDeleted": false,
			"id": "yAntY11JDi4DoeARXBacX",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1714.1360872867824,
			"y": -1085.2335966487963,
			"strokeColor": "#ffffff",
			"backgroundColor": "#e9ecef",
			"width": 76.51686173499583,
			"height": 305.69410025169924,
			"seed": 1951687275,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577638,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 866,
			"versionNonce": 233193922,
			"isDeleted": false,
			"id": "YBIqjy2htsa4DLTsGFkuO",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -191.96814745554434,
			"y": 732.092505599582,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 588.5714808872768,
			"height": 876.8283168247768,
			"seed": 1830073228,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"id": "OEo2gw4tZjpm-QB0U9npo",
					"type": "arrow"
				}
			],
			"updated": 1692815577638,
			"link": null,
			"locked": false
		},
		{
			"type": "ellipse",
			"version": 752,
			"versionNonce": 1542009694,
			"isDeleted": false,
			"id": "HlKFbaEjzE4G3G8QsZG1T",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -210.91265218440475,
			"y": 239.80364167906305,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 94,
			"height": 52,
			"seed": 656045964,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "KOmb3hNR"
				}
			],
			"updated": 1692815577638,
			"link": null,
			"locked": true
		},
		{
			"type": "text",
			"version": 886,
			"versionNonce": 419215746,
			"isDeleted": false,
			"id": "KOmb3hNR",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -191.6466709001725,
			"y": 253.4188653682128,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 55,
			"height": 25,
			"seed": 121842740,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577638,
			"link": null,
			"locked": true,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "start",
			"rawText": "start",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "HlKFbaEjzE4G3G8QsZG1T",
			"originalText": "start",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "freedraw",
			"version": 258,
			"versionNonce": 224860062,
			"isDeleted": false,
			"id": "YEU34Dkrq4g2UUtqCKRRt",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1142.6032054964846,
			"y": -490.161098647069,
			"strokeColor": "#f08c00",
			"backgroundColor": "#ffd8a8",
			"width": 0.0001,
			"height": 0.0001,
			"seed": 879995444,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577638,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.0001,
					0.0001
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "ellipse",
			"version": 1299,
			"versionNonce": 837695810,
			"isDeleted": false,
			"id": "NzeAwS11Ue1jZeUqDoj4I",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -33.97377726942568,
			"y": 5798.690075071005,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 35.35451402270802,
			"height": 30.216021323334978,
			"seed": 1837402764,
			"groupIds": [
				"rz9oQN36t0NUtb0jQqXzN"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692815577638,
			"link": null,
			"locked": false
		},
		{
			"type": "freedraw",
			"version": 1082,
			"versionNonce": 1444836318,
			"isDeleted": false,
			"id": "V6pF5upVUQCJEMzD0YU4n",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -32.63434891226166,
			"y": 5806.932610514876,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 7.725873087445037,
			"height": 12.642329660491377,
			"seed": 815911180,
			"groupIds": [
				"rz9oQN36t0NUtb0jQqXzN"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577638,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					-0.23411357743629757
				],
				[
					0,
					-0.46822715487259514
				],
				[
					-7.246620131370148e-17,
					-1.1705857489025295
				],
				[
					0.2341135774362977,
					-2.1070579203687427
				],
				[
					0.23411357743629785,
					-3.511757246707551
				],
				[
					0.23411357743629757,
					-5.8529287445125915
				],
				[
					0.23411357743629757,
					-7.725855225723995
				],
				[
					0,
					-9.130572413783826
				],
				[
					0,
					-10.067026723529036
				],
				[
					0,
					-11.237612472431547
				],
				[
					0,
					-11.471743911588867
				],
				[
					0,
					-11.939971066461462
				],
				[
					0,
					-12.17408464389776
				],
				[
					0,
					-12.408198221334057
				],
				[
					0,
					-12.642329660491377
				],
				[
					0.23411357743629757,
					-12.642329660491377
				],
				[
					0.7023585940299343,
					-12.642329660491377
				],
				[
					1.1705857489025295,
					-12.408198221334057
				],
				[
					2.1070579203687614,
					-11.471743911588867
				],
				[
					2.341171497805059,
					-11.003498894995248
				],
				[
					2.8094165143986585,
					-10.301158162686356
				],
				[
					3.043530091834956,
					-9.598799568656421
				],
				[
					3.277643669271254,
					-9.130572413783826
				],
				[
					3.7458708241438488,
					-8.662327397190209
				],
				[
					3.980002263301188,
					-8.42821381975391
				],
				[
					4.2141158407374855,
					-8.194100242317614
				],
				[
					4.448229418173783,
					-7.725855225723995
				],
				[
					4.9164565730463785,
					-6.7894009159788045
				],
				[
					5.150588012203681,
					-6.321155899385187
				],
				[
					5.852928744512573,
					-6.087042321948889
				],
				[
					6.7894009159788045,
					-6.321155899385187
				],
				[
					7.725873087445037,
					-7.023514493415102
				],
				[
					7.725873087445037,
					-7.023514493415102
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.181640625,
				0.21484375,
				0.310546875,
				0.359375,
				0.40625,
				0.447265625,
				0.4853515625,
				0.49609375,
				0.501953125,
				0.51171875,
				0.5185546875,
				0.521484375,
				0.5263671875,
				0.53515625,
				0.5263671875,
				0.5263671875,
				0.53125,
				0.529296875,
				0.529296875,
				0.529296875,
				0.52734375,
				0.52734375,
				0.52734375,
				0.52734375,
				0.52734375,
				0.52734375,
				0.52734375,
				0.52734375,
				0.5302734375,
				0.537109375,
				0.529296875,
				0.4189453125,
				0.015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 1084,
			"versionNonce": 2014953730,
			"isDeleted": false,
			"id": "q_rxnEbEfWyfYrgr9JyaK",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -7.81793460787236,
			"y": 5801.547926786958,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 7.023514493415066,
			"height": 12.40821608305508,
			"seed": 1916065588,
			"groupIds": [
				"rz9oQN36t0NUtb0jQqXzN"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577638,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					-0.4682450165936367
				],
				[
					0.23413143915730197,
					-0.4682450165936367
				],
				[
					0.7023585940298972,
					-1.6388307654961476
				],
				[
					1.6388307654961292,
					-2.575302936962361
				],
				[
					2.5753029369623235,
					-3.745888685864872
				],
				[
					3.980002263301151,
					-4.682342995610081
				],
				[
					4.916474434767383,
					-5.618815167076294
				],
				[
					5.852928744512573,
					-6.7894009159788045
				],
				[
					6.087060183669875,
					-7.257645932572423
				],
				[
					6.55528733854247,
					-7.491759510008721
				],
				[
					6.789400915978768,
					-7.725873087445018
				],
				[
					7.023514493415066,
					-7.725873087445018
				],
				[
					7.023514493415066,
					-7.257645932572423
				],
				[
					7.023514493415066,
					-6.555287338542508
				],
				[
					7.023514493415066,
					-5.618815167076294
				],
				[
					7.023514493415066,
					-4.682342995610081
				],
				[
					7.023514493415066,
					-3.511757246707551
				],
				[
					6.789400915978768,
					-2.575302936962361
				],
				[
					6.789400915978768,
					-1.6388307654961476
				],
				[
					6.789400915978768,
					-0.4682450165936367
				],
				[
					6.55528733854247,
					0.46822715487259514
				],
				[
					6.321173761106173,
					1.4046993263388086
				],
				[
					6.087060183669875,
					2.3411714978050218
				],
				[
					6.087060183669875,
					2.5752850752413194
				],
				[
					6.087060183669875,
					2.809398652677617
				],
				[
					6.087060183669875,
					3.277625807550212
				],
				[
					5.852928744512573,
					3.74587082414383
				],
				[
					5.852928744512573,
					4.214097979016425
				],
				[
					5.852928744512573,
					4.448211556452741
				],
				[
					6.087060183669875,
					4.682342995610062
				],
				[
					6.321173761106173,
					4.682342995610062
				],
				[
					6.789400915978768,
					4.682342995610062
				],
				[
					6.789400915978768,
					4.682342995610062
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.177734375,
				0.2587890625,
				0.28125,
				0.3544921875,
				0.388671875,
				0.408203125,
				0.4228515625,
				0.435546875,
				0.455078125,
				0.4658203125,
				0.4736328125,
				0.486328125,
				0.4951171875,
				0.5126953125,
				0.5126953125,
				0.5126953125,
				0.5126953125,
				0.5126953125,
				0.51171875,
				0.51171875,
				0.51171875,
				0.517578125,
				0.51953125,
				0.525390625,
				0.525390625,
				0.525390625,
				0.525390625,
				0.525390625,
				0.53125,
				0.515625,
				0.486328125,
				0.296875,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 1110,
			"versionNonce": 2115614,
			"isDeleted": false,
			"id": "UKr2DF5CiKfEJAVZr18fg",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -17.460404189330404,
			"y": 5816.769940803635,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 4.426936146712468,
			"height": 2.459408970395818,
			"seed": 1546858124,
			"groupIds": [
				"rz9oQN36t0NUtb0jQqXzN"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577638,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.09837485771173488,
					0
				],
				[
					-0.19675722094399972,
					-4.163336342344337e-17
				],
				[
					-0.295132078655716,
					-0.19675722094399048
				],
				[
					-0.5902566517909021,
					-0.39350693636743245
				],
				[
					-0.9837635881583155,
					-0.6886390150231491
				],
				[
					-1.4756453822374829,
					-0.8853887304465995
				],
				[
					-1.7707774608932176,
					-1.1805208091023165
				],
				[
					-2.0659020340283667,
					-1.6724026031814738
				],
				[
					-2.1642843972606305,
					-1.8691523186049248
				],
				[
					-2.2626592549723665,
					-1.9675271763166509
				],
				[
					-2.2626592549723665,
					-2.0659020340283765
				],
				[
					-2.164284397260632,
					-2.065902034028376
				],
				[
					-2.065902034028367,
					-2.0659020340283765
				],
				[
					-1.9675271763166504,
					-2.1642843972606407
				],
				[
					-1.672402603181483,
					-2.164284397260641
				],
				[
					-1.2788956668140503,
					-2.262659254972367
				],
				[
					-0.9837635881583154,
					-2.164284397260641
				],
				[
					-0.5902566517909018,
					-2.065902034028377
				],
				[
					-0.19675722094399994,
					-2.0659020340283765
				],
				[
					0.09837485771173504,
					-1.9675271763166506
				],
				[
					0.3935069363674325,
					-1.967527176316651
				],
				[
					0.5902566517908836,
					-1.9675271763166506
				],
				[
					0.8853887304465997,
					-2.065902034028376
				],
				[
					1.0821384458700507,
					-2.164284397260641
				],
				[
					1.1805133035817852,
					-2.164284397260642
				],
				[
					1.278888161293502,
					-2.164284397260641
				],
				[
					1.377270524525767,
					-2.1642843972606416
				],
				[
					1.4756453822374849,
					-2.164284397260641
				],
				[
					1.574020239949218,
					-2.2626592549723674
				],
				[
					1.672395097660953,
					-2.3610341126840924
				],
				[
					1.7707699553726697,
					-2.361034112684093
				],
				[
					1.8691523186049341,
					-2.3610341126840924
				],
				[
					1.96752717631665,
					-2.4594089703958186
				],
				[
					2.0659020340283663,
					-2.361034112684092
				],
				[
					2.1642768917401014,
					-2.3610341126840924
				],
				[
					2.0659020340283663,
					-2.2626592549723665
				],
				[
					1.9675271763166509,
					-2.164284397260641
				],
				[
					1.8691523186049341,
					-2.0659020340283765
				],
				[
					1.7707699553726697,
					-1.9675271763166504
				],
				[
					1.6723950976609527,
					-1.8691523186049257
				],
				[
					1.5740202399492182,
					-1.6724026031814736
				],
				[
					1.377270524525767,
					-1.4756453822374926
				],
				[
					1.2788881612935024,
					-1.2788956668140417
				],
				[
					1.1805133035817859,
					-1.1805208091023154
				],
				[
					1.082138445870051,
					-1.0821384458700511
				],
				[
					0.9837635881583158,
					-0.9837635881583251
				],
				[
					0.7870063672143349,
					-0.8853887304465996
				],
				[
					0.6886315095026185,
					-0.7870138727348743
				],
				[
					0.5902566517908835,
					-0.6886390150231486
				],
				[
					0.4918817940791674,
					-0.5902566517908836
				],
				[
					0.39350693636743245,
					-0.49188179407915816
				],
				[
					0.2951245731351675,
					-0.3935069363674324
				],
				[
					0.2951245731351676,
					-0.29513207865571606
				],
				[
					0.1967497154234513,
					-0.19675722094399048
				],
				[
					0.19674971542345118,
					-0.0983748577117256
				],
				[
					0.2951245731351675,
					-0.09837485771172573
				],
				[
					0.4918817940791673,
					-0.1967572209439904
				],
				[
					0,
					0
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.171875,
				0.232421875,
				0.373046875,
				0.4453125,
				0.47265625,
				0.4912109375,
				0.5068359375,
				0.517578125,
				0.5234375,
				0.5234375,
				0.5234375,
				0.5234375,
				0.51953125,
				0.51953125,
				0.5166015625,
				0.5166015625,
				0.513671875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.513671875,
				0.51171875,
				0.51171875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.5166015625,
				0.513671875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.521484375,
				0.521484375,
				0.513671875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.4873046875,
				0.4306640625,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 1070,
			"versionNonce": 1191071938,
			"isDeleted": false,
			"id": "Yfh_XLg8KcOcVOorHfD5X",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -18.050660841121555,
			"y": 5817.655329534082,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 0.29512457313518725,
			"height": 3.443172558554153,
			"seed": 90357044,
			"groupIds": [
				"rz9oQN36t0NUtb0jQqXzN"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577638,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-6.938893903907228e-18,
					0.09837485771172562
				],
				[
					0.09837485771173488,
					0.2951245731351768
				],
				[
					0.09837485771173482,
					0.7870063672143441
				],
				[
					0.09837485771173493,
					1.1805133035817859
				],
				[
					0.19674971542346986,
					1.4756453822374926
				],
				[
					0.1967497154234692,
					1.8691448130843946
				],
				[
					0.19674971542346986,
					2.065902034028386
				],
				[
					0.19674971542346986,
					2.3610266071635624
				],
				[
					0.19674971542347008,
					2.6561586858192694
				],
				[
					0.09837485771173538,
					2.6561586858192694
				],
				[
					0.09837485771173471,
					2.7545335435309948
				],
				[
					0.09837485771173493,
					2.951290764474986
				],
				[
					0,
					3.1480404798984365
				],
				[
					-1.3322676295501878e-15,
					3.2464153376101628
				],
				[
					-2.220446049250313e-16,
					3.3447901953218877
				],
				[
					0,
					3.443172558554153
				],
				[
					0.19674971542347075,
					3.443172558554153
				],
				[
					0.2951245731351857,
					3.344790195321888
				],
				[
					0.2951245731351857,
					3.344790195321888
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.1953125,
				0.30078125,
				0.3388671875,
				0.37109375,
				0.38671875,
				0.3994140625,
				0.4111328125,
				0.42578125,
				0.4345703125,
				0.4501953125,
				0.4560546875,
				0.4677734375,
				0.470703125,
				0.470703125,
				0.470703125,
				0.470703125,
				0.474609375,
				0.3720703125,
				0.275390625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 1104,
			"versionNonce": 1801294942,
			"isDeleted": false,
			"id": "2nMooQr71Hc2BdbyZblro",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -21.00195160559639,
			"y": 5820.606620298557,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 8.066858420690073,
			"height": 2.3610341126840924,
			"seed": 225779596,
			"groupIds": [
				"rz9oQN36t0NUtb0jQqXzN"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577638,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					0.09837485771172562
				],
				[
					0.09837485771171633,
					0.19674971542345124
				],
				[
					0.29512457313518625,
					0.2951245731351768
				],
				[
					0.3934994308469025,
					0.4918817940791673
				],
				[
					0.5902566517908836,
					0.6886315095026185
				],
				[
					0.7870063672143349,
					0.8853812249260605
				],
				[
					0.9837635881583343,
					0.9837635881583253
				],
				[
					1.1805133035817674,
					1.0821384458700507
				],
				[
					1.2788881612935021,
					0.9837635881583253
				],
				[
					1.475645382237502,
					0.9837635881583253
				],
				[
					1.5740202399492182,
					0.8853812249260602
				],
				[
					1.6723950976609347,
					0.7870063672143349
				],
				[
					1.7707699553726512,
					0.5902566517908931
				],
				[
					1.869144813084386,
					0.3934994308469025
				],
				[
					2.0659020340283862,
					0.09837485771172576
				],
				[
					2.2626517494518184,
					-0.09838236323226501
				],
				[
					2.361026607163553,
					-0.1967572209439902
				],
				[
					2.361026607163553,
					-0.2951320786557161
				],
				[
					2.459408970395818,
					-0.39350693636744155
				],
				[
					2.459408970395818,
					-0.49188179407915805
				],
				[
					2.557783828107553,
					-0.4918817940791582
				],
				[
					2.5577838281075533,
					-0.5902641573114237
				],
				[
					2.7545335435309855,
					-0.5902641573114233
				],
				[
					2.852908401242702,
					-0.5902641573114229
				],
				[
					2.9512907644749666,
					-0.4918817940791582
				],
				[
					3.049665622186702,
					-0.49188179407915805
				],
				[
					3.049665622186702,
					-0.39350693636744144
				],
				[
					3.1480404798984365,
					-0.3935069363674417
				],
				[
					3.246415337610153,
					-0.3935069363674417
				],
				[
					3.246415337610153,
					-0.2951320786557161
				],
				[
					3.3447901953218695,
					-0.19675722094399076
				],
				[
					3.3447901953218695,
					-0.09838236323226515
				],
				[
					3.443172558554134,
					0.19674971542345124
				],
				[
					3.541547416265869,
					0.2951245731351768
				],
				[
					3.73829713168932,
					0.4918817940791673
				],
				[
					3.8366719894010366,
					0.6886315095026185
				],
				[
					3.9350543526333013,
					0.7870063672143349
				],
				[
					4.033429210345036,
					0.9837635881583251
				],
				[
					4.131804068056753,
					1.082138445870051
				],
				[
					4.328553783480204,
					1.3772630190052277
				],
				[
					4.426936146712468,
					1.4756453822374926
				],
				[
					4.62368586213592,
					1.574020239949218
				],
				[
					4.722060719847655,
					1.5740202399492182
				],
				[
					4.918817940791636,
					1.6723950976609439
				],
				[
					5.115567656215087,
					1.6723950976609439
				],
				[
					5.312317371638539,
					1.5740202399492182
				],
				[
					5.50907459258252,
					1.5740202399492182
				],
				[
					5.804199165717706,
					1.3772630190052277
				],
				[
					6.197706102085139,
					1.1805133035817765
				],
				[
					6.492838180740854,
					0.8853812249260605
				],
				[
					6.787962753876022,
					0.6886315095026185
				],
				[
					7.083094832531738,
					0.3934994308469025
				],
				[
					7.378226911187454,
					0.09837485771172562
				],
				[
					7.673351484322621,
					-0.09838236323226486
				],
				[
					7.7717263420343565,
					-0.19675722094399048
				],
				[
					7.8701087052666026,
					-0.3935069363674417
				],
				[
					7.968483562978338,
					-0.49188179407915805
				],
				[
					8.066858420690073,
					-0.6886390150231485
				],
				[
					8.066858420690073,
					-0.6886390150231485
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.1865234375,
				0.2373046875,
				0.265625,
				0.294921875,
				0.326171875,
				0.3505859375,
				0.3662109375,
				0.373046875,
				0.3798828125,
				0.392578125,
				0.396484375,
				0.3984375,
				0.3984375,
				0.4013671875,
				0.408203125,
				0.41015625,
				0.41015625,
				0.41015625,
				0.41015625,
				0.412109375,
				0.4228515625,
				0.4140625,
				0.4072265625,
				0.4072265625,
				0.4111328125,
				0.4091796875,
				0.3955078125,
				0.3310546875,
				0.3837890625,
				0.384765625,
				0.3955078125,
				0.3974609375,
				0.3974609375,
				0.3974609375,
				0.3974609375,
				0.3974609375,
				0.3974609375,
				0.3974609375,
				0.3974609375,
				0.4013671875,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.40625,
				0.41015625,
				0.4150390625,
				0.423828125,
				0.427734375,
				0.427734375,
				0.4345703125,
				0.3779296875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 1082,
			"versionNonce": 842721410,
			"isDeleted": false,
			"id": "_zCrRh9zfx9fXrJSpZSWD",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -25.13376317917374,
			"y": 5807.030679779764,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 6.984727480340533,
			"height": 4.722060719847645,
			"seed": 612637748,
			"groupIds": [
				"rz9oQN36t0NUtb0jQqXzN"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577638,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.19675722094399978,
					0.19675722094399034
				],
				[
					-0.5902566517909023,
					0.3935069363674417
				],
				[
					-1.180520809102334,
					0.688639015023158
				],
				[
					-1.9675271763166504,
					1.5740202399492178
				],
				[
					-2.3610341126841017,
					2.2626592549723763
				],
				[
					-2.5577838281075342,
					2.85291590676326
				],
				[
					-2.6561661913397985,
					3.2464228431307016
				],
				[
					-2.656166191339799,
					3.5415474162658773
				],
				[
					-2.3610341126841012,
					3.8366794949215848
				],
				[
					-1.9675271763166515,
					4.0334292103450355
				],
				[
					-1.2788956668140505,
					4.033429210345036
				],
				[
					-0.29513207865571633,
					3.8366794949215866
				],
				[
					0.39350693636743306,
					3.639929779498134
				],
				[
					0.8853887304466004,
					3.3447977008424266
				],
				[
					1.475645382237483,
					3.049665622186711
				],
				[
					1.9675271763166513,
					2.6561661913398087
				],
				[
					2.7545335435309855,
					2.2626592549723767
				],
				[
					3.738297131689321,
					1.4756453822374929
				],
				[
					4.0334292103450355,
					0.9837635881583349
				],
				[
					4.230178925768469,
					0.688639015023158
				],
				[
					4.328561289000734,
					0.39350693636744216
				],
				[
					4.230178925768469,
					0.19675722094399029
				],
				[
					4.131804068056753,
					0
				],
				[
					3.6399222739775854,
					-0.1967497154234421
				],
				[
					3.148040479898418,
					-0.39350693636743284
				],
				[
					2.4594089703958186,
					-0.5902566517908838
				],
				[
					1.377270524525767,
					-0.6886315095026093
				],
				[
					1.180513303581786,
					-0.5902566517908836
				],
				[
					0.7870063672143349,
					-0.491881794079158
				],
				[
					0.6886315095026185,
					-0.4918817940791581
				],
				[
					0.39350693636743245,
					-0.39350693636743245
				],
				[
					0.3935069363674324,
					-0.2951245731351676
				],
				[
					0.4918817940791488,
					-0.29512457313516754
				],
				[
					0,
					0
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.171875,
				0.201171875,
				0.2529296875,
				0.3037109375,
				0.361328125,
				0.38671875,
				0.4130859375,
				0.423828125,
				0.42578125,
				0.42578125,
				0.419921875,
				0.4150390625,
				0.4033203125,
				0.400390625,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.408203125,
				0.4306640625,
				0.45703125,
				0.47265625,
				0.4775390625,
				0.482421875,
				0.4951171875,
				0.4970703125,
				0.4970703125,
				0.4970703125,
				0.466796875,
				0.4140625,
				0.0263671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 1081,
			"versionNonce": 1369921694,
			"isDeleted": false,
			"id": "e2Qu-qt_5B5zkqklfchjJ",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -10.67244143545446,
			"y": 5806.046916191606,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 5.902581528949971,
			"height": 4.426936146712469,
			"seed": 1839629836,
			"groupIds": [
				"rz9oQN36t0NUtb0jQqXzN"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577638,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.1967497154234327,
					-0.09837485771172569
				],
				[
					-0.7870063672143535,
					-0.09837485771172566
				],
				[
					-1.2788881612934837,
					-1.1102230246251565e-16
				],
				[
					-1.770769955372651,
					0.2951320786557159
				],
				[
					-2.262651749451819,
					0.6886390150231582
				],
				[
					-2.8529159067632506,
					1.377270524525767
				],
				[
					-3.0496656221867204,
					1.96752717631666
				],
				[
					-2.9512907644749666,
					2.5577838281075436
				],
				[
					-2.6561586858192694,
					3.049665622186711
				],
				[
					-2.2626517494518197,
					3.443172558554144
				],
				[
					-1.4756453822375022,
					3.73830463720986
				],
				[
					-0.9837635881583342,
					3.8366794949215857
				],
				[
					-0.3935069363674506,
					3.7383046372098594
				],
				[
					0.09837485771171606,
					3.541547416265869
				],
				[
					1.082138445870051,
					3.049665622186711
				],
				[
					1.8691523186049164,
					2.557783828107543
				],
				[
					2.361034112684083,
					2.1642843972606416
				],
				[
					2.6561661913398185,
					1.7707774608932088
				],
				[
					2.8529159067632506,
					1.377270524525768
				],
				[
					2.852915906763251,
					0.9837635881583262
				],
				[
					2.8529159067632506,
					0.6886390150231572
				],
				[
					2.754541049051534,
					0.3935069363674415
				],
				[
					2.557783828107553,
					0
				],
				[
					2.1642843972606505,
					-0.196749715423451
				],
				[
					1.1805208091023158,
					-0.4918817940791578
				],
				[
					0.39350693636745093,
					-0.5902566517908837
				],
				[
					-0.09837485771171625,
					-0.5902566517908837
				],
				[
					-0.5902566517908837,
					-0.3935069363674417
				],
				[
					-0.9837635881583346,
					-0.1967497154234511
				],
				[
					-1.2788881612934837,
					-1.1102230246251565e-16
				],
				[
					-1.278888161293484,
					0.19675722094399062
				],
				[
					-1.278888161293484,
					0.49188179407916777
				],
				[
					0,
					0
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.173828125,
				0.1923828125,
				0.294921875,
				0.3798828125,
				0.447265625,
				0.4873046875,
				0.4912109375,
				0.486328125,
				0.484375,
				0.482421875,
				0.48046875,
				0.4697265625,
				0.4658203125,
				0.470703125,
				0.4677734375,
				0.474609375,
				0.4765625,
				0.4765625,
				0.478515625,
				0.48046875,
				0.4921875,
				0.4951171875,
				0.5,
				0.5126953125,
				0.521484375,
				0.5234375,
				0.525390625,
				0.525390625,
				0.525390625,
				0.505859375,
				0.423828125,
				0.1904296875,
				0.01171875,
				0
			]
		},
		{
			"type": "rectangle",
			"version": 230,
			"versionNonce": 26118210,
			"isDeleted": false,
			"id": "7exzTn1ZVMkh-C_pRGh0f",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -24.467044835585,
			"y": 325.2239109915015,
			"strokeColor": "#2f9e44",
			"backgroundColor": "#b2f2bb",
			"width": 20.307711087740472,
			"height": 43.07687612680286,
			"seed": 974048436,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"id": "yYQDDnOFiaxCo_W096L8v",
					"type": "arrow"
				}
			],
			"updated": 1692815577638,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 217,
			"versionNonce": 179213534,
			"isDeleted": false,
			"id": "hGClCcpgUB2Wb5wpQViYv",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 6.99227868313028,
			"y": 293.0467701763057,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 105.84622896634608,
			"height": 26.46151029146631,
			"seed": 2136820364,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"id": "yYQDDnOFiaxCo_W096L8v",
					"type": "arrow"
				}
			],
			"updated": 1692815577638,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 253,
			"versionNonce": 752365570,
			"isDeleted": false,
			"id": "zr88awLpto0_9jF4Zc6kd",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 85.14619995716873,
			"y": 192.82239743789495,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 68.3076359675481,
			"height": 178.69208783835091,
			"seed": 1752203788,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"id": "t-rPGxHvHZymj7iVl-bA5",
					"type": "arrow"
				}
			],
			"updated": 1692815577638,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 343,
			"versionNonce": 1342458142,
			"isDeleted": false,
			"id": "kaS7G9xv2dkFm2aHO6myO",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -168.43075128982673,
			"y": 155.81609954078843,
			"strokeColor": "#e03131",
			"backgroundColor": "#ffc9c9",
			"width": 142,
			"height": 35,
			"seed": 861415476,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "DLyswqdy"
				},
				{
					"id": "yYQDDnOFiaxCo_W096L8v",
					"type": "arrow"
				}
			],
			"updated": 1692815577638,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 393,
			"versionNonce": 1477894082,
			"isDeleted": false,
			"id": "DLyswqdy",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -151.93075128982673,
			"y": 160.81609954078843,
			"strokeColor": "#e03131",
			"backgroundColor": "#ffffff",
			"width": 109,
			"height": 25,
			"seed": 1104051892,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577638,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Push / Pull",
			"rawText": "Push / Pull",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "kaS7G9xv2dkFm2aHO6myO",
			"originalText": "Push / Pull",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "arrow",
			"version": 750,
			"versionNonce": 18445662,
			"isDeleted": false,
			"id": "yYQDDnOFiaxCo_W096L8v",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -72.54014823091144,
			"y": 200.3205775389187,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#ffffff",
			"width": 44.29205193439428,
			"height": 140.95077756114785,
			"seed": 1285821452,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692815577638,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "kaS7G9xv2dkFm2aHO6myO",
				"gap": 9.504477998130284,
				"focus": -0.21444386555402759
			},
			"endBinding": {
				"elementId": "7exzTn1ZVMkh-C_pRGh0f",
				"gap": 3.7810514609321615,
				"focus": -0.7215102717536837
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
					44.29205193439428,
					140.95077756114785
				]
			]
		},
		{
			"type": "rectangle",
			"version": 381,
			"versionNonce": 1332320130,
			"isDeleted": false,
			"id": "1iDkDkBe9QkbdOosuf6Zz",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -28.315300944273417,
			"y": 72.16220643682189,
			"strokeColor": "#e03131",
			"backgroundColor": "#ffc9c9",
			"width": 142,
			"height": 35,
			"seed": 1298865676,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "1dPpCltE"
				},
				{
					"id": "t-rPGxHvHZymj7iVl-bA5",
					"type": "arrow"
				}
			],
			"updated": 1692815577638,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 437,
			"versionNonce": 1732188574,
			"isDeleted": false,
			"id": "1dPpCltE",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -6.815300944273417,
			"y": 77.16220643682189,
			"strokeColor": "#e03131",
			"backgroundColor": "#ffffff",
			"width": 99,
			"height": 25,
			"seed": 1895005324,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577638,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Long Jump",
			"rawText": "Long Jump",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "1iDkDkBe9QkbdOosuf6Zz",
			"originalText": "Long Jump",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "arrow",
			"version": 790,
			"versionNonce": 51337026,
			"isDeleted": false,
			"id": "t-rPGxHvHZymj7iVl-bA5",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 22.742856216464823,
			"y": 116.51929726791485,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 53.10609704155393,
			"height": 85.71313983434982,
			"seed": 319663156,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692815577639,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "1iDkDkBe9QkbdOosuf6Zz",
				"gap": 9.357090831092961,
				"focus": 0.4469788149535266
			},
			"endBinding": {
				"elementId": "zr88awLpto0_9jF4Zc6kd",
				"gap": 9.29724669914998,
				"focus": 0.06787604307301731
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
					53.10609704155393,
					85.71313983434982
				]
			]
		},
		{
			"type": "rectangle",
			"version": 322,
			"versionNonce": 2040935902,
			"isDeleted": false,
			"id": "aSbpxGZVi2ZGTW9k2OEjP",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 369.56574281665354,
			"y": 199.28478295698108,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 278.76924954927875,
			"height": 118.15382737379804,
			"seed": 1601324172,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"id": "vnHhPxWImF4qbsKUzUAst",
					"type": "arrow"
				}
			],
			"updated": 1692815577639,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 265,
			"versionNonce": 57089794,
			"isDeleted": false,
			"id": "6ALrck5u2eokCbpKgncUm",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 400.0540458370832,
			"y": 241.53533152255025,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 48.61534705528857,
			"height": 38.15387432391833,
			"seed": 1073558580,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577639,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 234,
			"versionNonce": 559925790,
			"isDeleted": false,
			"id": "xMnGiAJGVLHDDmPLQxr02",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 560.334879685644,
			"y": 239.90015818234156,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 47.38469050480762,
			"height": 38.76920259915869,
			"seed": 1372442420,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577639,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 259,
			"versionNonce": 2096099010,
			"isDeleted": false,
			"id": "LHI9AV0PAqDXGdJmcrf-z",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 458.7964181471823,
			"y": 254.0539761661156,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 98.46153846153857,
			"height": 14.769240159254764,
			"seed": 332415756,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577639,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 297,
			"versionNonce": 2103236190,
			"isDeleted": false,
			"id": "d_YkcfQbrC8G-VtXl-7vd",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 396.0272061579997,
			"y": 146.97709064928864,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 212.30769230769238,
			"height": 53.53844275841351,
			"seed": 1477017012,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577639,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 246,
			"versionNonce": 877184642,
			"isDeleted": false,
			"id": "cDsaYqjgHhZI3YUNls5NW",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 402.18105231184586,
			"y": 321.7462838584232,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 48.000018780048094,
			"height": 48.61539400540869,
			"seed": 1039855412,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577639,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 232,
			"versionNonce": 644766366,
			"isDeleted": false,
			"id": "F-_DSpM15M9PVpz_zijUJ",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 564.0272249380478,
			"y": 323.59245648462525,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 51.69227013221166,
			"height": 44.307720477764406,
			"seed": 1252658356,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577639,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 591,
			"versionNonce": 36742722,
			"isDeleted": false,
			"id": "VyOs6RK2NWtgwG1fcRnCB",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 214.2964451435015,
			"y": 143.66938132217774,
			"strokeColor": "#e03131",
			"backgroundColor": "#ffc9c9",
			"width": 142,
			"height": 35,
			"seed": 1801862324,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "2NrlQHM3"
				},
				{
					"id": "vnHhPxWImF4qbsKUzUAst",
					"type": "arrow"
				}
			],
			"updated": 1692815577639,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 628,
			"versionNonce": 1933924062,
			"isDeleted": false,
			"id": "2NrlQHM3",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 253.2964451435015,
			"y": 148.66938132217774,
			"strokeColor": "#e03131",
			"backgroundColor": "#ffffff",
			"width": 64,
			"height": 25,
			"seed": 1113884212,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577639,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Crouch",
			"rawText": "Crouch",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "VyOs6RK2NWtgwG1fcRnCB",
			"originalText": "Crouch",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "arrow",
			"version": 514,
			"versionNonce": 1334218242,
			"isDeleted": false,
			"id": "vnHhPxWImF4qbsKUzUAst",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 280.64112420637014,
			"y": 184.5540154868413,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 65.1830035040029,
			"height": 142.94726386994438,
			"seed": 1103978804,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692815577639,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "VyOs6RK2NWtgwG1fcRnCB",
				"gap": 5.8846341646635665,
				"focus": 0.19395519661517316
			},
			"endBinding": {
				"elementId": "aSbpxGZVi2ZGTW9k2OEjP",
				"gap": 16,
				"focus": -1.1703316642324542
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
					65.1830035040029,
					142.94726386994438
				]
			]
		},
		{
			"type": "rectangle",
			"version": 408,
			"versionNonce": 1014156062,
			"isDeleted": false,
			"id": "6NbYIzqbSD_0WfVgxgWYK",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1544.2986118569181,
			"y": 302.743931094599,
			"strokeColor": "#1971c2",
			"backgroundColor": "#a5d8ff",
			"width": 30.222167968750455,
			"height": 29.333428276909782,
			"seed": 1890051124,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"id": "G43xsgHquC9Mv6R4y8A-B",
					"type": "arrow"
				}
			],
			"updated": 1692815577639,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 531,
			"versionNonce": 290028994,
			"isDeleted": false,
			"id": "foVZEP6Mstv_g8_m9GCz5",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1106.0299785863076,
			"y": 225.45663051013167,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 278.76924954927875,
			"height": 118.15382737379804,
			"seed": 37377292,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577639,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 442,
			"versionNonce": 543668062,
			"isDeleted": false,
			"id": "BzuVugCYztSzXqA2WwoHa",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1139.2607102569805,
			"y": 267.9181314115738,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 48.61534705528857,
			"height": 38.15387432391833,
			"seed": 1422119820,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577639,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 443,
			"versionNonce": 1150842242,
			"isDeleted": false,
			"id": "Jz7LHgDAuWbNNXh7IEWvA",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1296.7991154552976,
			"y": 266.07200573549204,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 47.38469050480762,
			"height": 38.76920259915869,
			"seed": 1184465420,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577639,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 468,
			"versionNonce": 1198857118,
			"isDeleted": false,
			"id": "7ZoY9aU3D7aUl9PspqpOL",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1195.2606539168362,
			"y": 280.2258237192662,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 98.46153846153857,
			"height": 14.769240159254764,
			"seed": 2125815948,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577639,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 506,
			"versionNonce": 1790080322,
			"isDeleted": false,
			"id": "qvGnJkVOLT0qrovOEkMjU",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1132.4914419276536,
			"y": 173.14893820243918,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 212.30769230769238,
			"height": 53.53844275841351,
			"seed": 886140684,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577639,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 481,
			"versionNonce": 667678686,
			"isDeleted": false,
			"id": "sxSfeNa4smOb_yGW-EbOt",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1133.311900494694,
			"y": 347.91813141157365,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 53.33340636685369,
			"height": 19.282033545339118,
			"seed": 426225036,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577639,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 467,
			"versionNonce": 83262722,
			"isDeleted": false,
			"id": "904GTZpteqOihyU2SRUSS",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1288.047070516729,
			"y": 349.7643040377758,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 64.13666032318405,
			"height": 13.19660936665332,
			"seed": 1035082764,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577639,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 314,
			"versionNonce": 1232948254,
			"isDeleted": false,
			"id": "JNz40Je2_J0pRzEQ08kLo",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 829.4148475015719,
			"y": 87.50792560311322,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 279.11112467447913,
			"height": 178.66665310329878,
			"seed": 1919132556,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577639,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 199,
			"versionNonce": 283348162,
			"isDeleted": false,
			"id": "DNwjvfdPNKz-uPuXDYfzy",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 850.7480587645925,
			"y": 272.3969094355783,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 68.44455295138891,
			"height": 84.44444444444446,
			"seed": 740051892,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577639,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 190,
			"versionNonce": 175773790,
			"isDeleted": false,
			"id": "Ege9gy9WThtrh8svTOUak",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1029.4147796847315,
			"y": 268.84134031665474,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 64.888916015625,
			"height": 92.4444580078125,
			"seed": 897599628,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577639,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 110,
			"versionNonce": 68723842,
			"isDeleted": false,
			"id": "J1VUD524ySrKMh7NfG4C9",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 854.3036957003562,
			"y": 182.61921303800898,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 63.11102973090283,
			"height": 66.66666666666663,
			"seed": 1602299828,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577639,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 117,
			"versionNonce": 1653824670,
			"isDeleted": false,
			"id": "IzVIG9znHdCSbVvpQeZ3l",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1023.1925845892451,
			"y": 187.9525328079742,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 63.999972873263914,
			"height": 56.88890245225696,
			"seed": 1238268044,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577639,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 123,
			"versionNonce": 1213514818,
			"isDeleted": false,
			"id": "NLhD3ojWTE1bQuC2-zr1p",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 926.303614320148,
			"y": 227.9525328079742,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 88.00008138020826,
			"height": 10.666639539930657,
			"seed": 2014850444,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577639,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 133,
			"versionNonce": 662313182,
			"isDeleted": false,
			"id": "6fjTZ-r1kkZQNcfdMcPqX",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 934.3036957003562,
			"y": 195.06360322898115,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 73.77780490451391,
			"height": 10.666707356770871,
			"seed": 1457167884,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577639,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 163,
			"versionNonce": 930540546,
			"isDeleted": false,
			"id": "2cRB3zV7vrP4rCCEk0KkR",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 858.7481401448011,
			"y": -25.38086834219962,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 213.33333333333337,
			"height": 111.99998643663184,
			"seed": 1927374988,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577639,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 88,
			"versionNonce": 1354714398,
			"isDeleted": false,
			"id": "sdhSsyBxr42GfAD0_w65b",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 853.4147525579957,
			"y": -89.38090903230477,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 24.888916015625,
			"height": 63.11109754774304,
			"seed": 1311981748,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577639,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 78,
			"versionNonce": 394140610,
			"isDeleted": false,
			"id": "wByu0mF9XlI46eMgNwchw",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1052.5258772324748,
			"y": -86.71421523890206,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 26.666666666666742,
			"height": 60.44440375434033,
			"seed": 145013900,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577639,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 642,
			"versionNonce": 1003747678,
			"isDeleted": false,
			"id": "T7xX1vRVs2kmq1f6MDKRD",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 624.3541292349211,
			"y": 16.795904266701143,
			"strokeColor": "#e03131",
			"backgroundColor": "#ffc9c9",
			"width": 142,
			"height": 35,
			"seed": 1923258636,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "GJioXrEd"
				},
				{
					"id": "xes7YulzvHsRvyWjRbd8E",
					"type": "arrow"
				}
			],
			"updated": 1692815577639,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 683,
			"versionNonce": 378098562,
			"isDeleted": false,
			"id": "GJioXrEd",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 672.8541292349211,
			"y": 21.795904266701143,
			"strokeColor": "#e03131",
			"backgroundColor": "#ffffff",
			"width": 45,
			"height": 25,
			"seed": 394499980,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577639,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Climb",
			"rawText": "Climb",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "T7xX1vRVs2kmq1f6MDKRD",
			"originalText": "Climb",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 759,
			"versionNonce": 1879645598,
			"isDeleted": false,
			"id": "v8nASpz1U_pt9LmVbFx-t",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1449.5001647789404,
			"y": 127.91046767623448,
			"strokeColor": "#e03131",
			"backgroundColor": "#ffc9c9",
			"width": 142,
			"height": 60,
			"seed": 1761238412,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "wRrxYeIM"
				},
				{
					"id": "G43xsgHquC9Mv6R4y8A-B",
					"type": "arrow"
				}
			],
			"updated": 1692815577639,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 814,
			"versionNonce": 1188533058,
			"isDeleted": false,
			"id": "wRrxYeIM",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1474.0001647789404,
			"y": 132.91046767623448,
			"strokeColor": "#e03131",
			"backgroundColor": "#ffffff",
			"width": 93,
			"height": 50,
			"seed": 1735314444,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577639,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Elevator \nswitch",
			"rawText": "Elevator switch",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "v8nASpz1U_pt9LmVbFx-t",
			"originalText": "Elevator switch",
			"lineHeight": 1.25,
			"baseline": 42
		},
		{
			"type": "arrow",
			"version": 292,
			"versionNonce": 1653586398,
			"isDeleted": false,
			"id": "G43xsgHquC9Mv6R4y8A-B",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1520.8188765837028,
			"y": 193.4104812396024,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#ffffff",
			"width": 32.16427262700313,
			"height": 104.00002835976966,
			"seed": 562117644,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692815577639,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "v8nASpz1U_pt9LmVbFx-t",
				"gap": 5.500013563367929,
				"focus": 0.13278667236257244
			},
			"endBinding": {
				"elementId": "6NbYIzqbSD_0WfVgxgWYK",
				"gap": 5.333421495226958,
				"focus": -0.012269979538803941
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
					32.16427262700313,
					104.00002835976966
				]
			]
		},
		{
			"type": "arrow",
			"version": 260,
			"versionNonce": 449305346,
			"isDeleted": false,
			"id": "xes7YulzvHsRvyWjRbd8E",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 699.5182137536979,
			"y": 62.13423631767961,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#ffffff",
			"width": 86.17006446619007,
			"height": 175.19148495026326,
			"seed": 1024286476,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692815577639,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "T7xX1vRVs2kmq1f6MDKRD",
				"gap": 10.338332050978465,
				"focus": 0.11969384088584989
			},
			"endBinding": {
				"elementId": "5klc1K9ePNcSVni53X3Nn",
				"gap": 8.077835758805008,
				"focus": -1.073391073168541
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
					86.17006446619007,
					175.19148495026326
				]
			]
		},
		{
			"type": "rectangle",
			"version": 374,
			"versionNonce": 980995614,
			"isDeleted": false,
			"id": "5klc1K9ePNcSVni53X3Nn",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 793.7661139786929,
			"y": 31.30290903493608,
			"strokeColor": "#2f9e44",
			"backgroundColor": "#b2f2bb",
			"width": 23.863212389823733,
			"height": 212.85464034121264,
			"seed": 632136244,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"id": "xes7YulzvHsRvyWjRbd8E",
					"type": "arrow"
				}
			],
			"updated": 1692815577639,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 106,
			"versionNonce": 1624844994,
			"isDeleted": false,
			"id": "Y7fJsHIE",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 759.6368798366417,
			"y": -167.6028192970614,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#ffffff",
			"width": 111,
			"height": 25,
			"seed": 932992052,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577639,
			"link": null,
			"locked": true,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "TUTORIAL",
			"rawText": "TUTORIAL",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "TUTORIAL",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 267,
			"versionNonce": 347429470,
			"isDeleted": false,
			"id": "XnebrG71",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -5.886840556461948,
			"y": 777.8257032065044,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#ffffff",
			"width": 183,
			"height": 25,
			"seed": 211356300,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577639,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "INTO CINEMATIC",
			"rawText": "INTO CINEMATIC",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "INTO CINEMATIC",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 1025,
			"versionNonce": 1068139138,
			"isDeleted": false,
			"id": "ZBcE1Rliu50_x7Nx22vqp",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -32.2650513483602,
			"y": 1386.5120849243992,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 262.32521637929153,
			"height": 28.19622309967368,
			"seed": 2143940788,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"id": "_mietLvlAYAj5-ftXET9w",
					"type": "arrow"
				}
			],
			"updated": 1692815577639,
			"link": null,
			"locked": false
		},
		{
			"type": "ellipse",
			"version": 259,
			"versionNonce": 1209425566,
			"isDeleted": false,
			"id": "8UvF3xTzgd-e3PWziWyGl",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 5.541774468647645,
			"y": 850.3968527600753,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 165.71428571428578,
			"height": 149.71426827566972,
			"seed": 1059258932,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692815577639,
			"link": null,
			"locked": false
		},
		{
			"type": "arrow",
			"version": 1284,
			"versionNonce": 838525506,
			"isDeleted": false,
			"id": "_mietLvlAYAj5-ftXET9w",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 100.29443772626041,
			"y": 1384.1505860868926,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#ffffff",
			"width": 1.474547716111374,
			"height": 187.09821216886354,
			"seed": 585920268,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692815577639,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "ZBcE1Rliu50_x7Nx22vqp",
				"focus": 0.011629147508439358,
				"gap": 2.3614988375065877
			},
			"endBinding": {
				"elementId": "PGJcDCtJG7v5h0AEWRoXX",
				"focus": 0.009267201674963282,
				"gap": 2.932997188209356
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
					-1.474547716111374,
					-187.09821216886354
				]
			]
		},
		{
			"type": "rectangle",
			"version": 973,
			"versionNonce": 692902622,
			"isDeleted": false,
			"id": "PGJcDCtJG7v5h0AEWRoXX",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -35.547267477322066,
			"y": 1167.923823047143,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 270.99491105402103,
			"height": 26.195553682676746,
			"seed": 1592823052,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"id": "_mietLvlAYAj5-ftXET9w",
					"type": "arrow"
				}
			],
			"updated": 1692815577639,
			"link": null,
			"locked": false
		},
		{
			"type": "arrow",
			"version": 1176,
			"versionNonce": 44648962,
			"isDeleted": false,
			"id": "OEo2gw4tZjpm-QB0U9npo",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 408.9787594310835,
			"y": 886.2840999214857,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#ffffff",
			"width": 654.3551768025136,
			"height": 8.411144119942264,
			"seed": 359118004,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "58qwBuPV"
				}
			],
			"updated": 1692815577639,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "YBIqjy2htsa4DLTsGFkuO",
				"focus": -0.651665339485639,
				"gap": 12.375425999351023
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
					654.3551768025136,
					8.411144119942264
				]
			]
		},
		{
			"type": "text",
			"version": 206,
			"versionNonce": 1323945758,
			"isDeleted": false,
			"id": "58qwBuPV",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1498.1092590240587,
			"y": 779.1183704974148,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#ffffff",
			"width": 477,
			"height": 75,
			"seed": 1902859276,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577639,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "1. While waiting for the elevator to reach floor, \nmove the camera to the other side of the \nbuilding and focus on the gray cat",
			"rawText": "1. While waiting for the elevator to reach floor, \nmove the camera to the other side of the \nbuilding and focus on the gray cat",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "OEo2gw4tZjpm-QB0U9npo",
			"originalText": "1. While waiting for the elevator to reach floor, \nmove the camera to the other side of the \nbuilding and focus on the gray cat",
			"lineHeight": 1.25,
			"baseline": 67
		},
		{
			"type": "rectangle",
			"version": 1290,
			"versionNonce": 1219803586,
			"isDeleted": false,
			"id": "HXcVYA1K7l01JNCC2QpCC",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1096.9337897492226,
			"y": 798.0328468985338,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 476.1496364030638,
			"height": 836.5155826729024,
			"seed": 485214388,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"id": "W9jot7yLA_jUoBJDG53sh",
					"type": "arrow"
				}
			],
			"updated": 1692815577639,
			"link": null,
			"locked": false
		},
		{
			"type": "line",
			"version": 431,
			"versionNonce": 1432238942,
			"isDeleted": false,
			"id": "t4WlaNxnb6ossFkkluBWl",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 31.84459268895057,
			"y": 983.0159154001383,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 0,
			"height": 561.3094887108336,
			"seed": 373035404,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692815577639,
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
					561.3094887108336
				]
			]
		},
		{
			"type": "line",
			"version": 512,
			"versionNonce": 1664889218,
			"isDeleted": false,
			"id": "pQh9BthTMC4fnElaHJhDQ",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 152.40036343705037,
			"y": 977.6583202548038,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 2.909062373174038,
			"height": 576.6649439427764,
			"seed": 820614068,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692815577639,
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
					2.909062373174038,
					576.6649439427764
				]
			]
		},
		{
			"type": "text",
			"version": 319,
			"versionNonce": 586882974,
			"isDeleted": false,
			"id": "pJILEGOk",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 430.4159855904843,
			"y": 1283.8281061289251,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 263,
			"height": 50,
			"seed": 1313737524,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577639,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "3. Cat get on elevator \nand clicks the inside switch",
			"rawText": "3. Cat get on elevator \nand clicks the inside switch",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "3. Cat get on elevator \nand clicks the inside switch",
			"lineHeight": 1.25,
			"baseline": 42
		},
		{
			"type": "arrow",
			"version": 1157,
			"versionNonce": 1971237186,
			"isDeleted": false,
			"id": "W9jot7yLA_jUoBJDG53sh",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1071.4626673096639,
			"y": 1022.8754086100341,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#ffffff",
			"width": 642.4922400664336,
			"height": 12.811413961797264,
			"seed": 2019456308,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "QZ8r8jyF"
				}
			],
			"updated": 1692815577639,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "HXcVYA1K7l01JNCC2QpCC",
				"focus": 0.4448175645398406,
				"gap": 25.471122439558826
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
					-642.4922400664336,
					-12.811413961797264
				]
			]
		},
		{
			"type": "text",
			"version": 261,
			"versionNonce": 737246174,
			"isDeleted": false,
			"id": "QZ8r8jyF",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1492.9685788604977,
			"y": 977.746483834019,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#ffffff",
			"width": 486,
			"height": 75,
			"seed": 1690414772,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577639,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "2. While waiting for the elevator to reach floor, \nmove the camera to the other side of the \nbuilding and focus on the gray cat",
			"rawText": "2. While waiting for the elevator to reach floor, \nmove the camera to the other side of the \nbuilding and focus on the gray cat",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "W9jot7yLA_jUoBJDG53sh",
			"originalText": "2. While waiting for the elevator to reach floor, \nmove the camera to the other side of the \nbuilding and focus on the gray cat",
			"lineHeight": 1.25,
			"baseline": 67
		},
		{
			"type": "text",
			"version": 402,
			"versionNonce": 1658534146,
			"isDeleted": false,
			"id": "d882DXuB",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 432.6737830959171,
			"y": 1380.4947924004853,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 289,
			"height": 75,
			"seed": 873213068,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577639,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "4. title of the game and\nroll the intro credits as the \nelevator goes down",
			"rawText": "4. title of the game and\nroll the intro credits as the \nelevator goes down",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "4. title of the game and\nroll the intro credits as the \nelevator goes down",
			"lineHeight": 1.25,
			"baseline": 67
		},
		{
			"type": "text",
			"version": 491,
			"versionNonce": 911364126,
			"isDeleted": false,
			"id": "3Zjzee5i",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 978.7309512390502,
			"y": 1894.618111489639,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 84,
			"height": 25,
			"seed": 408174092,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577639,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "PUZZLE",
			"rawText": "PUZZLE",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "PUZZLE",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 736,
			"versionNonce": 1255196866,
			"isDeleted": false,
			"id": "7W-qMHqpCE7Pcvs15-oY_",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2011.8913228084932,
			"y": 2485.2524533896108,
			"strokeColor": "#1971c2",
			"backgroundColor": "#a5d8ff",
			"width": 30.222167968750455,
			"height": 29.333428276909782,
			"seed": 172018683,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"id": "AiEYb1ApHqwEtu3TojmH-",
					"type": "arrow"
				}
			],
			"updated": 1692815577639,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 1089,
			"versionNonce": 504274014,
			"isDeleted": false,
			"id": "7Xr79sz6BovKJxRp-yF_u",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1918.6689649525888,
			"y": 2310.4190454577515,
			"strokeColor": "#e03131",
			"backgroundColor": "#ffc9c9",
			"width": 142,
			"height": 60,
			"seed": 1775998107,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "jsWk1e1G"
				},
				{
					"id": "AiEYb1ApHqwEtu3TojmH-",
					"type": "arrow"
				}
			],
			"updated": 1692815577639,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 1144,
			"versionNonce": 83779714,
			"isDeleted": false,
			"id": "jsWk1e1G",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1943.1689649525888,
			"y": 2315.4190454577515,
			"strokeColor": "#e03131",
			"backgroundColor": "#ffffff",
			"width": 93,
			"height": 50,
			"seed": 1750354235,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577639,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Elevator \nswitch",
			"rawText": "Elevator switch",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "7Xr79sz6BovKJxRp-yF_u",
			"originalText": "Elevator switch",
			"lineHeight": 1.25,
			"baseline": 42
		},
		{
			"type": "arrow",
			"version": 1289,
			"versionNonce": 418865310,
			"isDeleted": false,
			"id": "AiEYb1ApHqwEtu3TojmH-",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1989.6691005862695,
			"y": 2375.9190590211197,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#ffffff",
			"width": 31.111111111111768,
			"height": 103.99997287326369,
			"seed": 1259170267,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692815577640,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "7Xr79sz6BovKJxRp-yF_u",
				"gap": 5.500013563368157,
				"focus": 0.13278667236257705
			},
			"endBinding": {
				"elementId": "7W-qMHqpCE7Pcvs15-oY_",
				"gap": 5.333421495227185,
				"focus": -0.012269979538832555
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
					31.111111111111768,
					103.99997287326369
				]
			]
		},
		{
			"type": "rectangle",
			"version": 1560,
			"versionNonce": 488833090,
			"isDeleted": false,
			"id": "Fn4UgTzg1od6t6K2npH-R",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 300.3054515528081,
			"y": 2319.6229261927497,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 6.944606225318786,
			"height": 244.87244722049914,
			"seed": 1895341205,
			"groupIds": [
				"YK_dD1KkxpBH9Dj53H8lT"
			],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577640,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 1862,
			"versionNonce": 2059246814,
			"isDeleted": false,
			"id": "zhXGkC4YbqiCLV-T2-coI",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 251.7110979813508,
			"y": 2283.8145149265397,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 31.22364688381393,
			"height": 97.1896141027234,
			"seed": 1060604731,
			"groupIds": [
				"YK_dD1KkxpBH9Dj53H8lT"
			],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577640,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 1779,
			"versionNonce": 1327343618,
			"isDeleted": false,
			"id": "ARJcuWE2HgDkHPIvuTbK9",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 258.60104694132883,
			"y": 2294.299078763413,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 16.844730284522374,
			"height": 20.202732403515,
			"seed": 2134439675,
			"groupIds": [
				"YK_dD1KkxpBH9Dj53H8lT"
			],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577640,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 1880,
			"versionNonce": 2029146398,
			"isDeleted": false,
			"id": "aZ_CriysNbR77PP9Hhp6s",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 258.60095552298776,
			"y": 2320.3608251041055,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 16.844730284522374,
			"height": 20.202732403515,
			"seed": 98821563,
			"groupIds": [
				"YK_dD1KkxpBH9Dj53H8lT"
			],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577640,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 1917,
			"versionNonce": 49108930,
			"isDeleted": false,
			"id": "lSmneoBqG0x_gPLaUxpI8",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 258.90051057182677,
			"y": 2345.5237920253544,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 16.844730284522374,
			"height": 20.202732403515,
			"seed": 277821883,
			"groupIds": [
				"YK_dD1KkxpBH9Dj53H8lT"
			],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577640,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 1732,
			"versionNonce": 1862696286,
			"isDeleted": false,
			"id": "WParWrYmFprVT0wSILdRe",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 284.09569732582963,
			"y": 2321.856355341622,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 21.572114467904527,
			"height": 13.986315955714222,
			"seed": 1944771451,
			"groupIds": [
				"YK_dD1KkxpBH9Dj53H8lT"
			],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577640,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 1483,
			"versionNonce": 1219563394,
			"isDeleted": false,
			"id": "eV4QznhSUshhoqk6jRuQs",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -141.16308431548873,
			"y": 2313.7628434497406,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 7.060475045087857,
			"height": 248.95807576916474,
			"seed": 1009046139,
			"groupIds": [
				"2o_Z7V_cW37eVlljNkuq6"
			],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577640,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 1785,
			"versionNonce": 575349150,
			"isDeleted": false,
			"id": "JCVrLmsJNBSrM7c-xIREh",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -116.44207718198572,
			"y": 2277.356978819495,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 31.744604731664786,
			"height": 98.81119573233943,
			"seed": 2121976603,
			"groupIds": [
				"2o_Z7V_cW37eVlljNkuq6"
			],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577640,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 1702,
			"versionNonce": 1420283714,
			"isDeleted": false,
			"id": "1ZXIn_gWoebGxHc5WFqaH",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -108.82815820439623,
			"y": 2288.0164746824835,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 17.125779915569865,
			"height": 20.539809364217433,
			"seed": 1086894011,
			"groupIds": [
				"2o_Z7V_cW37eVlljNkuq6"
			],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577640,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 1803,
			"versionNonce": 99696094,
			"isDeleted": false,
			"id": "8x13e8-0wO4-xTMA7YYv3",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -108.82806526076615,
			"y": 2314.513053998818,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 17.125779915569865,
			"height": 20.539809364217433,
			"seed": 355532891,
			"groupIds": [
				"2o_Z7V_cW37eVlljNkuq6"
			],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577640,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 1840,
			"versionNonce": 2066781954,
			"isDeleted": false,
			"id": "wGV1-VW1k6BL07_SRF9j8",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -109.132618302124,
			"y": 2340.095858011539,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 17.125779915569865,
			"height": 20.539809364217433,
			"seed": 629554427,
			"groupIds": [
				"2o_Z7V_cW37eVlljNkuq6"
			],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577640,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 1655,
			"versionNonce": 2131350046,
			"isDeleted": false,
			"id": "8gDYhZsCV6W0XuUOp7zf2",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -139.55443899773604,
			"y": 2316.0335367416214,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 21.932039186775775,
			"height": 14.219673740176873,
			"seed": 1028318619,
			"groupIds": [
				"2o_Z7V_cW37eVlljNkuq6"
			],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577640,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 692,
			"versionNonce": 751462082,
			"isDeleted": false,
			"id": "wBp8WhoR",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1716.4480812612067,
			"y": 2058.1313617436335,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 420,
			"height": 150,
			"seed": 1555044187,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577640,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "5. Get to the end of the level\nand click the elevator button to \nstart the level ending animation, which\ncat jump on platform and clicks to go up\nas level ends with more credits and screen\ndarkens",
			"rawText": "5. Get to the end of the level\nand click the elevator button to \nstart the level ending animation, which\ncat jump on platform and clicks to go up\nas level ends with more credits and screen\ndarkens",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "5. Get to the end of the level\nand click the elevator button to \nstart the level ending animation, which\ncat jump on platform and clicks to go up\nas level ends with more credits and screen\ndarkens",
			"lineHeight": 1.25,
			"baseline": 142
		},
		{
			"type": "rectangle",
			"version": 741,
			"versionNonce": 679861854,
			"isDeleted": false,
			"id": "xDNRLtWfY4sO9VGfGUG1I",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 814.1913526799306,
			"y": 2379.223916376561,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 216.97789849175354,
			"height": 199.11107042100673,
			"seed": 637809668,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577640,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 734,
			"versionNonce": 1913929346,
			"isDeleted": false,
			"id": "pSEp5XrLIROjgQlD-Z5_1",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 592.646076983611,
			"y": 2500.1946809279684,
			"strokeColor": "#2f9e44",
			"backgroundColor": "#b2f2bb",
			"width": 128.2442093361281,
			"height": 76.34670383327615,
			"seed": 1659968772,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577640,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 492,
			"versionNonce": 389440158,
			"isDeleted": false,
			"id": "EA7L_mB_KuNW4GI96Jqsk",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 482.78723535992435,
			"y": 2198.7849814135484,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 19.555538116939715,
			"height": 202.92061941964312,
			"seed": 607118980,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577640,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 594,
			"versionNonce": 1741495874,
			"isDeleted": false,
			"id": "Xp9ZEtK6JetMYfV0mR0mx",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 482.69488159417074,
			"y": 2521.8585459512246,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 18.66666279141872,
			"height": 62.47621566530279,
			"seed": 192374788,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577640,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 1165,
			"versionNonce": 499932894,
			"isDeleted": false,
			"id": "cS1GuGRrnvCSnVCvrpwVw",
			"fillStyle": "cross-hatch",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1004.4084734307362,
			"y": 2539.7672659442037,
			"strokeColor": "#ff0000",
			"backgroundColor": "#ff0000",
			"width": 110.89528111049094,
			"height": 52.95248849051312,
			"seed": 108442116,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577640,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 1092,
			"versionNonce": 986973698,
			"isDeleted": false,
			"id": "-INHi7JX6coT6FLq2lbXJ",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 928.4831687278431,
			"y": 2143.967703713763,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 101.28558766943767,
			"height": 165.81878714276144,
			"seed": 449495868,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577640,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 1140,
			"versionNonce": 282645278,
			"isDeleted": false,
			"id": "uU0SgVi6V-JkiWOuWo_Vs",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1095.053980724954,
			"y": 2119.8139694577026,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 252.08894856770857,
			"height": 469.7777777777779,
			"seed": 1806109060,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577640,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 1363,
			"versionNonce": 606598594,
			"isDeleted": false,
			"id": "PCKHg0UHCTLOLr-cBVPPO",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1412.1873900131498,
			"y": 2230.513847726474,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 127.11121961805631,
			"height": 32.8444688585069,
			"seed": 1593236540,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"id": "Zz73Z1DvFjH1SafkNSBJh",
					"type": "arrow"
				},
				{
					"id": "qcdYMsY4RErCX9fJOMFHY",
					"type": "arrow"
				}
			],
			"updated": 1692815577640,
			"link": null,
			"locked": false
		},
		{
			"type": "arrow",
			"version": 894,
			"versionNonce": 181190494,
			"isDeleted": false,
			"id": "qcdYMsY4RErCX9fJOMFHY",
			"fillStyle": "cross-hatch",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1479.3932666538715,
			"y": 2276.369452110154,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#ff0000",
			"width": 1.1829647763779576,
			"height": 257.0667046440974,
			"seed": 168037636,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692815577640,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "PCKHg0UHCTLOLr-cBVPPO",
				"focus": -0.0552373981371625,
				"gap": 13.011135525172904
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
					1.1829647763779576,
					257.0667046440974
				]
			]
		},
		{
			"type": "arrow",
			"version": 877,
			"versionNonce": 1692921218,
			"isDeleted": false,
			"id": "Zz73Z1DvFjH1SafkNSBJh",
			"fillStyle": "cross-hatch",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1474.769509343086,
			"y": 2223.569403282029,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#ff0000",
			"width": 6.7624179474660195,
			"height": 275.73323567708337,
			"seed": 760696196,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692815577640,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "PCKHg0UHCTLOLr-cBVPPO",
				"focus": -0.006260596919338932,
				"gap": 6.944444444445253
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
					-6.7624179474660195,
					-275.73323567708337
				]
			]
		},
		{
			"type": "rectangle",
			"version": 1213,
			"versionNonce": 804856734,
			"isDeleted": false,
			"id": "46m4UKCzfzkKVjeRumRyh",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1129.238882106937,
			"y": 1924.1917448618901,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 252.08894856770857,
			"height": 48.44443088107633,
			"seed": 110967100,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577640,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 341,
			"versionNonce": 1112730946,
			"isDeleted": false,
			"id": "bYLndyoR",
			"fillStyle": "cross-hatch",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 606.7835581458914,
			"y": 2382.469500599195,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#ff0000",
			"width": 116,
			"height": 50,
			"seed": 1905489212,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577640,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "push trash\ncan to climb",
			"rawText": "push trash\ncan to climb",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "push trash\ncan to climb",
			"lineHeight": 1.25,
			"baseline": 42
		},
		{
			"type": "text",
			"version": 428,
			"versionNonce": 1921974238,
			"isDeleted": false,
			"id": "TH8nHuZN",
			"fillStyle": "cross-hatch",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 985.8336153562725,
			"y": 2063.3203027562254,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#ff0000",
			"width": 96,
			"height": 50,
			"seed": 1251638460,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577640,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "wall jump \nto get up",
			"rawText": "wall jump \nto get up",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "wall jump \nto get up",
			"lineHeight": 1.25,
			"baseline": 42
		},
		{
			"type": "text",
			"version": 385,
			"versionNonce": 29881602,
			"isDeleted": false,
			"id": "znUFCY96",
			"fillStyle": "cross-hatch",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1194.2593655670291,
			"y": 2011.5666116942753,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#ff0000",
			"width": 206,
			"height": 50,
			"seed": 1390596028,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577640,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "can go down or wait \nto go up for treat",
			"rawText": "can go down or wait \nto go up for treat",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "can go down or wait \nto go up for treat",
			"lineHeight": 1.25,
			"baseline": 42
		},
		{
			"type": "diamond",
			"version": 333,
			"versionNonce": 1453282334,
			"isDeleted": false,
			"id": "QatbZX52MN0rkx_3ixty8",
			"fillStyle": "cross-hatch",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1185.859432705702,
			"y": 1834.4999206135467,
			"strokeColor": "#6741d9",
			"backgroundColor": "#9c36b5",
			"width": 36.000010172526345,
			"height": 56.66666666666663,
			"seed": 1366665276,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692815577640,
			"link": null,
			"locked": false
		},
		{
			"type": "diamond",
			"version": 116,
			"versionNonce": 1690698946,
			"isDeleted": false,
			"id": "rFVeWVsI2BdutRdN1e7zB",
			"fillStyle": "cross-hatch",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 991.6592482923371,
			"y": 290.26177814586697,
			"strokeColor": "#6741d9",
			"backgroundColor": "#9c36b5",
			"width": 36.000010172526345,
			"height": 56.66666666666663,
			"seed": 1955343492,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692815577640,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 367,
			"versionNonce": 907747422,
			"isDeleted": false,
			"id": "WuLo0oNq",
			"fillStyle": "cross-hatch",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1605.4627259883457,
			"y": 2479.26199152671,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#9c36b5",
			"width": 297,
			"height": 25,
			"seed": 2040259844,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577640,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "another small view before exit",
			"rawText": "another small view before exit",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "another small view before exit",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 491,
			"versionNonce": 619453570,
			"isDeleted": false,
			"id": "aTqZLtwX",
			"fillStyle": "cross-hatch",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1028.4040962432541,
			"y": 2705.8184087829563,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#9c36b5",
			"width": 96,
			"height": 25,
			"seed": 894557188,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577640,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Death pit",
			"rawText": "Death pit",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Death pit",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 1163,
			"versionNonce": 80962718,
			"isDeleted": false,
			"id": "lSTLxID39Ze5d-a052si7",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1229.291951626403,
			"y": 1079.3168366674097,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 262.32521637929153,
			"height": 28.19622309967368,
			"seed": 1068631612,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577640,
			"link": null,
			"locked": false
		},
		{
			"type": "ellipse",
			"version": 442,
			"versionNonce": 1878604866,
			"isDeleted": false,
			"id": "1eSNYcc7cI7F8MHAUrH2S",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1272.215728197229,
			"y": 869.8053605255377,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 165.71428571428578,
			"height": 149.71426827566972,
			"seed": 1418583740,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692815577640,
			"link": null,
			"locked": false
		},
		{
			"type": "arrow",
			"version": 1321,
			"versionNonce": 343482590,
			"isDeleted": false,
			"id": "U8jpRJ4acxuuvpGC8L2_P",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1348.4889926201197,
			"y": 1477.8746109204385,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#ffffff",
			"width": 5.919061272260478,
			"height": 346.0217649033159,
			"seed": 22718268,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692815577640,
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
					-5.919061272260478,
					-346.0217649033159
				]
			]
		},
		{
			"type": "rectangle",
			"version": 1261,
			"versionNonce": 1674339330,
			"isDeleted": false,
			"id": "XbJHELSQ1QVyVcwpxm4Y5",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1218.2382511224407,
			"y": 1503.9287352254214,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 270.99491105402103,
			"height": 26.195553682676746,
			"seed": 2054840252,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577640,
			"link": null,
			"locked": false
		},
		{
			"type": "line",
			"version": 539,
			"versionNonce": 1486705950,
			"isDeleted": false,
			"id": "hXmv_zkP50fs_oBqCHxpJ",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1291.8017421480893,
			"y": 987.8206671431487,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 0,
			"height": 606.1048346240736,
			"seed": 403638332,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692815577640,
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
					606.1048346240736
				]
			]
		},
		{
			"type": "line",
			"version": 658,
			"versionNonce": 174363586,
			"isDeleted": false,
			"id": "baTcQ65rcAsakjqR8RKVL",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1420.3572687555627,
			"y": 980.8630964118763,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 0,
			"height": 622.6623809412831,
			"seed": 1576706236,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692815577640,
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
					622.6623809412831
				]
			]
		},
		{
			"type": "rectangle",
			"version": 896,
			"versionNonce": 716243294,
			"isDeleted": false,
			"id": "UtSethQJu7XmNgLcNvBvm",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1447.6247185774666,
			"y": 1463.2956762579813,
			"strokeColor": "#1971c2",
			"backgroundColor": "#a5d8ff",
			"width": 30.222167968750455,
			"height": 29.333428276909782,
			"seed": 1865539204,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577640,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 682,
			"versionNonce": 1440795522,
			"isDeleted": false,
			"id": "7nygdy7GvPlWzKlOjpDDX",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 194.25331965168357,
			"y": 1119.638519449946,
			"strokeColor": "#1971c2",
			"backgroundColor": "#a5d8ff",
			"width": 30.222167968750455,
			"height": 29.333428276909782,
			"seed": 2085712956,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577640,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 399,
			"versionNonce": 235218334,
			"isDeleted": false,
			"id": "jgRpGetjiVQE90x50ebYC",
			"fillStyle": "cross-hatch",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -399.6032964677097,
			"y": -243.17291178751543,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 2022.8796630408895,
			"height": 727.1293594522735,
			"seed": 644995360,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577640,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 458,
			"versionNonce": 478153538,
			"isDeleted": false,
			"id": "e1xMYUrR36gc22nRL6DN_",
			"fillStyle": "cross-hatch",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -442.2697698563825,
			"y": 4160.160981034749,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 6088.666763305664,
			"height": 2076.666666666667,
			"seed": 1543803104,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577640,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 88,
			"versionNonce": 1942667742,
			"isDeleted": false,
			"id": "8AmIuv51",
			"fillStyle": "cross-hatch",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -349.93818015227197,
			"y": -197.83971069702113,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 64,
			"height": 25,
			"seed": 970132768,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577640,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Level 1",
			"rawText": "Level 1",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Level 1",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 207,
			"versionNonce": 346116866,
			"isDeleted": false,
			"id": "xbzj1fqc",
			"fillStyle": "cross-hatch",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -358.2702123612653,
			"y": 4222.160136715087,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 73,
			"height": 25,
			"seed": 1587988704,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577640,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Level 3",
			"rawText": "Level 3",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Level 3",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 267,
			"versionNonce": 2131940894,
			"isDeleted": false,
			"id": "cSSYf3yhivg4RN_sBwLlF",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 883.9030386380197,
			"y": -52.511515481863455,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 168.19051106770806,
			"height": 30.857146732390735,
			"seed": 1094287648,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577640,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 435,
			"versionNonce": 1354998466,
			"isDeleted": false,
			"id": "M-n1SqZvbk3DzyI9z2fx1",
			"fillStyle": "cross-hatch",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -202.24053494131385,
			"y": 5097.515003985269,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 5570.666910807291,
			"height": 775.9999593098956,
			"seed": 719096096,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577640,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 235,
			"versionNonce": 1221485150,
			"isDeleted": false,
			"id": "2W_5mrn1DTUDlF8GggYdr",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -130.65020911450938,
			"y": 5136.581003334228,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 1554.6666971842442,
			"height": 719.9999999999995,
			"seed": 1190780192,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577640,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 392,
			"versionNonce": 998636162,
			"isDeleted": false,
			"id": "HEEr5pLfPbgh1KMcTjair",
			"fillStyle": "cross-hatch",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1894.4259486198873,
			"y": 5135.2476903459465,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#ffffff",
			"width": 1536.0001118977866,
			"height": 703.999837239583,
			"seed": 1651613920,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577640,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 414,
			"versionNonce": 600729246,
			"isDeleted": false,
			"id": "Q_eTQqm6nz-i6Wzhf0aNl",
			"fillStyle": "cross-hatch",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3899.0931035678027,
			"y": 5141.914255287351,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#ffffff",
			"width": 1391.9994099934893,
			"height": 720.0002034505211,
			"seed": 335910112,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577640,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 526,
			"versionNonce": 329734722,
			"isDeleted": false,
			"id": "mxv0w8DOg_Fwpk8o3xU5K",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -205.51048084284824,
			"y": 5738.860363182008,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 82.4445088704428,
			"height": 128.80948021298389,
			"seed": 2075166944,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577640,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 647,
			"versionNonce": 1623450334,
			"isDeleted": false,
			"id": "th4u_CA751RAmdtbEuENF",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -203.24750287944642,
			"y": 5102.066439425575,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 75.51111178927943,
			"height": 487.1428881448413,
			"seed": 294251744,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577640,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 302,
			"versionNonce": 1745273346,
			"isDeleted": false,
			"id": "1W89ZfLC",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -237.2696501640595,
			"y": 5663.304578986821,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 152,
			"height": 25,
			"seed": 1857176864,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577640,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "window entrance",
			"rawText": "window entrance",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "window entrance",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 271,
			"versionNonce": 306173726,
			"isDeleted": false,
			"id": "1xAcZOHy",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1008.1081676256545,
			"y": 5216.415730788036,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 96,
			"height": 25,
			"seed": 436855072,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577640,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "living room",
			"rawText": "living room",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "living room",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 377,
			"versionNonce": 329462210,
			"isDeleted": false,
			"id": "HM41WlYg",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 61.09217174517909,
			"y": 5213.374478958565,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 65,
			"height": 25,
			"seed": 733215968,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577640,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "kitchen",
			"rawText": "kitchen",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "kitchen",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 225,
			"versionNonce": 1353925470,
			"isDeleted": false,
			"id": "VNBXdAFo",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1380.5525578166266,
			"y": 5809.304660367026,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 84,
			"height": 25,
			"seed": 197839136,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577640,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "pet door",
			"rawText": "pet door",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "pet door",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 684,
			"versionNonce": 966502786,
			"isDeleted": false,
			"id": "SQXyZB-1SFZsHBvgiCTsQ",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1375.7744799493307,
			"y": 5107.399827012381,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 74.44452921549487,
			"height": 658.9205472431486,
			"seed": 1330532640,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577640,
			"link": null,
			"locked": false
		},
		{
			"type": "ellipse",
			"version": 1285,
			"versionNonce": 2121213854,
			"isDeleted": false,
			"id": "ajSbOYeSxw9UhXF4_QpXH",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -121.41881897196163,
			"y": 283.73579776423225,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 27.292840097560045,
			"height": 23.326046508023218,
			"seed": 905589142,
			"groupIds": [
				"iQEMO0gNTVn8bmnhxrNnL"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692815577640,
			"link": null,
			"locked": false
		},
		{
			"type": "freedraw",
			"version": 1068,
			"versionNonce": 1093609794,
			"isDeleted": false,
			"id": "6SVUathFlo3HkkPsbW9hN",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -120.38481228328999,
			"y": 290.09883818740354,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 5.9641894286609345,
			"height": 9.759576433798838,
			"seed": 439062230,
			"groupIds": [
				"iQEMO0gNTVn8bmnhxrNnL"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577641,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					-0.18073008808811764
				],
				[
					0,
					-0.36146017617623527
				],
				[
					-5.594217597396797e-17,
					-0.9036642292624609
				],
				[
					0.18073008808811777,
					-1.62659837043679
				],
				[
					0.18073008808811789,
					-2.710992687787354
				],
				[
					0.18073008808811766,
					-4.518321146312261
				],
				[
					0.18073008808811766,
					-5.964175639839061
				],
				[
					0,
					-7.048583746011483
				],
				[
					0,
					-7.771504098363969
				],
				[
					0,
					-8.675168327626416
				],
				[
					0,
					-8.855912204536391
				],
				[
					0,
					-9.217372380712627
				],
				[
					0,
					-9.398102468800744
				],
				[
					0,
					-9.578832556888862
				],
				[
					0,
					-9.759576433798838
				],
				[
					0.18073008808811766,
					-9.759576433798838
				],
				[
					0.5422040530862257,
					-9.759576433798838
				],
				[
					0.903664229262461,
					-9.578832556888862
				],
				[
					1.6265983704368043,
					-8.855912204536391
				],
				[
					1.807328458524922,
					-8.494438239538297
				],
				[
					2.1688024235230015,
					-7.952247975273944
				],
				[
					2.349532511611119,
					-7.410043922187718
				],
				[
					2.530262599699237,
					-7.048583746011483
				],
				[
					2.891722775875472,
					-6.68710978101339
				],
				[
					3.0724666527854625,
					-6.506379692925272
				],
				[
					3.2531967408735802,
					-6.325649604837155
				],
				[
					3.433926828961698,
					-5.964175639839061
				],
				[
					3.7953870051379335,
					-5.24125528748659
				],
				[
					3.976130882047895,
					-4.879781322488497
				],
				[
					4.518321146312248,
					-4.699051234400379
				],
				[
					5.241255287486591,
					-4.879781322488497
				],
				[
					5.9641894286609345,
					-5.421985375574708
				],
				[
					5.9641894286609345,
					-5.421985375574708
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.181640625,
				0.21484375,
				0.310546875,
				0.359375,
				0.40625,
				0.447265625,
				0.4853515625,
				0.49609375,
				0.501953125,
				0.51171875,
				0.5185546875,
				0.521484375,
				0.5263671875,
				0.53515625,
				0.5263671875,
				0.5263671875,
				0.53125,
				0.529296875,
				0.529296875,
				0.529296875,
				0.52734375,
				0.52734375,
				0.52734375,
				0.52734375,
				0.52734375,
				0.52734375,
				0.52734375,
				0.52734375,
				0.5302734375,
				0.537109375,
				0.529296875,
				0.4189453125,
				0.015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 1070,
			"versionNonce": 195331038,
			"isDeleted": false,
			"id": "A5pdzeIB6hqUjI_qlMEH_",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -101.22713338069028,
			"y": 285.94199100608944,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 5.42198537557468,
			"height": 9.578846345710721,
			"seed": 1119831062,
			"groupIds": [
				"iQEMO0gNTVn8bmnhxrNnL"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577641,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					-0.361473964998108
				],
				[
					0.18074387690996163,
					-0.361473964998108
				],
				[
					0.542204053086197,
					-1.2651381942605546
				],
				[
					1.2651381942605402,
					-1.9880723354348837
				],
				[
					1.9880723354348546,
					-2.8917365646973305
				],
				[
					3.0724666527854336,
					-3.6146569170498157
				],
				[
					3.795400793959777,
					-4.337591058224144
				],
				[
					4.518321146312247,
					-5.241255287486591
				],
				[
					4.699065023222209,
					-5.602729252484685
				],
				[
					5.060525199398445,
					-5.7834593405728025
				],
				[
					5.241255287486562,
					-5.96418942866092
				],
				[
					5.42198537557468,
					-5.96418942866092
				],
				[
					5.42198537557468,
					-5.602729252484685
				],
				[
					5.42198537557468,
					-5.060525199398474
				],
				[
					5.42198537557468,
					-4.337591058224144
				],
				[
					5.42198537557468,
					-3.6146569170498157
				],
				[
					5.42198537557468,
					-2.7109926877873542
				],
				[
					5.241255287486562,
					-1.9880723354348837
				],
				[
					5.241255287486562,
					-1.2651381942605546
				],
				[
					5.241255287486562,
					-0.361473964998108
				],
				[
					5.060525199398445,
					0.3614601761762353
				],
				[
					4.879795111310327,
					1.0843943173505644
				],
				[
					4.699065023222209,
					1.8073284585248934
				],
				[
					4.699065023222209,
					1.9880585466130112
				],
				[
					4.699065023222209,
					2.1687886347011287
				],
				[
					4.699065023222209,
					2.530248810877364
				],
				[
					4.518321146312247,
					2.891722775875458
				],
				[
					4.518321146312247,
					3.253182952051693
				],
				[
					4.518321146312247,
					3.433913040139825
				],
				[
					4.699065023222209,
					3.614656917049801
				],
				[
					4.879795111310327,
					3.614656917049801
				],
				[
					5.241255287486562,
					3.614656917049801
				],
				[
					5.241255287486562,
					3.614656917049801
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.177734375,
				0.2587890625,
				0.28125,
				0.3544921875,
				0.388671875,
				0.408203125,
				0.4228515625,
				0.435546875,
				0.455078125,
				0.4658203125,
				0.4736328125,
				0.486328125,
				0.4951171875,
				0.5126953125,
				0.5126953125,
				0.5126953125,
				0.5126953125,
				0.5126953125,
				0.51171875,
				0.51171875,
				0.51171875,
				0.517578125,
				0.51953125,
				0.525390625,
				0.525390625,
				0.525390625,
				0.525390625,
				0.525390625,
				0.53125,
				0.515625,
				0.486328125,
				0.296875,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 1097,
			"versionNonce": 1371320578,
			"isDeleted": false,
			"id": "CLFelb3D87emi8e2fJ1Cr",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -108.67088950935008,
			"y": 297.6930221262793,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 3.4174889321552437,
			"height": 1.8986049623084706,
			"seed": 564810070,
			"groupIds": [
				"iQEMO0gNTVn8bmnhxrNnL"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577641,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.07594303967584129,
					0
				],
				[
					-0.15189187343420177,
					-3.213996181392311e-17
				],
				[
					-0.22783491311002868,
					-0.15189187343419458
				],
				[
					-0.45566403213753826,
					-0.3037779527858557
				],
				[
					-0.7594419849233793,
					-0.5316128658958847
				],
				[
					-1.1391629773850764,
					-0.6834989452475524
				],
				[
					-1.3669978904951194,
					-0.9113338583575817
				],
				[
					-1.5948270095226005,
					-1.291054850819271
				],
				[
					-1.67077584328096,
					-1.442940930170939
				],
				[
					-1.7467188829568023,
					-1.5188839698467735
				],
				[
					-1.7467188829568023,
					-1.5948270095226076
				],
				[
					-1.6707758432809612,
					-1.5948270095226071
				],
				[
					-1.594827009522601,
					-1.5948270095226076
				],
				[
					-1.5188839698467735,
					-1.6707758432809676
				],
				[
					-1.2910548508192783,
					-1.6707758432809678
				],
				[
					-0.9872768980334226,
					-1.746718882956802
				],
				[
					-0.7594419849233792,
					-1.6707758432809678
				],
				[
					-0.45566403213753803,
					-1.594827009522608
				],
				[
					-0.15189187343420193,
					-1.5948270095226076
				],
				[
					0.07594303967584141,
					-1.5188839698467733
				],
				[
					0.3037779527858558,
					-1.5188839698467738
				],
				[
					0.455664032137524,
					-1.5188839698467733
				],
				[
					0.6834989452475527,
					-1.5948270095226071
				],
				[
					0.8353850245992208,
					-1.6707758432809678
				],
				[
					0.9113280642750619,
					-1.6707758432809685
				],
				[
					0.9872711039508891,
					-1.6707758432809678
				],
				[
					1.0632199377092497,
					-1.6707758432809683
				],
				[
					1.139162977385078,
					-1.6707758432809678
				],
				[
					1.2151060170609178,
					-1.7467188829568026
				],
				[
					1.2910490567367592,
					-1.8226619226326362
				],
				[
					1.3669920964125866,
					-1.8226619226326364
				],
				[
					1.4429409301709466,
					-1.8226619226326362
				],
				[
					1.5188839698467733,
					-1.8986049623084706
				],
				[
					1.5948270095226003,
					-1.8226619226326357
				],
				[
					1.6707700491984416,
					-1.8226619226326362
				],
				[
					1.5948270095226003,
					-1.7467188829568019
				],
				[
					1.518883969846774,
					-1.6707758432809678
				],
				[
					1.4429409301709466,
					-1.5948270095226076
				],
				[
					1.3669920964125866,
					-1.518883969846773
				],
				[
					1.291049056736759,
					-1.4429409301709397
				],
				[
					1.215106017060918,
					-1.2910548508192707
				],
				[
					1.0632199377092497,
					-1.1391629773850835
				],
				[
					0.9872711039508895,
					-0.9872768980334156
				],
				[
					0.9113280642750623,
					-0.911333858357581
				],
				[
					0.835385024599221,
					-0.8353850245992209
				],
				[
					0.7594419849233796,
					-0.7594419849233864
				],
				[
					0.6075501114891924,
					-0.6834989452475525
				],
				[
					0.5316070718133653,
					-0.6075559055717186
				],
				[
					0.4556640321375239,
					-0.5316128658958844
				],
				[
					0.3797209924616971,
					-0.4556640321375238
				],
				[
					0.30377795278585573,
					-0.37972099246168983
				],
				[
					0.2278291190274952,
					-0.3037779527858556
				],
				[
					0.22782911902749528,
					-0.22783491311002868
				],
				[
					0.1518860793516683,
					-0.15189187343419458
				],
				[
					0.15188607935166823,
					-0.0759430396758341
				],
				[
					0.2278291190274952,
					-0.0759430396758342
				],
				[
					0.37972099246169705,
					-0.15189187343419452
				],
				[
					0,
					0
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.171875,
				0.232421875,
				0.373046875,
				0.4453125,
				0.47265625,
				0.4912109375,
				0.5068359375,
				0.517578125,
				0.5234375,
				0.5234375,
				0.5234375,
				0.5234375,
				0.51953125,
				0.51953125,
				0.5166015625,
				0.5166015625,
				0.513671875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.513671875,
				0.51171875,
				0.51171875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.5166015625,
				0.513671875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.521484375,
				0.521484375,
				0.513671875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.4873046875,
				0.4306640625,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 1057,
			"versionNonce": 979654686,
			"isDeleted": false,
			"id": "nm3Hu8fWgXGVA4DzyTggY",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -109.1265535414878,
			"y": 298.376521071527,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 0.2278291190275104,
			"height": 2.6580469472318646,
			"seed": 574731926,
			"groupIds": [
				"iQEMO0gNTVn8bmnhxrNnL"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577641,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-5.356660302320523e-18,
					0.07594303967583413
				],
				[
					0.07594303967584133,
					0.22782911902750236
				],
				[
					0.07594303967584129,
					0.6075501114891994
				],
				[
					0.07594303967584137,
					0.9113280642750622
				],
				[
					0.15188607935168275,
					1.1391629773850838
				],
				[
					0.15188607935168222,
					1.44293513608842
				],
				[
					0.15188607935168275,
					1.594827009522615
				],
				[
					0.15188607935168275,
					1.8226561285501173
				],
				[
					0.1518860793516829,
					2.050491041660139
				],
				[
					0.07594303967584172,
					2.050491041660139
				],
				[
					0.0759430396758412,
					2.126434081335973
				],
				[
					0.07594303967584137,
					2.278325954770168
				],
				[
					0,
					2.4302120341218356
				],
				[
					-1.0284787780455404e-15,
					2.5061550737976703
				],
				[
					-1.7141312967425674e-16,
					2.582098113473504
				],
				[
					0,
					2.6580469472318646
				],
				[
					0.15188607935168344,
					2.6580469472318646
				],
				[
					0.22782911902750938,
					2.582098113473504
				],
				[
					0.22782911902750938,
					2.582098113473504
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.1953125,
				0.30078125,
				0.3388671875,
				0.37109375,
				0.38671875,
				0.3994140625,
				0.4111328125,
				0.42578125,
				0.4345703125,
				0.4501953125,
				0.4560546875,
				0.4677734375,
				0.470703125,
				0.470703125,
				0.470703125,
				0.470703125,
				0.474609375,
				0.3720703125,
				0.275390625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 1090,
			"versionNonce": 1321418946,
			"isDeleted": false,
			"id": "wTsEY9FB-MaCBsbQ2ZWxr",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -111.40487949625785,
			"y": 300.65484702629703,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 6.227421958738777,
			"height": 1.8226619226326364,
			"seed": 2100982742,
			"groupIds": [
				"iQEMO0gNTVn8bmnhxrNnL"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577641,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					0.07594303967583413
				],
				[
					0.07594303967582697,
					0.15188607935166826
				],
				[
					0.22782911902750963,
					0.22782911902750236
				],
				[
					0.3037721587033365,
					0.379720992461697
				],
				[
					0.4556640321375239,
					0.5316070718133652
				],
				[
					0.6075501114891922,
					0.6834931511650263
				],
				[
					0.7594419849233937,
					0.7594419849233868
				],
				[
					0.911328064275048,
					0.8353850245992207
				],
				[
					0.9872711039508891,
					0.7594419849233868
				],
				[
					1.1391629773850909,
					0.7594419849233868
				],
				[
					1.2151060170609178,
					0.6834931511650261
				],
				[
					1.291049056736745,
					0.6075501114891922
				],
				[
					1.3669920964125721,
					0.45566403213753126
				],
				[
					1.4429351360884133,
					0.3037721587033365
				],
				[
					1.5948270095226154,
					0.07594303967583424
				],
				[
					1.7467130888742688,
					-0.07594883375836059
				],
				[
					1.82265612855011,
					-0.15189187343419439
				],
				[
					1.82265612855011,
					-0.22783491311002874
				],
				[
					1.8986049623084706,
					-0.3037779527858627
				],
				[
					1.8986049623084706,
					-0.37972099246168983
				],
				[
					1.9745480019843118,
					-0.37972099246168994
				],
				[
					1.9745480019843122,
					-0.45566982622005087
				],
				[
					2.1264340813359657,
					-0.45566982622005064
				],
				[
					2.202377121011793,
					-0.4556698262200503
				],
				[
					2.2783259547701533,
					-0.37972099246168994
				],
				[
					2.3542689944459947,
					-0.37972099246168983
				],
				[
					2.3542689944459947,
					-0.30377795278586267
				],
				[
					2.4302120341218356,
					-0.30377795278586284
				],
				[
					2.506155073797663,
					-0.30377795278586284
				],
				[
					2.506155073797663,
					-0.22783491311002874
				],
				[
					2.58209811347349,
					-0.15189187343419483
				],
				[
					2.58209811347349,
					-0.0759488337583607
				],
				[
					2.6580469472318504,
					0.15188607935166826
				],
				[
					2.7339899869076913,
					0.22782911902750236
				],
				[
					2.8858760662593594,
					0.379720992461697
				],
				[
					2.9618191059351866,
					0.5316070718133652
				],
				[
					3.037767939693547,
					0.6075501114891922
				],
				[
					3.1137109793693885,
					0.7594419849233865
				],
				[
					3.1896540190452156,
					0.8353850245992209
				],
				[
					3.3415400983968837,
					1.0632141436267233
				],
				[
					3.4174889321552437,
					1.1391629773850838
				],
				[
					3.5693750115069123,
					1.2151060170609176
				],
				[
					3.645318051182754,
					1.2151060170609178
				],
				[
					3.7972099246169413,
					1.291049056736752
				],
				[
					3.9490960039686094,
					1.291049056736752
				],
				[
					4.100982083320278,
					1.2151060170609178
				],
				[
					4.252873956754465,
					1.2151060170609178
				],
				[
					4.480703075781975,
					1.0632141436267233
				],
				[
					4.78448102856783,
					0.911328064275055
				],
				[
					5.012315941677859,
					0.6834931511650263
				],
				[
					5.240145060705355,
					0.5316070718133652
				],
				[
					5.467979973815383,
					0.3037721587033365
				],
				[
					5.695814886925412,
					0.07594303967583413
				],
				[
					5.923644005952907,
					-0.07594883375836048
				],
				[
					5.999587045628748,
					-0.1518918734341946
				],
				[
					6.075535879387094,
					-0.30377795278586284
				],
				[
					6.151478919062936,
					-0.37972099246168983
				],
				[
					6.227421958738777,
					-0.5316128658958844
				],
				[
					6.227421958738777,
					-0.5316128658958844
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.1865234375,
				0.2373046875,
				0.265625,
				0.294921875,
				0.326171875,
				0.3505859375,
				0.3662109375,
				0.373046875,
				0.3798828125,
				0.392578125,
				0.396484375,
				0.3984375,
				0.3984375,
				0.4013671875,
				0.408203125,
				0.41015625,
				0.41015625,
				0.41015625,
				0.41015625,
				0.412109375,
				0.4228515625,
				0.4140625,
				0.4072265625,
				0.4072265625,
				0.4111328125,
				0.4091796875,
				0.3955078125,
				0.3310546875,
				0.3837890625,
				0.384765625,
				0.3955078125,
				0.3974609375,
				0.3974609375,
				0.3974609375,
				0.3974609375,
				0.3974609375,
				0.3974609375,
				0.3974609375,
				0.3974609375,
				0.4013671875,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.40625,
				0.41015625,
				0.4150390625,
				0.423828125,
				0.427734375,
				0.427734375,
				0.4345703125,
				0.3779296875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 1068,
			"versionNonce": 1654629470,
			"isDeleted": false,
			"id": "0V-xt6JQ_YCeV5Zj3HnQy",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -114.59453930938565,
			"y": 290.17454531672115,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 5.39204272822206,
			"height": 3.6453180511827465,
			"seed": 212437270,
			"groupIds": [
				"iQEMO0gNTVn8bmnhxrNnL"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577641,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.15189187343420177,
					0.1518918734341945
				],
				[
					-0.45566403213753826,
					0.30377795278586284
				],
				[
					-0.9113338583575953,
					0.5316128658958917
				],
				[
					-1.518883969846773,
					1.2151060170609176
				],
				[
					-1.8226619226326433,
					1.7467188829568097
				],
				[
					-1.9745480019842971,
					2.2023829150943337
				],
				[
					-2.050496835742657,
					2.5061608678801965
				],
				[
					-2.0504968357426576,
					2.733989986907698
				],
				[
					-1.822661922632643,
					2.96182490001772
				],
				[
					-1.518883969846774,
					3.113710979369388
				],
				[
					-0.9872768980334224,
					3.1137109793693885
				],
				[
					-0.22783491311002887,
					2.9618249000177213
				],
				[
					0.3037779527858561,
					2.8099388206660523
				],
				[
					0.6834989452475531,
					2.58210390755603
				],
				[
					1.1391629773850762,
					2.354268994446002
				],
				[
					1.5188839698467738,
					2.050496835742665
				],
				[
					2.1264340813359652,
					1.7467188829568099
				],
				[
					2.88587606625936,
					1.139162977385084
				],
				[
					3.1137109793693876,
					0.7594419849233941
				],
				[
					3.2655970587210423,
					0.5316128658958917
				],
				[
					3.3415458924794024,
					0.3037779527858632
				],
				[
					3.2655970587210423,
					0.15189187343419447
				],
				[
					3.189654019045215,
					0
				],
				[
					2.809933026583518,
					-0.1518860793516612
				],
				[
					2.430212034121821,
					-0.303777952785856
				],
				[
					1.8986049623084706,
					-0.4556640321375241
				],
				[
					1.0632199377092495,
					-0.5316070718133581
				],
				[
					0.9113280642750622,
					-0.4556640321375239
				],
				[
					0.6075501114891921,
					-0.3797209924616898
				],
				[
					0.5316070718133652,
					-0.3797209924616899
				],
				[
					0.3037779527858557,
					-0.30377795278585573
				],
				[
					0.3037779527858556,
					-0.22782911902749525
				],
				[
					0.3797209924616826,
					-0.2278291190274952
				],
				[
					0,
					0
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.171875,
				0.201171875,
				0.2529296875,
				0.3037109375,
				0.361328125,
				0.38671875,
				0.4130859375,
				0.423828125,
				0.42578125,
				0.42578125,
				0.419921875,
				0.4150390625,
				0.4033203125,
				0.400390625,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.408203125,
				0.4306640625,
				0.45703125,
				0.47265625,
				0.4775390625,
				0.482421875,
				0.4951171875,
				0.4970703125,
				0.4970703125,
				0.4970703125,
				0.466796875,
				0.4140625,
				0.0263671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 1068,
			"versionNonce": 1407309954,
			"isDeleted": false,
			"id": "VZcX1KZXug7DWX_L3-FvN",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -103.43074444864476,
			"y": 289.4151033317979,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 4.556651909540335,
			"height": 3.4174889321552446,
			"seed": 537130582,
			"groupIds": [
				"iQEMO0gNTVn8bmnhxrNnL"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577641,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.15188607935165394,
					-0.07594303967583418
				],
				[
					-0.6075501114892065,
					-0.07594303967583416
				],
				[
					-0.9872711039508748,
					-8.570656483712831e-17
				],
				[
					-1.3669920964125717,
					0.22783491311002857
				],
				[
					-1.746713088874269,
					0.5316128658958919
				],
				[
					-2.202382915094326,
					1.0632199377092497
				],
				[
					-2.3542689944460085,
					1.5188839698467806
				],
				[
					-2.278325954770153,
					1.9745480019843047
				],
				[
					-2.0504910416601385,
					2.354268994446002
				],
				[
					-1.7467130888742697,
					2.658046947231858
				],
				[
					-1.1391629773850909,
					2.8858818603418865
				],
				[
					-0.7594419849233935,
					2.961824900017721
				],
				[
					-0.30377795278586966,
					2.885881860341886
				],
				[
					0.07594303967582673,
					2.7339899869076913
				],
				[
					0.8353850245992208,
					2.354268994446002
				],
				[
					1.4429409301709326,
					1.9745480019843042
				],
				[
					1.8226619226326288,
					1.6707758432809685
				],
				[
					2.0504968357426727,
					1.3669978904951126
				],
				[
					2.202382915094326,
					1.0632199377092504
				],
				[
					2.202382915094326,
					0.7594419849233874
				],
				[
					2.202382915094326,
					0.5316128658958911
				],
				[
					2.126439875418499,
					0.30377795278586267
				],
				[
					1.9745480019843116,
					0
				],
				[
					1.6707758432809752,
					-0.15188607935166806
				],
				[
					0.9113338583575813,
					-0.3797209924616896
				],
				[
					0.30377795278586994,
					-0.455664032137524
				],
				[
					-0.07594303967582688,
					-0.455664032137524
				],
				[
					-0.45566403213752393,
					-0.30377795278586284
				],
				[
					-0.7594419849233939,
					-0.15188607935166815
				],
				[
					-0.9872711039508748,
					-8.570656483712831e-17
				],
				[
					-0.9872711039508749,
					0.15189187343419472
				],
				[
					-0.9872711039508749,
					0.3797209924616973
				],
				[
					0,
					0
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.173828125,
				0.1923828125,
				0.294921875,
				0.3798828125,
				0.447265625,
				0.4873046875,
				0.4912109375,
				0.486328125,
				0.484375,
				0.482421875,
				0.48046875,
				0.4697265625,
				0.4658203125,
				0.470703125,
				0.4677734375,
				0.474609375,
				0.4765625,
				0.4765625,
				0.478515625,
				0.48046875,
				0.4921875,
				0.4951171875,
				0.5,
				0.5126953125,
				0.521484375,
				0.5234375,
				0.525390625,
				0.525390625,
				0.525390625,
				0.505859375,
				0.423828125,
				0.1904296875,
				0.01171875,
				0
			]
		},
		{
			"type": "rectangle",
			"version": 206,
			"versionNonce": 908552350,
			"isDeleted": false,
			"id": "OwTFqoBkYLm2pfAuyk5v8",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -431.1288652405251,
			"y": -453.3712770056493,
			"strokeColor": "#f08c00",
			"backgroundColor": "#ffd8a8",
			"width": 397,
			"height": 183,
			"seed": 1556822157,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "NyonXevM"
				}
			],
			"updated": 1692815577641,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 204,
			"versionNonce": 819427394,
			"isDeleted": false,
			"id": "NyonXevM",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -283.6288652405251,
			"y": -374.3712770056493,
			"strokeColor": "#f08c00",
			"backgroundColor": "transparent",
			"width": 102,
			"height": 25,
			"seed": 1982112803,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577641,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "parking lot",
			"rawText": "parking lot",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "OwTFqoBkYLm2pfAuyk5v8",
			"originalText": "parking lot",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 115,
			"versionNonce": 78423262,
			"isDeleted": false,
			"id": "mIzoYf2G",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -278.5763632686202,
			"y": -483.61243551551513,
			"strokeColor": "#f08c00",
			"backgroundColor": "#ffd8a8",
			"width": 64,
			"height": 25,
			"seed": 1069881773,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577641,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Level 1",
			"rawText": "Level 1",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Level 1",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 245,
			"versionNonce": 1703092226,
			"isDeleted": false,
			"id": "xhtibnLuR3MqzFSClmEYV",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 520.9104469166955,
			"y": -486.58362504720594,
			"strokeColor": "#f08c00",
			"backgroundColor": "#ffd8a8",
			"width": 397,
			"height": 183,
			"seed": 47801005,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "qL98QAo1"
				}
			],
			"updated": 1692815577641,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 173,
			"versionNonce": 2143312158,
			"isDeleted": false,
			"id": "qL98QAo1",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 652.9104469166955,
			"y": -407.58362504720594,
			"strokeColor": "#f08c00",
			"backgroundColor": "transparent",
			"width": 133,
			"height": 25,
			"seed": 1050181325,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577641,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "building puzzle",
			"rawText": "building puzzle",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "xhtibnLuR3MqzFSClmEYV",
			"originalText": "building puzzle",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 165,
			"versionNonce": 501469122,
			"isDeleted": false,
			"id": "ANQHjpkg",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 675.9084183186101,
			"y": -516.4547000018148,
			"strokeColor": "#f08c00",
			"backgroundColor": "#ffd8a8",
			"width": 73,
			"height": 25,
			"seed": 1079149837,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577641,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Level 2",
			"rawText": "Level 2",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Level 2",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 215,
			"versionNonce": 2127791454,
			"isDeleted": false,
			"id": "BqBeaw50BaZB-6Ift_cF2",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 961.6364620949023,
			"y": -490.99184302440074,
			"strokeColor": "#f08c00",
			"backgroundColor": "#ffd8a8",
			"width": 397,
			"height": 183,
			"seed": 2041532909,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "VzRCZTgr"
				}
			],
			"updated": 1692815577641,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 122,
			"versionNonce": 773359490,
			"isDeleted": false,
			"id": "VzRCZTgr",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1074.6364620949023,
			"y": -411.99184302440074,
			"strokeColor": "#f08c00",
			"backgroundColor": "transparent",
			"width": 171,
			"height": 25,
			"seed": 60178819,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577641,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "apartment floor 1",
			"rawText": "apartment floor 1",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "BqBeaw50BaZB-6Ift_cF2",
			"originalText": "apartment floor 1",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 158,
			"versionNonce": 1127688606,
			"isDeleted": false,
			"id": "hsmRdwOT",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1115.890295572216,
			"y": -518.771406732584,
			"strokeColor": "#f08c00",
			"backgroundColor": "#ffd8a8",
			"width": 73,
			"height": 25,
			"seed": 489196621,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577641,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Level 3",
			"rawText": "Level 3",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Level 3",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 312,
			"versionNonce": 241190722,
			"isDeleted": false,
			"id": "Z3RLRBXr7-g3SwIVJsdYx",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2230.006158456532,
			"y": -473.1392952013434,
			"strokeColor": "#f08c00",
			"backgroundColor": "#ffd8a8",
			"width": 331,
			"height": 164,
			"seed": 2012608707,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "XFxnWaUJ"
				}
			],
			"updated": 1692815577641,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 308,
			"versionNonce": 1008485854,
			"isDeleted": false,
			"id": "XFxnWaUJ",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2318.506158456532,
			"y": -403.6392952013434,
			"strokeColor": "#f08c00",
			"backgroundColor": "transparent",
			"width": 154,
			"height": 25,
			"seed": 1980404419,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577641,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Factory space 1",
			"rawText": "Factory space 1",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "Z3RLRBXr7-g3SwIVJsdYx",
			"originalText": "Factory space 1",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 258,
			"versionNonce": 1461325570,
			"isDeleted": false,
			"id": "RhZtrxjb",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2354.415182781816,
			"y": -501.1242583583036,
			"strokeColor": "#f08c00",
			"backgroundColor": "#ffd8a8",
			"width": 72,
			"height": 25,
			"seed": 526462403,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577641,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Level 6",
			"rawText": "Level 6",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Level 6",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 316,
			"versionNonce": 1251203614,
			"isDeleted": false,
			"id": "DEcJ-pOC1rpUyZ2UEEqpA",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1844.2498329948799,
			"y": -467.73635450901986,
			"strokeColor": "#f08c00",
			"backgroundColor": "#ffd8a8",
			"width": 362,
			"height": 164,
			"seed": 1453635587,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "OBxeOJcW"
				}
			],
			"updated": 1692815577641,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 319,
			"versionNonce": 1019535042,
			"isDeleted": false,
			"id": "OBxeOJcW",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1949.2498329948799,
			"y": -398.23635450901986,
			"strokeColor": "#f08c00",
			"backgroundColor": "transparent",
			"width": 152,
			"height": 25,
			"seed": 838123427,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577641,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Crowded street",
			"rawText": "Crowded street",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "DEcJ-pOC1rpUyZ2UEEqpA",
			"originalText": "Crowded street",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 248,
			"versionNonce": 93251166,
			"isDeleted": false,
			"id": "01i6Y166",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1968.6588573201636,
			"y": -497.05463065426136,
			"strokeColor": "#f08c00",
			"backgroundColor": "#ffd8a8",
			"width": 71,
			"height": 25,
			"seed": 555930435,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577641,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Level 5",
			"rawText": "Level 5",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Level 5",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "freedraw",
			"version": 274,
			"versionNonce": 201307778,
			"isDeleted": false,
			"id": "ClZURmkP_8kqkAiaqYe4G",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1580.549909729795,
			"y": -488.8416330168834,
			"strokeColor": "#f08c00",
			"backgroundColor": "#ffd8a8",
			"width": 0.0001,
			"height": 0.0001,
			"seed": 1066131917,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577641,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.0001,
					0.0001
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "rectangle",
			"version": 233,
			"versionNonce": 2111728286,
			"isDeleted": false,
			"id": "XiSJAS0ZOQiyX1wVCxc1y",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1402.916499661546,
			"y": -487.6723570491633,
			"strokeColor": "#f08c00",
			"backgroundColor": "#ffd8a8",
			"width": 397,
			"height": 183,
			"seed": 1017651245,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "sMkOQ8YJ"
				}
			],
			"updated": 1692815577641,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 141,
			"versionNonce": 629773890,
			"isDeleted": false,
			"id": "sMkOQ8YJ",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1511.416499661546,
			"y": -408.6723570491633,
			"strokeColor": "#f08c00",
			"backgroundColor": "transparent",
			"width": 180,
			"height": 25,
			"seed": 476942989,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577641,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "apartment floor 2",
			"rawText": "apartment floor 2",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "XiSJAS0ZOQiyX1wVCxc1y",
			"originalText": "apartment floor 2",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 176,
			"versionNonce": 36923102,
			"isDeleted": false,
			"id": "LmD2A6AP",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1553.8369998055264,
			"y": -517.4519411023985,
			"strokeColor": "#f08c00",
			"backgroundColor": "#ffd8a8",
			"width": 72,
			"height": 25,
			"seed": 462797037,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577641,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Level 4",
			"rawText": "Level 4",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Level 4",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 348,
			"versionNonce": 2051112450,
			"isDeleted": false,
			"id": "WbMsjUufJxHYd6ftvm0GG",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2597.9164437126483,
			"y": -464.73632399144196,
			"strokeColor": "#f08c00",
			"backgroundColor": "#ffd8a8",
			"width": 361,
			"height": 164,
			"seed": 1999324131,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "RZzEna0D"
				}
			],
			"updated": 1692815577641,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 349,
			"versionNonce": 1662966558,
			"isDeleted": false,
			"id": "RZzEna0D",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2696.9164437126483,
			"y": -395.23632399144196,
			"strokeColor": "#f08c00",
			"backgroundColor": "transparent",
			"width": 163,
			"height": 25,
			"seed": 1031720835,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577641,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Factory space 2",
			"rawText": "Factory space 2",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "WbMsjUufJxHYd6ftvm0GG",
			"originalText": "Factory space 2",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 290,
			"versionNonce": 119958978,
			"isDeleted": false,
			"id": "AfdVGiEy",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2722.3254680379323,
			"y": -492.7212871484022,
			"strokeColor": "#f08c00",
			"backgroundColor": "#ffd8a8",
			"width": 70,
			"height": 25,
			"seed": 1956636451,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577641,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Level 7",
			"rawText": "Level 7",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Level 7",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 359,
			"versionNonce": 923912030,
			"isDeleted": false,
			"id": "jeukbq5pLzghIPv4j-zBw",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2977.297016803701,
			"y": -457.64095437997435,
			"strokeColor": "#f08c00",
			"backgroundColor": "#ffd8a8",
			"width": 374,
			"height": 164,
			"seed": 1840769645,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "9iaSVHGq"
				}
			],
			"updated": 1692815577641,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 358,
			"versionNonce": 1364682114,
			"isDeleted": false,
			"id": "9iaSVHGq",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3082.797016803701,
			"y": -388.14095437997435,
			"strokeColor": "#f08c00",
			"backgroundColor": "transparent",
			"width": 163,
			"height": 25,
			"seed": 629806285,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577641,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Factory space 3",
			"rawText": "Factory space 3",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "jeukbq5pLzghIPv4j-zBw",
			"originalText": "Factory space 3",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 265,
			"versionNonce": 509422494,
			"isDeleted": false,
			"id": "7KiHeXge",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3095.992104187021,
			"y": -497.05455436031605,
			"strokeColor": "#f08c00",
			"backgroundColor": "#ffd8a8",
			"width": 74,
			"height": 25,
			"seed": 1248326445,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577641,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Level 8",
			"rawText": "Level 8",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Level 8",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 359,
			"versionNonce": 1645438274,
			"isDeleted": false,
			"id": "C8FyTY1kYw7jwavHLkmVv",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3371.89280130891,
			"y": -467.40295360104983,
			"strokeColor": "#f08c00",
			"backgroundColor": "#ffd8a8",
			"width": 374,
			"height": 164,
			"seed": 20285069,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "kyuLcY9D"
				}
			],
			"updated": 1692815577641,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 371,
			"versionNonce": 120719326,
			"isDeleted": false,
			"id": "kyuLcY9D",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3488.89280130891,
			"y": -397.90295360104983,
			"strokeColor": "#f08c00",
			"backgroundColor": "transparent",
			"width": 140,
			"height": 25,
			"seed": 188689645,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577641,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Factory roof 1",
			"rawText": "Factory roof 1",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "C8FyTY1kYw7jwavHLkmVv",
			"originalText": "Factory roof 1",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 300,
			"versionNonce": 1119448322,
			"isDeleted": false,
			"id": "eNsn9j25",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3496.3018256341948,
			"y": -495.38791675800985,
			"strokeColor": "#f08c00",
			"backgroundColor": "#ffd8a8",
			"width": 71,
			"height": 25,
			"seed": 1174734669,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577641,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Level 9",
			"rawText": "Level 9",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Level 9",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 382,
			"versionNonce": 1906400286,
			"isDeleted": false,
			"id": "u_-JbtvptTtTIuBDQzcuu",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3779.6071327995614,
			"y": -477.4030407941299,
			"strokeColor": "#f08c00",
			"backgroundColor": "#ffd8a8",
			"width": 374,
			"height": 164,
			"seed": 1070874723,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "v3ivSRJL"
				}
			],
			"updated": 1692815577641,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 393,
			"versionNonce": 2026405058,
			"isDeleted": false,
			"id": "v3ivSRJL",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3892.1071327995614,
			"y": -407.9030407941299,
			"strokeColor": "#f08c00",
			"backgroundColor": "transparent",
			"width": 149,
			"height": 25,
			"seed": 1892957187,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577641,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Factory roof 2",
			"rawText": "Factory roof 2",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "u_-JbtvptTtTIuBDQzcuu",
			"originalText": "Factory roof 2",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 325,
			"versionNonce": 865871966,
			"isDeleted": false,
			"id": "Be4UxvXF",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3904.016157124846,
			"y": -505.3880039510899,
			"strokeColor": "#f08c00",
			"backgroundColor": "#ffd8a8",
			"width": 78,
			"height": 25,
			"seed": 1670628259,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577641,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Level 10",
			"rawText": "Level 10",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Level 10",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 1116,
			"versionNonce": 31429762,
			"isDeleted": false,
			"id": "r8ayFx0fVQl1RDAw0R9sB",
			"fillStyle": "cross-hatch",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -403.0698976207502,
			"y": 1801.5968104713832,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 2624.665985107422,
			"height": 856.5797641681093,
			"seed": 314037726,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577641,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 408,
			"versionNonce": 1022586014,
			"isDeleted": false,
			"id": "BC7X5gmz",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -334.3519860033679,
			"y": 1847.7157457643402,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 73,
			"height": 25.066297977152026,
			"seed": 771163778,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577641,
			"link": null,
			"locked": false,
			"fontSize": 20.05303838172162,
			"fontFamily": 1,
			"text": "Level 2",
			"rawText": "Level 2",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Level 2",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 377,
			"versionNonce": 1337832514,
			"isDeleted": false,
			"id": "HYVV9mU2xG5naXqXHayGF",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -249.63071340160093,
			"y": 164.9960823393393,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 20.134598314704938,
			"height": 202.00415300136902,
			"seed": 1233844674,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577641,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 386,
			"versionNonce": 1532504286,
			"isDeleted": false,
			"id": "BYhMAUsiOeivGbf3xaEv6",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -223.15938217411036,
			"y": 305.6994408723425,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 85.95516585973473,
			"height": 58.439001392477714,
			"seed": 845451102,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577641,
			"link": null,
			"locked": false
		},
		{
			"type": "diamond",
			"version": 187,
			"versionNonce": 1145166850,
			"isDeleted": false,
			"id": "LRVN3P5L7Polv33P6ZUVZ",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 167.8268155756778,
			"y": -654.7166622874852,
			"strokeColor": "#f08c00",
			"backgroundColor": "#ffd8a8",
			"width": 208,
			"height": 170,
			"seed": 731593218,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "K9zb3C8G"
				}
			],
			"updated": 1692815577641,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 311,
			"versionNonce": 2119916830,
			"isDeleted": false,
			"id": "K9zb3C8G",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 227.8268155756778,
			"y": -594.7166622874852,
			"strokeColor": "#f08c00",
			"backgroundColor": "transparent",
			"width": 88,
			"height": 50,
			"seed": 1299492062,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577641,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Cinematic\n2",
			"rawText": "Cinematic 2",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "LRVN3P5L7Polv33P6ZUVZ",
			"originalText": "Cinematic 2",
			"lineHeight": 1.25,
			"baseline": 42
		},
		{
			"type": "rectangle",
			"version": 247,
			"versionNonce": 761990082,
			"isDeleted": false,
			"id": "dO36kUvX46Ak79lSmrJ2P",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -409.2073257959371,
			"y": 640.9953117620513,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 2210,
			"height": 1071.3334147135415,
			"seed": 448672898,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577641,
			"link": null,
			"locked": true
		},
		{
			"type": "text",
			"version": 183,
			"versionNonce": 2070808926,
			"isDeleted": false,
			"id": "CCzK6JWe",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -359.59467350267175,
			"y": 689.6418929392449,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 103,
			"height": 25,
			"seed": 1204408030,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577641,
			"link": null,
			"locked": true,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Cinematic 1",
			"rawText": "Cinematic 1",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Cinematic 1",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 1072,
			"versionNonce": 1096303490,
			"isDeleted": false,
			"id": "qj-oYKOn2vAD-rJeyKib6",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -432.1253156836551,
			"y": 2587.9094883176467,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 2604.089155409071,
			"height": 68.88880072699597,
			"seed": 2109380866,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577641,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 566,
			"versionNonce": 1373711774,
			"isDeleted": false,
			"id": "733ZSQU4yGEjc0VeSJVvY",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -249.57517226895447,
			"y": 371.37768971993694,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 1845.0079284013652,
			"height": 73.72612868522441,
			"seed": 982680030,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577641,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 1379,
			"versionNonce": 440959810,
			"isDeleted": false,
			"id": "obmJL3-B085N6w5xj5H0p",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -584.8890158851463,
			"y": 766.1989006568565,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 145,
			"height": 699,
			"seed": 378809922,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "RrDHGcxz"
				}
			],
			"updated": 1692815577641,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 271,
			"versionNonce": 1860553182,
			"isDeleted": false,
			"id": "RrDHGcxz",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -544.3890158851463,
			"y": 1103.1989006568565,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 64,
			"height": 25,
			"seed": 1580530957,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577641,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Level 1",
			"rawText": "Level 1",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "obmJL3-B085N6w5xj5H0p",
			"originalText": "Level 1",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 1789,
			"versionNonce": 849005314,
			"isDeleted": false,
			"id": "sQzjFZhk34-5MCp4yXjvK",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1832.3966635233364,
			"y": 784.6130705133367,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 166,
			"height": 735,
			"seed": 1828947714,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "B6D0cq9k"
				}
			],
			"updated": 1692815577641,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 516,
			"versionNonce": 1905057310,
			"isDeleted": false,
			"id": "B6D0cq9k",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1878.8966635233364,
			"y": 1139.6130705133367,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 73,
			"height": 25,
			"seed": 1480918605,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577642,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Level 2",
			"rawText": "Level 2",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "sQzjFZhk34-5MCp4yXjvK",
			"originalText": "Level 2",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "diamond",
			"version": 270,
			"versionNonce": 1624120002,
			"isDeleted": false,
			"id": "75ch7j9x_FbyVK3CVmxTg",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -889.3330144131852,
			"y": -601.4651924287838,
			"strokeColor": "#f08c00",
			"backgroundColor": "#ffd8a8",
			"width": 208,
			"height": 170,
			"seed": 674741485,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "9ZWnqF35"
				}
			],
			"updated": 1692815577642,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 399,
			"versionNonce": 1858562654,
			"isDeleted": false,
			"id": "9ZWnqF35",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -829.3330144131852,
			"y": -541.4651924287838,
			"strokeColor": "#f08c00",
			"backgroundColor": "transparent",
			"width": 88,
			"height": 50,
			"seed": 1433114445,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577642,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Cinematic\n1",
			"rawText": "Cinematic 1",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "75ch7j9x_FbyVK3CVmxTg",
			"originalText": "Cinematic 1",
			"lineHeight": 1.25,
			"baseline": 42
		},
		{
			"type": "diamond",
			"version": 497,
			"versionNonce": 1400992386,
			"isDeleted": false,
			"id": "fnI-R6UmaXkH1t5ZCGvBI",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1456.0954458574913,
			"y": -622.3725982324127,
			"strokeColor": "#f08c00",
			"backgroundColor": "#ffd8a8",
			"width": 208,
			"height": 170,
			"seed": 318594339,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "eU2e0gUt"
				}
			],
			"updated": 1692815577642,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 651,
			"versionNonce": 895905438,
			"isDeleted": false,
			"id": "eU2e0gUt",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1396.0954458574913,
			"y": -562.3725982324127,
			"strokeColor": "#f08c00",
			"backgroundColor": "transparent",
			"width": 88,
			"height": 50,
			"seed": 1648083139,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577642,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Cinematic\nTitle",
			"rawText": "Cinematic Title",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "fnI-R6UmaXkH1t5ZCGvBI",
			"originalText": "Cinematic Title",
			"lineHeight": 1.25,
			"baseline": 42
		},
		{
			"type": "rectangle",
			"version": 558,
			"versionNonce": 225694274,
			"isDeleted": false,
			"id": "X5CGBxh53j0De92UPrSUL",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1156.3824623644123,
			"y": -424.9267491488625,
			"strokeColor": "#f08c00",
			"backgroundColor": "#ffd8a8",
			"width": 227,
			"height": 168,
			"seed": 1241595043,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "Yo1XFulB"
				}
			],
			"updated": 1692815577642,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 274,
			"versionNonce": 303753950,
			"isDeleted": false,
			"id": "Yo1XFulB",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1091.3824623644123,
			"y": -353.4267491488625,
			"strokeColor": "#f08c00",
			"backgroundColor": "transparent",
			"width": 97,
			"height": 25,
			"seed": 1421256717,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577642,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Main Menu",
			"rawText": "Main Menu",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "X5CGBxh53j0De92UPrSUL",
			"originalText": "Main Menu",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 306,
			"versionNonce": 1636055554,
			"isDeleted": false,
			"id": "Z0vJrjprMLWGp6e5ZavrZ",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1595.2285147321566,
			"y": -162.5212437791232,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 1014.9448591489845,
			"height": 519.9559251517505,
			"seed": 1394836151,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577642,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 439,
			"versionNonce": 326491934,
			"isDeleted": false,
			"id": "n3FZ3cSvU3Md_-RmXigCs",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -857.8665839845478,
			"y": 10.063224281224677,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 207,
			"height": 59,
			"seed": 1475832535,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "FlNNEoYi"
				}
			],
			"updated": 1692815577642,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 390,
			"versionNonce": 1857137090,
			"isDeleted": false,
			"id": "FlNNEoYi",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -789.8665839845478,
			"y": 27.063224281224677,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 71,
			"height": 25,
			"seed": 1889988121,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577642,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "START",
			"rawText": "START",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "n3FZ3cSvU3Md_-RmXigCs",
			"originalText": "START",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 422,
			"versionNonce": 1307069278,
			"isDeleted": false,
			"id": "a96M2AzcPlNNkbqJGCl04",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -856.5483633258118,
			"y": 104.29055804365373,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 207,
			"height": 59,
			"seed": 1149009753,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "D2d1xSMr"
				}
			],
			"updated": 1692815577642,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 378,
			"versionNonce": 471540098,
			"isDeleted": false,
			"id": "D2d1xSMr",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -780.5483633258118,
			"y": 121.29055804365373,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 55,
			"height": 25,
			"seed": 1732586553,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577642,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "QUIT",
			"rawText": "QUIT",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "a96M2AzcPlNNkbqJGCl04",
			"originalText": "QUIT",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 187,
			"versionNonce": 532885406,
			"isDeleted": false,
			"id": "jqAvLTlE",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1560.3427881591394,
			"y": -213.34048757983078,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 402,
			"height": 25,
			"seed": 1478519129,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577642,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Cutscene to go to the Main Menu screen",
			"rawText": "Cutscene to go to the Main Menu screen",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Cutscene to go to the Main Menu screen",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "text",
			"version": 529,
			"versionNonce": 352297282,
			"isDeleted": false,
			"id": "XTNuy0YH",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1405.1110833351445,
			"y": 736.315501890764,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 256,
			"height": 450,
			"seed": 342644699,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577642,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "PLAYER\n-----------------------\n* movement\n    + run / infinite runner\n    + sprint\n    + crouch\n    + jump\n    + climb ledge\n    + climb ladder / net\n    + wall jump\n    + zipline top / bottom\n    + swim\n    + press trigger\n    + jetpack\n    - push / pull\n    - charge jump\n    - dash\n    - double jump",
			"rawText": "PLAYER\n-----------------------\n* movement\n    + run / infinite runner\n    + sprint\n    + crouch\n    + jump\n    + climb ledge\n    + climb ladder / net\n    + wall jump\n    + zipline top / bottom\n    + swim\n    + press trigger\n    + jetpack\n    - push / pull\n    - charge jump\n    - dash\n    - double jump",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "PLAYER\n-----------------------\n* movement\n    + run / infinite runner\n    + sprint\n    + crouch\n    + jump\n    + climb ledge\n    + climb ladder / net\n    + wall jump\n    + zipline top / bottom\n    + swim\n    + press trigger\n    + jetpack\n    - push / pull\n    - charge jump\n    - dash\n    - double jump",
			"lineHeight": 1.25,
			"baseline": 442
		},
		{
			"type": "text",
			"version": 423,
			"versionNonce": 1966574558,
			"isDeleted": false,
			"id": "1WhKaQif",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1112.0555277795886,
			"y": 772.1488352240974,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 227,
			"height": 350,
			"seed": 1173748155,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577642,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "LEVEL STRUCTURES\n----------------------------\n+ floor\n+ death zone\n+ ziplines top / bottom\n+ water\n+ push areas\n+ trigger areas\n+ moving platforms\n+ moving ladders\n+ rotating platforms\n+ path mover\n- elevator\n",
			"rawText": "LEVEL STRUCTURES\n----------------------------\n+ floor\n+ death zone\n+ ziplines top / bottom\n+ water\n+ push areas\n+ trigger areas\n+ moving platforms\n+ moving ladders\n+ rotating platforms\n+ path mover\n- elevator\n",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "LEVEL STRUCTURES\n----------------------------\n+ floor\n+ death zone\n+ ziplines top / bottom\n+ water\n+ push areas\n+ trigger areas\n+ moving platforms\n+ moving ladders\n+ rotating platforms\n+ path mover\n- elevator\n",
			"lineHeight": 1.25,
			"baseline": 342
		},
		{
			"type": "diamond",
			"version": 148,
			"versionNonce": 1153313026,
			"isDeleted": false,
			"id": "CnvPjcHIFqgD6HSdXdeMQ",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4.043228667797393,
			"y": 260.1362733312613,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 10.068348289245812,
			"height": 10.873816152385476,
			"seed": 1224120741,
			"groupIds": [
				"Hyshp04nNcsf4WTqKOUyX"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692815577642,
			"link": null,
			"locked": false
		},
		{
			"type": "diamond",
			"version": 159,
			"versionNonce": 206987294,
			"isDeleted": false,
			"id": "26hXkMi7m1tXnONopam6f",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 16.93071447803203,
			"y": 258.9280715365518,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 10.068348289245812,
			"height": 11.679284015525141,
			"seed": 424015531,
			"groupIds": [
				"Hyshp04nNcsf4WTqKOUyX"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692815577642,
			"link": null,
			"locked": false
		},
		{
			"type": "diamond",
			"version": 194,
			"versionNonce": 1389738178,
			"isDeleted": false,
			"id": "QhqxuzNruJ5aUn2j745BC",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 12.90337516233371,
			"y": 259.73353939969144,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 4.83280717883799,
			"height": 14.095687604944136,
			"seed": 1596969451,
			"groupIds": [
				"Hyshp04nNcsf4WTqKOUyX"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692815577642,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 729,
			"versionNonce": 957394014,
			"isDeleted": false,
			"id": "lXgzfUYUjIleNfYcb-R5a",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1306.2586660421487,
			"y": -1252.6556610585328,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 1263.0112473720012,
			"height": 498.32656465513617,
			"seed": 1106745477,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577642,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 300,
			"versionNonce": 518344834,
			"isDeleted": false,
			"id": "GyIFFF5J",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1261.917030662494,
			"y": -1236.8617342301218,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 103,
			"height": 25,
			"seed": 1975154341,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577642,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "CutScene 1",
			"rawText": "CutScene 1",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "CutScene 1",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 980,
			"versionNonce": 691499166,
			"isDeleted": false,
			"id": "-VcPgvEhQkkntfeiOgcEW",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1300.9788238768842,
			"y": -837.2743382340205,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 601.2245657418165,
			"height": 73.78925648971065,
			"seed": 172692491,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577642,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 960,
			"versionNonce": 1017901122,
			"isDeleted": false,
			"id": "1aOdrhSgI8Wj-9DubGtE9",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1294.6051327464493,
			"y": -1035.8506085554911,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 25.164756782125778,
			"height": 192.79242683341394,
			"seed": 692183627,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577642,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 1093,
			"versionNonce": 679193822,
			"isDeleted": false,
			"id": "Gz2VIclNX-Xt0Z1uGHyJe",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1268.2310975843616,
			"y": -908.6069018419712,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 118.84431563405535,
			"height": 14.211318627006436,
			"seed": 1585751307,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577642,
			"link": null,
			"locked": false
		},
		{
			"type": "ellipse",
			"version": 1512,
			"versionNonce": 1879611394,
			"isDeleted": false,
			"id": "lQ3zY2_5mp8K5GJ9-em-W",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1255.9314384958639,
			"y": -873.8433198345446,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 27.292840097560045,
			"height": 23.326046508023218,
			"seed": 1619515147,
			"groupIds": [
				"maMjK93mPtv7BG89btwtn"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"id": "njVB8vb_Y04G2rX8HNl4i",
					"type": "arrow"
				}
			],
			"updated": 1692815577642,
			"link": null,
			"locked": false
		},
		{
			"type": "freedraw",
			"version": 1294,
			"versionNonce": 1684955422,
			"isDeleted": false,
			"id": "GDWv0xSIasQ1JKFk_9aEZ",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1254.8974318071923,
			"y": -867.4802794113733,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 5.9641894286609345,
			"height": 9.759576433798838,
			"seed": 1194245547,
			"groupIds": [
				"maMjK93mPtv7BG89btwtn"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577642,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					-0.18073008808811764
				],
				[
					0,
					-0.36146017617623527
				],
				[
					-5.594217597396797e-17,
					-0.9036642292624609
				],
				[
					0.18073008808811777,
					-1.62659837043679
				],
				[
					0.18073008808811789,
					-2.710992687787354
				],
				[
					0.18073008808811766,
					-4.518321146312261
				],
				[
					0.18073008808811766,
					-5.964175639839061
				],
				[
					0,
					-7.048583746011483
				],
				[
					0,
					-7.771504098363969
				],
				[
					0,
					-8.675168327626416
				],
				[
					0,
					-8.855912204536391
				],
				[
					0,
					-9.217372380712627
				],
				[
					0,
					-9.398102468800744
				],
				[
					0,
					-9.578832556888862
				],
				[
					0,
					-9.759576433798838
				],
				[
					0.18073008808811766,
					-9.759576433798838
				],
				[
					0.5422040530862257,
					-9.759576433798838
				],
				[
					0.903664229262461,
					-9.578832556888862
				],
				[
					1.6265983704368043,
					-8.855912204536391
				],
				[
					1.807328458524922,
					-8.494438239538297
				],
				[
					2.1688024235230015,
					-7.952247975273944
				],
				[
					2.349532511611119,
					-7.410043922187718
				],
				[
					2.530262599699237,
					-7.048583746011483
				],
				[
					2.891722775875472,
					-6.68710978101339
				],
				[
					3.0724666527854625,
					-6.506379692925272
				],
				[
					3.2531967408735802,
					-6.325649604837155
				],
				[
					3.433926828961698,
					-5.964175639839061
				],
				[
					3.7953870051379335,
					-5.24125528748659
				],
				[
					3.976130882047895,
					-4.879781322488497
				],
				[
					4.518321146312248,
					-4.699051234400379
				],
				[
					5.241255287486591,
					-4.879781322488497
				],
				[
					5.9641894286609345,
					-5.421985375574708
				],
				[
					5.9641894286609345,
					-5.421985375574708
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.181640625,
				0.21484375,
				0.310546875,
				0.359375,
				0.40625,
				0.447265625,
				0.4853515625,
				0.49609375,
				0.501953125,
				0.51171875,
				0.5185546875,
				0.521484375,
				0.5263671875,
				0.53515625,
				0.5263671875,
				0.5263671875,
				0.53125,
				0.529296875,
				0.529296875,
				0.529296875,
				0.52734375,
				0.52734375,
				0.52734375,
				0.52734375,
				0.52734375,
				0.52734375,
				0.52734375,
				0.52734375,
				0.5302734375,
				0.537109375,
				0.529296875,
				0.4189453125,
				0.015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 1296,
			"versionNonce": 687491010,
			"isDeleted": false,
			"id": "hvqxj5a1z4zdp-DOjDIC1",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1235.7397529045925,
			"y": -871.6371265926872,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 5.42198537557468,
			"height": 9.578846345710721,
			"seed": 293589067,
			"groupIds": [
				"maMjK93mPtv7BG89btwtn"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577642,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					-0.361473964998108
				],
				[
					0.18074387690996163,
					-0.361473964998108
				],
				[
					0.542204053086197,
					-1.2651381942605546
				],
				[
					1.2651381942605402,
					-1.9880723354348837
				],
				[
					1.9880723354348546,
					-2.8917365646973305
				],
				[
					3.0724666527854336,
					-3.6146569170498157
				],
				[
					3.795400793959777,
					-4.337591058224144
				],
				[
					4.518321146312247,
					-5.241255287486591
				],
				[
					4.699065023222209,
					-5.602729252484685
				],
				[
					5.060525199398445,
					-5.7834593405728025
				],
				[
					5.241255287486562,
					-5.96418942866092
				],
				[
					5.42198537557468,
					-5.96418942866092
				],
				[
					5.42198537557468,
					-5.602729252484685
				],
				[
					5.42198537557468,
					-5.060525199398474
				],
				[
					5.42198537557468,
					-4.337591058224144
				],
				[
					5.42198537557468,
					-3.6146569170498157
				],
				[
					5.42198537557468,
					-2.7109926877873542
				],
				[
					5.241255287486562,
					-1.9880723354348837
				],
				[
					5.241255287486562,
					-1.2651381942605546
				],
				[
					5.241255287486562,
					-0.361473964998108
				],
				[
					5.060525199398445,
					0.3614601761762353
				],
				[
					4.879795111310327,
					1.0843943173505644
				],
				[
					4.699065023222209,
					1.8073284585248934
				],
				[
					4.699065023222209,
					1.9880585466130112
				],
				[
					4.699065023222209,
					2.1687886347011287
				],
				[
					4.699065023222209,
					2.530248810877364
				],
				[
					4.518321146312247,
					2.891722775875458
				],
				[
					4.518321146312247,
					3.253182952051693
				],
				[
					4.518321146312247,
					3.433913040139825
				],
				[
					4.699065023222209,
					3.614656917049801
				],
				[
					4.879795111310327,
					3.614656917049801
				],
				[
					5.241255287486562,
					3.614656917049801
				],
				[
					5.241255287486562,
					3.614656917049801
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.177734375,
				0.2587890625,
				0.28125,
				0.3544921875,
				0.388671875,
				0.408203125,
				0.4228515625,
				0.435546875,
				0.455078125,
				0.4658203125,
				0.4736328125,
				0.486328125,
				0.4951171875,
				0.5126953125,
				0.5126953125,
				0.5126953125,
				0.5126953125,
				0.5126953125,
				0.51171875,
				0.51171875,
				0.51171875,
				0.517578125,
				0.51953125,
				0.525390625,
				0.525390625,
				0.525390625,
				0.525390625,
				0.525390625,
				0.53125,
				0.515625,
				0.486328125,
				0.296875,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 1323,
			"versionNonce": 813731166,
			"isDeleted": false,
			"id": "z7FHJY7NGznvDnxpcLoUv",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1243.1835090332522,
			"y": -859.8860954724975,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 3.4174889321552437,
			"height": 1.8986049623084706,
			"seed": 559255275,
			"groupIds": [
				"maMjK93mPtv7BG89btwtn"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577642,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.07594303967584129,
					0
				],
				[
					-0.15189187343420177,
					-3.213996181392311e-17
				],
				[
					-0.22783491311002868,
					-0.15189187343419458
				],
				[
					-0.45566403213753826,
					-0.3037779527858557
				],
				[
					-0.7594419849233793,
					-0.5316128658958847
				],
				[
					-1.1391629773850764,
					-0.6834989452475524
				],
				[
					-1.3669978904951194,
					-0.9113338583575817
				],
				[
					-1.5948270095226005,
					-1.291054850819271
				],
				[
					-1.67077584328096,
					-1.442940930170939
				],
				[
					-1.7467188829568023,
					-1.5188839698467735
				],
				[
					-1.7467188829568023,
					-1.5948270095226076
				],
				[
					-1.6707758432809612,
					-1.5948270095226071
				],
				[
					-1.594827009522601,
					-1.5948270095226076
				],
				[
					-1.5188839698467735,
					-1.6707758432809676
				],
				[
					-1.2910548508192783,
					-1.6707758432809678
				],
				[
					-0.9872768980334226,
					-1.746718882956802
				],
				[
					-0.7594419849233792,
					-1.6707758432809678
				],
				[
					-0.45566403213753803,
					-1.594827009522608
				],
				[
					-0.15189187343420193,
					-1.5948270095226076
				],
				[
					0.07594303967584141,
					-1.5188839698467733
				],
				[
					0.3037779527858558,
					-1.5188839698467738
				],
				[
					0.455664032137524,
					-1.5188839698467733
				],
				[
					0.6834989452475527,
					-1.5948270095226071
				],
				[
					0.8353850245992208,
					-1.6707758432809678
				],
				[
					0.9113280642750619,
					-1.6707758432809685
				],
				[
					0.9872711039508891,
					-1.6707758432809678
				],
				[
					1.0632199377092497,
					-1.6707758432809683
				],
				[
					1.139162977385078,
					-1.6707758432809678
				],
				[
					1.2151060170609178,
					-1.7467188829568026
				],
				[
					1.2910490567367592,
					-1.8226619226326362
				],
				[
					1.3669920964125866,
					-1.8226619226326364
				],
				[
					1.4429409301709466,
					-1.8226619226326362
				],
				[
					1.5188839698467733,
					-1.8986049623084706
				],
				[
					1.5948270095226003,
					-1.8226619226326357
				],
				[
					1.6707700491984416,
					-1.8226619226326362
				],
				[
					1.5948270095226003,
					-1.7467188829568019
				],
				[
					1.518883969846774,
					-1.6707758432809678
				],
				[
					1.4429409301709466,
					-1.5948270095226076
				],
				[
					1.3669920964125866,
					-1.518883969846773
				],
				[
					1.291049056736759,
					-1.4429409301709397
				],
				[
					1.215106017060918,
					-1.2910548508192707
				],
				[
					1.0632199377092497,
					-1.1391629773850835
				],
				[
					0.9872711039508895,
					-0.9872768980334156
				],
				[
					0.9113280642750623,
					-0.911333858357581
				],
				[
					0.835385024599221,
					-0.8353850245992209
				],
				[
					0.7594419849233796,
					-0.7594419849233864
				],
				[
					0.6075501114891924,
					-0.6834989452475525
				],
				[
					0.5316070718133653,
					-0.6075559055717186
				],
				[
					0.4556640321375239,
					-0.5316128658958844
				],
				[
					0.3797209924616971,
					-0.4556640321375238
				],
				[
					0.30377795278585573,
					-0.37972099246168983
				],
				[
					0.2278291190274952,
					-0.3037779527858556
				],
				[
					0.22782911902749528,
					-0.22783491311002868
				],
				[
					0.1518860793516683,
					-0.15189187343419458
				],
				[
					0.15188607935166823,
					-0.0759430396758341
				],
				[
					0.2278291190274952,
					-0.0759430396758342
				],
				[
					0.37972099246169705,
					-0.15189187343419452
				],
				[
					0,
					0
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.171875,
				0.232421875,
				0.373046875,
				0.4453125,
				0.47265625,
				0.4912109375,
				0.5068359375,
				0.517578125,
				0.5234375,
				0.5234375,
				0.5234375,
				0.5234375,
				0.51953125,
				0.51953125,
				0.5166015625,
				0.5166015625,
				0.513671875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.513671875,
				0.51171875,
				0.51171875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.5166015625,
				0.513671875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.521484375,
				0.521484375,
				0.513671875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.4873046875,
				0.4306640625,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 1283,
			"versionNonce": 2141192066,
			"isDeleted": false,
			"id": "zs3jpu8sOKRx7UF3lVlpo",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1243.63917306539,
			"y": -859.2025965272497,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 0.2278291190275104,
			"height": 2.6580469472318646,
			"seed": 960133515,
			"groupIds": [
				"maMjK93mPtv7BG89btwtn"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577642,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-5.356660302320523e-18,
					0.07594303967583413
				],
				[
					0.07594303967584133,
					0.22782911902750236
				],
				[
					0.07594303967584129,
					0.6075501114891994
				],
				[
					0.07594303967584137,
					0.9113280642750622
				],
				[
					0.15188607935168275,
					1.1391629773850838
				],
				[
					0.15188607935168222,
					1.44293513608842
				],
				[
					0.15188607935168275,
					1.594827009522615
				],
				[
					0.15188607935168275,
					1.8226561285501173
				],
				[
					0.1518860793516829,
					2.050491041660139
				],
				[
					0.07594303967584172,
					2.050491041660139
				],
				[
					0.0759430396758412,
					2.126434081335973
				],
				[
					0.07594303967584137,
					2.278325954770168
				],
				[
					0,
					2.4302120341218356
				],
				[
					-1.0284787780455404e-15,
					2.5061550737976703
				],
				[
					-1.7141312967425674e-16,
					2.582098113473504
				],
				[
					0,
					2.6580469472318646
				],
				[
					0.15188607935168344,
					2.6580469472318646
				],
				[
					0.22782911902750938,
					2.582098113473504
				],
				[
					0.22782911902750938,
					2.582098113473504
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.1953125,
				0.30078125,
				0.3388671875,
				0.37109375,
				0.38671875,
				0.3994140625,
				0.4111328125,
				0.42578125,
				0.4345703125,
				0.4501953125,
				0.4560546875,
				0.4677734375,
				0.470703125,
				0.470703125,
				0.470703125,
				0.470703125,
				0.474609375,
				0.3720703125,
				0.275390625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 1316,
			"versionNonce": 1241723294,
			"isDeleted": false,
			"id": "XFYRbg2HRIZj18aXfhbgk",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1245.91749902016,
			"y": -856.9242705724797,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 6.227421958738777,
			"height": 1.8226619226326364,
			"seed": 1718161451,
			"groupIds": [
				"maMjK93mPtv7BG89btwtn"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577642,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					0.07594303967583413
				],
				[
					0.07594303967582697,
					0.15188607935166826
				],
				[
					0.22782911902750963,
					0.22782911902750236
				],
				[
					0.3037721587033365,
					0.379720992461697
				],
				[
					0.4556640321375239,
					0.5316070718133652
				],
				[
					0.6075501114891922,
					0.6834931511650263
				],
				[
					0.7594419849233937,
					0.7594419849233868
				],
				[
					0.911328064275048,
					0.8353850245992207
				],
				[
					0.9872711039508891,
					0.7594419849233868
				],
				[
					1.1391629773850909,
					0.7594419849233868
				],
				[
					1.2151060170609178,
					0.6834931511650261
				],
				[
					1.291049056736745,
					0.6075501114891922
				],
				[
					1.3669920964125721,
					0.45566403213753126
				],
				[
					1.4429351360884133,
					0.3037721587033365
				],
				[
					1.5948270095226154,
					0.07594303967583424
				],
				[
					1.7467130888742688,
					-0.07594883375836059
				],
				[
					1.82265612855011,
					-0.15189187343419439
				],
				[
					1.82265612855011,
					-0.22783491311002874
				],
				[
					1.8986049623084706,
					-0.3037779527858627
				],
				[
					1.8986049623084706,
					-0.37972099246168983
				],
				[
					1.9745480019843118,
					-0.37972099246168994
				],
				[
					1.9745480019843122,
					-0.45566982622005087
				],
				[
					2.1264340813359657,
					-0.45566982622005064
				],
				[
					2.202377121011793,
					-0.4556698262200503
				],
				[
					2.2783259547701533,
					-0.37972099246168994
				],
				[
					2.3542689944459947,
					-0.37972099246168983
				],
				[
					2.3542689944459947,
					-0.30377795278586267
				],
				[
					2.4302120341218356,
					-0.30377795278586284
				],
				[
					2.506155073797663,
					-0.30377795278586284
				],
				[
					2.506155073797663,
					-0.22783491311002874
				],
				[
					2.58209811347349,
					-0.15189187343419483
				],
				[
					2.58209811347349,
					-0.0759488337583607
				],
				[
					2.6580469472318504,
					0.15188607935166826
				],
				[
					2.7339899869076913,
					0.22782911902750236
				],
				[
					2.8858760662593594,
					0.379720992461697
				],
				[
					2.9618191059351866,
					0.5316070718133652
				],
				[
					3.037767939693547,
					0.6075501114891922
				],
				[
					3.1137109793693885,
					0.7594419849233865
				],
				[
					3.1896540190452156,
					0.8353850245992209
				],
				[
					3.3415400983968837,
					1.0632141436267233
				],
				[
					3.4174889321552437,
					1.1391629773850838
				],
				[
					3.5693750115069123,
					1.2151060170609176
				],
				[
					3.645318051182754,
					1.2151060170609178
				],
				[
					3.7972099246169413,
					1.291049056736752
				],
				[
					3.9490960039686094,
					1.291049056736752
				],
				[
					4.100982083320278,
					1.2151060170609178
				],
				[
					4.252873956754465,
					1.2151060170609178
				],
				[
					4.480703075781975,
					1.0632141436267233
				],
				[
					4.78448102856783,
					0.911328064275055
				],
				[
					5.012315941677859,
					0.6834931511650263
				],
				[
					5.240145060705355,
					0.5316070718133652
				],
				[
					5.467979973815383,
					0.3037721587033365
				],
				[
					5.695814886925412,
					0.07594303967583413
				],
				[
					5.923644005952907,
					-0.07594883375836048
				],
				[
					5.999587045628748,
					-0.1518918734341946
				],
				[
					6.075535879387094,
					-0.30377795278586284
				],
				[
					6.151478919062936,
					-0.37972099246168983
				],
				[
					6.227421958738777,
					-0.5316128658958844
				],
				[
					6.227421958738777,
					-0.5316128658958844
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.1865234375,
				0.2373046875,
				0.265625,
				0.294921875,
				0.326171875,
				0.3505859375,
				0.3662109375,
				0.373046875,
				0.3798828125,
				0.392578125,
				0.396484375,
				0.3984375,
				0.3984375,
				0.4013671875,
				0.408203125,
				0.41015625,
				0.41015625,
				0.41015625,
				0.41015625,
				0.412109375,
				0.4228515625,
				0.4140625,
				0.4072265625,
				0.4072265625,
				0.4111328125,
				0.4091796875,
				0.3955078125,
				0.3310546875,
				0.3837890625,
				0.384765625,
				0.3955078125,
				0.3974609375,
				0.3974609375,
				0.3974609375,
				0.3974609375,
				0.3974609375,
				0.3974609375,
				0.3974609375,
				0.3974609375,
				0.4013671875,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.40625,
				0.41015625,
				0.4150390625,
				0.423828125,
				0.427734375,
				0.427734375,
				0.4345703125,
				0.3779296875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 1294,
			"versionNonce": 809025346,
			"isDeleted": false,
			"id": "uyiOcuHme0J4AD_i6ha70",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1249.107158833288,
			"y": -867.4045722820555,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 5.39204272822206,
			"height": 3.6453180511827465,
			"seed": 718000843,
			"groupIds": [
				"maMjK93mPtv7BG89btwtn"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577642,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.15189187343420177,
					0.1518918734341945
				],
				[
					-0.45566403213753826,
					0.30377795278586284
				],
				[
					-0.9113338583575953,
					0.5316128658958917
				],
				[
					-1.518883969846773,
					1.2151060170609176
				],
				[
					-1.8226619226326433,
					1.7467188829568097
				],
				[
					-1.9745480019842971,
					2.2023829150943337
				],
				[
					-2.050496835742657,
					2.5061608678801965
				],
				[
					-2.0504968357426576,
					2.733989986907698
				],
				[
					-1.822661922632643,
					2.96182490001772
				],
				[
					-1.518883969846774,
					3.113710979369388
				],
				[
					-0.9872768980334224,
					3.1137109793693885
				],
				[
					-0.22783491311002887,
					2.9618249000177213
				],
				[
					0.3037779527858561,
					2.8099388206660523
				],
				[
					0.6834989452475531,
					2.58210390755603
				],
				[
					1.1391629773850762,
					2.354268994446002
				],
				[
					1.5188839698467738,
					2.050496835742665
				],
				[
					2.1264340813359652,
					1.7467188829568099
				],
				[
					2.88587606625936,
					1.139162977385084
				],
				[
					3.1137109793693876,
					0.7594419849233941
				],
				[
					3.2655970587210423,
					0.5316128658958917
				],
				[
					3.3415458924794024,
					0.3037779527858632
				],
				[
					3.2655970587210423,
					0.15189187343419447
				],
				[
					3.189654019045215,
					0
				],
				[
					2.809933026583518,
					-0.1518860793516612
				],
				[
					2.430212034121821,
					-0.303777952785856
				],
				[
					1.8986049623084706,
					-0.4556640321375241
				],
				[
					1.0632199377092495,
					-0.5316070718133581
				],
				[
					0.9113280642750622,
					-0.4556640321375239
				],
				[
					0.6075501114891921,
					-0.3797209924616898
				],
				[
					0.5316070718133652,
					-0.3797209924616899
				],
				[
					0.3037779527858557,
					-0.30377795278585573
				],
				[
					0.3037779527858556,
					-0.22782911902749525
				],
				[
					0.3797209924616826,
					-0.2278291190274952
				],
				[
					0,
					0
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.171875,
				0.201171875,
				0.2529296875,
				0.3037109375,
				0.361328125,
				0.38671875,
				0.4130859375,
				0.423828125,
				0.42578125,
				0.42578125,
				0.419921875,
				0.4150390625,
				0.4033203125,
				0.400390625,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.408203125,
				0.4306640625,
				0.45703125,
				0.47265625,
				0.4775390625,
				0.482421875,
				0.4951171875,
				0.4970703125,
				0.4970703125,
				0.4970703125,
				0.466796875,
				0.4140625,
				0.0263671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 1294,
			"versionNonce": 472337886,
			"isDeleted": false,
			"id": "RT4uoqBZD_0cdrcZC733d",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1237.943363972547,
			"y": -868.1640142669788,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 4.556651909540335,
			"height": 3.4174889321552446,
			"seed": 1727873387,
			"groupIds": [
				"maMjK93mPtv7BG89btwtn"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577642,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.15188607935165394,
					-0.07594303967583418
				],
				[
					-0.6075501114892065,
					-0.07594303967583416
				],
				[
					-0.9872711039508748,
					-8.570656483712831e-17
				],
				[
					-1.3669920964125717,
					0.22783491311002857
				],
				[
					-1.746713088874269,
					0.5316128658958919
				],
				[
					-2.202382915094326,
					1.0632199377092497
				],
				[
					-2.3542689944460085,
					1.5188839698467806
				],
				[
					-2.278325954770153,
					1.9745480019843047
				],
				[
					-2.0504910416601385,
					2.354268994446002
				],
				[
					-1.7467130888742697,
					2.658046947231858
				],
				[
					-1.1391629773850909,
					2.8858818603418865
				],
				[
					-0.7594419849233935,
					2.961824900017721
				],
				[
					-0.30377795278586966,
					2.885881860341886
				],
				[
					0.07594303967582673,
					2.7339899869076913
				],
				[
					0.8353850245992208,
					2.354268994446002
				],
				[
					1.4429409301709326,
					1.9745480019843042
				],
				[
					1.8226619226326288,
					1.6707758432809685
				],
				[
					2.0504968357426727,
					1.3669978904951126
				],
				[
					2.202382915094326,
					1.0632199377092504
				],
				[
					2.202382915094326,
					0.7594419849233874
				],
				[
					2.202382915094326,
					0.5316128658958911
				],
				[
					2.126439875418499,
					0.30377795278586267
				],
				[
					1.9745480019843116,
					0
				],
				[
					1.6707758432809752,
					-0.15188607935166806
				],
				[
					0.9113338583575813,
					-0.3797209924616896
				],
				[
					0.30377795278586994,
					-0.455664032137524
				],
				[
					-0.07594303967582688,
					-0.455664032137524
				],
				[
					-0.45566403213752393,
					-0.30377795278586284
				],
				[
					-0.7594419849233939,
					-0.15188607935166815
				],
				[
					-0.9872711039508748,
					-8.570656483712831e-17
				],
				[
					-0.9872711039508749,
					0.15189187343419472
				],
				[
					-0.9872711039508749,
					0.3797209924616973
				],
				[
					0,
					0
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.173828125,
				0.1923828125,
				0.294921875,
				0.3798828125,
				0.447265625,
				0.4873046875,
				0.4912109375,
				0.486328125,
				0.484375,
				0.482421875,
				0.48046875,
				0.4697265625,
				0.4658203125,
				0.470703125,
				0.4677734375,
				0.474609375,
				0.4765625,
				0.4765625,
				0.478515625,
				0.48046875,
				0.4921875,
				0.4951171875,
				0.5,
				0.5126953125,
				0.521484375,
				0.5234375,
				0.525390625,
				0.525390625,
				0.525390625,
				0.505859375,
				0.423828125,
				0.1904296875,
				0.01171875,
				0
			]
		},
		{
			"type": "diamond",
			"version": 416,
			"versionNonce": 388204290,
			"isDeleted": false,
			"id": "JID83xs5pcBmoHyj5uRNP",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1152.3865416318836,
			"y": -929.6629882971663,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 10.068348289245812,
			"height": 10.873816152385476,
			"seed": 71818251,
			"groupIds": [
				"TEvjYfTOb-sk9NXxFOnU0"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692815577642,
			"link": null,
			"locked": false
		},
		{
			"type": "diamond",
			"version": 427,
			"versionNonce": 66970142,
			"isDeleted": false,
			"id": "FluPkzQl_9ueLD_U9qw4Y",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1139.4990558216489,
			"y": -930.8711900918759,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 10.068348289245812,
			"height": 11.679284015525141,
			"seed": 1587946155,
			"groupIds": [
				"TEvjYfTOb-sk9NXxFOnU0"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692815577642,
			"link": null,
			"locked": false
		},
		{
			"type": "diamond",
			"version": 463,
			"versionNonce": 752834242,
			"isDeleted": false,
			"id": "XKGvsgISRF-CNbcjkXlXg",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1143.5263951373472,
			"y": -930.0657222287361,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 4.83280717883799,
			"height": 14.095687604944136,
			"seed": 1858245963,
			"groupIds": [
				"TEvjYfTOb-sk9NXxFOnU0"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"id": "uFnPsIf6BjVAUXvHQSSDy",
					"type": "arrow"
				}
			],
			"updated": 1692815577642,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 1382,
			"versionNonce": 343404126,
			"isDeleted": false,
			"id": "aJxdpPVora44uGTCBYN5q",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -670.7432841949517,
			"y": -1227.6739222421577,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 3.6755016503132074,
			"height": 464.14185022568955,
			"seed": 1806171563,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577642,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 1141,
			"versionNonce": 34287234,
			"isDeleted": false,
			"id": "X3ci-KDQYhEwuV4BCuFP0",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -954.6495030802416,
			"y": -979.7421946215725,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 118.84431563405535,
			"height": 25.11856861489944,
			"seed": 1802866565,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577642,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 1266,
			"versionNonce": 1516663454,
			"isDeleted": false,
			"id": "qkzOHhyxJ7UgJ_cNdl0Wv",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -828.610169886812,
			"y": -1130.6258194540917,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 118.84431563405535,
			"height": 279.62106833240153,
			"seed": 342446885,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577642,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 414,
			"versionNonce": 996544066,
			"isDeleted": false,
			"id": "zQLFDFiWv1H52GoRrO0VT",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -939.3148674360857,
			"y": -927.5195567787923,
			"strokeColor": "#2f9e44",
			"backgroundColor": "#b2f2bb",
			"width": 39.6983777328835,
			"height": 70.95095942919585,
			"seed": 1351694603,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577642,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 1176,
			"versionNonce": 544894686,
			"isDeleted": false,
			"id": "oIKqW6_1Oq8TP9NNoSPHA",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1164.3674062711398,
			"y": -898.3203935553015,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 11.310163539294983,
			"height": 53.46981859810939,
			"seed": 1699144331,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"id": "uFnPsIf6BjVAUXvHQSSDy",
					"type": "arrow"
				}
			],
			"updated": 1692815577642,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 1038,
			"versionNonce": 231667202,
			"isDeleted": false,
			"id": "uwU8icvPdXGY6KWx-T9W0",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -648.8964869792082,
			"y": -845.2432001005836,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 601.2245657418165,
			"height": 73.78925648971065,
			"seed": 259141061,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577642,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 1018,
			"versionNonce": 860152606,
			"isDeleted": false,
			"id": "MB8vPxsot-RGOfkLITIk7",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -642.5227958487733,
			"y": -1043.8194704220546,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 25.164756782125778,
			"height": 192.79242683341394,
			"seed": 2060594469,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577642,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 1151,
			"versionNonce": 977593794,
			"isDeleted": false,
			"id": "eOmda7Yb2sJE335VAnv_Y",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -616.1487606866851,
			"y": -916.5757637085344,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 118.84431563405535,
			"height": 14.211318627006436,
			"seed": 750469253,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577642,
			"link": null,
			"locked": false
		},
		{
			"type": "ellipse",
			"version": 1612,
			"versionNonce": 624349022,
			"isDeleted": false,
			"id": "FI5xlLNLEp2a5YKorqvQ-",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -537.03626411242,
			"y": -947.7792870668022,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 27.292840097560045,
			"height": 23.326046508023218,
			"seed": 451602405,
			"groupIds": [
				"Oi-XvYPBwhfoeNH4S6ez3"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"id": "jLNjsLyXZVqcAweKXlE6Q",
					"type": "arrow"
				}
			],
			"updated": 1692815577642,
			"link": null,
			"locked": false
		},
		{
			"type": "freedraw",
			"version": 1394,
			"versionNonce": 166124930,
			"isDeleted": false,
			"id": "QjdmCZ9xtMKaLatkIONKT",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -536.0022574237489,
			"y": -941.416246643631,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 5.9641894286609345,
			"height": 9.759576433798838,
			"seed": 661562181,
			"groupIds": [
				"Oi-XvYPBwhfoeNH4S6ez3"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577642,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					-0.18073008808811764
				],
				[
					0,
					-0.36146017617623527
				],
				[
					-5.594217597396797e-17,
					-0.9036642292624609
				],
				[
					0.18073008808811777,
					-1.62659837043679
				],
				[
					0.18073008808811789,
					-2.710992687787354
				],
				[
					0.18073008808811766,
					-4.518321146312261
				],
				[
					0.18073008808811766,
					-5.964175639839061
				],
				[
					0,
					-7.048583746011483
				],
				[
					0,
					-7.771504098363969
				],
				[
					0,
					-8.675168327626416
				],
				[
					0,
					-8.855912204536391
				],
				[
					0,
					-9.217372380712627
				],
				[
					0,
					-9.398102468800744
				],
				[
					0,
					-9.578832556888862
				],
				[
					0,
					-9.759576433798838
				],
				[
					0.18073008808811766,
					-9.759576433798838
				],
				[
					0.5422040530862257,
					-9.759576433798838
				],
				[
					0.903664229262461,
					-9.578832556888862
				],
				[
					1.6265983704368043,
					-8.855912204536391
				],
				[
					1.807328458524922,
					-8.494438239538297
				],
				[
					2.1688024235230015,
					-7.952247975273944
				],
				[
					2.349532511611119,
					-7.410043922187718
				],
				[
					2.530262599699237,
					-7.048583746011483
				],
				[
					2.891722775875472,
					-6.68710978101339
				],
				[
					3.0724666527854625,
					-6.506379692925272
				],
				[
					3.2531967408735802,
					-6.325649604837155
				],
				[
					3.433926828961698,
					-5.964175639839061
				],
				[
					3.7953870051379335,
					-5.24125528748659
				],
				[
					3.976130882047895,
					-4.879781322488497
				],
				[
					4.518321146312248,
					-4.699051234400379
				],
				[
					5.241255287486591,
					-4.879781322488497
				],
				[
					5.9641894286609345,
					-5.421985375574708
				],
				[
					5.9641894286609345,
					-5.421985375574708
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.181640625,
				0.21484375,
				0.310546875,
				0.359375,
				0.40625,
				0.447265625,
				0.4853515625,
				0.49609375,
				0.501953125,
				0.51171875,
				0.5185546875,
				0.521484375,
				0.5263671875,
				0.53515625,
				0.5263671875,
				0.5263671875,
				0.53125,
				0.529296875,
				0.529296875,
				0.529296875,
				0.52734375,
				0.52734375,
				0.52734375,
				0.52734375,
				0.52734375,
				0.52734375,
				0.52734375,
				0.52734375,
				0.5302734375,
				0.537109375,
				0.529296875,
				0.4189453125,
				0.015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 1396,
			"versionNonce": 312554398,
			"isDeleted": false,
			"id": "KrQG0McLYGFbfvXPazT4n",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -516.8445785211486,
			"y": -945.5730938249449,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 5.42198537557468,
			"height": 9.578846345710721,
			"seed": 379843237,
			"groupIds": [
				"Oi-XvYPBwhfoeNH4S6ez3"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577642,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					-0.361473964998108
				],
				[
					0.18074387690996163,
					-0.361473964998108
				],
				[
					0.542204053086197,
					-1.2651381942605546
				],
				[
					1.2651381942605402,
					-1.9880723354348837
				],
				[
					1.9880723354348546,
					-2.8917365646973305
				],
				[
					3.0724666527854336,
					-3.6146569170498157
				],
				[
					3.795400793959777,
					-4.337591058224144
				],
				[
					4.518321146312247,
					-5.241255287486591
				],
				[
					4.699065023222209,
					-5.602729252484685
				],
				[
					5.060525199398445,
					-5.7834593405728025
				],
				[
					5.241255287486562,
					-5.96418942866092
				],
				[
					5.42198537557468,
					-5.96418942866092
				],
				[
					5.42198537557468,
					-5.602729252484685
				],
				[
					5.42198537557468,
					-5.060525199398474
				],
				[
					5.42198537557468,
					-4.337591058224144
				],
				[
					5.42198537557468,
					-3.6146569170498157
				],
				[
					5.42198537557468,
					-2.7109926877873542
				],
				[
					5.241255287486562,
					-1.9880723354348837
				],
				[
					5.241255287486562,
					-1.2651381942605546
				],
				[
					5.241255287486562,
					-0.361473964998108
				],
				[
					5.060525199398445,
					0.3614601761762353
				],
				[
					4.879795111310327,
					1.0843943173505644
				],
				[
					4.699065023222209,
					1.8073284585248934
				],
				[
					4.699065023222209,
					1.9880585466130112
				],
				[
					4.699065023222209,
					2.1687886347011287
				],
				[
					4.699065023222209,
					2.530248810877364
				],
				[
					4.518321146312247,
					2.891722775875458
				],
				[
					4.518321146312247,
					3.253182952051693
				],
				[
					4.518321146312247,
					3.433913040139825
				],
				[
					4.699065023222209,
					3.614656917049801
				],
				[
					4.879795111310327,
					3.614656917049801
				],
				[
					5.241255287486562,
					3.614656917049801
				],
				[
					5.241255287486562,
					3.614656917049801
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.177734375,
				0.2587890625,
				0.28125,
				0.3544921875,
				0.388671875,
				0.408203125,
				0.4228515625,
				0.435546875,
				0.455078125,
				0.4658203125,
				0.4736328125,
				0.486328125,
				0.4951171875,
				0.5126953125,
				0.5126953125,
				0.5126953125,
				0.5126953125,
				0.5126953125,
				0.51171875,
				0.51171875,
				0.51171875,
				0.517578125,
				0.51953125,
				0.525390625,
				0.525390625,
				0.525390625,
				0.525390625,
				0.525390625,
				0.53125,
				0.515625,
				0.486328125,
				0.296875,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 1423,
			"versionNonce": 1240718658,
			"isDeleted": false,
			"id": "7tjd_fIrc4OnXbITA0bbb",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -524.2883346498086,
			"y": -933.8220627047549,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 3.4174889321552437,
			"height": 1.8986049623084706,
			"seed": 1161319941,
			"groupIds": [
				"Oi-XvYPBwhfoeNH4S6ez3"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577642,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.07594303967584129,
					0
				],
				[
					-0.15189187343420177,
					-3.213996181392311e-17
				],
				[
					-0.22783491311002868,
					-0.15189187343419458
				],
				[
					-0.45566403213753826,
					-0.3037779527858557
				],
				[
					-0.7594419849233793,
					-0.5316128658958847
				],
				[
					-1.1391629773850764,
					-0.6834989452475524
				],
				[
					-1.3669978904951194,
					-0.9113338583575817
				],
				[
					-1.5948270095226005,
					-1.291054850819271
				],
				[
					-1.67077584328096,
					-1.442940930170939
				],
				[
					-1.7467188829568023,
					-1.5188839698467735
				],
				[
					-1.7467188829568023,
					-1.5948270095226076
				],
				[
					-1.6707758432809612,
					-1.5948270095226071
				],
				[
					-1.594827009522601,
					-1.5948270095226076
				],
				[
					-1.5188839698467735,
					-1.6707758432809676
				],
				[
					-1.2910548508192783,
					-1.6707758432809678
				],
				[
					-0.9872768980334226,
					-1.746718882956802
				],
				[
					-0.7594419849233792,
					-1.6707758432809678
				],
				[
					-0.45566403213753803,
					-1.594827009522608
				],
				[
					-0.15189187343420193,
					-1.5948270095226076
				],
				[
					0.07594303967584141,
					-1.5188839698467733
				],
				[
					0.3037779527858558,
					-1.5188839698467738
				],
				[
					0.455664032137524,
					-1.5188839698467733
				],
				[
					0.6834989452475527,
					-1.5948270095226071
				],
				[
					0.8353850245992208,
					-1.6707758432809678
				],
				[
					0.9113280642750619,
					-1.6707758432809685
				],
				[
					0.9872711039508891,
					-1.6707758432809678
				],
				[
					1.0632199377092497,
					-1.6707758432809683
				],
				[
					1.139162977385078,
					-1.6707758432809678
				],
				[
					1.2151060170609178,
					-1.7467188829568026
				],
				[
					1.2910490567367592,
					-1.8226619226326362
				],
				[
					1.3669920964125866,
					-1.8226619226326364
				],
				[
					1.4429409301709466,
					-1.8226619226326362
				],
				[
					1.5188839698467733,
					-1.8986049623084706
				],
				[
					1.5948270095226003,
					-1.8226619226326357
				],
				[
					1.6707700491984416,
					-1.8226619226326362
				],
				[
					1.5948270095226003,
					-1.7467188829568019
				],
				[
					1.518883969846774,
					-1.6707758432809678
				],
				[
					1.4429409301709466,
					-1.5948270095226076
				],
				[
					1.3669920964125866,
					-1.518883969846773
				],
				[
					1.291049056736759,
					-1.4429409301709397
				],
				[
					1.215106017060918,
					-1.2910548508192707
				],
				[
					1.0632199377092497,
					-1.1391629773850835
				],
				[
					0.9872711039508895,
					-0.9872768980334156
				],
				[
					0.9113280642750623,
					-0.911333858357581
				],
				[
					0.835385024599221,
					-0.8353850245992209
				],
				[
					0.7594419849233796,
					-0.7594419849233864
				],
				[
					0.6075501114891924,
					-0.6834989452475525
				],
				[
					0.5316070718133653,
					-0.6075559055717186
				],
				[
					0.4556640321375239,
					-0.5316128658958844
				],
				[
					0.3797209924616971,
					-0.4556640321375238
				],
				[
					0.30377795278585573,
					-0.37972099246168983
				],
				[
					0.2278291190274952,
					-0.3037779527858556
				],
				[
					0.22782911902749528,
					-0.22783491311002868
				],
				[
					0.1518860793516683,
					-0.15189187343419458
				],
				[
					0.15188607935166823,
					-0.0759430396758341
				],
				[
					0.2278291190274952,
					-0.0759430396758342
				],
				[
					0.37972099246169705,
					-0.15189187343419452
				],
				[
					0,
					0
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.171875,
				0.232421875,
				0.373046875,
				0.4453125,
				0.47265625,
				0.4912109375,
				0.5068359375,
				0.517578125,
				0.5234375,
				0.5234375,
				0.5234375,
				0.5234375,
				0.51953125,
				0.51953125,
				0.5166015625,
				0.5166015625,
				0.513671875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.513671875,
				0.51171875,
				0.51171875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.5166015625,
				0.513671875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.521484375,
				0.521484375,
				0.513671875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.4873046875,
				0.4306640625,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 1383,
			"versionNonce": 1706364894,
			"isDeleted": false,
			"id": "YzXoGVqYSEfegbFH2REJb",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -524.7439986819461,
			"y": -933.1385637595072,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 0.2278291190275104,
			"height": 2.6580469472318646,
			"seed": 506023269,
			"groupIds": [
				"Oi-XvYPBwhfoeNH4S6ez3"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577642,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-5.356660302320523e-18,
					0.07594303967583413
				],
				[
					0.07594303967584133,
					0.22782911902750236
				],
				[
					0.07594303967584129,
					0.6075501114891994
				],
				[
					0.07594303967584137,
					0.9113280642750622
				],
				[
					0.15188607935168275,
					1.1391629773850838
				],
				[
					0.15188607935168222,
					1.44293513608842
				],
				[
					0.15188607935168275,
					1.594827009522615
				],
				[
					0.15188607935168275,
					1.8226561285501173
				],
				[
					0.1518860793516829,
					2.050491041660139
				],
				[
					0.07594303967584172,
					2.050491041660139
				],
				[
					0.0759430396758412,
					2.126434081335973
				],
				[
					0.07594303967584137,
					2.278325954770168
				],
				[
					0,
					2.4302120341218356
				],
				[
					-1.0284787780455404e-15,
					2.5061550737976703
				],
				[
					-1.7141312967425674e-16,
					2.582098113473504
				],
				[
					0,
					2.6580469472318646
				],
				[
					0.15188607935168344,
					2.6580469472318646
				],
				[
					0.22782911902750938,
					2.582098113473504
				],
				[
					0.22782911902750938,
					2.582098113473504
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.1953125,
				0.30078125,
				0.3388671875,
				0.37109375,
				0.38671875,
				0.3994140625,
				0.4111328125,
				0.42578125,
				0.4345703125,
				0.4501953125,
				0.4560546875,
				0.4677734375,
				0.470703125,
				0.470703125,
				0.470703125,
				0.470703125,
				0.474609375,
				0.3720703125,
				0.275390625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 1416,
			"versionNonce": 1204479234,
			"isDeleted": false,
			"id": "5Dc9bCCExxwZp1ALUKcnN",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -527.0223246367166,
			"y": -930.8602378047372,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 6.227421958738777,
			"height": 1.8226619226326364,
			"seed": 1355045061,
			"groupIds": [
				"Oi-XvYPBwhfoeNH4S6ez3"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577642,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					0.07594303967583413
				],
				[
					0.07594303967582697,
					0.15188607935166826
				],
				[
					0.22782911902750963,
					0.22782911902750236
				],
				[
					0.3037721587033365,
					0.379720992461697
				],
				[
					0.4556640321375239,
					0.5316070718133652
				],
				[
					0.6075501114891922,
					0.6834931511650263
				],
				[
					0.7594419849233937,
					0.7594419849233868
				],
				[
					0.911328064275048,
					0.8353850245992207
				],
				[
					0.9872711039508891,
					0.7594419849233868
				],
				[
					1.1391629773850909,
					0.7594419849233868
				],
				[
					1.2151060170609178,
					0.6834931511650261
				],
				[
					1.291049056736745,
					0.6075501114891922
				],
				[
					1.3669920964125721,
					0.45566403213753126
				],
				[
					1.4429351360884133,
					0.3037721587033365
				],
				[
					1.5948270095226154,
					0.07594303967583424
				],
				[
					1.7467130888742688,
					-0.07594883375836059
				],
				[
					1.82265612855011,
					-0.15189187343419439
				],
				[
					1.82265612855011,
					-0.22783491311002874
				],
				[
					1.8986049623084706,
					-0.3037779527858627
				],
				[
					1.8986049623084706,
					-0.37972099246168983
				],
				[
					1.9745480019843118,
					-0.37972099246168994
				],
				[
					1.9745480019843122,
					-0.45566982622005087
				],
				[
					2.1264340813359657,
					-0.45566982622005064
				],
				[
					2.202377121011793,
					-0.4556698262200503
				],
				[
					2.2783259547701533,
					-0.37972099246168994
				],
				[
					2.3542689944459947,
					-0.37972099246168983
				],
				[
					2.3542689944459947,
					-0.30377795278586267
				],
				[
					2.4302120341218356,
					-0.30377795278586284
				],
				[
					2.506155073797663,
					-0.30377795278586284
				],
				[
					2.506155073797663,
					-0.22783491311002874
				],
				[
					2.58209811347349,
					-0.15189187343419483
				],
				[
					2.58209811347349,
					-0.0759488337583607
				],
				[
					2.6580469472318504,
					0.15188607935166826
				],
				[
					2.7339899869076913,
					0.22782911902750236
				],
				[
					2.8858760662593594,
					0.379720992461697
				],
				[
					2.9618191059351866,
					0.5316070718133652
				],
				[
					3.037767939693547,
					0.6075501114891922
				],
				[
					3.1137109793693885,
					0.7594419849233865
				],
				[
					3.1896540190452156,
					0.8353850245992209
				],
				[
					3.3415400983968837,
					1.0632141436267233
				],
				[
					3.4174889321552437,
					1.1391629773850838
				],
				[
					3.5693750115069123,
					1.2151060170609176
				],
				[
					3.645318051182754,
					1.2151060170609178
				],
				[
					3.7972099246169413,
					1.291049056736752
				],
				[
					3.9490960039686094,
					1.291049056736752
				],
				[
					4.100982083320278,
					1.2151060170609178
				],
				[
					4.252873956754465,
					1.2151060170609178
				],
				[
					4.480703075781975,
					1.0632141436267233
				],
				[
					4.78448102856783,
					0.911328064275055
				],
				[
					5.012315941677859,
					0.6834931511650263
				],
				[
					5.240145060705355,
					0.5316070718133652
				],
				[
					5.467979973815383,
					0.3037721587033365
				],
				[
					5.695814886925412,
					0.07594303967583413
				],
				[
					5.923644005952907,
					-0.07594883375836048
				],
				[
					5.999587045628748,
					-0.1518918734341946
				],
				[
					6.075535879387094,
					-0.30377795278586284
				],
				[
					6.151478919062936,
					-0.37972099246168983
				],
				[
					6.227421958738777,
					-0.5316128658958844
				],
				[
					6.227421958738777,
					-0.5316128658958844
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.1865234375,
				0.2373046875,
				0.265625,
				0.294921875,
				0.326171875,
				0.3505859375,
				0.3662109375,
				0.373046875,
				0.3798828125,
				0.392578125,
				0.396484375,
				0.3984375,
				0.3984375,
				0.4013671875,
				0.408203125,
				0.41015625,
				0.41015625,
				0.41015625,
				0.41015625,
				0.412109375,
				0.4228515625,
				0.4140625,
				0.4072265625,
				0.4072265625,
				0.4111328125,
				0.4091796875,
				0.3955078125,
				0.3310546875,
				0.3837890625,
				0.384765625,
				0.3955078125,
				0.3974609375,
				0.3974609375,
				0.3974609375,
				0.3974609375,
				0.3974609375,
				0.3974609375,
				0.3974609375,
				0.3974609375,
				0.4013671875,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.40625,
				0.41015625,
				0.4150390625,
				0.423828125,
				0.427734375,
				0.427734375,
				0.4345703125,
				0.3779296875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 1394,
			"versionNonce": 444818462,
			"isDeleted": false,
			"id": "hMMpBTqWJD4j6qo-lzikv",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -530.2119844498445,
			"y": -941.3405395143131,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 5.39204272822206,
			"height": 3.6453180511827465,
			"seed": 1185347621,
			"groupIds": [
				"Oi-XvYPBwhfoeNH4S6ez3"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577642,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.15189187343420177,
					0.1518918734341945
				],
				[
					-0.45566403213753826,
					0.30377795278586284
				],
				[
					-0.9113338583575953,
					0.5316128658958917
				],
				[
					-1.518883969846773,
					1.2151060170609176
				],
				[
					-1.8226619226326433,
					1.7467188829568097
				],
				[
					-1.9745480019842971,
					2.2023829150943337
				],
				[
					-2.050496835742657,
					2.5061608678801965
				],
				[
					-2.0504968357426576,
					2.733989986907698
				],
				[
					-1.822661922632643,
					2.96182490001772
				],
				[
					-1.518883969846774,
					3.113710979369388
				],
				[
					-0.9872768980334224,
					3.1137109793693885
				],
				[
					-0.22783491311002887,
					2.9618249000177213
				],
				[
					0.3037779527858561,
					2.8099388206660523
				],
				[
					0.6834989452475531,
					2.58210390755603
				],
				[
					1.1391629773850762,
					2.354268994446002
				],
				[
					1.5188839698467738,
					2.050496835742665
				],
				[
					2.1264340813359652,
					1.7467188829568099
				],
				[
					2.88587606625936,
					1.139162977385084
				],
				[
					3.1137109793693876,
					0.7594419849233941
				],
				[
					3.2655970587210423,
					0.5316128658958917
				],
				[
					3.3415458924794024,
					0.3037779527858632
				],
				[
					3.2655970587210423,
					0.15189187343419447
				],
				[
					3.189654019045215,
					0
				],
				[
					2.809933026583518,
					-0.1518860793516612
				],
				[
					2.430212034121821,
					-0.303777952785856
				],
				[
					1.8986049623084706,
					-0.4556640321375241
				],
				[
					1.0632199377092495,
					-0.5316070718133581
				],
				[
					0.9113280642750622,
					-0.4556640321375239
				],
				[
					0.6075501114891921,
					-0.3797209924616898
				],
				[
					0.5316070718133652,
					-0.3797209924616899
				],
				[
					0.3037779527858557,
					-0.30377795278585573
				],
				[
					0.3037779527858556,
					-0.22782911902749525
				],
				[
					0.3797209924616826,
					-0.2278291190274952
				],
				[
					0,
					0
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.171875,
				0.201171875,
				0.2529296875,
				0.3037109375,
				0.361328125,
				0.38671875,
				0.4130859375,
				0.423828125,
				0.42578125,
				0.42578125,
				0.419921875,
				0.4150390625,
				0.4033203125,
				0.400390625,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.408203125,
				0.4306640625,
				0.45703125,
				0.47265625,
				0.4775390625,
				0.482421875,
				0.4951171875,
				0.4970703125,
				0.4970703125,
				0.4970703125,
				0.466796875,
				0.4140625,
				0.0263671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 1394,
			"versionNonce": 1290466498,
			"isDeleted": false,
			"id": "bI33XyYV5hrbcLolbgdfT",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -519.0481895891032,
			"y": -942.0999814992365,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 4.556651909540335,
			"height": 3.4174889321552446,
			"seed": 1505667973,
			"groupIds": [
				"Oi-XvYPBwhfoeNH4S6ez3"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577642,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.15188607935165394,
					-0.07594303967583418
				],
				[
					-0.6075501114892065,
					-0.07594303967583416
				],
				[
					-0.9872711039508748,
					-8.570656483712831e-17
				],
				[
					-1.3669920964125717,
					0.22783491311002857
				],
				[
					-1.746713088874269,
					0.5316128658958919
				],
				[
					-2.202382915094326,
					1.0632199377092497
				],
				[
					-2.3542689944460085,
					1.5188839698467806
				],
				[
					-2.278325954770153,
					1.9745480019843047
				],
				[
					-2.0504910416601385,
					2.354268994446002
				],
				[
					-1.7467130888742697,
					2.658046947231858
				],
				[
					-1.1391629773850909,
					2.8858818603418865
				],
				[
					-0.7594419849233935,
					2.961824900017721
				],
				[
					-0.30377795278586966,
					2.885881860341886
				],
				[
					0.07594303967582673,
					2.7339899869076913
				],
				[
					0.8353850245992208,
					2.354268994446002
				],
				[
					1.4429409301709326,
					1.9745480019843042
				],
				[
					1.8226619226326288,
					1.6707758432809685
				],
				[
					2.0504968357426727,
					1.3669978904951126
				],
				[
					2.202382915094326,
					1.0632199377092504
				],
				[
					2.202382915094326,
					0.7594419849233874
				],
				[
					2.202382915094326,
					0.5316128658958911
				],
				[
					2.126439875418499,
					0.30377795278586267
				],
				[
					1.9745480019843116,
					0
				],
				[
					1.6707758432809752,
					-0.15188607935166806
				],
				[
					0.9113338583575813,
					-0.3797209924616896
				],
				[
					0.30377795278586994,
					-0.455664032137524
				],
				[
					-0.07594303967582688,
					-0.455664032137524
				],
				[
					-0.45566403213752393,
					-0.30377795278586284
				],
				[
					-0.7594419849233939,
					-0.15188607935166815
				],
				[
					-0.9872711039508748,
					-8.570656483712831e-17
				],
				[
					-0.9872711039508749,
					0.15189187343419472
				],
				[
					-0.9872711039508749,
					0.3797209924616973
				],
				[
					0,
					0
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.173828125,
				0.1923828125,
				0.294921875,
				0.3798828125,
				0.447265625,
				0.4873046875,
				0.4912109375,
				0.486328125,
				0.484375,
				0.482421875,
				0.48046875,
				0.4697265625,
				0.4658203125,
				0.470703125,
				0.4677734375,
				0.474609375,
				0.4765625,
				0.4765625,
				0.478515625,
				0.48046875,
				0.4921875,
				0.4951171875,
				0.5,
				0.5126953125,
				0.521484375,
				0.5234375,
				0.525390625,
				0.525390625,
				0.525390625,
				0.505859375,
				0.423828125,
				0.1904296875,
				0.01171875,
				0
			]
		},
		{
			"type": "diamond",
			"version": 506,
			"versionNonce": 50147422,
			"isDeleted": false,
			"id": "fdqbI4CLdCzkhdAZEK5_9",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -436.87429572873157,
			"y": -1057.9563163287473,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 10.068348289245812,
			"height": 10.873816152385476,
			"seed": 1246294757,
			"groupIds": [
				"GjWRZrhxg50ZbRqZHdlv1"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692815577642,
			"link": null,
			"locked": false
		},
		{
			"type": "diamond",
			"version": 517,
			"versionNonce": 452136066,
			"isDeleted": false,
			"id": "l4wjnJPsqCNOJECwUIvcf",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -423.9868099184971,
			"y": -1059.1645181234564,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 10.068348289245812,
			"height": 11.679284015525141,
			"seed": 1960005189,
			"groupIds": [
				"GjWRZrhxg50ZbRqZHdlv1"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692815577642,
			"link": null,
			"locked": false
		},
		{
			"type": "diamond",
			"version": 552,
			"versionNonce": 183727262,
			"isDeleted": false,
			"id": "dHQmcRy5dFTqtkIMJPRK4",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -428.01414923419566,
			"y": -1058.3590502603172,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 4.83280717883799,
			"height": 14.095687604944136,
			"seed": 1211841957,
			"groupIds": [
				"GjWRZrhxg50ZbRqZHdlv1"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692815577642,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 1199,
			"versionNonce": 1738681410,
			"isDeleted": false,
			"id": "cXs1x-7Dhfi0SY_x_X-e5",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -302.56716618256564,
			"y": -987.7110564881355,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 118.84431563405535,
			"height": 25.11856861489944,
			"seed": 2075017477,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577642,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 1326,
			"versionNonce": 2081894622,
			"isDeleted": false,
			"id": "GNb2F1x2gSlsvs9Ia1BPU",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -176.5278329891355,
			"y": -1137.1337221951599,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 118.84431563405535,
			"height": 279.62106833240153,
			"seed": 78239845,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"id": "2T7qPB3iz7qv15TN5FIZo",
					"type": "arrow"
				}
			],
			"updated": 1692815577642,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 472,
			"versionNonce": 1490506754,
			"isDeleted": false,
			"id": "fElLBgOhETNydOACXk5WK",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -287.2325305384095,
			"y": -935.4884186453555,
			"strokeColor": "#2f9e44",
			"backgroundColor": "#b2f2bb",
			"width": 39.6983777328835,
			"height": 70.95095942919585,
			"seed": 1291551685,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577642,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 1233,
			"versionNonce": 1106863390,
			"isDeleted": false,
			"id": "z9obaBu_UlsbaQPbweYjg",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -512.2850693734638,
			"y": -906.2892554218647,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 11.310163539294983,
			"height": 53.46981859810939,
			"seed": 683721509,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577642,
			"link": null,
			"locked": false
		},
		{
			"type": "arrow",
			"version": 299,
			"versionNonce": 9536450,
			"isDeleted": false,
			"id": "jLNjsLyXZVqcAweKXlE6Q",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -504.93407218363177,
			"y": -938.6907407853803,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 57.50978416496446,
			"height": 89.6476047277389,
			"seed": 1482479243,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692815577642,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "FI5xlLNLEp2a5YKorqvQ-",
				"focus": 1.0797607620701242,
				"gap": 5.03164136958689
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
					57.50978416496446,
					-89.6476047277389
				]
			]
		},
		{
			"type": "arrow",
			"version": 211,
			"versionNonce": 772477278,
			"isDeleted": false,
			"id": "liu932DjphUjP_itAGHuz",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -400.909021414652,
			"y": -1078.2365405974263,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 109.09944348941781,
			"height": 89.64760472773867,
			"seed": 2007911717,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692815577643,
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
					109.09944348941781,
					-89.64760472773867
				]
			]
		},
		{
			"type": "arrow",
			"version": 291,
			"versionNonce": 1492106114,
			"isDeleted": false,
			"id": "2T7qPB3iz7qv15TN5FIZo",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -268.97481068326294,
			"y": -1183.953055606552,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 106.69920027299901,
			"height": 40.36463664885332,
			"seed": 603992331,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692815577643,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": {
				"elementId": "GNb2F1x2gSlsvs9Ia1BPU",
				"focus": 0.795965307274205,
				"gap": 6.454696762538788
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
					106.69920027299901,
					40.36463664885332
				]
			]
		},
		{
			"type": "arrow",
			"version": 280,
			"versionNonce": 1000158622,
			"isDeleted": false,
			"id": "njVB8vb_Y04G2rX8HNl4i",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1236.4923560467842,
			"y": -879.489492380269,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 34.67501692299311,
			"height": 77.80735504671657,
			"seed": 427171397,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692815577643,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "lQ3zY2_5mp8K5GJ9-em-W",
				"focus": -0.1315654987437959,
				"gap": 6.412410754017584
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
					34.67501692299311,
					-77.80735504671657
				]
			]
		},
		{
			"type": "arrow",
			"version": 331,
			"versionNonce": 1076951874,
			"isDeleted": false,
			"id": "uFnPsIf6BjVAUXvHQSSDy",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1192.5142858029878,
			"y": -952.2224547065475,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 28.56952701308842,
			"height": 38.455923450729415,
			"seed": 479338309,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692815577643,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": {
				"elementId": "oIKqW6_1Oq8TP9NNoSPHA",
				"focus": 1.0230306099372974,
				"gap": 15.446137700516601
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
					28.56952701308842,
					38.455923450729415
				]
			]
		},
		{
			"type": "text",
			"version": 175,
			"versionNonce": 1407242718,
			"isDeleted": false,
			"id": "UlGhBpfj",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1572.7909135584803,
			"y": -145.4934299773808,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 97,
			"height": 25,
			"seed": 1436339499,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577643,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Main Menu",
			"rawText": "Main Menu",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Main Menu",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "ellipse",
			"version": 462,
			"versionNonce": 1957970690,
			"isDeleted": false,
			"id": "biHX-rWme4v_l-_0J3_Zy",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1114.3002380464382,
			"y": 140.51256209692906,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 80.30778567340849,
			"height": 152.9672108064924,
			"seed": 752564555,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692815577643,
			"link": null,
			"locked": false
		},
		{
			"type": "ellipse",
			"version": 433,
			"versionNonce": 300344862,
			"isDeleted": false,
			"id": "UVKRIp3Gn22GSahK6dAY1",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1141.0694999375742,
			"y": 248.8643364181945,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 165.7144783737001,
			"height": 48.43961675538924,
			"seed": 1868290027,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692815577643,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 247,
			"versionNonce": 284725954,
			"isDeleted": false,
			"id": "PmgQIw_A9hsW4Be3lfXHm",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1506.9160791164363,
			"y": -83.83934708592636,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 571.0775870109048,
			"height": 355.6487651250948,
			"seed": 1006860523,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577643,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 254,
			"versionNonce": 111178334,
			"isDeleted": false,
			"id": "6QqRpAVA4ZmVOmkV5E1VH",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1559.1798761419889,
			"y": 266.7105110122855,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 673.055727548567,
			"height": 61.186884322596995,
			"seed": 666846949,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577643,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 192,
			"versionNonce": 127724162,
			"isDeleted": false,
			"id": "WC2MM6KPDq72fY6aBwVfA",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1501.8171720895539,
			"y": -76.19098654560167,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 282.9893399920111,
			"height": 345.4509510713287,
			"seed": 590431013,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577643,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 188,
			"versionNonce": 2094954142,
			"isDeleted": false,
			"id": "1AAWChE1yp48IaQ04ciLS",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1215.0036518273805,
			"y": -80.01516681576396,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 275.3409794516863,
			"height": 346.7256778280495,
			"seed": 228622245,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577643,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 213,
			"versionNonce": 526404162,
			"isDeleted": false,
			"id": "2ZpgAcH-X2mMzGSgtiiuW",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1492.8940847925082,
			"y": -74.91625978888095,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 555.7808659302557,
			"height": 168.26393188714172,
			"seed": 1030020293,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577643,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 180,
			"versionNonce": 1028780766,
			"isDeleted": false,
			"id": "1HDHHe2aqbfX8pPk9CeOJ",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1491.6193580357876,
			"y": 95.89712561170222,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 553.2314124168142,
			"height": 168.26393188714167,
			"seed": 687822795,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577643,
			"link": null,
			"locked": false
		},
		{
			"type": "ellipse",
			"version": 566,
			"versionNonce": 1864479234,
			"isDeleted": false,
			"id": "LINaexvpQ3Gf0OgBKk2Pt",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1136.6079562890538,
			"y": 108.64439317890998,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 80.30778567340849,
			"height": 62.461611079317656,
			"seed": 1714662539,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692815577643,
			"link": null,
			"locked": false
		},
		{
			"type": "freedraw",
			"version": 229,
			"versionNonce": 1384900382,
			"isDeleted": false,
			"id": "ca5IbFrD9mQcyhn-OS7MP",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1137.2453196674142,
			"y": 127.76529452972153,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 22.94508162097395,
			"height": 33.14289567474009,
			"seed": 607559237,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577643,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					-1.2747267567208382
				],
				[
					-2.220446049250313e-16,
					-3.8241802701622873
				],
				[
					0,
					-5.098907026883126
				],
				[
					0,
					-10.197814053766137
				],
				[
					0,
					-12.7472675672077
				],
				[
					-1.2747267567208382,
					-16.571447837369988
				],
				[
					-1.2747267567208382,
					-17.846174594090826
				],
				[
					-1.2747267567208382,
					-19.12090135081155
				],
				[
					-2.5494535134416765,
					-20.39562810753239
				],
				[
					-2.5494535134416765,
					-21.670354864253113
				],
				[
					-2.5494535134416765,
					-22.945081620973838
				],
				[
					-2.5494535134416765,
					-24.219808377694676
				],
				[
					-2.5494535134416765,
					-25.4945351344154
				],
				[
					-2.5494535134416765,
					-26.76926189113624
				],
				[
					-2.5494535134416765,
					-28.043988647856963
				],
				[
					-2.5494535134416765,
					-29.318715404577688
				],
				[
					-2.5494535134416765,
					-30.593442161298526
				],
				[
					-2.5494535134416765,
					-31.86816891801925
				],
				[
					-2.5494535134416765,
					-33.14289567474009
				],
				[
					-1.2747267567208382,
					-33.14289567474009
				],
				[
					0,
					-33.14289567474009
				],
				[
					2.549453513441449,
					-30.593442161298526
				],
				[
					3.8241802701622873,
					-29.318715404577688
				],
				[
					5.098907026882898,
					-28.043988647856963
				],
				[
					5.098907026882898,
					-26.76926189113624
				],
				[
					6.3736337836037364,
					-26.76926189113624
				],
				[
					6.3736337836037364,
					-25.4945351344154
				],
				[
					7.648360540324575,
					-24.219808377694676
				],
				[
					8.923087297045413,
					-22.945081620973838
				],
				[
					10.197814053766024,
					-22.945081620973838
				],
				[
					10.197814053766024,
					-21.670354864253113
				],
				[
					11.472540810486862,
					-21.670354864253113
				],
				[
					12.7472675672077,
					-20.39562810753239
				],
				[
					14.021994323928311,
					-19.12090135081155
				],
				[
					15.29672108064915,
					-19.12090135081155
				],
				[
					15.29672108064915,
					-17.846174594090826
				],
				[
					16.571447837369988,
					-17.846174594090826
				],
				[
					16.571447837369988,
					-16.571447837369988
				],
				[
					17.8461745940906,
					-16.571447837369988
				],
				[
					19.120901350811437,
					-16.571447837369988
				],
				[
					19.120901350811437,
					-15.296721080649263
				],
				[
					20.395628107532275,
					-15.296721080649263
				],
				[
					20.395628107532275,
					-15.296721080649263
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 251,
			"versionNonce": 1507860930,
			"isDeleted": false,
			"id": "61I21fuy-vC_lpWLxeU8i",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1082.432069128421,
			"y": 112.46857344907227,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 24.219808377694562,
			"height": 43.340709728506226,
			"seed": 667253323,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577643,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-1.2747267567208382,
					0
				],
				[
					-1.274726756720838,
					-1.274726756720725
				],
				[
					-1.2747267567208382,
					-2.549453513441563
				],
				[
					-2.220446049250313e-16,
					-3.8241802701622873
				],
				[
					2.549453513441449,
					-3.824180270162288
				],
				[
					5.098907026883126,
					-6.37363378360385
				],
				[
					7.648360540324575,
					-7.648360540324575
				],
				[
					8.923087297045413,
					-7.648360540324575
				],
				[
					10.197814053766024,
					-8.923087297045413
				],
				[
					11.472540810486862,
					-10.197814053766137
				],
				[
					12.7472675672077,
					-11.472540810486976
				],
				[
					12.7472675672077,
					-12.7472675672077
				],
				[
					12.7472675672077,
					-14.021994323928425
				],
				[
					14.021994323928539,
					-14.021994323928425
				],
				[
					14.021994323928539,
					-16.571447837369988
				],
				[
					15.29672108064915,
					-16.571447837369988
				],
				[
					16.571447837369988,
					-17.846174594090826
				],
				[
					16.571447837369988,
					-19.12090135081155
				],
				[
					17.846174594090826,
					-19.12090135081155
				],
				[
					17.846174594090826,
					-21.670354864253113
				],
				[
					19.120901350811437,
					-22.945081620973838
				],
				[
					19.120901350811437,
					-24.219808377694676
				],
				[
					20.395628107532275,
					-25.4945351344154
				],
				[
					20.395628107532275,
					-26.769261891136125
				],
				[
					20.395628107532275,
					-28.043988647856963
				],
				[
					21.670354864253113,
					-28.043988647856963
				],
				[
					21.670354864253113,
					-29.318715404577688
				],
				[
					21.670354864253113,
					-30.593442161298526
				],
				[
					21.670354864253113,
					-31.86816891801925
				],
				[
					21.670354864253113,
					-33.142895674739975
				],
				[
					21.670354864253113,
					-34.41762243146081
				],
				[
					22.945081620973724,
					-34.41762243146081
				],
				[
					22.945081620973724,
					-33.142895674739975
				],
				[
					22.945081620973724,
					-31.86816891801925
				],
				[
					22.945081620973724,
					-30.593442161298526
				],
				[
					22.945081620973724,
					-29.318715404577688
				],
				[
					22.945081620973724,
					-28.043988647856963
				],
				[
					22.945081620973724,
					-26.769261891136125
				],
				[
					22.945081620973724,
					-25.4945351344154
				],
				[
					22.945081620973724,
					-24.219808377694676
				],
				[
					22.945081620973724,
					-21.670354864253113
				],
				[
					22.945081620973724,
					-20.395628107532275
				],
				[
					22.945081620973724,
					-17.846174594090826
				],
				[
					22.945081620973724,
					-15.296721080649263
				],
				[
					22.945081620973724,
					-14.021994323928425
				],
				[
					22.945081620973724,
					-12.7472675672077
				],
				[
					22.945081620973724,
					-11.472540810486976
				],
				[
					22.945081620973724,
					-10.197814053766137
				],
				[
					22.945081620973724,
					-8.923087297045413
				],
				[
					22.945081620973724,
					-7.648360540324575
				],
				[
					22.945081620973724,
					-6.37363378360385
				],
				[
					22.945081620973724,
					-5.098907026883126
				],
				[
					22.945081620973724,
					-3.8241802701622873
				],
				[
					22.945081620973724,
					-2.549453513441563
				],
				[
					22.945081620973724,
					-1.2747267567207246
				],
				[
					22.945081620973724,
					0
				],
				[
					21.670354864253113,
					0
				],
				[
					21.670354864253113,
					1.2747267567207246
				],
				[
					21.670354864253113,
					2.549453513441563
				],
				[
					21.670354864253113,
					3.8241802701622873
				],
				[
					21.670354864253113,
					5.098907026883126
				],
				[
					21.670354864253113,
					6.37363378360385
				],
				[
					21.670354864253113,
					7.648360540324575
				],
				[
					21.670354864253113,
					8.923087297045413
				],
				[
					21.670354864253113,
					8.923087297045413
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "rectangle",
			"version": 925,
			"versionNonce": 1291670366,
			"isDeleted": false,
			"id": "J1HX7CQuV7ymEcnOJR1eL",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1818.074539640366,
			"y": -855.7944515714123,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 424.62978072127294,
			"height": 166.1992597870078,
			"seed": 1481281579,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577643,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 152,
			"versionNonce": 180001154,
			"isDeleted": false,
			"id": "nYOl2Kmq",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1785.9994807178348,
			"y": -823.5144410199507,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 144,
			"height": 25,
			"seed": 358978187,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577643,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Cutscene Title",
			"rawText": "Cutscene Title",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Cutscene Title",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 1063,
			"versionNonce": 116864926,
			"isDeleted": false,
			"id": "sR-31C7IIO2chestyZTBu",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 49.8897056842261,
			"y": -1245.9786960136685,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 1998.9828867737724,
			"height": 482.2560142746893,
			"seed": 777766661,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577643,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 49,
			"versionNonce": 1894783298,
			"isDeleted": false,
			"id": "3rV4nASB",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 117.55837814594531,
			"y": -1211.1293935226918,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 111,
			"height": 25,
			"seed": 581884389,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577643,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Cutscene 2",
			"rawText": "Cutscene 2",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Cutscene 2",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"type": "rectangle",
			"version": 1494,
			"versionNonce": 1756009438,
			"isDeleted": false,
			"id": "CUfGjvEVtrJCeg03aos10",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 62.0981011089367,
			"y": -846.7840297102757,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 118.84431563405535,
			"height": 76.54774988857169,
			"seed": 964355301,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577643,
			"link": null,
			"locked": false
		},
		{
			"type": "ellipse",
			"version": 1675,
			"versionNonce": 1004511490,
			"isDeleted": false,
			"id": "7UlEBX1OCittHTFFVFd4a",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 94.72520674772863,
			"y": -897.9164522660882,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 27.292840097560045,
			"height": 23.326046508023218,
			"seed": 1184695365,
			"groupIds": [
				"RMnnZnlUtuTYNpbr3edmh"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692815577643,
			"link": null,
			"locked": false
		},
		{
			"type": "freedraw",
			"version": 1457,
			"versionNonce": 740845598,
			"isDeleted": false,
			"id": "btDHDijMP9wxPMoJ4_uy1",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 95.7592134363997,
			"y": -891.553411842917,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 5.9641894286609345,
			"height": 9.759576433798838,
			"seed": 1667117989,
			"groupIds": [
				"RMnnZnlUtuTYNpbr3edmh"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577643,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					-0.18073008808811764
				],
				[
					0,
					-0.36146017617623527
				],
				[
					-5.594217597396797e-17,
					-0.9036642292624609
				],
				[
					0.18073008808811777,
					-1.62659837043679
				],
				[
					0.18073008808811789,
					-2.710992687787354
				],
				[
					0.18073008808811766,
					-4.518321146312261
				],
				[
					0.18073008808811766,
					-5.964175639839061
				],
				[
					0,
					-7.048583746011483
				],
				[
					0,
					-7.771504098363969
				],
				[
					0,
					-8.675168327626416
				],
				[
					0,
					-8.855912204536391
				],
				[
					0,
					-9.217372380712627
				],
				[
					0,
					-9.398102468800744
				],
				[
					0,
					-9.578832556888862
				],
				[
					0,
					-9.759576433798838
				],
				[
					0.18073008808811766,
					-9.759576433798838
				],
				[
					0.5422040530862257,
					-9.759576433798838
				],
				[
					0.903664229262461,
					-9.578832556888862
				],
				[
					1.6265983704368043,
					-8.855912204536391
				],
				[
					1.807328458524922,
					-8.494438239538297
				],
				[
					2.1688024235230015,
					-7.952247975273944
				],
				[
					2.349532511611119,
					-7.410043922187718
				],
				[
					2.530262599699237,
					-7.048583746011483
				],
				[
					2.891722775875472,
					-6.68710978101339
				],
				[
					3.0724666527854625,
					-6.506379692925272
				],
				[
					3.2531967408735802,
					-6.325649604837155
				],
				[
					3.433926828961698,
					-5.964175639839061
				],
				[
					3.7953870051379335,
					-5.24125528748659
				],
				[
					3.976130882047895,
					-4.879781322488497
				],
				[
					4.518321146312248,
					-4.699051234400379
				],
				[
					5.241255287486591,
					-4.879781322488497
				],
				[
					5.9641894286609345,
					-5.421985375574708
				],
				[
					5.9641894286609345,
					-5.421985375574708
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.181640625,
				0.21484375,
				0.310546875,
				0.359375,
				0.40625,
				0.447265625,
				0.4853515625,
				0.49609375,
				0.501953125,
				0.51171875,
				0.5185546875,
				0.521484375,
				0.5263671875,
				0.53515625,
				0.5263671875,
				0.5263671875,
				0.53125,
				0.529296875,
				0.529296875,
				0.529296875,
				0.52734375,
				0.52734375,
				0.52734375,
				0.52734375,
				0.52734375,
				0.52734375,
				0.52734375,
				0.52734375,
				0.5302734375,
				0.537109375,
				0.529296875,
				0.4189453125,
				0.015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 1459,
			"versionNonce": 1460154562,
			"isDeleted": false,
			"id": "QQ2rqrJ7Wxt31AgDFn5Ml",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 114.91689233900001,
			"y": -895.7102590242308,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 5.42198537557468,
			"height": 9.578846345710721,
			"seed": 1661105925,
			"groupIds": [
				"RMnnZnlUtuTYNpbr3edmh"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577643,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					-0.361473964998108
				],
				[
					0.18074387690996163,
					-0.361473964998108
				],
				[
					0.542204053086197,
					-1.2651381942605546
				],
				[
					1.2651381942605402,
					-1.9880723354348837
				],
				[
					1.9880723354348546,
					-2.8917365646973305
				],
				[
					3.0724666527854336,
					-3.6146569170498157
				],
				[
					3.795400793959777,
					-4.337591058224144
				],
				[
					4.518321146312247,
					-5.241255287486591
				],
				[
					4.699065023222209,
					-5.602729252484685
				],
				[
					5.060525199398445,
					-5.7834593405728025
				],
				[
					5.241255287486562,
					-5.96418942866092
				],
				[
					5.42198537557468,
					-5.96418942866092
				],
				[
					5.42198537557468,
					-5.602729252484685
				],
				[
					5.42198537557468,
					-5.060525199398474
				],
				[
					5.42198537557468,
					-4.337591058224144
				],
				[
					5.42198537557468,
					-3.6146569170498157
				],
				[
					5.42198537557468,
					-2.7109926877873542
				],
				[
					5.241255287486562,
					-1.9880723354348837
				],
				[
					5.241255287486562,
					-1.2651381942605546
				],
				[
					5.241255287486562,
					-0.361473964998108
				],
				[
					5.060525199398445,
					0.3614601761762353
				],
				[
					4.879795111310327,
					1.0843943173505644
				],
				[
					4.699065023222209,
					1.8073284585248934
				],
				[
					4.699065023222209,
					1.9880585466130112
				],
				[
					4.699065023222209,
					2.1687886347011287
				],
				[
					4.699065023222209,
					2.530248810877364
				],
				[
					4.518321146312247,
					2.891722775875458
				],
				[
					4.518321146312247,
					3.253182952051693
				],
				[
					4.518321146312247,
					3.433913040139825
				],
				[
					4.699065023222209,
					3.614656917049801
				],
				[
					4.879795111310327,
					3.614656917049801
				],
				[
					5.241255287486562,
					3.614656917049801
				],
				[
					5.241255287486562,
					3.614656917049801
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.177734375,
				0.2587890625,
				0.28125,
				0.3544921875,
				0.388671875,
				0.408203125,
				0.4228515625,
				0.435546875,
				0.455078125,
				0.4658203125,
				0.4736328125,
				0.486328125,
				0.4951171875,
				0.5126953125,
				0.5126953125,
				0.5126953125,
				0.5126953125,
				0.5126953125,
				0.51171875,
				0.51171875,
				0.51171875,
				0.517578125,
				0.51953125,
				0.525390625,
				0.525390625,
				0.525390625,
				0.525390625,
				0.525390625,
				0.53125,
				0.515625,
				0.486328125,
				0.296875,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 1486,
			"versionNonce": 560051294,
			"isDeleted": false,
			"id": "fwH_KoFyu6-P-GobP60n8",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 107.47313621034004,
			"y": -883.9592279040409,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 3.4174889321552437,
			"height": 1.8986049623084706,
			"seed": 537349733,
			"groupIds": [
				"RMnnZnlUtuTYNpbr3edmh"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577643,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.07594303967584129,
					0
				],
				[
					-0.15189187343420177,
					-3.213996181392311e-17
				],
				[
					-0.22783491311002868,
					-0.15189187343419458
				],
				[
					-0.45566403213753826,
					-0.3037779527858557
				],
				[
					-0.7594419849233793,
					-0.5316128658958847
				],
				[
					-1.1391629773850764,
					-0.6834989452475524
				],
				[
					-1.3669978904951194,
					-0.9113338583575817
				],
				[
					-1.5948270095226005,
					-1.291054850819271
				],
				[
					-1.67077584328096,
					-1.442940930170939
				],
				[
					-1.7467188829568023,
					-1.5188839698467735
				],
				[
					-1.7467188829568023,
					-1.5948270095226076
				],
				[
					-1.6707758432809612,
					-1.5948270095226071
				],
				[
					-1.594827009522601,
					-1.5948270095226076
				],
				[
					-1.5188839698467735,
					-1.6707758432809676
				],
				[
					-1.2910548508192783,
					-1.6707758432809678
				],
				[
					-0.9872768980334226,
					-1.746718882956802
				],
				[
					-0.7594419849233792,
					-1.6707758432809678
				],
				[
					-0.45566403213753803,
					-1.594827009522608
				],
				[
					-0.15189187343420193,
					-1.5948270095226076
				],
				[
					0.07594303967584141,
					-1.5188839698467733
				],
				[
					0.3037779527858558,
					-1.5188839698467738
				],
				[
					0.455664032137524,
					-1.5188839698467733
				],
				[
					0.6834989452475527,
					-1.5948270095226071
				],
				[
					0.8353850245992208,
					-1.6707758432809678
				],
				[
					0.9113280642750619,
					-1.6707758432809685
				],
				[
					0.9872711039508891,
					-1.6707758432809678
				],
				[
					1.0632199377092497,
					-1.6707758432809683
				],
				[
					1.139162977385078,
					-1.6707758432809678
				],
				[
					1.2151060170609178,
					-1.7467188829568026
				],
				[
					1.2910490567367592,
					-1.8226619226326362
				],
				[
					1.3669920964125866,
					-1.8226619226326364
				],
				[
					1.4429409301709466,
					-1.8226619226326362
				],
				[
					1.5188839698467733,
					-1.8986049623084706
				],
				[
					1.5948270095226003,
					-1.8226619226326357
				],
				[
					1.6707700491984416,
					-1.8226619226326362
				],
				[
					1.5948270095226003,
					-1.7467188829568019
				],
				[
					1.518883969846774,
					-1.6707758432809678
				],
				[
					1.4429409301709466,
					-1.5948270095226076
				],
				[
					1.3669920964125866,
					-1.518883969846773
				],
				[
					1.291049056736759,
					-1.4429409301709397
				],
				[
					1.215106017060918,
					-1.2910548508192707
				],
				[
					1.0632199377092497,
					-1.1391629773850835
				],
				[
					0.9872711039508895,
					-0.9872768980334156
				],
				[
					0.9113280642750623,
					-0.911333858357581
				],
				[
					0.835385024599221,
					-0.8353850245992209
				],
				[
					0.7594419849233796,
					-0.7594419849233864
				],
				[
					0.6075501114891924,
					-0.6834989452475525
				],
				[
					0.5316070718133653,
					-0.6075559055717186
				],
				[
					0.4556640321375239,
					-0.5316128658958844
				],
				[
					0.3797209924616971,
					-0.4556640321375238
				],
				[
					0.30377795278585573,
					-0.37972099246168983
				],
				[
					0.2278291190274952,
					-0.3037779527858556
				],
				[
					0.22782911902749528,
					-0.22783491311002868
				],
				[
					0.1518860793516683,
					-0.15189187343419458
				],
				[
					0.15188607935166823,
					-0.0759430396758341
				],
				[
					0.2278291190274952,
					-0.0759430396758342
				],
				[
					0.37972099246169705,
					-0.15189187343419452
				],
				[
					0,
					0
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.171875,
				0.232421875,
				0.373046875,
				0.4453125,
				0.47265625,
				0.4912109375,
				0.5068359375,
				0.517578125,
				0.5234375,
				0.5234375,
				0.5234375,
				0.5234375,
				0.51953125,
				0.51953125,
				0.5166015625,
				0.5166015625,
				0.513671875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.513671875,
				0.51171875,
				0.51171875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.5166015625,
				0.513671875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.521484375,
				0.521484375,
				0.513671875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.4873046875,
				0.4306640625,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 1446,
			"versionNonce": 1711851650,
			"isDeleted": false,
			"id": "XO1D58sg40xR7F8Si_wVN",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 107.01747217820252,
			"y": -883.2757289587931,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 0.2278291190275104,
			"height": 2.6580469472318646,
			"seed": 1228552645,
			"groupIds": [
				"RMnnZnlUtuTYNpbr3edmh"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577643,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-5.356660302320523e-18,
					0.07594303967583413
				],
				[
					0.07594303967584133,
					0.22782911902750236
				],
				[
					0.07594303967584129,
					0.6075501114891994
				],
				[
					0.07594303967584137,
					0.9113280642750622
				],
				[
					0.15188607935168275,
					1.1391629773850838
				],
				[
					0.15188607935168222,
					1.44293513608842
				],
				[
					0.15188607935168275,
					1.594827009522615
				],
				[
					0.15188607935168275,
					1.8226561285501173
				],
				[
					0.1518860793516829,
					2.050491041660139
				],
				[
					0.07594303967584172,
					2.050491041660139
				],
				[
					0.0759430396758412,
					2.126434081335973
				],
				[
					0.07594303967584137,
					2.278325954770168
				],
				[
					0,
					2.4302120341218356
				],
				[
					-1.0284787780455404e-15,
					2.5061550737976703
				],
				[
					-1.7141312967425674e-16,
					2.582098113473504
				],
				[
					0,
					2.6580469472318646
				],
				[
					0.15188607935168344,
					2.6580469472318646
				],
				[
					0.22782911902750938,
					2.582098113473504
				],
				[
					0.22782911902750938,
					2.582098113473504
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.1953125,
				0.30078125,
				0.3388671875,
				0.37109375,
				0.38671875,
				0.3994140625,
				0.4111328125,
				0.42578125,
				0.4345703125,
				0.4501953125,
				0.4560546875,
				0.4677734375,
				0.470703125,
				0.470703125,
				0.470703125,
				0.470703125,
				0.474609375,
				0.3720703125,
				0.275390625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 1479,
			"versionNonce": 1915189406,
			"isDeleted": false,
			"id": "Y0HzAR2T2YraKjrd9fuba",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 104.73914622343204,
			"y": -880.9974030040231,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 6.227421958738777,
			"height": 1.8226619226326364,
			"seed": 1471723813,
			"groupIds": [
				"RMnnZnlUtuTYNpbr3edmh"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577643,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					0.07594303967583413
				],
				[
					0.07594303967582697,
					0.15188607935166826
				],
				[
					0.22782911902750963,
					0.22782911902750236
				],
				[
					0.3037721587033365,
					0.379720992461697
				],
				[
					0.4556640321375239,
					0.5316070718133652
				],
				[
					0.6075501114891922,
					0.6834931511650263
				],
				[
					0.7594419849233937,
					0.7594419849233868
				],
				[
					0.911328064275048,
					0.8353850245992207
				],
				[
					0.9872711039508891,
					0.7594419849233868
				],
				[
					1.1391629773850909,
					0.7594419849233868
				],
				[
					1.2151060170609178,
					0.6834931511650261
				],
				[
					1.291049056736745,
					0.6075501114891922
				],
				[
					1.3669920964125721,
					0.45566403213753126
				],
				[
					1.4429351360884133,
					0.3037721587033365
				],
				[
					1.5948270095226154,
					0.07594303967583424
				],
				[
					1.7467130888742688,
					-0.07594883375836059
				],
				[
					1.82265612855011,
					-0.15189187343419439
				],
				[
					1.82265612855011,
					-0.22783491311002874
				],
				[
					1.8986049623084706,
					-0.3037779527858627
				],
				[
					1.8986049623084706,
					-0.37972099246168983
				],
				[
					1.9745480019843118,
					-0.37972099246168994
				],
				[
					1.9745480019843122,
					-0.45566982622005087
				],
				[
					2.1264340813359657,
					-0.45566982622005064
				],
				[
					2.202377121011793,
					-0.4556698262200503
				],
				[
					2.2783259547701533,
					-0.37972099246168994
				],
				[
					2.3542689944459947,
					-0.37972099246168983
				],
				[
					2.3542689944459947,
					-0.30377795278586267
				],
				[
					2.4302120341218356,
					-0.30377795278586284
				],
				[
					2.506155073797663,
					-0.30377795278586284
				],
				[
					2.506155073797663,
					-0.22783491311002874
				],
				[
					2.58209811347349,
					-0.15189187343419483
				],
				[
					2.58209811347349,
					-0.0759488337583607
				],
				[
					2.6580469472318504,
					0.15188607935166826
				],
				[
					2.7339899869076913,
					0.22782911902750236
				],
				[
					2.8858760662593594,
					0.379720992461697
				],
				[
					2.9618191059351866,
					0.5316070718133652
				],
				[
					3.037767939693547,
					0.6075501114891922
				],
				[
					3.1137109793693885,
					0.7594419849233865
				],
				[
					3.1896540190452156,
					0.8353850245992209
				],
				[
					3.3415400983968837,
					1.0632141436267233
				],
				[
					3.4174889321552437,
					1.1391629773850838
				],
				[
					3.5693750115069123,
					1.2151060170609176
				],
				[
					3.645318051182754,
					1.2151060170609178
				],
				[
					3.7972099246169413,
					1.291049056736752
				],
				[
					3.9490960039686094,
					1.291049056736752
				],
				[
					4.100982083320278,
					1.2151060170609178
				],
				[
					4.252873956754465,
					1.2151060170609178
				],
				[
					4.480703075781975,
					1.0632141436267233
				],
				[
					4.78448102856783,
					0.911328064275055
				],
				[
					5.012315941677859,
					0.6834931511650263
				],
				[
					5.240145060705355,
					0.5316070718133652
				],
				[
					5.467979973815383,
					0.3037721587033365
				],
				[
					5.695814886925412,
					0.07594303967583413
				],
				[
					5.923644005952907,
					-0.07594883375836048
				],
				[
					5.999587045628748,
					-0.1518918734341946
				],
				[
					6.075535879387094,
					-0.30377795278586284
				],
				[
					6.151478919062936,
					-0.37972099246168983
				],
				[
					6.227421958738777,
					-0.5316128658958844
				],
				[
					6.227421958738777,
					-0.5316128658958844
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.1865234375,
				0.2373046875,
				0.265625,
				0.294921875,
				0.326171875,
				0.3505859375,
				0.3662109375,
				0.373046875,
				0.3798828125,
				0.392578125,
				0.396484375,
				0.3984375,
				0.3984375,
				0.4013671875,
				0.408203125,
				0.41015625,
				0.41015625,
				0.41015625,
				0.41015625,
				0.412109375,
				0.4228515625,
				0.4140625,
				0.4072265625,
				0.4072265625,
				0.4111328125,
				0.4091796875,
				0.3955078125,
				0.3310546875,
				0.3837890625,
				0.384765625,
				0.3955078125,
				0.3974609375,
				0.3974609375,
				0.3974609375,
				0.3974609375,
				0.3974609375,
				0.3974609375,
				0.3974609375,
				0.3974609375,
				0.4013671875,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.40625,
				0.41015625,
				0.4150390625,
				0.423828125,
				0.427734375,
				0.427734375,
				0.4345703125,
				0.3779296875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 1457,
			"versionNonce": 1084254274,
			"isDeleted": false,
			"id": "ZY2PyrOm1fRzopgPQEMbD",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 101.5494864103041,
			"y": -891.4777047135991,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 5.39204272822206,
			"height": 3.6453180511827465,
			"seed": 1156598917,
			"groupIds": [
				"RMnnZnlUtuTYNpbr3edmh"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577643,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.15189187343420177,
					0.1518918734341945
				],
				[
					-0.45566403213753826,
					0.30377795278586284
				],
				[
					-0.9113338583575953,
					0.5316128658958917
				],
				[
					-1.518883969846773,
					1.2151060170609176
				],
				[
					-1.8226619226326433,
					1.7467188829568097
				],
				[
					-1.9745480019842971,
					2.2023829150943337
				],
				[
					-2.050496835742657,
					2.5061608678801965
				],
				[
					-2.0504968357426576,
					2.733989986907698
				],
				[
					-1.822661922632643,
					2.96182490001772
				],
				[
					-1.518883969846774,
					3.113710979369388
				],
				[
					-0.9872768980334224,
					3.1137109793693885
				],
				[
					-0.22783491311002887,
					2.9618249000177213
				],
				[
					0.3037779527858561,
					2.8099388206660523
				],
				[
					0.6834989452475531,
					2.58210390755603
				],
				[
					1.1391629773850762,
					2.354268994446002
				],
				[
					1.5188839698467738,
					2.050496835742665
				],
				[
					2.1264340813359652,
					1.7467188829568099
				],
				[
					2.88587606625936,
					1.139162977385084
				],
				[
					3.1137109793693876,
					0.7594419849233941
				],
				[
					3.2655970587210423,
					0.5316128658958917
				],
				[
					3.3415458924794024,
					0.3037779527858632
				],
				[
					3.2655970587210423,
					0.15189187343419447
				],
				[
					3.189654019045215,
					0
				],
				[
					2.809933026583518,
					-0.1518860793516612
				],
				[
					2.430212034121821,
					-0.303777952785856
				],
				[
					1.8986049623084706,
					-0.4556640321375241
				],
				[
					1.0632199377092495,
					-0.5316070718133581
				],
				[
					0.9113280642750622,
					-0.4556640321375239
				],
				[
					0.6075501114891921,
					-0.3797209924616898
				],
				[
					0.5316070718133652,
					-0.3797209924616899
				],
				[
					0.3037779527858557,
					-0.30377795278585573
				],
				[
					0.3037779527858556,
					-0.22782911902749525
				],
				[
					0.3797209924616826,
					-0.2278291190274952
				],
				[
					0,
					0
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.171875,
				0.201171875,
				0.2529296875,
				0.3037109375,
				0.361328125,
				0.38671875,
				0.4130859375,
				0.423828125,
				0.42578125,
				0.42578125,
				0.419921875,
				0.4150390625,
				0.4033203125,
				0.400390625,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.408203125,
				0.4306640625,
				0.45703125,
				0.47265625,
				0.4775390625,
				0.482421875,
				0.4951171875,
				0.4970703125,
				0.4970703125,
				0.4970703125,
				0.466796875,
				0.4140625,
				0.0263671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 1457,
			"versionNonce": 1714074846,
			"isDeleted": false,
			"id": "9p6flAfvBGjaWbm7IHEBT",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 112.71328127104539,
			"y": -892.2371466985225,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 4.556651909540335,
			"height": 3.4174889321552446,
			"seed": 10384357,
			"groupIds": [
				"RMnnZnlUtuTYNpbr3edmh"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577643,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.15188607935165394,
					-0.07594303967583418
				],
				[
					-0.6075501114892065,
					-0.07594303967583416
				],
				[
					-0.9872711039508748,
					-8.570656483712831e-17
				],
				[
					-1.3669920964125717,
					0.22783491311002857
				],
				[
					-1.746713088874269,
					0.5316128658958919
				],
				[
					-2.202382915094326,
					1.0632199377092497
				],
				[
					-2.3542689944460085,
					1.5188839698467806
				],
				[
					-2.278325954770153,
					1.9745480019843047
				],
				[
					-2.0504910416601385,
					2.354268994446002
				],
				[
					-1.7467130888742697,
					2.658046947231858
				],
				[
					-1.1391629773850909,
					2.8858818603418865
				],
				[
					-0.7594419849233935,
					2.961824900017721
				],
				[
					-0.30377795278586966,
					2.885881860341886
				],
				[
					0.07594303967582673,
					2.7339899869076913
				],
				[
					0.8353850245992208,
					2.354268994446002
				],
				[
					1.4429409301709326,
					1.9745480019843042
				],
				[
					1.8226619226326288,
					1.6707758432809685
				],
				[
					2.0504968357426727,
					1.3669978904951126
				],
				[
					2.202382915094326,
					1.0632199377092504
				],
				[
					2.202382915094326,
					0.7594419849233874
				],
				[
					2.202382915094326,
					0.5316128658958911
				],
				[
					2.126439875418499,
					0.30377795278586267
				],
				[
					1.9745480019843116,
					0
				],
				[
					1.6707758432809752,
					-0.15188607935166806
				],
				[
					0.9113338583575813,
					-0.3797209924616896
				],
				[
					0.30377795278586994,
					-0.455664032137524
				],
				[
					-0.07594303967582688,
					-0.455664032137524
				],
				[
					-0.45566403213752393,
					-0.30377795278586284
				],
				[
					-0.7594419849233939,
					-0.15188607935166815
				],
				[
					-0.9872711039508748,
					-8.570656483712831e-17
				],
				[
					-0.9872711039508749,
					0.15189187343419472
				],
				[
					-0.9872711039508749,
					0.3797209924616973
				],
				[
					0,
					0
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.173828125,
				0.1923828125,
				0.294921875,
				0.3798828125,
				0.447265625,
				0.4873046875,
				0.4912109375,
				0.486328125,
				0.484375,
				0.482421875,
				0.48046875,
				0.4697265625,
				0.4658203125,
				0.470703125,
				0.4677734375,
				0.474609375,
				0.4765625,
				0.4765625,
				0.478515625,
				0.48046875,
				0.4921875,
				0.4951171875,
				0.5,
				0.5126953125,
				0.521484375,
				0.5234375,
				0.525390625,
				0.525390625,
				0.525390625,
				0.505859375,
				0.423828125,
				0.1904296875,
				0.01171875,
				0
			]
		},
		{
			"type": "diamond",
			"version": 578,
			"versionNonce": 1856901122,
			"isDeleted": false,
			"id": "5oh_oC549L92KFDIl4bym",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 200.7999207339995,
			"y": -1042.308990552679,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 10.068348289245812,
			"height": 10.873816152385476,
			"seed": 1337223307,
			"groupIds": [
				"8fRJ3C3E_AB2goEYzNh1M"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692815577643,
			"link": null,
			"locked": false
		},
		{
			"type": "diamond",
			"version": 587,
			"versionNonce": 654076190,
			"isDeleted": false,
			"id": "9vIvIfitEb7Mp0GqElvGj",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 213.6874065442339,
			"y": -1043.5171923473881,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 10.068348289245812,
			"height": 11.679284015525141,
			"seed": 365764395,
			"groupIds": [
				"8fRJ3C3E_AB2goEYzNh1M"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692815577643,
			"link": null,
			"locked": false
		},
		{
			"type": "diamond",
			"version": 622,
			"versionNonce": 607174594,
			"isDeleted": false,
			"id": "VUn8YBQcEu4m4MKXbiK-Y",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 209.66006722853535,
			"y": -1042.7117244842489,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 4.83280717883799,
			"height": 14.095687604944136,
			"seed": 282460619,
			"groupIds": [
				"8fRJ3C3E_AB2goEYzNh1M"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692815577643,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 451,
			"versionNonce": 67999070,
			"isDeleted": false,
			"id": "jDr6ww01Dn_yj_V58cQuH",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 157.06743462140673,
			"y": -894.273609697083,
			"strokeColor": "#1971c2",
			"backgroundColor": "#a5d8ff",
			"width": 30.222167968750455,
			"height": 29.333428276909782,
			"seed": 294688811,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577643,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 1594,
			"versionNonce": 1028093826,
			"isDeleted": false,
			"id": "Q2IOdNz1cU9rf9FLONKOV",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 203.09027325116836,
			"y": -836.8344600123924,
			"strokeColor": "#2f9e44",
			"backgroundColor": "#b2f2bb",
			"width": 153.39518267385216,
			"height": 16.365029766123357,
			"seed": 2045943755,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577643,
			"link": null,
			"locked": false
		},
		{
			"type": "arrow",
			"version": 91,
			"versionNonce": 917453214,
			"isDeleted": false,
			"id": "5Meyn14lCksrPXqoIDYhF",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 74.37861113065173,
			"y": -980.1219319251899,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#b2f2bb",
			"width": 113.84309963014448,
			"height": 35.95045251478257,
			"seed": 998350949,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692815577643,
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
					113.84309963014448,
					-35.95045251478257
				]
			]
		},
		{
			"type": "arrow",
			"version": 156,
			"versionNonce": 976303938,
			"isDeleted": false,
			"id": "z5dX6f8QBb2Ya9WEG2cBW",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 226.56886010989717,
			"y": -1077.1881537151028,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#b2f2bb",
			"width": 40.743846183420146,
			"height": 75.49595028104318,
			"seed": 1050991589,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692815577643,
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
					40.743846183420146,
					-75.49595028104318
				]
			]
		},
		{
			"type": "rectangle",
			"version": 1529,
			"versionNonce": 638735838,
			"isDeleted": false,
			"id": "GJ0TY1mYcPRhtVPUc5_Xn",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 390.9457711633038,
			"y": -858.6826311392788,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 118.84431563405535,
			"height": 76.54774988857169,
			"seed": 1719776677,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577643,
			"link": null,
			"locked": false
		},
		{
			"type": "ellipse",
			"version": 1710,
			"versionNonce": 994901762,
			"isDeleted": false,
			"id": "IdX_Uj0tVtMBf5F_kljho",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 423.5728768020957,
			"y": -909.8150536950914,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 27.292840097560045,
			"height": 23.326046508023218,
			"seed": 2053486853,
			"groupIds": [
				"WEOBv_5_ilbBPWwaJTbs3"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692815577643,
			"link": null,
			"locked": false
		},
		{
			"type": "freedraw",
			"version": 1492,
			"versionNonce": 726133278,
			"isDeleted": false,
			"id": "Tc63h685xreCl9uQ7cBVA",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 424.6068834907668,
			"y": -903.4520132719201,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 5.9641894286609345,
			"height": 9.759576433798838,
			"seed": 766660709,
			"groupIds": [
				"WEOBv_5_ilbBPWwaJTbs3"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577643,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					-0.18073008808811764
				],
				[
					0,
					-0.36146017617623527
				],
				[
					-5.594217597396797e-17,
					-0.9036642292624609
				],
				[
					0.18073008808811777,
					-1.62659837043679
				],
				[
					0.18073008808811789,
					-2.710992687787354
				],
				[
					0.18073008808811766,
					-4.518321146312261
				],
				[
					0.18073008808811766,
					-5.964175639839061
				],
				[
					0,
					-7.048583746011483
				],
				[
					0,
					-7.771504098363969
				],
				[
					0,
					-8.675168327626416
				],
				[
					0,
					-8.855912204536391
				],
				[
					0,
					-9.217372380712627
				],
				[
					0,
					-9.398102468800744
				],
				[
					0,
					-9.578832556888862
				],
				[
					0,
					-9.759576433798838
				],
				[
					0.18073008808811766,
					-9.759576433798838
				],
				[
					0.5422040530862257,
					-9.759576433798838
				],
				[
					0.903664229262461,
					-9.578832556888862
				],
				[
					1.6265983704368043,
					-8.855912204536391
				],
				[
					1.807328458524922,
					-8.494438239538297
				],
				[
					2.1688024235230015,
					-7.952247975273944
				],
				[
					2.349532511611119,
					-7.410043922187718
				],
				[
					2.530262599699237,
					-7.048583746011483
				],
				[
					2.891722775875472,
					-6.68710978101339
				],
				[
					3.0724666527854625,
					-6.506379692925272
				],
				[
					3.2531967408735802,
					-6.325649604837155
				],
				[
					3.433926828961698,
					-5.964175639839061
				],
				[
					3.7953870051379335,
					-5.24125528748659
				],
				[
					3.976130882047895,
					-4.879781322488497
				],
				[
					4.518321146312248,
					-4.699051234400379
				],
				[
					5.241255287486591,
					-4.879781322488497
				],
				[
					5.9641894286609345,
					-5.421985375574708
				],
				[
					5.9641894286609345,
					-5.421985375574708
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.181640625,
				0.21484375,
				0.310546875,
				0.359375,
				0.40625,
				0.447265625,
				0.4853515625,
				0.49609375,
				0.501953125,
				0.51171875,
				0.5185546875,
				0.521484375,
				0.5263671875,
				0.53515625,
				0.5263671875,
				0.5263671875,
				0.53125,
				0.529296875,
				0.529296875,
				0.529296875,
				0.52734375,
				0.52734375,
				0.52734375,
				0.52734375,
				0.52734375,
				0.52734375,
				0.52734375,
				0.52734375,
				0.5302734375,
				0.537109375,
				0.529296875,
				0.4189453125,
				0.015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 1494,
			"versionNonce": 2098843330,
			"isDeleted": false,
			"id": "GsSXNMpDnlLCc-SQe7Ce5",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 443.7645623933671,
			"y": -907.608860453234,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 5.42198537557468,
			"height": 9.578846345710721,
			"seed": 775224261,
			"groupIds": [
				"WEOBv_5_ilbBPWwaJTbs3"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577643,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					-0.361473964998108
				],
				[
					0.18074387690996163,
					-0.361473964998108
				],
				[
					0.542204053086197,
					-1.2651381942605546
				],
				[
					1.2651381942605402,
					-1.9880723354348837
				],
				[
					1.9880723354348546,
					-2.8917365646973305
				],
				[
					3.0724666527854336,
					-3.6146569170498157
				],
				[
					3.795400793959777,
					-4.337591058224144
				],
				[
					4.518321146312247,
					-5.241255287486591
				],
				[
					4.699065023222209,
					-5.602729252484685
				],
				[
					5.060525199398445,
					-5.7834593405728025
				],
				[
					5.241255287486562,
					-5.96418942866092
				],
				[
					5.42198537557468,
					-5.96418942866092
				],
				[
					5.42198537557468,
					-5.602729252484685
				],
				[
					5.42198537557468,
					-5.060525199398474
				],
				[
					5.42198537557468,
					-4.337591058224144
				],
				[
					5.42198537557468,
					-3.6146569170498157
				],
				[
					5.42198537557468,
					-2.7109926877873542
				],
				[
					5.241255287486562,
					-1.9880723354348837
				],
				[
					5.241255287486562,
					-1.2651381942605546
				],
				[
					5.241255287486562,
					-0.361473964998108
				],
				[
					5.060525199398445,
					0.3614601761762353
				],
				[
					4.879795111310327,
					1.0843943173505644
				],
				[
					4.699065023222209,
					1.8073284585248934
				],
				[
					4.699065023222209,
					1.9880585466130112
				],
				[
					4.699065023222209,
					2.1687886347011287
				],
				[
					4.699065023222209,
					2.530248810877364
				],
				[
					4.518321146312247,
					2.891722775875458
				],
				[
					4.518321146312247,
					3.253182952051693
				],
				[
					4.518321146312247,
					3.433913040139825
				],
				[
					4.699065023222209,
					3.614656917049801
				],
				[
					4.879795111310327,
					3.614656917049801
				],
				[
					5.241255287486562,
					3.614656917049801
				],
				[
					5.241255287486562,
					3.614656917049801
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.177734375,
				0.2587890625,
				0.28125,
				0.3544921875,
				0.388671875,
				0.408203125,
				0.4228515625,
				0.435546875,
				0.455078125,
				0.4658203125,
				0.4736328125,
				0.486328125,
				0.4951171875,
				0.5126953125,
				0.5126953125,
				0.5126953125,
				0.5126953125,
				0.5126953125,
				0.51171875,
				0.51171875,
				0.51171875,
				0.517578125,
				0.51953125,
				0.525390625,
				0.525390625,
				0.525390625,
				0.525390625,
				0.525390625,
				0.53125,
				0.515625,
				0.486328125,
				0.296875,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 1521,
			"versionNonce": 1430320734,
			"isDeleted": false,
			"id": "yalM8GHGI8gMcyiO27wTg",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 436.32080626470713,
			"y": -895.857829333044,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 3.4174889321552437,
			"height": 1.8986049623084706,
			"seed": 336280357,
			"groupIds": [
				"WEOBv_5_ilbBPWwaJTbs3"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577643,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.07594303967584129,
					0
				],
				[
					-0.15189187343420177,
					-3.213996181392311e-17
				],
				[
					-0.22783491311002868,
					-0.15189187343419458
				],
				[
					-0.45566403213753826,
					-0.3037779527858557
				],
				[
					-0.7594419849233793,
					-0.5316128658958847
				],
				[
					-1.1391629773850764,
					-0.6834989452475524
				],
				[
					-1.3669978904951194,
					-0.9113338583575817
				],
				[
					-1.5948270095226005,
					-1.291054850819271
				],
				[
					-1.67077584328096,
					-1.442940930170939
				],
				[
					-1.7467188829568023,
					-1.5188839698467735
				],
				[
					-1.7467188829568023,
					-1.5948270095226076
				],
				[
					-1.6707758432809612,
					-1.5948270095226071
				],
				[
					-1.594827009522601,
					-1.5948270095226076
				],
				[
					-1.5188839698467735,
					-1.6707758432809676
				],
				[
					-1.2910548508192783,
					-1.6707758432809678
				],
				[
					-0.9872768980334226,
					-1.746718882956802
				],
				[
					-0.7594419849233792,
					-1.6707758432809678
				],
				[
					-0.45566403213753803,
					-1.594827009522608
				],
				[
					-0.15189187343420193,
					-1.5948270095226076
				],
				[
					0.07594303967584141,
					-1.5188839698467733
				],
				[
					0.3037779527858558,
					-1.5188839698467738
				],
				[
					0.455664032137524,
					-1.5188839698467733
				],
				[
					0.6834989452475527,
					-1.5948270095226071
				],
				[
					0.8353850245992208,
					-1.6707758432809678
				],
				[
					0.9113280642750619,
					-1.6707758432809685
				],
				[
					0.9872711039508891,
					-1.6707758432809678
				],
				[
					1.0632199377092497,
					-1.6707758432809683
				],
				[
					1.139162977385078,
					-1.6707758432809678
				],
				[
					1.2151060170609178,
					-1.7467188829568026
				],
				[
					1.2910490567367592,
					-1.8226619226326362
				],
				[
					1.3669920964125866,
					-1.8226619226326364
				],
				[
					1.4429409301709466,
					-1.8226619226326362
				],
				[
					1.5188839698467733,
					-1.8986049623084706
				],
				[
					1.5948270095226003,
					-1.8226619226326357
				],
				[
					1.6707700491984416,
					-1.8226619226326362
				],
				[
					1.5948270095226003,
					-1.7467188829568019
				],
				[
					1.518883969846774,
					-1.6707758432809678
				],
				[
					1.4429409301709466,
					-1.5948270095226076
				],
				[
					1.3669920964125866,
					-1.518883969846773
				],
				[
					1.291049056736759,
					-1.4429409301709397
				],
				[
					1.215106017060918,
					-1.2910548508192707
				],
				[
					1.0632199377092497,
					-1.1391629773850835
				],
				[
					0.9872711039508895,
					-0.9872768980334156
				],
				[
					0.9113280642750623,
					-0.911333858357581
				],
				[
					0.835385024599221,
					-0.8353850245992209
				],
				[
					0.7594419849233796,
					-0.7594419849233864
				],
				[
					0.6075501114891924,
					-0.6834989452475525
				],
				[
					0.5316070718133653,
					-0.6075559055717186
				],
				[
					0.4556640321375239,
					-0.5316128658958844
				],
				[
					0.3797209924616971,
					-0.4556640321375238
				],
				[
					0.30377795278585573,
					-0.37972099246168983
				],
				[
					0.2278291190274952,
					-0.3037779527858556
				],
				[
					0.22782911902749528,
					-0.22783491311002868
				],
				[
					0.1518860793516683,
					-0.15189187343419458
				],
				[
					0.15188607935166823,
					-0.0759430396758341
				],
				[
					0.2278291190274952,
					-0.0759430396758342
				],
				[
					0.37972099246169705,
					-0.15189187343419452
				],
				[
					0,
					0
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.171875,
				0.232421875,
				0.373046875,
				0.4453125,
				0.47265625,
				0.4912109375,
				0.5068359375,
				0.517578125,
				0.5234375,
				0.5234375,
				0.5234375,
				0.5234375,
				0.51953125,
				0.51953125,
				0.5166015625,
				0.5166015625,
				0.513671875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.513671875,
				0.51171875,
				0.51171875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.5166015625,
				0.513671875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.521484375,
				0.521484375,
				0.513671875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.4873046875,
				0.4306640625,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 1481,
			"versionNonce": 1412867714,
			"isDeleted": false,
			"id": "gD1pnd3dRQuHuJ68pzjrJ",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 435.8651422325696,
			"y": -895.1743303877963,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 0.2278291190275104,
			"height": 2.6580469472318646,
			"seed": 396529285,
			"groupIds": [
				"WEOBv_5_ilbBPWwaJTbs3"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577643,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-5.356660302320523e-18,
					0.07594303967583413
				],
				[
					0.07594303967584133,
					0.22782911902750236
				],
				[
					0.07594303967584129,
					0.6075501114891994
				],
				[
					0.07594303967584137,
					0.9113280642750622
				],
				[
					0.15188607935168275,
					1.1391629773850838
				],
				[
					0.15188607935168222,
					1.44293513608842
				],
				[
					0.15188607935168275,
					1.594827009522615
				],
				[
					0.15188607935168275,
					1.8226561285501173
				],
				[
					0.1518860793516829,
					2.050491041660139
				],
				[
					0.07594303967584172,
					2.050491041660139
				],
				[
					0.0759430396758412,
					2.126434081335973
				],
				[
					0.07594303967584137,
					2.278325954770168
				],
				[
					0,
					2.4302120341218356
				],
				[
					-1.0284787780455404e-15,
					2.5061550737976703
				],
				[
					-1.7141312967425674e-16,
					2.582098113473504
				],
				[
					0,
					2.6580469472318646
				],
				[
					0.15188607935168344,
					2.6580469472318646
				],
				[
					0.22782911902750938,
					2.582098113473504
				],
				[
					0.22782911902750938,
					2.582098113473504
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.1953125,
				0.30078125,
				0.3388671875,
				0.37109375,
				0.38671875,
				0.3994140625,
				0.4111328125,
				0.42578125,
				0.4345703125,
				0.4501953125,
				0.4560546875,
				0.4677734375,
				0.470703125,
				0.470703125,
				0.470703125,
				0.470703125,
				0.474609375,
				0.3720703125,
				0.275390625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 1514,
			"versionNonce": 751729310,
			"isDeleted": false,
			"id": "8JzdEdSMVsZD_8GA08p3c",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 433.58681627779913,
			"y": -892.8960044330263,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 6.227421958738777,
			"height": 1.8226619226326364,
			"seed": 129529317,
			"groupIds": [
				"WEOBv_5_ilbBPWwaJTbs3"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577643,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					0.07594303967583413
				],
				[
					0.07594303967582697,
					0.15188607935166826
				],
				[
					0.22782911902750963,
					0.22782911902750236
				],
				[
					0.3037721587033365,
					0.379720992461697
				],
				[
					0.4556640321375239,
					0.5316070718133652
				],
				[
					0.6075501114891922,
					0.6834931511650263
				],
				[
					0.7594419849233937,
					0.7594419849233868
				],
				[
					0.911328064275048,
					0.8353850245992207
				],
				[
					0.9872711039508891,
					0.7594419849233868
				],
				[
					1.1391629773850909,
					0.7594419849233868
				],
				[
					1.2151060170609178,
					0.6834931511650261
				],
				[
					1.291049056736745,
					0.6075501114891922
				],
				[
					1.3669920964125721,
					0.45566403213753126
				],
				[
					1.4429351360884133,
					0.3037721587033365
				],
				[
					1.5948270095226154,
					0.07594303967583424
				],
				[
					1.7467130888742688,
					-0.07594883375836059
				],
				[
					1.82265612855011,
					-0.15189187343419439
				],
				[
					1.82265612855011,
					-0.22783491311002874
				],
				[
					1.8986049623084706,
					-0.3037779527858627
				],
				[
					1.8986049623084706,
					-0.37972099246168983
				],
				[
					1.9745480019843118,
					-0.37972099246168994
				],
				[
					1.9745480019843122,
					-0.45566982622005087
				],
				[
					2.1264340813359657,
					-0.45566982622005064
				],
				[
					2.202377121011793,
					-0.4556698262200503
				],
				[
					2.2783259547701533,
					-0.37972099246168994
				],
				[
					2.3542689944459947,
					-0.37972099246168983
				],
				[
					2.3542689944459947,
					-0.30377795278586267
				],
				[
					2.4302120341218356,
					-0.30377795278586284
				],
				[
					2.506155073797663,
					-0.30377795278586284
				],
				[
					2.506155073797663,
					-0.22783491311002874
				],
				[
					2.58209811347349,
					-0.15189187343419483
				],
				[
					2.58209811347349,
					-0.0759488337583607
				],
				[
					2.6580469472318504,
					0.15188607935166826
				],
				[
					2.7339899869076913,
					0.22782911902750236
				],
				[
					2.8858760662593594,
					0.379720992461697
				],
				[
					2.9618191059351866,
					0.5316070718133652
				],
				[
					3.037767939693547,
					0.6075501114891922
				],
				[
					3.1137109793693885,
					0.7594419849233865
				],
				[
					3.1896540190452156,
					0.8353850245992209
				],
				[
					3.3415400983968837,
					1.0632141436267233
				],
				[
					3.4174889321552437,
					1.1391629773850838
				],
				[
					3.5693750115069123,
					1.2151060170609176
				],
				[
					3.645318051182754,
					1.2151060170609178
				],
				[
					3.7972099246169413,
					1.291049056736752
				],
				[
					3.9490960039686094,
					1.291049056736752
				],
				[
					4.100982083320278,
					1.2151060170609178
				],
				[
					4.252873956754465,
					1.2151060170609178
				],
				[
					4.480703075781975,
					1.0632141436267233
				],
				[
					4.78448102856783,
					0.911328064275055
				],
				[
					5.012315941677859,
					0.6834931511650263
				],
				[
					5.240145060705355,
					0.5316070718133652
				],
				[
					5.467979973815383,
					0.3037721587033365
				],
				[
					5.695814886925412,
					0.07594303967583413
				],
				[
					5.923644005952907,
					-0.07594883375836048
				],
				[
					5.999587045628748,
					-0.1518918734341946
				],
				[
					6.075535879387094,
					-0.30377795278586284
				],
				[
					6.151478919062936,
					-0.37972099246168983
				],
				[
					6.227421958738777,
					-0.5316128658958844
				],
				[
					6.227421958738777,
					-0.5316128658958844
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.1865234375,
				0.2373046875,
				0.265625,
				0.294921875,
				0.326171875,
				0.3505859375,
				0.3662109375,
				0.373046875,
				0.3798828125,
				0.392578125,
				0.396484375,
				0.3984375,
				0.3984375,
				0.4013671875,
				0.408203125,
				0.41015625,
				0.41015625,
				0.41015625,
				0.41015625,
				0.412109375,
				0.4228515625,
				0.4140625,
				0.4072265625,
				0.4072265625,
				0.4111328125,
				0.4091796875,
				0.3955078125,
				0.3310546875,
				0.3837890625,
				0.384765625,
				0.3955078125,
				0.3974609375,
				0.3974609375,
				0.3974609375,
				0.3974609375,
				0.3974609375,
				0.3974609375,
				0.3974609375,
				0.3974609375,
				0.4013671875,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.40625,
				0.41015625,
				0.4150390625,
				0.423828125,
				0.427734375,
				0.427734375,
				0.4345703125,
				0.3779296875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 1492,
			"versionNonce": 694322754,
			"isDeleted": false,
			"id": "ZIbI9QmfIo9qpGEoSXjwj",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 430.3971564646712,
			"y": -903.3763061426023,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 5.39204272822206,
			"height": 3.6453180511827465,
			"seed": 2136633669,
			"groupIds": [
				"WEOBv_5_ilbBPWwaJTbs3"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577643,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.15189187343420177,
					0.1518918734341945
				],
				[
					-0.45566403213753826,
					0.30377795278586284
				],
				[
					-0.9113338583575953,
					0.5316128658958917
				],
				[
					-1.518883969846773,
					1.2151060170609176
				],
				[
					-1.8226619226326433,
					1.7467188829568097
				],
				[
					-1.9745480019842971,
					2.2023829150943337
				],
				[
					-2.050496835742657,
					2.5061608678801965
				],
				[
					-2.0504968357426576,
					2.733989986907698
				],
				[
					-1.822661922632643,
					2.96182490001772
				],
				[
					-1.518883969846774,
					3.113710979369388
				],
				[
					-0.9872768980334224,
					3.1137109793693885
				],
				[
					-0.22783491311002887,
					2.9618249000177213
				],
				[
					0.3037779527858561,
					2.8099388206660523
				],
				[
					0.6834989452475531,
					2.58210390755603
				],
				[
					1.1391629773850762,
					2.354268994446002
				],
				[
					1.5188839698467738,
					2.050496835742665
				],
				[
					2.1264340813359652,
					1.7467188829568099
				],
				[
					2.88587606625936,
					1.139162977385084
				],
				[
					3.1137109793693876,
					0.7594419849233941
				],
				[
					3.2655970587210423,
					0.5316128658958917
				],
				[
					3.3415458924794024,
					0.3037779527858632
				],
				[
					3.2655970587210423,
					0.15189187343419447
				],
				[
					3.189654019045215,
					0
				],
				[
					2.809933026583518,
					-0.1518860793516612
				],
				[
					2.430212034121821,
					-0.303777952785856
				],
				[
					1.8986049623084706,
					-0.4556640321375241
				],
				[
					1.0632199377092495,
					-0.5316070718133581
				],
				[
					0.9113280642750622,
					-0.4556640321375239
				],
				[
					0.6075501114891921,
					-0.3797209924616898
				],
				[
					0.5316070718133652,
					-0.3797209924616899
				],
				[
					0.3037779527858557,
					-0.30377795278585573
				],
				[
					0.3037779527858556,
					-0.22782911902749525
				],
				[
					0.3797209924616826,
					-0.2278291190274952
				],
				[
					0,
					0
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.171875,
				0.201171875,
				0.2529296875,
				0.3037109375,
				0.361328125,
				0.38671875,
				0.4130859375,
				0.423828125,
				0.42578125,
				0.42578125,
				0.419921875,
				0.4150390625,
				0.4033203125,
				0.400390625,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.408203125,
				0.4306640625,
				0.45703125,
				0.47265625,
				0.4775390625,
				0.482421875,
				0.4951171875,
				0.4970703125,
				0.4970703125,
				0.4970703125,
				0.466796875,
				0.4140625,
				0.0263671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 1492,
			"versionNonce": 2023847646,
			"isDeleted": false,
			"id": "i-armKSdxKBZqDBK9y1lI",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 441.5609513254125,
			"y": -904.1357481275256,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 4.556651909540335,
			"height": 3.4174889321552446,
			"seed": 1541800101,
			"groupIds": [
				"WEOBv_5_ilbBPWwaJTbs3"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577643,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.15188607935165394,
					-0.07594303967583418
				],
				[
					-0.6075501114892065,
					-0.07594303967583416
				],
				[
					-0.9872711039508748,
					-8.570656483712831e-17
				],
				[
					-1.3669920964125717,
					0.22783491311002857
				],
				[
					-1.746713088874269,
					0.5316128658958919
				],
				[
					-2.202382915094326,
					1.0632199377092497
				],
				[
					-2.3542689944460085,
					1.5188839698467806
				],
				[
					-2.278325954770153,
					1.9745480019843047
				],
				[
					-2.0504910416601385,
					2.354268994446002
				],
				[
					-1.7467130888742697,
					2.658046947231858
				],
				[
					-1.1391629773850909,
					2.8858818603418865
				],
				[
					-0.7594419849233935,
					2.961824900017721
				],
				[
					-0.30377795278586966,
					2.885881860341886
				],
				[
					0.07594303967582673,
					2.7339899869076913
				],
				[
					0.8353850245992208,
					2.354268994446002
				],
				[
					1.4429409301709326,
					1.9745480019843042
				],
				[
					1.8226619226326288,
					1.6707758432809685
				],
				[
					2.0504968357426727,
					1.3669978904951126
				],
				[
					2.202382915094326,
					1.0632199377092504
				],
				[
					2.202382915094326,
					0.7594419849233874
				],
				[
					2.202382915094326,
					0.5316128658958911
				],
				[
					2.126439875418499,
					0.30377795278586267
				],
				[
					1.9745480019843116,
					0
				],
				[
					1.6707758432809752,
					-0.15188607935166806
				],
				[
					0.9113338583575813,
					-0.3797209924616896
				],
				[
					0.30377795278586994,
					-0.455664032137524
				],
				[
					-0.07594303967582688,
					-0.455664032137524
				],
				[
					-0.45566403213752393,
					-0.30377795278586284
				],
				[
					-0.7594419849233939,
					-0.15188607935166815
				],
				[
					-0.9872711039508748,
					-8.570656483712831e-17
				],
				[
					-0.9872711039508749,
					0.15189187343419472
				],
				[
					-0.9872711039508749,
					0.3797209924616973
				],
				[
					0,
					0
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.173828125,
				0.1923828125,
				0.294921875,
				0.3798828125,
				0.447265625,
				0.4873046875,
				0.4912109375,
				0.486328125,
				0.484375,
				0.482421875,
				0.48046875,
				0.4697265625,
				0.4658203125,
				0.470703125,
				0.4677734375,
				0.474609375,
				0.4765625,
				0.4765625,
				0.478515625,
				0.48046875,
				0.4921875,
				0.4951171875,
				0.5,
				0.5126953125,
				0.521484375,
				0.5234375,
				0.525390625,
				0.525390625,
				0.525390625,
				0.505859375,
				0.423828125,
				0.1904296875,
				0.01171875,
				0
			]
		},
		{
			"type": "rectangle",
			"version": 486,
			"versionNonce": 1971088898,
			"isDeleted": false,
			"id": "0ktv1NmwCNQBiqMznppZb",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 485.9151046757738,
			"y": -906.172211126086,
			"strokeColor": "#1971c2",
			"backgroundColor": "#a5d8ff",
			"width": 30.222167968750455,
			"height": 29.333428276909782,
			"seed": 1802634789,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577643,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 1629,
			"versionNonce": 21687070,
			"isDeleted": false,
			"id": "cJl-YW83M5emNrmEJ9zay",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 531.9379433055354,
			"y": -848.7330614413954,
			"strokeColor": "#2f9e44",
			"backgroundColor": "#b2f2bb",
			"width": 153.39518267385216,
			"height": 16.365029766123357,
			"seed": 234355077,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577643,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 1457,
			"versionNonce": 1032019394,
			"isDeleted": false,
			"id": "Kb3iUHDFGXVmXq6eBKDwv",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 367.6198602840245,
			"y": -1230.8928150850616,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 3.6755016503132074,
			"height": 464.14185022568955,
			"seed": 129111531,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577643,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 1619,
			"versionNonce": 1429985118,
			"isDeleted": false,
			"id": "JcRMcMxtHdJPa5W1KEbW-",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 473.9661834454673,
			"y": -1110.5047251467092,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 50.1423385288886,
			"height": 33.61531296661438,
			"seed": 48934795,
			"groupIds": [
				"BImaMKRp79-uLZd0ek8LN"
			],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577643,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 1729,
			"versionNonce": 244733314,
			"isDeleted": false,
			"id": "6YKVn8Ou0JJ2Nt9OUHMOu",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 487.665515229676,
			"y": -1102.0496700917915,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 21.193026891152638,
			"height": 12.993885498638106,
			"seed": 263076069,
			"groupIds": [
				"BImaMKRp79-uLZd0ek8LN"
			],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577643,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 1774,
			"versionNonce": 214252446,
			"isDeleted": false,
			"id": "e3sifxOSpb1DGlkMztnGs",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 474.64322278306827,
			"y": -1124.1722799469312,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 21.193026891152638,
			"height": 12.993885498638106,
			"seed": 1605111973,
			"groupIds": [
				"BImaMKRp79-uLZd0ek8LN"
			],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577643,
			"link": null,
			"locked": false
		},
		{
			"type": "arrow",
			"version": 197,
			"versionNonce": 2046055746,
			"isDeleted": false,
			"id": "7e04ulfVsv1ISiECxtnsO",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 543.4896215927939,
			"y": -1091.164002467134,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#b2f2bb",
			"width": 269.75748611772747,
			"height": 2.5609887922569214,
			"seed": 415139115,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692815577644,
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
					269.75748611772747,
					2.5609887922569214
				]
			]
		},
		{
			"type": "arrow",
			"version": 156,
			"versionNonce": 236459998,
			"isDeleted": false,
			"id": "zeaU4xjRJbNGnzUsNadrc",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 820.0764111565398,
			"y": -1039.9442266219955,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#b2f2bb",
			"width": 309.0259809323335,
			"height": 2.560988792257149,
			"seed": 1912131531,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692815577644,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "SiEASAgVfRMiV8uQuFDS6",
				"focus": 0.7506656067129628,
				"gap": 25.090472327450414
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
					-309.0259809323335,
					-2.560988792257149
				]
			]
		},
		{
			"type": "rectangle",
			"version": 1654,
			"versionNonce": 284974338,
			"isDeleted": false,
			"id": "SiEASAgVfRMiV8uQuFDS6",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 845.1668834839903,
			"y": -1077.364438635529,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 118.84431563405535,
			"height": 308.74406705319797,
			"seed": 964874213,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"id": "zeaU4xjRJbNGnzUsNadrc",
					"type": "arrow"
				}
			],
			"updated": 1692815577644,
			"link": null,
			"locked": false
		},
		{
			"type": "ellipse",
			"version": 1750,
			"versionNonce": 1363504158,
			"isDeleted": false,
			"id": "7Vmqyef-T0N6jEH3ybB4D",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 855.088778160641,
			"y": -1108.6309940045142,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 27.292840097560045,
			"height": 23.326046508023218,
			"seed": 752717157,
			"groupIds": [
				"cc6Mwfh3S8J7ftJWavf9d"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692815577644,
			"link": null,
			"locked": false
		},
		{
			"type": "freedraw",
			"version": 1532,
			"versionNonce": 1630366914,
			"isDeleted": false,
			"id": "y_EcDvWOI5i7OyZS3mAQ6",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 856.1227848493121,
			"y": -1102.267953581343,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 5.9641894286609345,
			"height": 9.759576433798838,
			"seed": 2129696965,
			"groupIds": [
				"cc6Mwfh3S8J7ftJWavf9d"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577644,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					-0.18073008808811764
				],
				[
					0,
					-0.36146017617623527
				],
				[
					-5.594217597396797e-17,
					-0.9036642292624609
				],
				[
					0.18073008808811777,
					-1.62659837043679
				],
				[
					0.18073008808811789,
					-2.710992687787354
				],
				[
					0.18073008808811766,
					-4.518321146312261
				],
				[
					0.18073008808811766,
					-5.964175639839061
				],
				[
					0,
					-7.048583746011483
				],
				[
					0,
					-7.771504098363969
				],
				[
					0,
					-8.675168327626416
				],
				[
					0,
					-8.855912204536391
				],
				[
					0,
					-9.217372380712627
				],
				[
					0,
					-9.398102468800744
				],
				[
					0,
					-9.578832556888862
				],
				[
					0,
					-9.759576433798838
				],
				[
					0.18073008808811766,
					-9.759576433798838
				],
				[
					0.5422040530862257,
					-9.759576433798838
				],
				[
					0.903664229262461,
					-9.578832556888862
				],
				[
					1.6265983704368043,
					-8.855912204536391
				],
				[
					1.807328458524922,
					-8.494438239538297
				],
				[
					2.1688024235230015,
					-7.952247975273944
				],
				[
					2.349532511611119,
					-7.410043922187718
				],
				[
					2.530262599699237,
					-7.048583746011483
				],
				[
					2.891722775875472,
					-6.68710978101339
				],
				[
					3.0724666527854625,
					-6.506379692925272
				],
				[
					3.2531967408735802,
					-6.325649604837155
				],
				[
					3.433926828961698,
					-5.964175639839061
				],
				[
					3.7953870051379335,
					-5.24125528748659
				],
				[
					3.976130882047895,
					-4.879781322488497
				],
				[
					4.518321146312248,
					-4.699051234400379
				],
				[
					5.241255287486591,
					-4.879781322488497
				],
				[
					5.9641894286609345,
					-5.421985375574708
				],
				[
					5.9641894286609345,
					-5.421985375574708
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.181640625,
				0.21484375,
				0.310546875,
				0.359375,
				0.40625,
				0.447265625,
				0.4853515625,
				0.49609375,
				0.501953125,
				0.51171875,
				0.5185546875,
				0.521484375,
				0.5263671875,
				0.53515625,
				0.5263671875,
				0.5263671875,
				0.53125,
				0.529296875,
				0.529296875,
				0.529296875,
				0.52734375,
				0.52734375,
				0.52734375,
				0.52734375,
				0.52734375,
				0.52734375,
				0.52734375,
				0.52734375,
				0.5302734375,
				0.537109375,
				0.529296875,
				0.4189453125,
				0.015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 1534,
			"versionNonce": 608057438,
			"isDeleted": false,
			"id": "pqlPZ4DeCxI7YrePmdt-x",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 875.2804637519122,
			"y": -1106.4248007626568,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 5.42198537557468,
			"height": 9.578846345710721,
			"seed": 1699428389,
			"groupIds": [
				"cc6Mwfh3S8J7ftJWavf9d"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577644,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					-0.361473964998108
				],
				[
					0.18074387690996163,
					-0.361473964998108
				],
				[
					0.542204053086197,
					-1.2651381942605546
				],
				[
					1.2651381942605402,
					-1.9880723354348837
				],
				[
					1.9880723354348546,
					-2.8917365646973305
				],
				[
					3.0724666527854336,
					-3.6146569170498157
				],
				[
					3.795400793959777,
					-4.337591058224144
				],
				[
					4.518321146312247,
					-5.241255287486591
				],
				[
					4.699065023222209,
					-5.602729252484685
				],
				[
					5.060525199398445,
					-5.7834593405728025
				],
				[
					5.241255287486562,
					-5.96418942866092
				],
				[
					5.42198537557468,
					-5.96418942866092
				],
				[
					5.42198537557468,
					-5.602729252484685
				],
				[
					5.42198537557468,
					-5.060525199398474
				],
				[
					5.42198537557468,
					-4.337591058224144
				],
				[
					5.42198537557468,
					-3.6146569170498157
				],
				[
					5.42198537557468,
					-2.7109926877873542
				],
				[
					5.241255287486562,
					-1.9880723354348837
				],
				[
					5.241255287486562,
					-1.2651381942605546
				],
				[
					5.241255287486562,
					-0.361473964998108
				],
				[
					5.060525199398445,
					0.3614601761762353
				],
				[
					4.879795111310327,
					1.0843943173505644
				],
				[
					4.699065023222209,
					1.8073284585248934
				],
				[
					4.699065023222209,
					1.9880585466130112
				],
				[
					4.699065023222209,
					2.1687886347011287
				],
				[
					4.699065023222209,
					2.530248810877364
				],
				[
					4.518321146312247,
					2.891722775875458
				],
				[
					4.518321146312247,
					3.253182952051693
				],
				[
					4.518321146312247,
					3.433913040139825
				],
				[
					4.699065023222209,
					3.614656917049801
				],
				[
					4.879795111310327,
					3.614656917049801
				],
				[
					5.241255287486562,
					3.614656917049801
				],
				[
					5.241255287486562,
					3.614656917049801
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.177734375,
				0.2587890625,
				0.28125,
				0.3544921875,
				0.388671875,
				0.408203125,
				0.4228515625,
				0.435546875,
				0.455078125,
				0.4658203125,
				0.4736328125,
				0.486328125,
				0.4951171875,
				0.5126953125,
				0.5126953125,
				0.5126953125,
				0.5126953125,
				0.5126953125,
				0.51171875,
				0.51171875,
				0.51171875,
				0.517578125,
				0.51953125,
				0.525390625,
				0.525390625,
				0.525390625,
				0.525390625,
				0.525390625,
				0.53125,
				0.515625,
				0.486328125,
				0.296875,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 1561,
			"versionNonce": 1881572482,
			"isDeleted": false,
			"id": "bGwX8s_aAwewhhS9nEEvu",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 867.8367076232522,
			"y": -1094.6737696424668,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 3.4174889321552437,
			"height": 1.8986049623084706,
			"seed": 433777541,
			"groupIds": [
				"cc6Mwfh3S8J7ftJWavf9d"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577644,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.07594303967584129,
					0
				],
				[
					-0.15189187343420177,
					-3.213996181392311e-17
				],
				[
					-0.22783491311002868,
					-0.15189187343419458
				],
				[
					-0.45566403213753826,
					-0.3037779527858557
				],
				[
					-0.7594419849233793,
					-0.5316128658958847
				],
				[
					-1.1391629773850764,
					-0.6834989452475524
				],
				[
					-1.3669978904951194,
					-0.9113338583575817
				],
				[
					-1.5948270095226005,
					-1.291054850819271
				],
				[
					-1.67077584328096,
					-1.442940930170939
				],
				[
					-1.7467188829568023,
					-1.5188839698467735
				],
				[
					-1.7467188829568023,
					-1.5948270095226076
				],
				[
					-1.6707758432809612,
					-1.5948270095226071
				],
				[
					-1.594827009522601,
					-1.5948270095226076
				],
				[
					-1.5188839698467735,
					-1.6707758432809676
				],
				[
					-1.2910548508192783,
					-1.6707758432809678
				],
				[
					-0.9872768980334226,
					-1.746718882956802
				],
				[
					-0.7594419849233792,
					-1.6707758432809678
				],
				[
					-0.45566403213753803,
					-1.594827009522608
				],
				[
					-0.15189187343420193,
					-1.5948270095226076
				],
				[
					0.07594303967584141,
					-1.5188839698467733
				],
				[
					0.3037779527858558,
					-1.5188839698467738
				],
				[
					0.455664032137524,
					-1.5188839698467733
				],
				[
					0.6834989452475527,
					-1.5948270095226071
				],
				[
					0.8353850245992208,
					-1.6707758432809678
				],
				[
					0.9113280642750619,
					-1.6707758432809685
				],
				[
					0.9872711039508891,
					-1.6707758432809678
				],
				[
					1.0632199377092497,
					-1.6707758432809683
				],
				[
					1.139162977385078,
					-1.6707758432809678
				],
				[
					1.2151060170609178,
					-1.7467188829568026
				],
				[
					1.2910490567367592,
					-1.8226619226326362
				],
				[
					1.3669920964125866,
					-1.8226619226326364
				],
				[
					1.4429409301709466,
					-1.8226619226326362
				],
				[
					1.5188839698467733,
					-1.8986049623084706
				],
				[
					1.5948270095226003,
					-1.8226619226326357
				],
				[
					1.6707700491984416,
					-1.8226619226326362
				],
				[
					1.5948270095226003,
					-1.7467188829568019
				],
				[
					1.518883969846774,
					-1.6707758432809678
				],
				[
					1.4429409301709466,
					-1.5948270095226076
				],
				[
					1.3669920964125866,
					-1.518883969846773
				],
				[
					1.291049056736759,
					-1.4429409301709397
				],
				[
					1.215106017060918,
					-1.2910548508192707
				],
				[
					1.0632199377092497,
					-1.1391629773850835
				],
				[
					0.9872711039508895,
					-0.9872768980334156
				],
				[
					0.9113280642750623,
					-0.911333858357581
				],
				[
					0.835385024599221,
					-0.8353850245992209
				],
				[
					0.7594419849233796,
					-0.7594419849233864
				],
				[
					0.6075501114891924,
					-0.6834989452475525
				],
				[
					0.5316070718133653,
					-0.6075559055717186
				],
				[
					0.4556640321375239,
					-0.5316128658958844
				],
				[
					0.3797209924616971,
					-0.4556640321375238
				],
				[
					0.30377795278585573,
					-0.37972099246168983
				],
				[
					0.2278291190274952,
					-0.3037779527858556
				],
				[
					0.22782911902749528,
					-0.22783491311002868
				],
				[
					0.1518860793516683,
					-0.15189187343419458
				],
				[
					0.15188607935166823,
					-0.0759430396758341
				],
				[
					0.2278291190274952,
					-0.0759430396758342
				],
				[
					0.37972099246169705,
					-0.15189187343419452
				],
				[
					0,
					0
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.171875,
				0.232421875,
				0.373046875,
				0.4453125,
				0.47265625,
				0.4912109375,
				0.5068359375,
				0.517578125,
				0.5234375,
				0.5234375,
				0.5234375,
				0.5234375,
				0.51953125,
				0.51953125,
				0.5166015625,
				0.5166015625,
				0.513671875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.513671875,
				0.51171875,
				0.51171875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.5166015625,
				0.513671875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.521484375,
				0.521484375,
				0.513671875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.4873046875,
				0.4306640625,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 1521,
			"versionNonce": 1859353758,
			"isDeleted": false,
			"id": "0WH7nkRTr6WntIEGsDfRM",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 867.3810435911147,
			"y": -1093.990270697219,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 0.2278291190275104,
			"height": 2.6580469472318646,
			"seed": 1021129445,
			"groupIds": [
				"cc6Mwfh3S8J7ftJWavf9d"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577644,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-5.356660302320523e-18,
					0.07594303967583413
				],
				[
					0.07594303967584133,
					0.22782911902750236
				],
				[
					0.07594303967584129,
					0.6075501114891994
				],
				[
					0.07594303967584137,
					0.9113280642750622
				],
				[
					0.15188607935168275,
					1.1391629773850838
				],
				[
					0.15188607935168222,
					1.44293513608842
				],
				[
					0.15188607935168275,
					1.594827009522615
				],
				[
					0.15188607935168275,
					1.8226561285501173
				],
				[
					0.1518860793516829,
					2.050491041660139
				],
				[
					0.07594303967584172,
					2.050491041660139
				],
				[
					0.0759430396758412,
					2.126434081335973
				],
				[
					0.07594303967584137,
					2.278325954770168
				],
				[
					0,
					2.4302120341218356
				],
				[
					-1.0284787780455404e-15,
					2.5061550737976703
				],
				[
					-1.7141312967425674e-16,
					2.582098113473504
				],
				[
					0,
					2.6580469472318646
				],
				[
					0.15188607935168344,
					2.6580469472318646
				],
				[
					0.22782911902750938,
					2.582098113473504
				],
				[
					0.22782911902750938,
					2.582098113473504
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.1953125,
				0.30078125,
				0.3388671875,
				0.37109375,
				0.38671875,
				0.3994140625,
				0.4111328125,
				0.42578125,
				0.4345703125,
				0.4501953125,
				0.4560546875,
				0.4677734375,
				0.470703125,
				0.470703125,
				0.470703125,
				0.470703125,
				0.474609375,
				0.3720703125,
				0.275390625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 1554,
			"versionNonce": 933667906,
			"isDeleted": false,
			"id": "H3vpPnm05jxGkbSthgupY",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 865.1027176363442,
			"y": -1091.711944742449,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 6.227421958738777,
			"height": 1.8226619226326364,
			"seed": 182423109,
			"groupIds": [
				"cc6Mwfh3S8J7ftJWavf9d"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577644,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					0.07594303967583413
				],
				[
					0.07594303967582697,
					0.15188607935166826
				],
				[
					0.22782911902750963,
					0.22782911902750236
				],
				[
					0.3037721587033365,
					0.379720992461697
				],
				[
					0.4556640321375239,
					0.5316070718133652
				],
				[
					0.6075501114891922,
					0.6834931511650263
				],
				[
					0.7594419849233937,
					0.7594419849233868
				],
				[
					0.911328064275048,
					0.8353850245992207
				],
				[
					0.9872711039508891,
					0.7594419849233868
				],
				[
					1.1391629773850909,
					0.7594419849233868
				],
				[
					1.2151060170609178,
					0.6834931511650261
				],
				[
					1.291049056736745,
					0.6075501114891922
				],
				[
					1.3669920964125721,
					0.45566403213753126
				],
				[
					1.4429351360884133,
					0.3037721587033365
				],
				[
					1.5948270095226154,
					0.07594303967583424
				],
				[
					1.7467130888742688,
					-0.07594883375836059
				],
				[
					1.82265612855011,
					-0.15189187343419439
				],
				[
					1.82265612855011,
					-0.22783491311002874
				],
				[
					1.8986049623084706,
					-0.3037779527858627
				],
				[
					1.8986049623084706,
					-0.37972099246168983
				],
				[
					1.9745480019843118,
					-0.37972099246168994
				],
				[
					1.9745480019843122,
					-0.45566982622005087
				],
				[
					2.1264340813359657,
					-0.45566982622005064
				],
				[
					2.202377121011793,
					-0.4556698262200503
				],
				[
					2.2783259547701533,
					-0.37972099246168994
				],
				[
					2.3542689944459947,
					-0.37972099246168983
				],
				[
					2.3542689944459947,
					-0.30377795278586267
				],
				[
					2.4302120341218356,
					-0.30377795278586284
				],
				[
					2.506155073797663,
					-0.30377795278586284
				],
				[
					2.506155073797663,
					-0.22783491311002874
				],
				[
					2.58209811347349,
					-0.15189187343419483
				],
				[
					2.58209811347349,
					-0.0759488337583607
				],
				[
					2.6580469472318504,
					0.15188607935166826
				],
				[
					2.7339899869076913,
					0.22782911902750236
				],
				[
					2.8858760662593594,
					0.379720992461697
				],
				[
					2.9618191059351866,
					0.5316070718133652
				],
				[
					3.037767939693547,
					0.6075501114891922
				],
				[
					3.1137109793693885,
					0.7594419849233865
				],
				[
					3.1896540190452156,
					0.8353850245992209
				],
				[
					3.3415400983968837,
					1.0632141436267233
				],
				[
					3.4174889321552437,
					1.1391629773850838
				],
				[
					3.5693750115069123,
					1.2151060170609176
				],
				[
					3.645318051182754,
					1.2151060170609178
				],
				[
					3.7972099246169413,
					1.291049056736752
				],
				[
					3.9490960039686094,
					1.291049056736752
				],
				[
					4.100982083320278,
					1.2151060170609178
				],
				[
					4.252873956754465,
					1.2151060170609178
				],
				[
					4.480703075781975,
					1.0632141436267233
				],
				[
					4.78448102856783,
					0.911328064275055
				],
				[
					5.012315941677859,
					0.6834931511650263
				],
				[
					5.240145060705355,
					0.5316070718133652
				],
				[
					5.467979973815383,
					0.3037721587033365
				],
				[
					5.695814886925412,
					0.07594303967583413
				],
				[
					5.923644005952907,
					-0.07594883375836048
				],
				[
					5.999587045628748,
					-0.1518918734341946
				],
				[
					6.075535879387094,
					-0.30377795278586284
				],
				[
					6.151478919062936,
					-0.37972099246168983
				],
				[
					6.227421958738777,
					-0.5316128658958844
				],
				[
					6.227421958738777,
					-0.5316128658958844
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.1865234375,
				0.2373046875,
				0.265625,
				0.294921875,
				0.326171875,
				0.3505859375,
				0.3662109375,
				0.373046875,
				0.3798828125,
				0.392578125,
				0.396484375,
				0.3984375,
				0.3984375,
				0.4013671875,
				0.408203125,
				0.41015625,
				0.41015625,
				0.41015625,
				0.41015625,
				0.412109375,
				0.4228515625,
				0.4140625,
				0.4072265625,
				0.4072265625,
				0.4111328125,
				0.4091796875,
				0.3955078125,
				0.3310546875,
				0.3837890625,
				0.384765625,
				0.3955078125,
				0.3974609375,
				0.3974609375,
				0.3974609375,
				0.3974609375,
				0.3974609375,
				0.3974609375,
				0.3974609375,
				0.3974609375,
				0.4013671875,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.40625,
				0.41015625,
				0.4150390625,
				0.423828125,
				0.427734375,
				0.427734375,
				0.4345703125,
				0.3779296875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 1532,
			"versionNonce": 1991653598,
			"isDeleted": false,
			"id": "QnQS5s1QqzVExaLtfNeCO",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 861.9130578232163,
			"y": -1102.192246452025,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 5.39204272822206,
			"height": 3.6453180511827465,
			"seed": 1388281253,
			"groupIds": [
				"cc6Mwfh3S8J7ftJWavf9d"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577644,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.15189187343420177,
					0.1518918734341945
				],
				[
					-0.45566403213753826,
					0.30377795278586284
				],
				[
					-0.9113338583575953,
					0.5316128658958917
				],
				[
					-1.518883969846773,
					1.2151060170609176
				],
				[
					-1.8226619226326433,
					1.7467188829568097
				],
				[
					-1.9745480019842971,
					2.2023829150943337
				],
				[
					-2.050496835742657,
					2.5061608678801965
				],
				[
					-2.0504968357426576,
					2.733989986907698
				],
				[
					-1.822661922632643,
					2.96182490001772
				],
				[
					-1.518883969846774,
					3.113710979369388
				],
				[
					-0.9872768980334224,
					3.1137109793693885
				],
				[
					-0.22783491311002887,
					2.9618249000177213
				],
				[
					0.3037779527858561,
					2.8099388206660523
				],
				[
					0.6834989452475531,
					2.58210390755603
				],
				[
					1.1391629773850762,
					2.354268994446002
				],
				[
					1.5188839698467738,
					2.050496835742665
				],
				[
					2.1264340813359652,
					1.7467188829568099
				],
				[
					2.88587606625936,
					1.139162977385084
				],
				[
					3.1137109793693876,
					0.7594419849233941
				],
				[
					3.2655970587210423,
					0.5316128658958917
				],
				[
					3.3415458924794024,
					0.3037779527858632
				],
				[
					3.2655970587210423,
					0.15189187343419447
				],
				[
					3.189654019045215,
					0
				],
				[
					2.809933026583518,
					-0.1518860793516612
				],
				[
					2.430212034121821,
					-0.303777952785856
				],
				[
					1.8986049623084706,
					-0.4556640321375241
				],
				[
					1.0632199377092495,
					-0.5316070718133581
				],
				[
					0.9113280642750622,
					-0.4556640321375239
				],
				[
					0.6075501114891921,
					-0.3797209924616898
				],
				[
					0.5316070718133652,
					-0.3797209924616899
				],
				[
					0.3037779527858557,
					-0.30377795278585573
				],
				[
					0.3037779527858556,
					-0.22782911902749525
				],
				[
					0.3797209924616826,
					-0.2278291190274952
				],
				[
					0,
					0
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.171875,
				0.201171875,
				0.2529296875,
				0.3037109375,
				0.361328125,
				0.38671875,
				0.4130859375,
				0.423828125,
				0.42578125,
				0.42578125,
				0.419921875,
				0.4150390625,
				0.4033203125,
				0.400390625,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.408203125,
				0.4306640625,
				0.45703125,
				0.47265625,
				0.4775390625,
				0.482421875,
				0.4951171875,
				0.4970703125,
				0.4970703125,
				0.4970703125,
				0.466796875,
				0.4140625,
				0.0263671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 1532,
			"versionNonce": 562875394,
			"isDeleted": false,
			"id": "G6NoYjob-XYgW_JKWj8iN",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 873.0768526839576,
			"y": -1102.9516884369484,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 4.556651909540335,
			"height": 3.4174889321552446,
			"seed": 732594437,
			"groupIds": [
				"cc6Mwfh3S8J7ftJWavf9d"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577644,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.15188607935165394,
					-0.07594303967583418
				],
				[
					-0.6075501114892065,
					-0.07594303967583416
				],
				[
					-0.9872711039508748,
					-8.570656483712831e-17
				],
				[
					-1.3669920964125717,
					0.22783491311002857
				],
				[
					-1.746713088874269,
					0.5316128658958919
				],
				[
					-2.202382915094326,
					1.0632199377092497
				],
				[
					-2.3542689944460085,
					1.5188839698467806
				],
				[
					-2.278325954770153,
					1.9745480019843047
				],
				[
					-2.0504910416601385,
					2.354268994446002
				],
				[
					-1.7467130888742697,
					2.658046947231858
				],
				[
					-1.1391629773850909,
					2.8858818603418865
				],
				[
					-0.7594419849233935,
					2.961824900017721
				],
				[
					-0.30377795278586966,
					2.885881860341886
				],
				[
					0.07594303967582673,
					2.7339899869076913
				],
				[
					0.8353850245992208,
					2.354268994446002
				],
				[
					1.4429409301709326,
					1.9745480019843042
				],
				[
					1.8226619226326288,
					1.6707758432809685
				],
				[
					2.0504968357426727,
					1.3669978904951126
				],
				[
					2.202382915094326,
					1.0632199377092504
				],
				[
					2.202382915094326,
					0.7594419849233874
				],
				[
					2.202382915094326,
					0.5316128658958911
				],
				[
					2.126439875418499,
					0.30377795278586267
				],
				[
					1.9745480019843116,
					0
				],
				[
					1.6707758432809752,
					-0.15188607935166806
				],
				[
					0.9113338583575813,
					-0.3797209924616896
				],
				[
					0.30377795278586994,
					-0.455664032137524
				],
				[
					-0.07594303967582688,
					-0.455664032137524
				],
				[
					-0.45566403213752393,
					-0.30377795278586284
				],
				[
					-0.7594419849233939,
					-0.15188607935166815
				],
				[
					-0.9872711039508748,
					-8.570656483712831e-17
				],
				[
					-0.9872711039508749,
					0.15189187343419472
				],
				[
					-0.9872711039508749,
					0.3797209924616973
				],
				[
					0,
					0
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.173828125,
				0.1923828125,
				0.294921875,
				0.3798828125,
				0.447265625,
				0.4873046875,
				0.4912109375,
				0.486328125,
				0.484375,
				0.482421875,
				0.48046875,
				0.4697265625,
				0.4658203125,
				0.470703125,
				0.4677734375,
				0.474609375,
				0.4765625,
				0.4765625,
				0.478515625,
				0.48046875,
				0.4921875,
				0.4951171875,
				0.5,
				0.5126953125,
				0.521484375,
				0.5234375,
				0.525390625,
				0.525390625,
				0.525390625,
				0.505859375,
				0.423828125,
				0.1904296875,
				0.01171875,
				0
			]
		},
		{
			"type": "rectangle",
			"version": 1516,
			"versionNonce": 595029278,
			"isDeleted": false,
			"id": "wvxDO5UCTTwsPWNllWZAj",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1000.160257299415,
			"y": -1237.6866338820619,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 3.6755016503132074,
			"height": 464.14185022568955,
			"seed": 1068965253,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577644,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 1556,
			"versionNonce": 64486338,
			"isDeleted": false,
			"id": "ONURK3ECReH6yeMUJpJZB",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1020.3244226207514,
			"y": -856.2983113959014,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 118.84431563405535,
			"height": 76.54774988857169,
			"seed": 909416485,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577644,
			"link": null,
			"locked": false
		},
		{
			"type": "ellipse",
			"version": 1781,
			"versionNonce": 1116215646,
			"isDeleted": false,
			"id": "G4rrr6bmbbIgHxnuJT42Y",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1220.4375057382465,
			"y": -895.5882910996846,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 27.292840097560045,
			"height": 23.326046508023218,
			"seed": 1184385925,
			"groupIds": [
				"_6_Tlu4gaIHZ9zC8NXi4v"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692815577644,
			"link": null,
			"locked": false
		},
		{
			"type": "freedraw",
			"version": 1563,
			"versionNonce": 480719746,
			"isDeleted": false,
			"id": "s7U8cY111-LM6eKyztpjk",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1221.4715124269176,
			"y": -889.2252506765134,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 5.9641894286609345,
			"height": 9.759576433798838,
			"seed": 720278245,
			"groupIds": [
				"_6_Tlu4gaIHZ9zC8NXi4v"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577644,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					-0.18073008808811764
				],
				[
					0,
					-0.36146017617623527
				],
				[
					-5.594217597396797e-17,
					-0.9036642292624609
				],
				[
					0.18073008808811777,
					-1.62659837043679
				],
				[
					0.18073008808811789,
					-2.710992687787354
				],
				[
					0.18073008808811766,
					-4.518321146312261
				],
				[
					0.18073008808811766,
					-5.964175639839061
				],
				[
					0,
					-7.048583746011483
				],
				[
					0,
					-7.771504098363969
				],
				[
					0,
					-8.675168327626416
				],
				[
					0,
					-8.855912204536391
				],
				[
					0,
					-9.217372380712627
				],
				[
					0,
					-9.398102468800744
				],
				[
					0,
					-9.578832556888862
				],
				[
					0,
					-9.759576433798838
				],
				[
					0.18073008808811766,
					-9.759576433798838
				],
				[
					0.5422040530862257,
					-9.759576433798838
				],
				[
					0.903664229262461,
					-9.578832556888862
				],
				[
					1.6265983704368043,
					-8.855912204536391
				],
				[
					1.807328458524922,
					-8.494438239538297
				],
				[
					2.1688024235230015,
					-7.952247975273944
				],
				[
					2.349532511611119,
					-7.410043922187718
				],
				[
					2.530262599699237,
					-7.048583746011483
				],
				[
					2.891722775875472,
					-6.68710978101339
				],
				[
					3.0724666527854625,
					-6.506379692925272
				],
				[
					3.2531967408735802,
					-6.325649604837155
				],
				[
					3.433926828961698,
					-5.964175639839061
				],
				[
					3.7953870051379335,
					-5.24125528748659
				],
				[
					3.976130882047895,
					-4.879781322488497
				],
				[
					4.518321146312248,
					-4.699051234400379
				],
				[
					5.241255287486591,
					-4.879781322488497
				],
				[
					5.9641894286609345,
					-5.421985375574708
				],
				[
					5.9641894286609345,
					-5.421985375574708
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.181640625,
				0.21484375,
				0.310546875,
				0.359375,
				0.40625,
				0.447265625,
				0.4853515625,
				0.49609375,
				0.501953125,
				0.51171875,
				0.5185546875,
				0.521484375,
				0.5263671875,
				0.53515625,
				0.5263671875,
				0.5263671875,
				0.53125,
				0.529296875,
				0.529296875,
				0.529296875,
				0.52734375,
				0.52734375,
				0.52734375,
				0.52734375,
				0.52734375,
				0.52734375,
				0.52734375,
				0.52734375,
				0.5302734375,
				0.537109375,
				0.529296875,
				0.4189453125,
				0.015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 1565,
			"versionNonce": 1262042526,
			"isDeleted": false,
			"id": "5S2f7cYDi8Mo22tiCz13t",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1240.6291913295179,
			"y": -893.3820978578273,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 5.42198537557468,
			"height": 9.578846345710721,
			"seed": 1875177029,
			"groupIds": [
				"_6_Tlu4gaIHZ9zC8NXi4v"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577644,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					-0.361473964998108
				],
				[
					0.18074387690996163,
					-0.361473964998108
				],
				[
					0.542204053086197,
					-1.2651381942605546
				],
				[
					1.2651381942605402,
					-1.9880723354348837
				],
				[
					1.9880723354348546,
					-2.8917365646973305
				],
				[
					3.0724666527854336,
					-3.6146569170498157
				],
				[
					3.795400793959777,
					-4.337591058224144
				],
				[
					4.518321146312247,
					-5.241255287486591
				],
				[
					4.699065023222209,
					-5.602729252484685
				],
				[
					5.060525199398445,
					-5.7834593405728025
				],
				[
					5.241255287486562,
					-5.96418942866092
				],
				[
					5.42198537557468,
					-5.96418942866092
				],
				[
					5.42198537557468,
					-5.602729252484685
				],
				[
					5.42198537557468,
					-5.060525199398474
				],
				[
					5.42198537557468,
					-4.337591058224144
				],
				[
					5.42198537557468,
					-3.6146569170498157
				],
				[
					5.42198537557468,
					-2.7109926877873542
				],
				[
					5.241255287486562,
					-1.9880723354348837
				],
				[
					5.241255287486562,
					-1.2651381942605546
				],
				[
					5.241255287486562,
					-0.361473964998108
				],
				[
					5.060525199398445,
					0.3614601761762353
				],
				[
					4.879795111310327,
					1.0843943173505644
				],
				[
					4.699065023222209,
					1.8073284585248934
				],
				[
					4.699065023222209,
					1.9880585466130112
				],
				[
					4.699065023222209,
					2.1687886347011287
				],
				[
					4.699065023222209,
					2.530248810877364
				],
				[
					4.518321146312247,
					2.891722775875458
				],
				[
					4.518321146312247,
					3.253182952051693
				],
				[
					4.518321146312247,
					3.433913040139825
				],
				[
					4.699065023222209,
					3.614656917049801
				],
				[
					4.879795111310327,
					3.614656917049801
				],
				[
					5.241255287486562,
					3.614656917049801
				],
				[
					5.241255287486562,
					3.614656917049801
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.177734375,
				0.2587890625,
				0.28125,
				0.3544921875,
				0.388671875,
				0.408203125,
				0.4228515625,
				0.435546875,
				0.455078125,
				0.4658203125,
				0.4736328125,
				0.486328125,
				0.4951171875,
				0.5126953125,
				0.5126953125,
				0.5126953125,
				0.5126953125,
				0.5126953125,
				0.51171875,
				0.51171875,
				0.51171875,
				0.517578125,
				0.51953125,
				0.525390625,
				0.525390625,
				0.525390625,
				0.525390625,
				0.525390625,
				0.53125,
				0.515625,
				0.486328125,
				0.296875,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 1592,
			"versionNonce": 238646082,
			"isDeleted": false,
			"id": "G2se5DPBJRM7eRxTL3Yo_",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1233.185435200858,
			"y": -881.6310667376373,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 3.4174889321552437,
			"height": 1.8986049623084706,
			"seed": 871947685,
			"groupIds": [
				"_6_Tlu4gaIHZ9zC8NXi4v"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577644,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.07594303967584129,
					0
				],
				[
					-0.15189187343420177,
					-3.213996181392311e-17
				],
				[
					-0.22783491311002868,
					-0.15189187343419458
				],
				[
					-0.45566403213753826,
					-0.3037779527858557
				],
				[
					-0.7594419849233793,
					-0.5316128658958847
				],
				[
					-1.1391629773850764,
					-0.6834989452475524
				],
				[
					-1.3669978904951194,
					-0.9113338583575817
				],
				[
					-1.5948270095226005,
					-1.291054850819271
				],
				[
					-1.67077584328096,
					-1.442940930170939
				],
				[
					-1.7467188829568023,
					-1.5188839698467735
				],
				[
					-1.7467188829568023,
					-1.5948270095226076
				],
				[
					-1.6707758432809612,
					-1.5948270095226071
				],
				[
					-1.594827009522601,
					-1.5948270095226076
				],
				[
					-1.5188839698467735,
					-1.6707758432809676
				],
				[
					-1.2910548508192783,
					-1.6707758432809678
				],
				[
					-0.9872768980334226,
					-1.746718882956802
				],
				[
					-0.7594419849233792,
					-1.6707758432809678
				],
				[
					-0.45566403213753803,
					-1.594827009522608
				],
				[
					-0.15189187343420193,
					-1.5948270095226076
				],
				[
					0.07594303967584141,
					-1.5188839698467733
				],
				[
					0.3037779527858558,
					-1.5188839698467738
				],
				[
					0.455664032137524,
					-1.5188839698467733
				],
				[
					0.6834989452475527,
					-1.5948270095226071
				],
				[
					0.8353850245992208,
					-1.6707758432809678
				],
				[
					0.9113280642750619,
					-1.6707758432809685
				],
				[
					0.9872711039508891,
					-1.6707758432809678
				],
				[
					1.0632199377092497,
					-1.6707758432809683
				],
				[
					1.139162977385078,
					-1.6707758432809678
				],
				[
					1.2151060170609178,
					-1.7467188829568026
				],
				[
					1.2910490567367592,
					-1.8226619226326362
				],
				[
					1.3669920964125866,
					-1.8226619226326364
				],
				[
					1.4429409301709466,
					-1.8226619226326362
				],
				[
					1.5188839698467733,
					-1.8986049623084706
				],
				[
					1.5948270095226003,
					-1.8226619226326357
				],
				[
					1.6707700491984416,
					-1.8226619226326362
				],
				[
					1.5948270095226003,
					-1.7467188829568019
				],
				[
					1.518883969846774,
					-1.6707758432809678
				],
				[
					1.4429409301709466,
					-1.5948270095226076
				],
				[
					1.3669920964125866,
					-1.518883969846773
				],
				[
					1.291049056736759,
					-1.4429409301709397
				],
				[
					1.215106017060918,
					-1.2910548508192707
				],
				[
					1.0632199377092497,
					-1.1391629773850835
				],
				[
					0.9872711039508895,
					-0.9872768980334156
				],
				[
					0.9113280642750623,
					-0.911333858357581
				],
				[
					0.835385024599221,
					-0.8353850245992209
				],
				[
					0.7594419849233796,
					-0.7594419849233864
				],
				[
					0.6075501114891924,
					-0.6834989452475525
				],
				[
					0.5316070718133653,
					-0.6075559055717186
				],
				[
					0.4556640321375239,
					-0.5316128658958844
				],
				[
					0.3797209924616971,
					-0.4556640321375238
				],
				[
					0.30377795278585573,
					-0.37972099246168983
				],
				[
					0.2278291190274952,
					-0.3037779527858556
				],
				[
					0.22782911902749528,
					-0.22783491311002868
				],
				[
					0.1518860793516683,
					-0.15189187343419458
				],
				[
					0.15188607935166823,
					-0.0759430396758341
				],
				[
					0.2278291190274952,
					-0.0759430396758342
				],
				[
					0.37972099246169705,
					-0.15189187343419452
				],
				[
					0,
					0
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.171875,
				0.232421875,
				0.373046875,
				0.4453125,
				0.47265625,
				0.4912109375,
				0.5068359375,
				0.517578125,
				0.5234375,
				0.5234375,
				0.5234375,
				0.5234375,
				0.51953125,
				0.51953125,
				0.5166015625,
				0.5166015625,
				0.513671875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.513671875,
				0.51171875,
				0.51171875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.5166015625,
				0.513671875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.521484375,
				0.521484375,
				0.513671875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.4873046875,
				0.4306640625,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 1552,
			"versionNonce": 582736350,
			"isDeleted": false,
			"id": "XeezJx13CzIFBKAcB_get",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1232.7297711687204,
			"y": -880.9475677923896,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 0.2278291190275104,
			"height": 2.6580469472318646,
			"seed": 1589108997,
			"groupIds": [
				"_6_Tlu4gaIHZ9zC8NXi4v"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577644,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-5.356660302320523e-18,
					0.07594303967583413
				],
				[
					0.07594303967584133,
					0.22782911902750236
				],
				[
					0.07594303967584129,
					0.6075501114891994
				],
				[
					0.07594303967584137,
					0.9113280642750622
				],
				[
					0.15188607935168275,
					1.1391629773850838
				],
				[
					0.15188607935168222,
					1.44293513608842
				],
				[
					0.15188607935168275,
					1.594827009522615
				],
				[
					0.15188607935168275,
					1.8226561285501173
				],
				[
					0.1518860793516829,
					2.050491041660139
				],
				[
					0.07594303967584172,
					2.050491041660139
				],
				[
					0.0759430396758412,
					2.126434081335973
				],
				[
					0.07594303967584137,
					2.278325954770168
				],
				[
					0,
					2.4302120341218356
				],
				[
					-1.0284787780455404e-15,
					2.5061550737976703
				],
				[
					-1.7141312967425674e-16,
					2.582098113473504
				],
				[
					0,
					2.6580469472318646
				],
				[
					0.15188607935168344,
					2.6580469472318646
				],
				[
					0.22782911902750938,
					2.582098113473504
				],
				[
					0.22782911902750938,
					2.582098113473504
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.1953125,
				0.30078125,
				0.3388671875,
				0.37109375,
				0.38671875,
				0.3994140625,
				0.4111328125,
				0.42578125,
				0.4345703125,
				0.4501953125,
				0.4560546875,
				0.4677734375,
				0.470703125,
				0.470703125,
				0.470703125,
				0.470703125,
				0.474609375,
				0.3720703125,
				0.275390625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 1585,
			"versionNonce": 1525529346,
			"isDeleted": false,
			"id": "wRfUi3YrfhdAyokgVqZxj",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1230.45144521395,
			"y": -878.6692418376196,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 6.227421958738777,
			"height": 1.8226619226326364,
			"seed": 360675429,
			"groupIds": [
				"_6_Tlu4gaIHZ9zC8NXi4v"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577644,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					0.07594303967583413
				],
				[
					0.07594303967582697,
					0.15188607935166826
				],
				[
					0.22782911902750963,
					0.22782911902750236
				],
				[
					0.3037721587033365,
					0.379720992461697
				],
				[
					0.4556640321375239,
					0.5316070718133652
				],
				[
					0.6075501114891922,
					0.6834931511650263
				],
				[
					0.7594419849233937,
					0.7594419849233868
				],
				[
					0.911328064275048,
					0.8353850245992207
				],
				[
					0.9872711039508891,
					0.7594419849233868
				],
				[
					1.1391629773850909,
					0.7594419849233868
				],
				[
					1.2151060170609178,
					0.6834931511650261
				],
				[
					1.291049056736745,
					0.6075501114891922
				],
				[
					1.3669920964125721,
					0.45566403213753126
				],
				[
					1.4429351360884133,
					0.3037721587033365
				],
				[
					1.5948270095226154,
					0.07594303967583424
				],
				[
					1.7467130888742688,
					-0.07594883375836059
				],
				[
					1.82265612855011,
					-0.15189187343419439
				],
				[
					1.82265612855011,
					-0.22783491311002874
				],
				[
					1.8986049623084706,
					-0.3037779527858627
				],
				[
					1.8986049623084706,
					-0.37972099246168983
				],
				[
					1.9745480019843118,
					-0.37972099246168994
				],
				[
					1.9745480019843122,
					-0.45566982622005087
				],
				[
					2.1264340813359657,
					-0.45566982622005064
				],
				[
					2.202377121011793,
					-0.4556698262200503
				],
				[
					2.2783259547701533,
					-0.37972099246168994
				],
				[
					2.3542689944459947,
					-0.37972099246168983
				],
				[
					2.3542689944459947,
					-0.30377795278586267
				],
				[
					2.4302120341218356,
					-0.30377795278586284
				],
				[
					2.506155073797663,
					-0.30377795278586284
				],
				[
					2.506155073797663,
					-0.22783491311002874
				],
				[
					2.58209811347349,
					-0.15189187343419483
				],
				[
					2.58209811347349,
					-0.0759488337583607
				],
				[
					2.6580469472318504,
					0.15188607935166826
				],
				[
					2.7339899869076913,
					0.22782911902750236
				],
				[
					2.8858760662593594,
					0.379720992461697
				],
				[
					2.9618191059351866,
					0.5316070718133652
				],
				[
					3.037767939693547,
					0.6075501114891922
				],
				[
					3.1137109793693885,
					0.7594419849233865
				],
				[
					3.1896540190452156,
					0.8353850245992209
				],
				[
					3.3415400983968837,
					1.0632141436267233
				],
				[
					3.4174889321552437,
					1.1391629773850838
				],
				[
					3.5693750115069123,
					1.2151060170609176
				],
				[
					3.645318051182754,
					1.2151060170609178
				],
				[
					3.7972099246169413,
					1.291049056736752
				],
				[
					3.9490960039686094,
					1.291049056736752
				],
				[
					4.100982083320278,
					1.2151060170609178
				],
				[
					4.252873956754465,
					1.2151060170609178
				],
				[
					4.480703075781975,
					1.0632141436267233
				],
				[
					4.78448102856783,
					0.911328064275055
				],
				[
					5.012315941677859,
					0.6834931511650263
				],
				[
					5.240145060705355,
					0.5316070718133652
				],
				[
					5.467979973815383,
					0.3037721587033365
				],
				[
					5.695814886925412,
					0.07594303967583413
				],
				[
					5.923644005952907,
					-0.07594883375836048
				],
				[
					5.999587045628748,
					-0.1518918734341946
				],
				[
					6.075535879387094,
					-0.30377795278586284
				],
				[
					6.151478919062936,
					-0.37972099246168983
				],
				[
					6.227421958738777,
					-0.5316128658958844
				],
				[
					6.227421958738777,
					-0.5316128658958844
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.1865234375,
				0.2373046875,
				0.265625,
				0.294921875,
				0.326171875,
				0.3505859375,
				0.3662109375,
				0.373046875,
				0.3798828125,
				0.392578125,
				0.396484375,
				0.3984375,
				0.3984375,
				0.4013671875,
				0.408203125,
				0.41015625,
				0.41015625,
				0.41015625,
				0.41015625,
				0.412109375,
				0.4228515625,
				0.4140625,
				0.4072265625,
				0.4072265625,
				0.4111328125,
				0.4091796875,
				0.3955078125,
				0.3310546875,
				0.3837890625,
				0.384765625,
				0.3955078125,
				0.3974609375,
				0.3974609375,
				0.3974609375,
				0.3974609375,
				0.3974609375,
				0.3974609375,
				0.3974609375,
				0.3974609375,
				0.4013671875,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.40625,
				0.41015625,
				0.4150390625,
				0.423828125,
				0.427734375,
				0.427734375,
				0.4345703125,
				0.3779296875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 1563,
			"versionNonce": 1612770846,
			"isDeleted": false,
			"id": "COJDLy1NOnFLV5sz99MDG",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1227.261785400822,
			"y": -889.1495435471955,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 5.39204272822206,
			"height": 3.6453180511827465,
			"seed": 1914512325,
			"groupIds": [
				"_6_Tlu4gaIHZ9zC8NXi4v"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577644,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.15189187343420177,
					0.1518918734341945
				],
				[
					-0.45566403213753826,
					0.30377795278586284
				],
				[
					-0.9113338583575953,
					0.5316128658958917
				],
				[
					-1.518883969846773,
					1.2151060170609176
				],
				[
					-1.8226619226326433,
					1.7467188829568097
				],
				[
					-1.9745480019842971,
					2.2023829150943337
				],
				[
					-2.050496835742657,
					2.5061608678801965
				],
				[
					-2.0504968357426576,
					2.733989986907698
				],
				[
					-1.822661922632643,
					2.96182490001772
				],
				[
					-1.518883969846774,
					3.113710979369388
				],
				[
					-0.9872768980334224,
					3.1137109793693885
				],
				[
					-0.22783491311002887,
					2.9618249000177213
				],
				[
					0.3037779527858561,
					2.8099388206660523
				],
				[
					0.6834989452475531,
					2.58210390755603
				],
				[
					1.1391629773850762,
					2.354268994446002
				],
				[
					1.5188839698467738,
					2.050496835742665
				],
				[
					2.1264340813359652,
					1.7467188829568099
				],
				[
					2.88587606625936,
					1.139162977385084
				],
				[
					3.1137109793693876,
					0.7594419849233941
				],
				[
					3.2655970587210423,
					0.5316128658958917
				],
				[
					3.3415458924794024,
					0.3037779527858632
				],
				[
					3.2655970587210423,
					0.15189187343419447
				],
				[
					3.189654019045215,
					0
				],
				[
					2.809933026583518,
					-0.1518860793516612
				],
				[
					2.430212034121821,
					-0.303777952785856
				],
				[
					1.8986049623084706,
					-0.4556640321375241
				],
				[
					1.0632199377092495,
					-0.5316070718133581
				],
				[
					0.9113280642750622,
					-0.4556640321375239
				],
				[
					0.6075501114891921,
					-0.3797209924616898
				],
				[
					0.5316070718133652,
					-0.3797209924616899
				],
				[
					0.3037779527858557,
					-0.30377795278585573
				],
				[
					0.3037779527858556,
					-0.22782911902749525
				],
				[
					0.3797209924616826,
					-0.2278291190274952
				],
				[
					0,
					0
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.171875,
				0.201171875,
				0.2529296875,
				0.3037109375,
				0.361328125,
				0.38671875,
				0.4130859375,
				0.423828125,
				0.42578125,
				0.42578125,
				0.419921875,
				0.4150390625,
				0.4033203125,
				0.400390625,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.408203125,
				0.4306640625,
				0.45703125,
				0.47265625,
				0.4775390625,
				0.482421875,
				0.4951171875,
				0.4970703125,
				0.4970703125,
				0.4970703125,
				0.466796875,
				0.4140625,
				0.0263671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 1563,
			"versionNonce": 1631783618,
			"isDeleted": false,
			"id": "6iD0jC2-eMElQoZafYZ6x",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1238.4255802615633,
			"y": -889.9089855321189,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 4.556651909540335,
			"height": 3.4174889321552446,
			"seed": 2024694565,
			"groupIds": [
				"_6_Tlu4gaIHZ9zC8NXi4v"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577644,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.15188607935165394,
					-0.07594303967583418
				],
				[
					-0.6075501114892065,
					-0.07594303967583416
				],
				[
					-0.9872711039508748,
					-8.570656483712831e-17
				],
				[
					-1.3669920964125717,
					0.22783491311002857
				],
				[
					-1.746713088874269,
					0.5316128658958919
				],
				[
					-2.202382915094326,
					1.0632199377092497
				],
				[
					-2.3542689944460085,
					1.5188839698467806
				],
				[
					-2.278325954770153,
					1.9745480019843047
				],
				[
					-2.0504910416601385,
					2.354268994446002
				],
				[
					-1.7467130888742697,
					2.658046947231858
				],
				[
					-1.1391629773850909,
					2.8858818603418865
				],
				[
					-0.7594419849233935,
					2.961824900017721
				],
				[
					-0.30377795278586966,
					2.885881860341886
				],
				[
					0.07594303967582673,
					2.7339899869076913
				],
				[
					0.8353850245992208,
					2.354268994446002
				],
				[
					1.4429409301709326,
					1.9745480019843042
				],
				[
					1.8226619226326288,
					1.6707758432809685
				],
				[
					2.0504968357426727,
					1.3669978904951126
				],
				[
					2.202382915094326,
					1.0632199377092504
				],
				[
					2.202382915094326,
					0.7594419849233874
				],
				[
					2.202382915094326,
					0.5316128658958911
				],
				[
					2.126439875418499,
					0.30377795278586267
				],
				[
					1.9745480019843116,
					0
				],
				[
					1.6707758432809752,
					-0.15188607935166806
				],
				[
					0.9113338583575813,
					-0.3797209924616896
				],
				[
					0.30377795278586994,
					-0.455664032137524
				],
				[
					-0.07594303967582688,
					-0.455664032137524
				],
				[
					-0.45566403213752393,
					-0.30377795278586284
				],
				[
					-0.7594419849233939,
					-0.15188607935166815
				],
				[
					-0.9872711039508748,
					-8.570656483712831e-17
				],
				[
					-0.9872711039508749,
					0.15189187343419472
				],
				[
					-0.9872711039508749,
					0.3797209924616973
				],
				[
					0,
					0
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.173828125,
				0.1923828125,
				0.294921875,
				0.3798828125,
				0.447265625,
				0.4873046875,
				0.4912109375,
				0.486328125,
				0.484375,
				0.482421875,
				0.48046875,
				0.4697265625,
				0.4658203125,
				0.470703125,
				0.4677734375,
				0.474609375,
				0.4765625,
				0.4765625,
				0.478515625,
				0.48046875,
				0.4921875,
				0.4951171875,
				0.5,
				0.5126953125,
				0.521484375,
				0.5234375,
				0.525390625,
				0.525390625,
				0.525390625,
				0.505859375,
				0.423828125,
				0.1904296875,
				0.01171875,
				0
			]
		},
		{
			"type": "rectangle",
			"version": 513,
			"versionNonce": 274299486,
			"isDeleted": false,
			"id": "QXOX05LU1Kka7qbHjCl6y",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1115.2937561332212,
			"y": -903.7878913827086,
			"strokeColor": "#1971c2",
			"backgroundColor": "#a5d8ff",
			"width": 30.222167968750455,
			"height": 29.333428276909782,
			"seed": 1302378117,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577644,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 1656,
			"versionNonce": 1473798786,
			"isDeleted": false,
			"id": "ZOri5qLJKbhaCVn9-hWUr",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1161.316594762983,
			"y": -846.348741698018,
			"strokeColor": "#2f9e44",
			"backgroundColor": "#b2f2bb",
			"width": 153.39518267385216,
			"height": 16.365029766123357,
			"seed": 733060581,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577644,
			"link": null,
			"locked": false
		},
		{
			"type": "arrow",
			"version": 65,
			"versionNonce": 2050391710,
			"isDeleted": false,
			"id": "pI0QV_QqRN7-_5o7toGY7",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1239.408228720584,
			"y": -811.179223969911,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#b2f2bb",
			"width": 1.8876796926788302,
			"height": 43.416632931612526,
			"seed": 916009061,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692815577644,
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
					-1.8876796926788302,
					43.416632931612526
				]
			]
		},
		{
			"type": "rectangle",
			"version": 1536,
			"versionNonce": 1231864386,
			"isDeleted": false,
			"id": "FBLP8Y5k8IfwbI7glAR8P",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1393.9072488632335,
			"y": -1233.4055818606748,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 3.6755016503132074,
			"height": 464.14185022568955,
			"seed": 1484494091,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577644,
			"link": null,
			"locked": false
		},
		{
			"type": "rectangle",
			"version": 1719,
			"versionNonce": 1651047134,
			"isDeleted": false,
			"id": "jsuyd1CMW1PlgJhAKUuQD",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1415.1205578637505,
			"y": -1234.5402670055835,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e1e1e",
			"width": 118.84431563405535,
			"height": 444.75342854661903,
			"seed": 823020581,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577644,
			"link": null,
			"locked": false
		},
		{
			"type": "ellipse",
			"version": 1942,
			"versionNonce": 283060738,
			"isDeleted": false,
			"id": "OxQ_jr437RKH2BpV0dp6r",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1615.2336409812456,
			"y": -950.919711060841,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 27.292840097560045,
			"height": 23.326046508023218,
			"seed": 605781893,
			"groupIds": [
				"ENAXjbMgandSiynAsjaLg"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692815577644,
			"link": null,
			"locked": false
		},
		{
			"type": "freedraw",
			"version": 1724,
			"versionNonce": 1333915422,
			"isDeleted": false,
			"id": "KAPEtir5YpVEx-r-4n5qi",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1616.2676476699166,
			"y": -944.5566706376698,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 5.9641894286609345,
			"height": 9.759576433798838,
			"seed": 1508591333,
			"groupIds": [
				"ENAXjbMgandSiynAsjaLg"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577644,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					-0.18073008808811764
				],
				[
					0,
					-0.36146017617623527
				],
				[
					-5.594217597396797e-17,
					-0.9036642292624609
				],
				[
					0.18073008808811777,
					-1.62659837043679
				],
				[
					0.18073008808811789,
					-2.710992687787354
				],
				[
					0.18073008808811766,
					-4.518321146312261
				],
				[
					0.18073008808811766,
					-5.964175639839061
				],
				[
					0,
					-7.048583746011483
				],
				[
					0,
					-7.771504098363969
				],
				[
					0,
					-8.675168327626416
				],
				[
					0,
					-8.855912204536391
				],
				[
					0,
					-9.217372380712627
				],
				[
					0,
					-9.398102468800744
				],
				[
					0,
					-9.578832556888862
				],
				[
					0,
					-9.759576433798838
				],
				[
					0.18073008808811766,
					-9.759576433798838
				],
				[
					0.5422040530862257,
					-9.759576433798838
				],
				[
					0.903664229262461,
					-9.578832556888862
				],
				[
					1.6265983704368043,
					-8.855912204536391
				],
				[
					1.807328458524922,
					-8.494438239538297
				],
				[
					2.1688024235230015,
					-7.952247975273944
				],
				[
					2.349532511611119,
					-7.410043922187718
				],
				[
					2.530262599699237,
					-7.048583746011483
				],
				[
					2.891722775875472,
					-6.68710978101339
				],
				[
					3.0724666527854625,
					-6.506379692925272
				],
				[
					3.2531967408735802,
					-6.325649604837155
				],
				[
					3.433926828961698,
					-5.964175639839061
				],
				[
					3.7953870051379335,
					-5.24125528748659
				],
				[
					3.976130882047895,
					-4.879781322488497
				],
				[
					4.518321146312248,
					-4.699051234400379
				],
				[
					5.241255287486591,
					-4.879781322488497
				],
				[
					5.9641894286609345,
					-5.421985375574708
				],
				[
					5.9641894286609345,
					-5.421985375574708
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.181640625,
				0.21484375,
				0.310546875,
				0.359375,
				0.40625,
				0.447265625,
				0.4853515625,
				0.49609375,
				0.501953125,
				0.51171875,
				0.5185546875,
				0.521484375,
				0.5263671875,
				0.53515625,
				0.5263671875,
				0.5263671875,
				0.53125,
				0.529296875,
				0.529296875,
				0.529296875,
				0.52734375,
				0.52734375,
				0.52734375,
				0.52734375,
				0.52734375,
				0.52734375,
				0.52734375,
				0.52734375,
				0.5302734375,
				0.537109375,
				0.529296875,
				0.4189453125,
				0.015625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 1726,
			"versionNonce": 1429117378,
			"isDeleted": false,
			"id": "Ohm35d9UAJCN-jRRfpVrk",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1635.425326572517,
			"y": -948.7135178189836,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 5.42198537557468,
			"height": 9.578846345710721,
			"seed": 84615749,
			"groupIds": [
				"ENAXjbMgandSiynAsjaLg"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577644,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					-0.361473964998108
				],
				[
					0.18074387690996163,
					-0.361473964998108
				],
				[
					0.542204053086197,
					-1.2651381942605546
				],
				[
					1.2651381942605402,
					-1.9880723354348837
				],
				[
					1.9880723354348546,
					-2.8917365646973305
				],
				[
					3.0724666527854336,
					-3.6146569170498157
				],
				[
					3.795400793959777,
					-4.337591058224144
				],
				[
					4.518321146312247,
					-5.241255287486591
				],
				[
					4.699065023222209,
					-5.602729252484685
				],
				[
					5.060525199398445,
					-5.7834593405728025
				],
				[
					5.241255287486562,
					-5.96418942866092
				],
				[
					5.42198537557468,
					-5.96418942866092
				],
				[
					5.42198537557468,
					-5.602729252484685
				],
				[
					5.42198537557468,
					-5.060525199398474
				],
				[
					5.42198537557468,
					-4.337591058224144
				],
				[
					5.42198537557468,
					-3.6146569170498157
				],
				[
					5.42198537557468,
					-2.7109926877873542
				],
				[
					5.241255287486562,
					-1.9880723354348837
				],
				[
					5.241255287486562,
					-1.2651381942605546
				],
				[
					5.241255287486562,
					-0.361473964998108
				],
				[
					5.060525199398445,
					0.3614601761762353
				],
				[
					4.879795111310327,
					1.0843943173505644
				],
				[
					4.699065023222209,
					1.8073284585248934
				],
				[
					4.699065023222209,
					1.9880585466130112
				],
				[
					4.699065023222209,
					2.1687886347011287
				],
				[
					4.699065023222209,
					2.530248810877364
				],
				[
					4.518321146312247,
					2.891722775875458
				],
				[
					4.518321146312247,
					3.253182952051693
				],
				[
					4.518321146312247,
					3.433913040139825
				],
				[
					4.699065023222209,
					3.614656917049801
				],
				[
					4.879795111310327,
					3.614656917049801
				],
				[
					5.241255287486562,
					3.614656917049801
				],
				[
					5.241255287486562,
					3.614656917049801
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.177734375,
				0.2587890625,
				0.28125,
				0.3544921875,
				0.388671875,
				0.408203125,
				0.4228515625,
				0.435546875,
				0.455078125,
				0.4658203125,
				0.4736328125,
				0.486328125,
				0.4951171875,
				0.5126953125,
				0.5126953125,
				0.5126953125,
				0.5126953125,
				0.5126953125,
				0.51171875,
				0.51171875,
				0.51171875,
				0.517578125,
				0.51953125,
				0.525390625,
				0.525390625,
				0.525390625,
				0.525390625,
				0.525390625,
				0.53125,
				0.515625,
				0.486328125,
				0.296875,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 1753,
			"versionNonce": 1307728734,
			"isDeleted": false,
			"id": "SvUZ459N4QwDMVUWVO_ZH",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1627.9815704438574,
			"y": -936.9624866987937,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 3.4174889321552437,
			"height": 1.8986049623084706,
			"seed": 710447525,
			"groupIds": [
				"ENAXjbMgandSiynAsjaLg"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577644,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.07594303967584129,
					0
				],
				[
					-0.15189187343420177,
					-3.213996181392311e-17
				],
				[
					-0.22783491311002868,
					-0.15189187343419458
				],
				[
					-0.45566403213753826,
					-0.3037779527858557
				],
				[
					-0.7594419849233793,
					-0.5316128658958847
				],
				[
					-1.1391629773850764,
					-0.6834989452475524
				],
				[
					-1.3669978904951194,
					-0.9113338583575817
				],
				[
					-1.5948270095226005,
					-1.291054850819271
				],
				[
					-1.67077584328096,
					-1.442940930170939
				],
				[
					-1.7467188829568023,
					-1.5188839698467735
				],
				[
					-1.7467188829568023,
					-1.5948270095226076
				],
				[
					-1.6707758432809612,
					-1.5948270095226071
				],
				[
					-1.594827009522601,
					-1.5948270095226076
				],
				[
					-1.5188839698467735,
					-1.6707758432809676
				],
				[
					-1.2910548508192783,
					-1.6707758432809678
				],
				[
					-0.9872768980334226,
					-1.746718882956802
				],
				[
					-0.7594419849233792,
					-1.6707758432809678
				],
				[
					-0.45566403213753803,
					-1.594827009522608
				],
				[
					-0.15189187343420193,
					-1.5948270095226076
				],
				[
					0.07594303967584141,
					-1.5188839698467733
				],
				[
					0.3037779527858558,
					-1.5188839698467738
				],
				[
					0.455664032137524,
					-1.5188839698467733
				],
				[
					0.6834989452475527,
					-1.5948270095226071
				],
				[
					0.8353850245992208,
					-1.6707758432809678
				],
				[
					0.9113280642750619,
					-1.6707758432809685
				],
				[
					0.9872711039508891,
					-1.6707758432809678
				],
				[
					1.0632199377092497,
					-1.6707758432809683
				],
				[
					1.139162977385078,
					-1.6707758432809678
				],
				[
					1.2151060170609178,
					-1.7467188829568026
				],
				[
					1.2910490567367592,
					-1.8226619226326362
				],
				[
					1.3669920964125866,
					-1.8226619226326364
				],
				[
					1.4429409301709466,
					-1.8226619226326362
				],
				[
					1.5188839698467733,
					-1.8986049623084706
				],
				[
					1.5948270095226003,
					-1.8226619226326357
				],
				[
					1.6707700491984416,
					-1.8226619226326362
				],
				[
					1.5948270095226003,
					-1.7467188829568019
				],
				[
					1.518883969846774,
					-1.6707758432809678
				],
				[
					1.4429409301709466,
					-1.5948270095226076
				],
				[
					1.3669920964125866,
					-1.518883969846773
				],
				[
					1.291049056736759,
					-1.4429409301709397
				],
				[
					1.215106017060918,
					-1.2910548508192707
				],
				[
					1.0632199377092497,
					-1.1391629773850835
				],
				[
					0.9872711039508895,
					-0.9872768980334156
				],
				[
					0.9113280642750623,
					-0.911333858357581
				],
				[
					0.835385024599221,
					-0.8353850245992209
				],
				[
					0.7594419849233796,
					-0.7594419849233864
				],
				[
					0.6075501114891924,
					-0.6834989452475525
				],
				[
					0.5316070718133653,
					-0.6075559055717186
				],
				[
					0.4556640321375239,
					-0.5316128658958844
				],
				[
					0.3797209924616971,
					-0.4556640321375238
				],
				[
					0.30377795278585573,
					-0.37972099246168983
				],
				[
					0.2278291190274952,
					-0.3037779527858556
				],
				[
					0.22782911902749528,
					-0.22783491311002868
				],
				[
					0.1518860793516683,
					-0.15189187343419458
				],
				[
					0.15188607935166823,
					-0.0759430396758341
				],
				[
					0.2278291190274952,
					-0.0759430396758342
				],
				[
					0.37972099246169705,
					-0.15189187343419452
				],
				[
					0,
					0
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.171875,
				0.232421875,
				0.373046875,
				0.4453125,
				0.47265625,
				0.4912109375,
				0.5068359375,
				0.517578125,
				0.5234375,
				0.5234375,
				0.5234375,
				0.5234375,
				0.51953125,
				0.51953125,
				0.5166015625,
				0.5166015625,
				0.513671875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.51171875,
				0.513671875,
				0.51171875,
				0.51171875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.5166015625,
				0.513671875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.521484375,
				0.521484375,
				0.513671875,
				0.513671875,
				0.513671875,
				0.513671875,
				0.4873046875,
				0.4306640625,
				0.013671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 1713,
			"versionNonce": 91885954,
			"isDeleted": false,
			"id": "tNqHImQQenu5kmpqljXmp",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1627.5259064117195,
			"y": -936.278987753546,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 0.2278291190275104,
			"height": 2.6580469472318646,
			"seed": 1459688709,
			"groupIds": [
				"ENAXjbMgandSiynAsjaLg"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577644,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-5.356660302320523e-18,
					0.07594303967583413
				],
				[
					0.07594303967584133,
					0.22782911902750236
				],
				[
					0.07594303967584129,
					0.6075501114891994
				],
				[
					0.07594303967584137,
					0.9113280642750622
				],
				[
					0.15188607935168275,
					1.1391629773850838
				],
				[
					0.15188607935168222,
					1.44293513608842
				],
				[
					0.15188607935168275,
					1.594827009522615
				],
				[
					0.15188607935168275,
					1.8226561285501173
				],
				[
					0.1518860793516829,
					2.050491041660139
				],
				[
					0.07594303967584172,
					2.050491041660139
				],
				[
					0.0759430396758412,
					2.126434081335973
				],
				[
					0.07594303967584137,
					2.278325954770168
				],
				[
					0,
					2.4302120341218356
				],
				[
					-1.0284787780455404e-15,
					2.5061550737976703
				],
				[
					-1.7141312967425674e-16,
					2.582098113473504
				],
				[
					0,
					2.6580469472318646
				],
				[
					0.15188607935168344,
					2.6580469472318646
				],
				[
					0.22782911902750938,
					2.582098113473504
				],
				[
					0.22782911902750938,
					2.582098113473504
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.1953125,
				0.30078125,
				0.3388671875,
				0.37109375,
				0.38671875,
				0.3994140625,
				0.4111328125,
				0.42578125,
				0.4345703125,
				0.4501953125,
				0.4560546875,
				0.4677734375,
				0.470703125,
				0.470703125,
				0.470703125,
				0.470703125,
				0.474609375,
				0.3720703125,
				0.275390625,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 1746,
			"versionNonce": 873152414,
			"isDeleted": false,
			"id": "qreJWMaXxwYKaBMIQS3yN",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1625.247580456949,
			"y": -934.0006617987759,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 6.227421958738777,
			"height": 1.8226619226326364,
			"seed": 377629797,
			"groupIds": [
				"ENAXjbMgandSiynAsjaLg"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577644,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					0.07594303967583413
				],
				[
					0.07594303967582697,
					0.15188607935166826
				],
				[
					0.22782911902750963,
					0.22782911902750236
				],
				[
					0.3037721587033365,
					0.379720992461697
				],
				[
					0.4556640321375239,
					0.5316070718133652
				],
				[
					0.6075501114891922,
					0.6834931511650263
				],
				[
					0.7594419849233937,
					0.7594419849233868
				],
				[
					0.911328064275048,
					0.8353850245992207
				],
				[
					0.9872711039508891,
					0.7594419849233868
				],
				[
					1.1391629773850909,
					0.7594419849233868
				],
				[
					1.2151060170609178,
					0.6834931511650261
				],
				[
					1.291049056736745,
					0.6075501114891922
				],
				[
					1.3669920964125721,
					0.45566403213753126
				],
				[
					1.4429351360884133,
					0.3037721587033365
				],
				[
					1.5948270095226154,
					0.07594303967583424
				],
				[
					1.7467130888742688,
					-0.07594883375836059
				],
				[
					1.82265612855011,
					-0.15189187343419439
				],
				[
					1.82265612855011,
					-0.22783491311002874
				],
				[
					1.8986049623084706,
					-0.3037779527858627
				],
				[
					1.8986049623084706,
					-0.37972099246168983
				],
				[
					1.9745480019843118,
					-0.37972099246168994
				],
				[
					1.9745480019843122,
					-0.45566982622005087
				],
				[
					2.1264340813359657,
					-0.45566982622005064
				],
				[
					2.202377121011793,
					-0.4556698262200503
				],
				[
					2.2783259547701533,
					-0.37972099246168994
				],
				[
					2.3542689944459947,
					-0.37972099246168983
				],
				[
					2.3542689944459947,
					-0.30377795278586267
				],
				[
					2.4302120341218356,
					-0.30377795278586284
				],
				[
					2.506155073797663,
					-0.30377795278586284
				],
				[
					2.506155073797663,
					-0.22783491311002874
				],
				[
					2.58209811347349,
					-0.15189187343419483
				],
				[
					2.58209811347349,
					-0.0759488337583607
				],
				[
					2.6580469472318504,
					0.15188607935166826
				],
				[
					2.7339899869076913,
					0.22782911902750236
				],
				[
					2.8858760662593594,
					0.379720992461697
				],
				[
					2.9618191059351866,
					0.5316070718133652
				],
				[
					3.037767939693547,
					0.6075501114891922
				],
				[
					3.1137109793693885,
					0.7594419849233865
				],
				[
					3.1896540190452156,
					0.8353850245992209
				],
				[
					3.3415400983968837,
					1.0632141436267233
				],
				[
					3.4174889321552437,
					1.1391629773850838
				],
				[
					3.5693750115069123,
					1.2151060170609176
				],
				[
					3.645318051182754,
					1.2151060170609178
				],
				[
					3.7972099246169413,
					1.291049056736752
				],
				[
					3.9490960039686094,
					1.291049056736752
				],
				[
					4.100982083320278,
					1.2151060170609178
				],
				[
					4.252873956754465,
					1.2151060170609178
				],
				[
					4.480703075781975,
					1.0632141436267233
				],
				[
					4.78448102856783,
					0.911328064275055
				],
				[
					5.012315941677859,
					0.6834931511650263
				],
				[
					5.240145060705355,
					0.5316070718133652
				],
				[
					5.467979973815383,
					0.3037721587033365
				],
				[
					5.695814886925412,
					0.07594303967583413
				],
				[
					5.923644005952907,
					-0.07594883375836048
				],
				[
					5.999587045628748,
					-0.1518918734341946
				],
				[
					6.075535879387094,
					-0.30377795278586284
				],
				[
					6.151478919062936,
					-0.37972099246168983
				],
				[
					6.227421958738777,
					-0.5316128658958844
				],
				[
					6.227421958738777,
					-0.5316128658958844
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.1865234375,
				0.2373046875,
				0.265625,
				0.294921875,
				0.326171875,
				0.3505859375,
				0.3662109375,
				0.373046875,
				0.3798828125,
				0.392578125,
				0.396484375,
				0.3984375,
				0.3984375,
				0.4013671875,
				0.408203125,
				0.41015625,
				0.41015625,
				0.41015625,
				0.41015625,
				0.412109375,
				0.4228515625,
				0.4140625,
				0.4072265625,
				0.4072265625,
				0.4111328125,
				0.4091796875,
				0.3955078125,
				0.3310546875,
				0.3837890625,
				0.384765625,
				0.3955078125,
				0.3974609375,
				0.3974609375,
				0.3974609375,
				0.3974609375,
				0.3974609375,
				0.3974609375,
				0.3974609375,
				0.3974609375,
				0.4013671875,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.40625,
				0.41015625,
				0.4150390625,
				0.423828125,
				0.427734375,
				0.427734375,
				0.4345703125,
				0.3779296875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 1724,
			"versionNonce": 1426100546,
			"isDeleted": false,
			"id": "YoAs6GmJFbzzfEb-dnait",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1622.057920643821,
			"y": -944.4809635083519,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 5.39204272822206,
			"height": 3.6453180511827465,
			"seed": 682186693,
			"groupIds": [
				"ENAXjbMgandSiynAsjaLg"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577644,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.15189187343420177,
					0.1518918734341945
				],
				[
					-0.45566403213753826,
					0.30377795278586284
				],
				[
					-0.9113338583575953,
					0.5316128658958917
				],
				[
					-1.518883969846773,
					1.2151060170609176
				],
				[
					-1.8226619226326433,
					1.7467188829568097
				],
				[
					-1.9745480019842971,
					2.2023829150943337
				],
				[
					-2.050496835742657,
					2.5061608678801965
				],
				[
					-2.0504968357426576,
					2.733989986907698
				],
				[
					-1.822661922632643,
					2.96182490001772
				],
				[
					-1.518883969846774,
					3.113710979369388
				],
				[
					-0.9872768980334224,
					3.1137109793693885
				],
				[
					-0.22783491311002887,
					2.9618249000177213
				],
				[
					0.3037779527858561,
					2.8099388206660523
				],
				[
					0.6834989452475531,
					2.58210390755603
				],
				[
					1.1391629773850762,
					2.354268994446002
				],
				[
					1.5188839698467738,
					2.050496835742665
				],
				[
					2.1264340813359652,
					1.7467188829568099
				],
				[
					2.88587606625936,
					1.139162977385084
				],
				[
					3.1137109793693876,
					0.7594419849233941
				],
				[
					3.2655970587210423,
					0.5316128658958917
				],
				[
					3.3415458924794024,
					0.3037779527858632
				],
				[
					3.2655970587210423,
					0.15189187343419447
				],
				[
					3.189654019045215,
					0
				],
				[
					2.809933026583518,
					-0.1518860793516612
				],
				[
					2.430212034121821,
					-0.303777952785856
				],
				[
					1.8986049623084706,
					-0.4556640321375241
				],
				[
					1.0632199377092495,
					-0.5316070718133581
				],
				[
					0.9113280642750622,
					-0.4556640321375239
				],
				[
					0.6075501114891921,
					-0.3797209924616898
				],
				[
					0.5316070718133652,
					-0.3797209924616899
				],
				[
					0.3037779527858557,
					-0.30377795278585573
				],
				[
					0.3037779527858556,
					-0.22782911902749525
				],
				[
					0.3797209924616826,
					-0.2278291190274952
				],
				[
					0,
					0
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.171875,
				0.201171875,
				0.2529296875,
				0.3037109375,
				0.361328125,
				0.38671875,
				0.4130859375,
				0.423828125,
				0.42578125,
				0.42578125,
				0.419921875,
				0.4150390625,
				0.4033203125,
				0.400390625,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.3984375,
				0.408203125,
				0.4306640625,
				0.45703125,
				0.47265625,
				0.4775390625,
				0.482421875,
				0.4951171875,
				0.4970703125,
				0.4970703125,
				0.4970703125,
				0.466796875,
				0.4140625,
				0.0263671875,
				0
			]
		},
		{
			"type": "freedraw",
			"version": 1724,
			"versionNonce": 1711119326,
			"isDeleted": false,
			"id": "mdFV8453TYQHoEJVbOAUz",
			"fillStyle": "hachure",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1633.2217155045623,
			"y": -945.2404054932753,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 4.556651909540335,
			"height": 3.4174889321552446,
			"seed": 2006193957,
			"groupIds": [
				"ENAXjbMgandSiynAsjaLg"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577644,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.15188607935165394,
					-0.07594303967583418
				],
				[
					-0.6075501114892065,
					-0.07594303967583416
				],
				[
					-0.9872711039508748,
					-8.570656483712831e-17
				],
				[
					-1.3669920964125717,
					0.22783491311002857
				],
				[
					-1.746713088874269,
					0.5316128658958919
				],
				[
					-2.202382915094326,
					1.0632199377092497
				],
				[
					-2.3542689944460085,
					1.5188839698467806
				],
				[
					-2.278325954770153,
					1.9745480019843047
				],
				[
					-2.0504910416601385,
					2.354268994446002
				],
				[
					-1.7467130888742697,
					2.658046947231858
				],
				[
					-1.1391629773850909,
					2.8858818603418865
				],
				[
					-0.7594419849233935,
					2.961824900017721
				],
				[
					-0.30377795278586966,
					2.885881860341886
				],
				[
					0.07594303967582673,
					2.7339899869076913
				],
				[
					0.8353850245992208,
					2.354268994446002
				],
				[
					1.4429409301709326,
					1.9745480019843042
				],
				[
					1.8226619226326288,
					1.6707758432809685
				],
				[
					2.0504968357426727,
					1.3669978904951126
				],
				[
					2.202382915094326,
					1.0632199377092504
				],
				[
					2.202382915094326,
					0.7594419849233874
				],
				[
					2.202382915094326,
					0.5316128658958911
				],
				[
					2.126439875418499,
					0.30377795278586267
				],
				[
					1.9745480019843116,
					0
				],
				[
					1.6707758432809752,
					-0.15188607935166806
				],
				[
					0.9113338583575813,
					-0.3797209924616896
				],
				[
					0.30377795278586994,
					-0.455664032137524
				],
				[
					-0.07594303967582688,
					-0.455664032137524
				],
				[
					-0.45566403213752393,
					-0.30377795278586284
				],
				[
					-0.7594419849233939,
					-0.15188607935166815
				],
				[
					-0.9872711039508748,
					-8.570656483712831e-17
				],
				[
					-0.9872711039508749,
					0.15189187343419472
				],
				[
					-0.9872711039508749,
					0.3797209924616973
				],
				[
					0,
					0
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.173828125,
				0.1923828125,
				0.294921875,
				0.3798828125,
				0.447265625,
				0.4873046875,
				0.4912109375,
				0.486328125,
				0.484375,
				0.482421875,
				0.48046875,
				0.4697265625,
				0.4658203125,
				0.470703125,
				0.4677734375,
				0.474609375,
				0.4765625,
				0.4765625,
				0.478515625,
				0.48046875,
				0.4921875,
				0.4951171875,
				0.5,
				0.5126953125,
				0.521484375,
				0.5234375,
				0.525390625,
				0.525390625,
				0.525390625,
				0.505859375,
				0.423828125,
				0.1904296875,
				0.01171875,
				0
			]
		},
		{
			"type": "rectangle",
			"version": 1817,
			"versionNonce": 924915970,
			"isDeleted": false,
			"id": "xXnniTdS4D5xmruB4XEWW",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1556.112730005982,
			"y": -901.6801616591746,
			"strokeColor": "#2f9e44",
			"backgroundColor": "#b2f2bb",
			"width": 153.39518267385216,
			"height": 16.365029766123357,
			"seed": 1270501861,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577644,
			"link": null,
			"locked": false
		},
		{
			"type": "arrow",
			"version": 241,
			"versionNonce": 433745950,
			"isDeleted": false,
			"id": "VgBul-HIp6EZds-sirVAC",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1634.2043639635835,
			"y": -866.5106439310674,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#b2f2bb",
			"width": 0.42654604721042233,
			"height": 72.63930584098136,
			"seed": 515951941,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692815577644,
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
					-0.42654604721042233,
					72.63930584098136
				]
			]
		},
		{
			"type": "arrow",
			"version": 322,
			"versionNonce": 1532668098,
			"isDeleted": false,
			"id": "O1AjqBlxJtpZJjZ5w4CLu",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1632.620016434469,
			"y": -1195.4316336609281,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#b2f2bb",
			"width": 1.0345875982579855,
			"height": 188.0688638329882,
			"seed": 1181893515,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1692815577644,
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
					1.0345875982579855,
					188.0688638329882
				]
			]
		},
		{
			"type": "text",
			"version": 385,
			"versionNonce": 462601310,
			"isDeleted": false,
			"id": "uo6I2VYy",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1796.721778879802,
			"y": -1186.317698635135,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#b2f2bb",
			"width": 201,
			"height": 300,
			"seed": 1392329989,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577644,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "      Credits\n\nCreddits ...... Credits\nCreddits ...... Credits\nCreddits ...... Credits\nCreddits ...... Credits\n\n\n\nCreddits ...... Credits\nCreddits ...... Credits\nCreddits ...... Credits",
			"rawText": "      Credits\n\nCreddits ...... Credits\nCreddits ...... Credits\nCreddits ...... Credits\nCreddits ...... Credits\n\n\n\nCreddits ...... Credits\nCreddits ...... Credits\nCreddits ...... Credits",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "      Credits\n\nCreddits ...... Credits\nCreddits ...... Credits\nCreddits ...... Credits\nCreddits ...... Credits\n\n\n\nCreddits ...... Credits\nCreddits ...... Credits\nCreddits ...... Credits",
			"lineHeight": 1.25,
			"baseline": 292
		},
		{
			"type": "rectangle",
			"version": 2312,
			"versionNonce": 692863106,
			"isDeleted": false,
			"id": "tKVKsN0kAZ4YWM9G7jEYR",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1801.6420546991365,
			"y": -1170.5974673956644,
			"strokeColor": "#ffffff",
			"backgroundColor": "#e9ecef",
			"width": 94.97770662217373,
			"height": 372.1870840854457,
			"seed": 387188293,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1692815577644,
			"link": null,
			"locked": false
		},
		{
			"id": "yyVrAr1kXGauiVD2O5OIO",
			"type": "rectangle",
			"x": 1912.6609173690226,
			"y": -203.46875777821714,
			"width": 146,
			"height": 35,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"seed": 1356149790,
			"version": 126,
			"versionNonce": 284655774,
			"isDeleted": false,
			"boundElements": [
				{
					"type": "text",
					"id": "Ag0HUSoO"
				}
			],
			"updated": 1692815577644,
			"link": null,
			"locked": false
		},
		{
			"id": "Ag0HUSoO",
			"type": "text",
			"x": 1927.6609173690226,
			"y": -198.46875777821714,
			"width": 116,
			"height": 25,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 1752925570,
			"version": 79,
			"versionNonce": 1018486850,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1692815577644,
			"link": null,
			"locked": false,
			"text": "LevelLoader",
			"rawText": "LevelLoader",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "center",
			"verticalAlign": "middle",
			"baseline": 17,
			"containerId": "yyVrAr1kXGauiVD2O5OIO",
			"originalText": "LevelLoader",
			"lineHeight": 1.25
		},
		{
			"type": "rectangle",
			"version": 174,
			"versionNonce": 1035582686,
			"isDeleted": false,
			"id": "EXlT0ITxlv2KcZ76gc2qh",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1956.7785949454237,
			"y": -154.70405369101627,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 146,
			"height": 35,
			"seed": 1023101982,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "x2LqxMHA"
				}
			],
			"updated": 1692815577644,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 137,
			"versionNonce": 1634961410,
			"isDeleted": false,
			"id": "x2LqxMHA",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1979.7785949454237,
			"y": -149.70405369101627,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 100,
			"height": 25,
			"seed": 1580734558,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1692815577644,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Crossfade",
			"rawText": "Crossfade",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "EXlT0ITxlv2KcZ76gc2qh",
			"originalText": "Crossfade",
			"lineHeight": 1.25,
			"baseline": 17
		},
		{
			"id": "ybRvbzcX",
			"type": "text",
			"x": 2182.016119226178,
			"y": -25.231004490333362,
			"width": 1020,
			"height": 775,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 746472514,
			"version": 73,
			"versionNonce": 260519874,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1692815577644,
			"link": null,
			"locked": false,
			"text": "public class LevelLoarer: MonoBehavior\n{\n\tpublic Animator transition;\n\tpublic float transitionTime = 1f;\n\tvoid Update()\n\t{\n\t\tif(Input.GetMouseButtonDown(0))\n\t\t{\n\t\t\tLoadNextLevel();\n\t\t}\n\t}\n\t\n\tpublic void LoadNextLevel()\n\t{\n\t\tStartCoroutine(\n\t\t\tLoadLevel(\n\t\t\t\tSceneManager.LoadScene(SceneManager.GetActiveScene().buildIndex + 1))\n\t\t);\n\t\t\n\t}\n\n\tIEnumerator LoadLevel(int levelIndex)\n\t{\n\t\t// Play animation\n\t\ttransition.setTrigger(\"Start\");\n\t\t// wait for animation\n\t\tyield return waitForSeconds(transitionTime);\n\t\t// load scene\n\t\tSceneManager.LoadScene(levelIndex)\n\t}\n}",
			"rawText": "public class LevelLoarer: MonoBehavior\n{\n\tpublic Animator transition;\n\tpublic float transitionTime = 1f;\n\tvoid Update()\n\t{\n\t\tif(Input.GetMouseButtonDown(0))\n\t\t{\n\t\t\tLoadNextLevel();\n\t\t}\n\t}\n\t\n\tpublic void LoadNextLevel()\n\t{\n\t\tStartCoroutine(\n\t\t\tLoadLevel(\n\t\t\t\tSceneManager.LoadScene(SceneManager.GetActiveScene().buildIndex + 1))\n\t\t);\n\t\t\n\t}\n\n\tIEnumerator LoadLevel(int levelIndex)\n\t{\n\t\t// Play animation\n\t\ttransition.setTrigger(\"Start\");\n\t\t// wait for animation\n\t\tyield return waitForSeconds(transitionTime);\n\t\t// load scene\n\t\tSceneManager.LoadScene(levelIndex)\n\t}\n}",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "left",
			"verticalAlign": "top",
			"baseline": 767,
			"containerId": null,
			"originalText": "public class LevelLoarer: MonoBehavior\n{\n\tpublic Animator transition;\n\tpublic float transitionTime = 1f;\n\tvoid Update()\n\t{\n\t\tif(Input.GetMouseButtonDown(0))\n\t\t{\n\t\t\tLoadNextLevel();\n\t\t}\n\t}\n\t\n\tpublic void LoadNextLevel()\n\t{\n\t\tStartCoroutine(\n\t\t\tLoadLevel(\n\t\t\t\tSceneManager.LoadScene(SceneManager.GetActiveScene().buildIndex + 1))\n\t\t);\n\t\t\n\t}\n\n\tIEnumerator LoadLevel(int levelIndex)\n\t{\n\t\t// Play animation\n\t\ttransition.setTrigger(\"Start\");\n\t\t// wait for animation\n\t\tyield return waitForSeconds(transitionTime);\n\t\t// load scene\n\t\tSceneManager.LoadScene(levelIndex)\n\t}\n}",
			"lineHeight": 1.25
		},
		{
			"id": "WUX54Ci29rx4i81DsEeZd",
			"type": "arrow",
			"x": 2414.941740580573,
			"y": 91.7025223992319,
			"width": 248.4045550989904,
			"height": 41.311321600853915,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"seed": 2084897054,
			"version": 51,
			"versionNonce": 449113026,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1692815587428,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					248.4045550989904,
					-41.311321600853915
				]
			],
			"lastCommittedPoint": null,
			"startBinding": null,
			"endBinding": {
				"elementId": "UhoZEfzm73j37KzRIVSSg",
				"focus": 0.5071220652971478,
				"gap": 10.141902299861158
			},
			"startArrowhead": null,
			"endArrowhead": "arrow"
		},
		{
			"id": "UhoZEfzm73j37KzRIVSSg",
			"type": "rectangle",
			"x": 2673.4881979794245,
			"y": 23.09298361101962,
			"width": 204,
			"height": 70,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"seed": 614035294,
			"version": 108,
			"versionNonce": 154878366,
			"isDeleted": false,
			"boundElements": [
				{
					"type": "text",
					"id": "pMOfPeGA"
				},
				{
					"id": "WUX54Ci29rx4i81DsEeZd",
					"type": "arrow"
				}
			],
			"updated": 1692815577644,
			"link": null,
			"locked": false
		},
		{
			"id": "pMOfPeGA",
			"type": "text",
			"x": 2678.9881979794245,
			"y": 33.09298361101962,
			"width": 193,
			"height": 50,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 1040288542,
			"version": 151,
			"versionNonce": 743026498,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1692815577644,
			"link": null,
			"locked": false,
			"text": "This is for testing \npurposes for now",
			"rawText": "This is for testing purposes for now",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "center",
			"verticalAlign": "middle",
			"baseline": 42,
			"containerId": "UhoZEfzm73j37KzRIVSSg",
			"originalText": "This is for testing purposes for now",
			"lineHeight": 1.25
		},
		{
			"id": "VS3uZCXkznTckS3gvQ3Nx",
			"type": "arrow",
			"x": 2406.8940773389104,
			"y": 328.8402957476034,
			"width": 237.6743374434409,
			"height": 63.3082596082246,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"seed": 787211906,
			"version": 39,
			"versionNonce": 287451486,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1692815587428,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					237.6743374434409,
					-63.3082596082246
				]
			],
			"lastCommittedPoint": null,
			"startBinding": null,
			"endBinding": {
				"elementId": "tEbgl9BK3fhGfimkwpWdE",
				"focus": 0.25373459924646113,
				"gap": 15.860918477487303
			},
			"startArrowhead": null,
			"endArrowhead": "arrow"
		},
		{
			"id": "tEbgl9BK3fhGfimkwpWdE",
			"type": "rectangle",
			"x": 2660.4293332598386,
			"y": 206.08276137367048,
			"width": 214,
			"height": 91,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"seed": 183844510,
			"version": 98,
			"versionNonce": 762595010,
			"isDeleted": false,
			"boundElements": [
				{
					"type": "text",
					"id": "EpxldSKq"
				},
				{
					"id": "VS3uZCXkznTckS3gvQ3Nx",
					"type": "arrow"
				}
			],
			"updated": 1692815577644,
			"link": null,
			"locked": false
		},
		{
			"id": "EpxldSKq",
			"type": "text",
			"x": 2679.9293332598386,
			"y": 226.58276137367048,
			"width": 175,
			"height": 50,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 2073582658,
			"version": 89,
			"versionNonce": 1206517342,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1692815577644,
			"link": null,
			"locked": false,
			"text": "This is how you \nstart a coroutine",
			"rawText": "This is how you start a coroutine",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "center",
			"verticalAlign": "middle",
			"baseline": 42,
			"containerId": "tEbgl9BK3fhGfimkwpWdE",
			"originalText": "This is how you start a coroutine",
			"lineHeight": 1.25
		},
		{
			"id": "6JhnnS7Tq9tjnkqRzOGPS",
			"type": "arrow",
			"x": 2623.6445231000544,
			"y": 416.82808870961804,
			"width": 105.3719315694807,
			"height": 48.67045290826212,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"seed": 1786776194,
			"version": 247,
			"versionNonce": 678830978,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1692815587429,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					105.3719315694807,
					48.67045290826212
				]
			],
			"lastCommittedPoint": null,
			"startBinding": null,
			"endBinding": {
				"elementId": "bthmCh6lZRPI9kXCW2Kdq",
				"focus": -0.48125272318294204,
				"gap": 19.038624717172752
			},
			"startArrowhead": null,
			"endArrowhead": "arrow"
		},
		{
			"id": "bthmCh6lZRPI9kXCW2Kdq",
			"type": "rectangle",
			"x": 2748.055079386708,
			"y": 411.9918480628069,
			"width": 160,
			"height": 110,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"seed": 1134620354,
			"version": 136,
			"versionNonce": 1870593602,
			"isDeleted": false,
			"boundElements": [
				{
					"type": "text",
					"id": "RuemmRxY"
				},
				{
					"id": "6JhnnS7Tq9tjnkqRzOGPS",
					"type": "arrow"
				}
			],
			"updated": 1692815577644,
			"link": null,
			"locked": false
		},
		{
			"id": "RuemmRxY",
			"type": "text",
			"x": 2758.555079386708,
			"y": 429.4918480628069,
			"width": 139,
			"height": 75,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 422492638,
			"version": 156,
			"versionNonce": 178814686,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1692815577644,
			"link": null,
			"locked": false,
			"text": "This is to go \nthe ne next \nscene",
			"rawText": "This is to go the ne next scene",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "center",
			"verticalAlign": "middle",
			"baseline": 67,
			"containerId": "bthmCh6lZRPI9kXCW2Kdq",
			"originalText": "This is to go the ne next scene",
			"lineHeight": 1.25
		},
		{
			"id": "WkklSFLUelMMPMqi3ScfM",
			"type": "rectangle",
			"x": 2686.5389641462484,
			"y": 555.7843950692283,
			"width": 165,
			"height": 210,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"seed": 1624992606,
			"version": 92,
			"versionNonce": 283235778,
			"isDeleted": false,
			"boundElements": [
				{
					"type": "text",
					"id": "MmUauxRW"
				},
				{
					"id": "NU4KKSvf7ybNM7g_YUorj",
					"type": "arrow"
				}
			],
			"updated": 1692815577645,
			"link": null,
			"locked": false
		},
		{
			"id": "MmUauxRW",
			"type": "text",
			"x": 2694.5389641462484,
			"y": 560.7843950692283,
			"width": 149,
			"height": 200,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 563467778,
			"version": 155,
			"versionNonce": 1193336670,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1692815577645,
			"link": null,
			"locked": false,
			"text": "The coroutine \nis needed \nbecause we \nneed to make \nthe game wait \nfor the \ntransition to \nfinish",
			"rawText": "The coroutine is needed because we need to make the game wait for the transition to finish",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "center",
			"verticalAlign": "middle",
			"baseline": 192,
			"containerId": "WkklSFLUelMMPMqi3ScfM",
			"originalText": "The coroutine is needed because we need to make the game wait for the transition to finish",
			"lineHeight": 1.25
		},
		{
			"id": "NU4KKSvf7ybNM7g_YUorj",
			"type": "arrow",
			"x": 2578.577559827708,
			"y": 512.863524447029,
			"width": 94.42594811486379,
			"height": 123.3975030388226,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"seed": 1913590814,
			"version": 62,
			"versionNonce": 1544637854,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1692815587429,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					94.42594811486379,
					123.3975030388226
				]
			],
			"lastCommittedPoint": null,
			"startBinding": null,
			"endBinding": {
				"elementId": "WkklSFLUelMMPMqi3ScfM",
				"focus": -0.47449039365962625,
				"gap": 13.535456203676858
			},
			"startArrowhead": null,
			"endArrowhead": "arrow"
		},
		{
			"id": "WJqiBa0Y",
			"type": "text",
			"x": 2250.0139752303503,
			"y": -174.851130466062,
			"width": 69,
			"height": 50,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 1667728286,
			"version": 39,
			"versionNonce": 1198158110,
			"isDeleted": true,
			"boundElements": null,
			"updated": 1692815577644,
			"link": null,
			"locked": false,
			"text": "Canvas\n",
			"rawText": "Canvas\n",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "left",
			"verticalAlign": "top",
			"baseline": 42,
			"containerId": null,
			"originalText": "Canvas\n",
			"lineHeight": 1.25
		},
		{
			"id": "gt9NnNuF",
			"type": "text",
			"x": 2680.5146275554303,
			"y": 90.62949654042373,
			"width": 10,
			"height": 25,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 264132098,
			"version": 5,
			"versionNonce": 1729032066,
			"isDeleted": true,
			"boundElements": null,
			"updated": 1692815577644,
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
			"id": "YbUw8NUA",
			"type": "text",
			"x": 2777.9881979794245,
			"y": 138.21870927162274,
			"width": 10,
			"height": 25,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 702249282,
			"version": 5,
			"versionNonce": 1507679710,
			"isDeleted": true,
			"boundElements": null,
			"updated": 1692815577644,
			"link": null,
			"locked": false,
			"text": "",
			"rawText": "",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "center",
			"verticalAlign": "middle",
			"baseline": 17,
			"containerId": "UhoZEfzm73j37KzRIVSSg",
			"originalText": "",
			"lineHeight": 1.25
		},
		{
			"id": "qxcmdSEU",
			"type": "text",
			"x": 2739.530824660954,
			"y": 128.185258334848,
			"width": 10,
			"height": 25,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 545425182,
			"version": 5,
			"versionNonce": 1133934338,
			"isDeleted": true,
			"boundElements": null,
			"updated": 1692815577644,
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
			"id": "aqOlUqxB",
			"type": "text",
			"x": 2785.9389832751813,
			"y": 488.720555188308,
			"width": 10,
			"height": 25,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 1786627614,
			"version": 5,
			"versionNonce": 42081922,
			"isDeleted": true,
			"boundElements": null,
			"updated": 1692815577644,
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
			"id": "peFD2dpm",
			"type": "text",
			"x": 2482.5420626914993,
			"y": 588.5115507321486,
			"width": 10,
			"height": 25,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 1816824414,
			"version": 5,
			"versionNonce": 826926594,
			"isDeleted": true,
			"boundElements": null,
			"updated": 1692815577645,
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
			"id": "nkaClPDT",
			"type": "text",
			"x": 2698.219503060101,
			"y": 636.7975301821227,
			"width": 10,
			"height": 25,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 1326127618,
			"version": 5,
			"versionNonce": 1295053598,
			"isDeleted": true,
			"boundElements": null,
			"updated": 1692815577645,
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
			"id": "IXPSngTx68PkyhhonYoLq",
			"type": "freedraw",
			"x": 2580.1871088490534,
			"y": 543.4446283923331,
			"width": 68.67340936853134,
			"height": 53.651088277748954,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 1569297886,
			"version": 77,
			"versionNonce": 1600507266,
			"isDeleted": true,
			"boundElements": null,
			"updated": 1692815577645,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.5365436288029741,
					0
				],
				[
					3.7555598064295737,
					-0.5365026962710999
				],
				[
					10.730217655549495,
					-2.1460107850843997
				],
				[
					20.387429918557245,
					-2.682554413887374
				],
				[
					27.36208776767762,
					-3.7555598064295737
				],
				[
					34.33674561679754,
					-5.365108827774861
				],
				[
					38.09230542322712,
					-5.365108827774861
				],
				[
					39.70185444457229,
					-5.365108827774861
				],
				[
					40.77485983711449,
					-5.365108827774861
				],
				[
					41.84786522965669,
					-5.365108827774861
				],
				[
					43.457414251001865,
					-5.365108827774861
				],
				[
					45.603425036086264,
					-3.2190571101584737
				],
				[
					48.28597944997364,
					0
				],
				[
					49.35898484251629,
					2.6825544138874875
				],
				[
					50.43207210012224,
					5.901652456577949
				],
				[
					52.57808288520664,
					9.120709566736537
				],
				[
					53.65108827774884,
					14.485818394511398
				],
				[
					54.72409367029104,
					16.631870112127785
				],
				[
					54.72409367029104,
					17.168372808398885
				],
				[
					54.72409367029104,
					18.241378200941085
				],
				[
					54.72409367029104,
					19.314424526015273
				],
				[
					54.72409367029104,
					20.923932614828573
				],
				[
					54.72409367029104,
					21.996978939902647
				],
				[
					54.72409367029104,
					22.533481636173747
				],
				[
					54.72409367029104,
					23.069984332444847
				],
				[
					54.187631906551815,
					23.069984332444847
				],
				[
					54.187631906551815,
					23.606487028715947
				],
				[
					53.65108827774884,
					24.142989724987046
				],
				[
					53.114626514009615,
					24.679533353790134
				],
				[
					52.04153925640367,
					25.752538746332334
				],
				[
					50.96853386386147,
					25.752538746332334
				],
				[
					49.89552847131927,
					26.289041442603434
				],
				[
					49.35898484251629,
					27.362087767677508
				],
				[
					48.28597944997364,
					28.435093160219708
				],
				[
					46.67643042862892,
					29.508098552761908
				],
				[
					46.67643042862892,
					30.044642181564996
				],
				[
					46.13996866488924,
					30.581144877836095
				],
				[
					46.13996866488924,
					31.117647574107195
				],
				[
					46.13996866488924,
					32.72719659545248
				],
				[
					45.603425036086264,
					33.26369929172358
				],
				[
					45.06696327234749,
					34.87320738053688
				],
				[
					45.06696327234749,
					35.94625370561096
				],
				[
					45.603425036086264,
					38.092305423227344
				],
				[
					46.13996866488924,
					39.701813512040644
				],
				[
					46.13996866488924,
					40.238316208311744
				],
				[
					46.67643042862892,
					40.238316208311744
				],
				[
					47.21297405743189,
					40.77485983711483
				],
				[
					47.74951768623487,
					41.31136253338593
				],
				[
					48.28597944997364,
					41.84786522965703
				],
				[
					48.28597944997364,
					42.38436792592813
				],
				[
					49.35898484251629,
					42.92087062219923
				],
				[
					49.89552847131927,
					43.457414251002206
				],
				[
					50.43207210012224,
					43.457414251002206
				],
				[
					52.04153925640367,
					43.457414251002206
				],
				[
					52.57808288520664,
					43.457414251002206
				],
				[
					53.65108827774884,
					43.993916947273306
				],
				[
					54.187631906551815,
					43.993916947273306
				],
				[
					57.406648084178414,
					44.530419643544406
				],
				[
					59.55274073432702,
					45.066922339815505
				],
				[
					61.69875151941142,
					45.066922339815505
				],
				[
					62.77175691195316,
					45.603425036086605
				],
				[
					63.844844169559565,
					45.603425036086605
				],
				[
					65.45431132584054,
					46.13996866488969
				],
				[
					65.99085495464396,
					46.67647136116079
				],
				[
					66.52739858344694,
					46.67647136116079
				],
				[
					67.06386034718616,
					46.67647136116079
				],
				[
					67.60040397598914,
					47.21297405743189
				],
				[
					68.13686573972836,
					47.21297405743189
				],
				[
					68.67340936853134,
					47.21297405743189
				],
				[
					68.67340936853134,
					47.74947675370299
				],
				[
					68.67340936853134,
					48.28597944997409
				],
				[
					68.67340936853134,
					48.28597944997409
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				68.67340936853134,
				48.28597944997409
			]
		},
		{
			"id": "rOP4ZfNKIOv7rHFtOrBih",
			"type": "freedraw",
			"x": 2648.8605182175847,
			"y": 591.7306078423072,
			"width": 56.87018632043964,
			"height": 115.88634249343136,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 1696609054,
			"version": 65,
			"versionNonce": 214516638,
			"isDeleted": true,
			"boundElements": null,
			"updated": 1692815577645,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.5365436288029741,
					0
				],
				[
					-2.1460107850843997,
					0.5365436288030878
				],
				[
					-4.8285651989717735,
					0.5365436288030878
				],
				[
					-6.974657849119922,
					1.0730463250741877
				],
				[
					-10.193674026746976,
					1.0730463250741877
				],
				[
					-11.266761284352924,
					1.6095490213452877
				],
				[
					-12.87622844063435,
					2.1460517176163876
				],
				[
					-13.949315698240298,
					2.6825544138874875
				],
				[
					-14.485777461979524,
					3.2190980426904616
				],
				[
					-15.558782854521723,
					3.7556007389615615
				],
				[
					-15.558782854521723,
					4.2921034352326615
				],
				[
					-16.095326483324698,
					4.2921034352326615
				],
				[
					-16.095326483324698,
					5.365108827774861
				],
				[
					-16.63187011212767,
					6.438155152849049
				],
				[
					-16.63187011212767,
					7.511160545391249
				],
				[
					-16.63187011212767,
					8.584206870465437
				],
				[
					-16.63187011212767,
					10.730217655549723
				],
				[
					-16.63187011212767,
					14.485818394511398
				],
				[
					-16.095326483324698,
					17.16837280839877
				],
				[
					-15.022321090782498,
					20.38742991855736
				],
				[
					-13.949315698240298,
					23.606487028715947
				],
				[
					-11.266761284352924,
					27.898590463948608
				],
				[
					-5.9016524565781765,
					33.80020198799457
				],
				[
					-5.365108827775202,
					35.40975100933986
				],
				[
					-3.7555598064295737,
					37.01925909815316
				],
				[
					-1.609549021345174,
					38.628808119498444
				],
				[
					-0.5365436288029741,
					40.77485983711472
				],
				[
					2.1460107850843997,
					42.92087062219912
				],
				[
					4.8285651989717735,
					45.603425036086605
				],
				[
					8.047663241662576,
					48.82252307877707
				],
				[
					9.657212263007295,
					50.43203116759037
				],
				[
					10.193674026746976,
					51.505077492664554
				],
				[
					10.73021765554995,
					54.18763190655204
				],
				[
					11.266761284352924,
					56.870186320439416
				],
				[
					12.339766676895124,
					59.016197105523815
				],
				[
					12.339766676895124,
					61.1622488231402
				],
				[
					12.339766676895124,
					63.84480323702769
				],
				[
					12.339766676895124,
					68.13690667226035
				],
				[
					12.339766676895124,
					70.81946108614773
				],
				[
					12.339766676895124,
					74.57502089257741
				],
				[
					12.339766676895124,
					75.11152358884851
				],
				[
					11.803223048091695,
					77.2575753064649
				],
				[
					8.58420687046555,
					81.01317604542646
				],
				[
					6.4381142203169475,
					82.62268413423976
				],
				[
					4.292103435232548,
					84.23223315558505
				],
				[
					1.609549021345174,
					86.37828487320132
				],
				[
					-5.9016524565781765,
					91.7433937009763
				],
				[
					-11.266761284352924,
					95.49895350740587
				],
				[
					-17.168331875866897,
					99.79105694263865
				],
				[
					-22.5334407036421,
					104.08311944533932
				],
				[
					-26.28900051007122,
					106.76567385922681
				],
				[
					-30.044642181564996,
					108.37522288057198
				],
				[
					-35.94621277307897,
					111.59432092326256
				],
				[
					-39.70177257950854,
					113.20378807954387
				],
				[
					-41.31132160085372,
					113.74033170834696
				],
				[
					-42.38432699339637,
					114.27687533714993
				],
				[
					-42.920870622199345,
					114.81333710088916
				],
				[
					-43.45741425100232,
					114.81333710088916
				],
				[
					-43.993876014741545,
					115.34988072969213
				],
				[
					-44.53041964354452,
					115.88634249343136
				],
				[
					-44.53041964354452,
					115.88634249343136
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				-44.53041964354452,
				115.88634249343136
			]
		}
	],
	"appState": {
		"theme": "dark",
		"viewBackgroundColor": "#ffffff",
		"currentItemStrokeColor": "#1e1e1e",
		"currentItemBackgroundColor": "transparent",
		"currentItemFillStyle": "hachure",
		"currentItemStrokeWidth": 1,
		"currentItemStrokeStyle": "solid",
		"currentItemRoughness": 1,
		"currentItemOpacity": 100,
		"currentItemFontFamily": 1,
		"currentItemFontSize": 20,
		"currentItemTextAlign": "left",
		"currentItemStartArrowhead": null,
		"currentItemEndArrowhead": "arrow",
		"scrollX": -1444.4154225124287,
		"scrollY": 357.6831072525803,
		"zoom": {
			"value": 0.39555803589522814
		},
		"currentItemRoundness": "round",
		"gridSize": null,
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