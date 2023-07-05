```toc
```

## Intro
The purpose of this is to find ways to get the most out of ChatGPT 4.0 or in other words, Artificial Intelligence. I have some ideas on how to use it properly so I will catalog and tests them and redefine them if needed. 

<u>End Goal</u>
The end goal is to be much more productive than I am now

<u>General Purpose Ideas</u>
- Act as an expert in { whatever technology I'm currently using } and answer me some questions. I want the answers to be in simple terms.

<u>Specific Projects Ideas</u>
1. Specify exactly the technology I'm using along with any outside libraries I might want to use.
	- i.e. Kotlin, Kotlin build kts plus Material something like that
2. Specify exactly what I'm trying to do, So they have a better understanding of where the questions are headed.
	- i.e. I'm trying to build an application.
3. Specify exactly what I want it to do. 
	- I want you to provide me with working code
4. Maybe provide the whole code?

<u>What I need to know for a specific project</u>
I need to have a good understanding of the structure of the project. (i.e. `onCreate()`, `onClick()`, `onEnd()`) Might want to use excalidraw for structure checkups. How is the code being executed, what executes first, 


## Experiment number 1
**Objective**
Make an simple app from start to finish using ChatGPT. The app is meant to be simple but complete with unit testing. The app is going to be a replica the game of Tetris and its going to be called Tetris Replica 1.

1. Technology I'm going to use:
	- Kotlin app using minimum SDK of API 29 Android 10.0, with the Kotlin DSL built configuration language.
2. What I'm trying to do in simple terms:
	- I want to make an Android Application. The application is going to be a replica of the game of Tetris. 
3. What I'm trying to do in a more technical terms:
	- I want the app to have three main screens:
		- intro screen showcasing the title.
			- This screen will only have the tile and a "Start" button which will start the game.
			- I want the title to have some kind of animation. 
		- game screen is where the game is going to be played
			- There's going to be a main window which will show the current game that is being played
			- A current score window which is going to be updated every time the player score a line.
			- another window where the next Tetris piece will show
			- a controller section with a d-pad and two buttons, one for turning the Tetris piece currently falling and another one that will instantly drop the piece.
		- credit screen where we can see all the previous scores
			- This will showcase the top ten scores
			- it will also have a button to play again
1. Explain the structure of the app and what is in every class.[^1] This could take a whole section to come up with a good diagram.
2. Here is the start up code



[^1]: I was thinking about coming up with the diagram first then let ChatGPT do the code but I think it might be a better idea to let ChatGPT help with the diagram as well.