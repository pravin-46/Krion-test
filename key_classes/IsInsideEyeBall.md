# Summary for IsInsideEyeBall.cs

Class Name: IsInsideEyeBall
Purpose: This class is used to determine whether a tool is inside the eye ball or not. It is attached to the eye ball game object in Unity.
Public Methods:
* `Start()`: The Start method is called once at the beginning of the program execution.
* `Update()`: The Update method is called repeatedly at fixed intervals during the program execution.
* `OnTriggerEnter()`: Called when the collision between two objects starts. The object that is colliding with the eye ball is passed as a parameter. If the tag name "RightTool" or "LeftTool" matches with the tag of the colliding object, then the corresponding boolean variable (isRightToolInside or isLeftToolInside) is set to true.
* `OnTriggerExit()`: Called when the collision between two objects ends. The object that was colliding with the eye ball is passed as a parameter. If the tag name "RightTool" or "LeftTool" matches with the tag of the colliding object, then the corresponding boolean variable (isRightToolInside or isLeftToolInside) is set to false.
Dependencies:
* `using System.Collections;`
* `using System.Collections.Generic;`
* `using UnityEngine;`
This class is part of a larger system that involves tracking the movement and position of game objects in a VR environment. The isRightToolInside and isLeftToolInside variables are used to determine whether a tool is being held by a human player or not.