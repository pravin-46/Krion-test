# Summary for LeftToolCollision.cs

Class Name: LeftToolCollision
Purpose: This class is responsible for detecting when the player's left hand is in contact with a specific game object. It also provides functionality to delay the cut effect for a few seconds after the player touches the object.
Public Methods:
Method Name: Awake
Parameters: None
Description: This method checks if an instance of this class already exists, and if it does, it destroys the current instance. If not, it sets the current instance as the only existing instance. It is called when the script is being initialized.
Returns: Nothing
Method Name: Start
Parameters: None
Description: This method is called after initialization is complete. In this case, we are initializing a variable to False and checking if the player has already selected the left tool (L_cutTemp) for cutting the object. If not, we instantiate the script to allow delay time (Six seconds) before executing the next part of the code, thus giving the player enough time to choose the right cutting tool.
Returns: Nothing
Method Name: Update
Parameters: None
Description: This method is called after every frame update. The purpose for this method is to handle user input when pressing a button. We obtain a list of buttons that are currently selected by calling a function from HapticPlugin and setting the value L_cutTemp to false if the left button has been selected. If the player has not yet chosen any cutting tools, we instantiate a script to delay the cut effect for six seconds.
Returns: Nothing
Method Name: OnTriggerEnter
Parameters: Collider other
Description: This method is called whenever the current gameObject overlaps with another collider. In this script, no actions are taken when this method occurs, but if it did occur, any game objects that were in contact would be listed in the object parameter and can be used to detect if a collision between two game objects has occurred.
Returns: Nothing
Method Name: OnTriggerExit
Parameters: Collider other
Description: This method is similar to OnTriggerEnter; however, this script will stop running once it encounters a situation where the player's left hand is not touching any particular object as designated by the specified tag. 
Returns: Nothing
Method Name: L_CutDelay
Parameters: None
Description: This method is similar to Update in that it waits until it reaches a certain part of its operation before executing further lines of code, but its main purpose is to give time for the player to select cutting tools if they have not chosen anything yet. 8 seconds later, this script will check whether the player's left hand is still touching some object (If they are, they will be able to cut), and if it has been selected in combination with the other objects (RightToolCollisionDetection), then an InstantiateSourceActor4L action will be instantiated. Additionally, L_cutTemp will be set back to True, and temp4HP will also be allowed to change poses again.
Returns: IEnumerator (An object that is used to control the flow of a coroutine)
Dependencies: HapticPlugin, Collision, WaitForSeconds, InstantiateSourceActor4L, MouseCutter 