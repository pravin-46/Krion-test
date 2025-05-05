# Summary for InputManager.cs

 Here is the summary in markdown format for the provided C# code:

Class Name: InputManager
Purpose: InputManager is a class that manages input events from the player. It is attached to a game object as a component and listens for specific key inputs to trigger animations on the Blade animator.

Public Methods:

* Start()
    * Description: Called when the script instance is being loaded. Sets the visibility of the mouse cursor to false to make it easier for the player to control the sword without any distractions due to showing the mouse cursor.
* Update()
    * Description: Called once per frame. Checks if the player has pressed the "Mouse0" key and sets a boolean value in the Blade animator, "In", to true if it is being held down. It also checks if the player has released the "Mouse0" key and sets the "In" parameter of the animator back to false if that is the case.

Dependencies:

* UnityEngine
    * Description: The InputManager class depends on the Unity Engine package, which provides a platform-independent set of functions for accessing the input events from the player.
* System.Collections
    * Description: The InputManager class also depends on the System.Collections namespace, which provides a set of generic collections that can be used to manage data in a variety of ways, such as storing and retrieving data, or filtering data based on certain criteria.
* System.Collections.Generic
    * Description: This namespace extends System.Collections and provides additional generic collection types, such as lists, queues, dictionaries, and sets, that can be used to manage more complex data structures in a efficient manner.