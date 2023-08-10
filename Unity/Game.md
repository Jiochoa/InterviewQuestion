```toc
```

## Story
This is going to be the whole story from start to end.

### Level 1
**<u>Cutscene #1</u>**
The level will start with a cutscene of the cat going after the butterfly. The butterfly will stand in the rail then the cat will charge jump to get it but it will escape once again. Once the cat is in the rail, the game will end the cutscene.

**<u>Level #1</u>**
The game start with the player going out trying to catch the butterfly that will move along the parking lot. This will also serve as a tutorial for the different movements the player can do.

The first one will be the butterfly standing on a storage room. the cat will need to drag a trashcan to reach it. This will also have a tutorial sign close by (maybe in neon)

Once reached, the butterfly will fly to the roof. The next will be the charge jump which will show once the cat reaches the first position of the butterfly. This will show the player how to charge jump to reach the roof of the storage room.

Once reached, the butterfly will fly trough some of the cars which will give the player some time to practice. no new movements here. 

Once reached, the butterfly will fly to the bottom of a car. The player will learn how to crouch wit a tutorial sign to reach the butterfly.

once reached, the butterfly will go to the top of a trailer truck . The player will need to learn how to climb ladders with a tutorial sign to reach it.

Once reached the butterfly will go to the elevator at the end of the parking lot ending the first level and starting Cutscene #2

**<u>Cutscene #2</u>**
Once reached, the butterfly will finally fly off the screen but the cat will notice another cat at the building next to it. Now we have a new objective. The can will then go to the elevator and click it to proceed. This zoom out a bit as the cat goes down the main focus will be the background to show off my incredible art skills as well as the credits which will be all me. I might add in a joke like "me again" "me but with a hat on" "surprise guest: me" "director emperor samurai: me" "hokage: me again" "artist: me but with glasses" "driver: me" "sound effects: me but with a cold" the scene will not reach the bottom it will just black out ending the cutscene.

### Level 2
**<u>Cutscene #1</u>**
The level will start with a cutscene of the cat reaching the bottom of the elevator and exiting the elvator. then the elevator will go up and fade away. 








## Player
The player is going to be a simple street cat. No special abilities yet, maybe later I'm still not sure.


### Movements
The movements will include any motions that can be done in an empty space like:

- [ ] MOVE
	- [ ] Code
		- [ ] walk
		- [ ] run
		- [x] sprint
		- [x] jump
		- [x] crawl
	- [x] Animations
		- [x] walk
		- [x] run
		- [x] sprint
		- [x] jump
		- [x] crawl

### Interactions
The interactions will include any motions that can be done either with the level or with objects in the level, like:
- [x] `wall jumping`
- [x] `wall slide`
- [x] `climbing ledges`
- [x] `ledge hanging`
- [ ] `rope swing`
- [x] `pull`
- [x] `push`

### Abilities 
The abilities will include anything that is not natural to a cat like with cybernetics like:
- [ ] `double jump`
- [ ] `shoot lazers`
- [ ] `sonar`


## Tutorial
1. Setting up the project
	- Install Unity
	- download asset
2. What's in it
	- Structure of the project
	- What can you do with it
3. How to adjust it to your needs
4. Adding your Sprites
5. Adding UI:
	- Start Menu / 
	- Intro Screen/ Credit Screen
	- 

**Questions to answer:**
1. How are abilities being used
2. Where is the Jump button being processed


**What I'm trying to do:**
The ability modules follow a certain order. I made a test print to see what's being ran first.

Look for other modules that also interact with a game object and copy their procedure.

### Scenes
#### Intro
**What**
This will explain a part of the story which as of now is nonexistent.

**How**
This is done with a `Timeline` which you can put things like words and animations as well as change scenes
#### MainMenu
**What**
This will start with a short chilling animation loop waiting for the player to chose

**How**
This will be a regular menu with two buttons on a `Canvas` object with a `MenuHandle` script [^1]
- Start
- Quit
#### Level_1
**What**
This will be the start of our adventure in the world of CyberCat Starting with a short animation of the cat leaving a building. Also, it will have the introduction to the main game mechanics with a tutorial with all the **main** things you can do.[^2]

**How**
Do it with an image telling how to do it just like in the stick figure example
#### Cutscene_1
**What**
This will be the introduction cinematic which will will be where the intro credits will roll as the cat waits for the lift to reach the bottom

**How**
Play cinematic then end the scene by switching to level 2

[^1]: Need to find a way to save the progress. maybe just the level
[^2]: Don't overwhelm the player, just show necessary for completing the next level