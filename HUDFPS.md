# Summary for HUDFPS.cs


Class Name: HUDFPS

Purpose: The class is responsible for calculating the frames per second (FPS) and updating a GUIText component with the current FPS value. The class is attached to a GameObject in the Unity scene, and it uses the UnityEngine.UI.GUIText component to display the FPS value.

Public Methods:

* Start
	+ Description: Called when the class is initialized. It gets the referenced GUIText component and checks if it is missing. If it is missing, the class disables itself by setting its enabled property to false.

* Update
	+ Description: Called every frame update. It calculates the current FPS based on the accumulated time and number of frames, updates the GUIText component with the FPS value, and resets the accumulator and counter for the next interval.
	+ Parameters: None
	+ Returns: Nothing

* updateInterval
	+ Description: The time interval between each frame calculation and update.
	+ Type: Float
	+ Default Value: 0.5

* accum
	+ Description: The accumulated FPS value over the current interval.
	+ Type: Float

* frames
	+ Description: The number of frames drawn over the current interval.
	+ Type: Int

* timeleft
	+ Description: The time left for the current interval.
	+ Type: Float

* guitext
	+ Description: A reference to the attached GUIText component.
	+ Type: Text

Dependencies: UnityEngine.UI.GUIText, UnityEngine (for the Time.deltaTime and Time.timeScale properties)