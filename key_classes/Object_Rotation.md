# Summary for Object_Rotation.cs


Class Name: Object_Rotation
Purpose: This class is responsible for rotating an object according to the user's input using a mouse. It derives from MonoBehaviour, which allows it to interact with the Unity scene.
Public Methods:

* void Update()
    * Called every frame by Unity to update the position and rotation of the object based on the user's input.

Dependencies:

* Using UnityEngine for accessing the Unity scene components such as Input, Camera, and Transform.
* Using System.Collections for handling collections of methods.

This class contains two fields:

* mprevPos: A vector to store the previous position of the mouse cursor.
* mposDelta: A vector to store the difference in positions between the current and previous frames.

The Update() method checks if the user is holding down the left mouse button, and if so, calculates the delta position of the mouse cursor as compared to the previous frame using Input.mousePosition - mprevPos. It then uses this delta to rotate the object around its own up axis (transform.up) by calling the Transform.Rotate() method, first with a positive angle depending on the direction of the movement and then again with a negative angle. Finally, it rotates the object around the right axis of the camera by calling Transform.Rotate() again.

Overall, this code allows the user to rotate an object in 3D space according to their mouse movements in Unity.