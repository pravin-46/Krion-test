# Summary for GameManager.cs


Class Name: GameManager
Purpose: The purpose of the GameManager class is to manage the game's state and provide utility functions for various operations. The class contains instances of other classes that are necessary for the game's operation.
Public Methods:
    - Awake(): Called when the object is created.
        - Check if an instance of this class already exists, and if so, destroy the current object.
        - Initialize the instance of this class.
    - Start(): Called after all objects have been initialized.
        - Set up the game data using the GameData component.
        - Change the eye configuration based on the player's choice.
    - Update(): Called every frame.
        - Check for keyboard input and perform actions accordingly.
    - RegionAlert(Vector2 Region):
        - Check which region of the visual cortex is being targeted by the current player.
        - Perform the corresponding actions based on the region.
    - FadePanel():
        - Set the panel to active.
        - Start a delayed coroutine that will deactivate the panel after 5 seconds.
    - IEnumerator PanelFadeOutDelay(): Called by the coroutine started in FadePanel().
        - Wait for 5 seconds.
        - Clear the texture on the DrawWithMouse class.
        - Deactivate the Grabber object.
    - Reset():
        - Disconnect all devices.
        - Reload the current scene.

Dependencies:

* GameData
* EyeConfiguration
* RightCollisionDetection
* Instruction_Logic

Note: The above summary is a simplified version of the code, and it may not capture all the details of the code.