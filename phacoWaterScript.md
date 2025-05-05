# Summary for phacoWaterScript.cs


Class Name: phacoWaterScript
Purpose: This class is responsible for managing the active state of two water GameObjects in the scene. It uses the Input.GetKeyDown() function to check for the press of two specific keys on the keyboard (Z and X), which will activate and deactivate the water GameObjects respectively.

Public Methods:

* Start() : This method is called before the first frame update, and it sets the active state of the water01 and water02 GameObjects to false using SetActive(false).
* Update() : This method is called once per frame, and it uses the Input.GetKeyDown() function to check for the press of two specific keys (Z and X) on the keyboard. If the key Z is pressed, the active state of the water01 and water02 GameObjects is set to true using SetActive(true). If the key X is pressed, the active state is set back to false.

Dependencies: This class depends on two GameObjects named "water01" and "water02", which must be present in the scene. It also depends on the Input.GetKeyDown() function, which is part of the UnityEngine namespace.