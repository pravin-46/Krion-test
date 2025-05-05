# Summary for InitialAudio.cs

Class Name: InitialAudio
Purpose: This class is used to control the initial audio system in a Unity project. It sets and enables three audio sources, audio09, audio10, and audio11, and delays their activation by specified times using coroutines.
Public Methods:
* Start()
	+ Description: Called before the first frame update, this method initializes the audio system by setting initial values for audio objects and starting an asynchronous audio delay routine.
	+ Parameters: none 
	+ Returns: void
* Update()
	+ Description: Called once per frame, this method is empty and serves as a placeholder for any required update logic of the audio system in the future.
	+ Parameters: none 
	+ Returns: void
* audiodelayInital()
	+ Description: A coroutine function that sets activates three audio sources at specified delays by using Unity's SetActive() and WaitForSeconds() methods respectively.
	+ Parameters: none 
	+ Returns: IEnumerator
Dependencies: UnityEngine