# Summary for Displays.cs

Class Name: Displays
Purpose: The Displays class is a MonoBehaviour in Unity that contains methods for interacting with displays connected to the device. It initializes and manages the display settings.
Public Methods:

* Start(): Upon starting the application, this method activates the second display if there are more than two displays connected. This is necessary for multi-display setups.
* Update(): This method is called once per frame and is empty in this case.
Dependencies: The Displays class depends on UnityEngine.CoreModule, which provides various classes and methods used throughout the functionality of the application.