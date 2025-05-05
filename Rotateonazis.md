# Summary for Rotateonazis.cs

Class Name: Rotateonazis
Purpose: The purpose of this class is to rotate the game object on an axis around a center point, while scaling its distance from the center point.

Public Methods:

* Start()
	+ Purpose: Finds the cube with the specified tag "Player" and sets it as the center point for rotation. Sets the initial position of the current game object to be on the desired radius from the center point, in the direction of the axis.

* Update()
	+ Purpose: Rotates the game object around the center point by a specified angle per second (rotationSpeed) and moves the object along its axis towards a desired position at a specified speed (radiusSpeed). The desired position is calculated as a normalized vector from the current position to the center point with a magnitude of radius.

Dependencies:

* MonoBehaviour
	+ Purpose: Represents a script that is attached to a Unity engine GameObject and has functionality to interact with the game engine.

* Transform
	+ Purpose: Contains information about the position, rotation, scale, and other properties of a Unity engine GameObject in 3D space.

* Vector3
	+ Purpose: Represents a 3D vector in a 3D cartesian coordinate system, used for mathematical operations related to 3D geometry and transformations.