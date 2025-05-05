# Summary for GameData.cs


Class Name: GameData

Purpose: This class provides a central location for storing and managing game data. It is a singleton, meaning there can only be one instance of this class in the entire game, and it is marked as non-Destroyed on load which means that it will persist across scenes.

Public Methods:

* ChoiceTree: This method returns an array of choices, which are used to decide what actions are available to the player in different situations.
* Start(): This method is called after the class has been instantiated and is used to perform any necessary initialization tasks.
* Update(): This method is called once per frame and is used to update any variables that need to be updated based on time elapsed.

Private Methods:

* Awake(): This method is called automatically when the scriptable object is loaded and is used to handle any special initialization tasks required at that point. It also checks if there are multiple instances of this class in the scene, and if so, destroys them all except for the one that was created first.