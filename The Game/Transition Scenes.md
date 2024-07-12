This will be a How-to transition from scene to scene so you need 2 scenes. 

**Structure**
We will make a new `GameObject` and call it `LevelLoader`, inside of it we will make a `Canvas` and call it `CrossFade`. Make sure its on "Scale with the Screen Size". Get an image in the canvas that will be the main fader image. Then you need to scale the image to the screen then make it black.

![[Pasted image 20230823103723.png]]

Add a "Canvas Group" for multiple things to fade like "Loading..." inside the fader. On the `Canvas` make a new animation and controller. **There will be 2 total animations:**
- one for when the game starts (`Crossfade_End`, meaning it goes away)
- one from when the game ends.(`Crossfade_Start`, meaning to black out the screen)

Starting with the `Crossfade_End`, select it and click "Record", move the timer to a second (or as long as you want the animation to be) then add the fade by making the Alpha of the Canvas Group to 0. We should now have 2 key frames for when it starts and where it ends. The final step is to make it not interactable and not cast any Raycast when the fader is not present. We do that on the "Canvas Group"

For the `Crossfade_Start`, copy every option on the `Crossfade_End` and paste them on `Crossfade_Start` but reverse the key frames so that it starts faded out and returns to full color.

As a last note, make sure they don't loop.

The animations are done. Now we need to set up the Animator so that the game plays it in the right time.

**Animator Controller**
The first is simple since its at the start so we set the Default animation to `Crossfade_End`, then we make a transition to `Crossfade_Start`. This transition will trigger at the end so we will need a trigger condition for the transition which will be used in code. We don't need a transition delay.

We will add a script into the `LevelLoader` game object:

```csharp
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
}
```

![[Pasted image 20230823123308.png]]


We will need to make a coroutine to stager the game while the animation ends

We just made the skeleton for most of the other transitions so well use that.

**Circle Wipe**
We will start by making another `gameObject` and calling it "CircleWipe" then we will follow the same steps aside from the last which is the Animator. We don't need to make another animator we can simply use a `ControllerOverride` and plug in the new animations. Now we just need to add the new `ControllerOverride` into the Animator as well as in the `LevelLoader` Script