# Summary for phacoProcedure.cs

Here is a summary of the provided C# code:

Class Name: phacoProcedure

Purpose: This class enables playing two audio clips sequentially, with a delay of 10 seconds in between.

Public Methods:

* Start()
    * Called once when the component is started.
    * Set both audio objects to inactive.
    * Starts the coroutine "phacoAudio" using the "StartCoroutine" method.
    
* Update()
    * Called every frame after "Start".
    * No functional code.
    
* phacoAudio()
    * Returns an enumerator (IEnumerator).
        // waits for 10 seconds before starting the coroutine
    * Activates audio object number 17 using the ".SetActive" method after waiting for 10 seconds.
        // waits for another 7 seconds after activating audio 17 before activating audio number 18 

Dependencies:
* UnityEngine (for GameObject and MonoBehaviour components)