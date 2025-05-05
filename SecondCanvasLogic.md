# Summary for SecondCanvasLogic.cs

Class Name: SecondCanvasLogic
Purpose: This class inherits from the MonoBehaviour class and provides a set of methods for controlling the panels in the second Canvas. The class is responsible for activating and deactivating the panels, and iterating through them in a circular fashion.

Public Methods:

* Start(): This method is called when the script is started or when the object it is attached to is enabled in the scene. In this method, we initialize the ToolPanels list and set the first panel as active.
* Update(): This method is called every frame when the script is enabled in the scene. We do not have any functionality here, but since it needs to exist in order for the script to work correctly, we leave it empty.
* NextPanel(): This method is responsible for cycling through the panels in a circular fashion. It first checks if the active panel has a next sibling and sets that panel as active. If there is no next sibling, it circles back to the first panel and sets it as active.
* PrevPanel(): This method works similarly to NextPanel(), but instead of checking for a next sibling, it checks for a previous sibling and sets that panel as active. If there is no previous sibling, it circles back to the last panel and sets it as active.

Dependencies:

* UnityEngine.MonoBehaviour (inherited)
* System.Collections.Generic (for List<GameObject> dependency)