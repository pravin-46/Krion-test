# Summary for Roation.cs

  Class Name: Rotation

Purpose: This class handles the rotation of a game object between a moving target and an offset in space (defined by Vector3 Offset). The class includes methods for starting the rotation, updating the direction of the game object based on the target's position, stopping the rotation when the target is no longer visible, and checking the visibility of the target's position to determine whether it should continue rotating or not. The class also includes debugging information such as drawing the raycast using Debug.DrawRay() and drawing a yellow line at the Raycast's maximum range via Debug.Log(".

Public Methods:

* Start(): This method is called on initialization of the script, where it makes sure that the game object, target, and offset parameters are set.

* Update(): This method gets called once every frame as long as the script component is enabled in the game object. It uses Raycasting to compute the distance between the game object and its target using Physics.Raycast(). If the raycast hits a transform, it will be drawn with Debug.DrawRay() and color yellow and then be set to the hit point on the vector Offset2. If nothing is hit, an error log of "else" is printed and a red line is drawn indicating the end of the raycast.

Dependencies: UnityEngine.Transform target, UnityEngine.Vector3 Offset, UnityEngine.Vector3 Offset2