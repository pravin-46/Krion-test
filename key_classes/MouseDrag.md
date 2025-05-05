# Summary for MouseDrag.cs

Class Name: MouseDrag
Purpose: Controls the placement and rotation of an object in relation to the user's mouse position.
Public Methods:

* Start()
    * Initializes the Animator component and sets the cursor to invisible.
* Update()
    * Updates the object's position based on the user's mouse input.
        + If the left mouse button is pressed, the "In" trigger is set.
        + If the left mouse button is released, the "Out" trigger is set.
        + The object's distance from the camera is updated based on the user's mouse position.
        + The object's rotation is updated based on the user's mouse rotation input.

Dependencies:

* Unity Engine
* Animator

Keywords: C#, game development, Unity, object placement, mouse input.