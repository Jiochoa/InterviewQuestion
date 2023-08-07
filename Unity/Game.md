```toc
```

Change of plans: 


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

### How to make it look like Limbo

- what are shaders and how to use them.
- how to apply a filter
- shadows in 2d?


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