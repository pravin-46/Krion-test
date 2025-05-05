# Summary for Cutter_Between_Grabber.cs


Class Name: Cutter_Between_Grabber 

Purpose: This class is used for cutting between grabbers in the Unity game engine. It contains methods that allow the player to cut different parts of an object using their hands as grabters.

Public Methods:

* Start(): Initializes the cutter by getting the component of CutMultiplePartsConcave from this game object, assigning the midpoint between the two grabber positions to midPoint, and enabling the quadDisplay MeshRenderer.  
* Update(): Updates the position and rotation of the cutter based on the distance between the two grabber objects (RayCataract.c.r and ChopperRayCast.c.r). If the player presses any input key while the game enters the trenching state in RunTime_State, it starts a coroutine that runs the Cut() method after 6 seconds to ensure there is no overlap or skipping of cuts. If the input key is not set and/or ChopperRayCast.c.r=0 and RayCataract.c.r=0 then no cut is processed. If any Grabber is not visible, its distance from the other Grabber will be calculated and used to determine cutter visibility for this frame. To lock the position between grabber, player has to press a button (HP.Buttons[0]==1 and HP2.Buttons[0]==1). A coroutine is started in this case that runs the Cut() method after 6 seconds.
* StopCoroutine(cutterTempDelay0()) :Stops any currently running cutterTempDelay0() coroutine, used to temporarily delay cutting during a trenching state.
* QuitGame(): Unused for now. It seems this method is part of the interface MonoBehaviour but has not been implemented.

Dependencies: 
HP2 and GameManager are dependencies required for Cutter_Between_Grabber to function. The HapticPlugin and CutMultiplePartsConcave both extend MonoBehavior and must be set up in Unity's Inspector before running.