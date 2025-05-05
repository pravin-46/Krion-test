# Summary for RightCollisionDetection.cs

Class Name: `RightCollisionDetection`
- The `RightCollisionDetection` class is responsible for detecting the presence of a right tool in the scene.
Purpose: This class implements the singleton pattern, which means that it allows only one instance of this class to exist at any given time. It also provides methods for handling when an object enters or exits the detection trigger area.
Public Methods: 
- The `Awake` method is called automatically by Unity. If the `Instance` variable is null, this sets it to the current instance of the class. Otherwise, it destroys the game object that triggered the awake call.
- The `OnTriggerEnter` method is called when an object enters the detection trigger area. It checks if the tag of the collided object is "RightTool" and if so, sets the `IsRightTool` variable to true.
- The `OnTriggerExit` method is called when an object exits the detection trigger area. It checks if the tag of the collided object is "RightTool" and if so, sets the `IsRightTool` variable to false.  
Dependencies: UnityEngine.dll, System.dll, and System.Runtime.Serialization.dll.