# Summary for ForcepsAnimator.cs

Class Name: ForcepsAnimator
Purpose: This class is responsible for animating the forceps character model and setting the HapticPlugin buttons.
Public Methods:
Method Name: Start
Parameters: None
Description: The Start method is called when the object is initialized, it stores a reference to the Animator component of the object in the ForcepepsAnime variable using GetComponent<Animator>() method.
Returns: Void

Method Name: Update
Parameters: None
Description: The Update method is called every frame, it checks if the HP.Buttons[0] variable is equal to 1 and updates the "HP_Buttons" parameter of the Animator component with a value of 1 using SetInteger method.
Returns: Void
Dependencies: HapticPlugin

Note: The class depends on HapticPlugin for the input of buttons, therefore it's important to make sure that HapticPlugin is included in the project dependencies and initialized properly before using this class.