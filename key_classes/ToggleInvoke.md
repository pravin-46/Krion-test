# Summary for ToggleInvoke.cs

 Class Name: ToggleInvoke
 Purpose: This class is responsible for handling the user's input for the choice tree. It contains a series of methods to handle the different choices that the player can make, and it also includes a coroutine to load a new scene after a certain condition is met.

Public Methods:

* Start(): Called when the class instance is created. This method finds the GameData object in the scene and assigns it to the GD variable. It also adds listeners to the Next and Back buttons to call the respective methods when clicked. Finally, it initializes an array of toggle groups in the scene to be used later.
* Next(): Called when the player clicks the Next button. This method checks which toggle is currently selected (if any) and assigns a value to the ChoiceTree property of the GameData object depending on the selection. If the index is 3, it starts an asynchronous loading process for a new scene using the SceneManager.LoadSceneAsync() method. Otherwise, it enables the next toggle group in the series and disables the current one.
* Quit(): Called when the player clicks the Back button. This method checks which toggle is currently selected (if any) and assigns a value to the ChoiceTree property of the GameData object depending on the selection. If the index is 0, it closes the application using the UnityEditor or Application.Quit() methods (depending if it's running in the editor or as an executable). Otherwise, it enables the previous toggle group in the series and disables the current one.
* LoadYourAsyncScene(): This is a coroutine method that loads a new scene asynchronously using the SceneManager.LoadSceneAsync() method. It yields until the loading process is complete before returning control back to the calling method.

Dependencies:
- UnityEngine: The core engine that allows for creating games and interactive experiences.
- UnityEngine.UI: Provides classes and scripts required for creating UI components in a game or interactive experience.
- UnityEngine.SceneManagement: Allows for loading and managing scenes in a game or interactive experience.

The class ToggleInvoke is responsible for handling the user's input for the choice tree, it contains a series of methods to handle the different choices that the player can make, and it also includes a coroutine to load a new scene after a certain condition is met. The Start method is called when the class instance is created and finds the GameData object in the scene and assigns it to the GD variable. It also adds listeners to the Next and Back buttons to call the respective methods when clicked. Finally, it initializes an array of toggle groups in the scene to be used later.
The Next method is called when the player clicks the Next button and it checks which toggle is currently selected (if any) and assigns a value to the ChoiceTree property of the GameData object depending on the selection. If the index is 3, it starts an asynchronous loading process for a new scene using the SceneManager.LoadSceneAsync() method. Otherwise, it enables the next toggle group in the series and disables the current one.
The Quit method is called when the player clicks the Back button and it checks which toggle is currently selected (if any) and assigns a value to the ChoiceTree property of the GameData object depending on the selection. If the index is 0, it closes the application using the UnityEditor or Application.Quit() methods (depending if it's running in the editor or as an executable). Otherwise, it enables the previous toggle group in the series and disables the current one.
The LoadYourAsyncScene method is a coroutine that loads a new scene asynchronously using the SceneManager.LoadSceneAsync() method. It yields until the loading process is complete before returning control back to the calling method.