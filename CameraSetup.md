# Summary for CameraSetup.cs


*Class Name: CameraSetup*
Purpose: The purpose of this class is to set up and manage the cameras used in a virtual reality (VR) application. It creates and activates the required camera objects, sets their properties, and handles user input to switch between mono and stereoscopic modes.
Public Methods:

*Method Name: Start*
Parameters: None
Description: This method is called when the script is initialized. It sets up the cameraHeadTransform and adds the required components (camera, black filters) to the game object. It also creates the left and right eye cameras.
Returns: Void

*Method Name: Update*
Parameters: None
Description: This method is called every frame. It sets the position and orientation of the camera head according to the user's input. If the user presses the "Alpha1" key, it activates the mono mode (single camera view), deactivates the stereo mode, and sets the camera head position and rotation from the OffsetT and OffsetR parameters respectively.
If the user presses the "Alpha2" key, it activates the stereoscopic mode (dual camera view), deactivates the mono mode, sets the camera head position and rotation according to the OffsetT and OffsetR parameters, and activates the left and right eye cameras.
Returns: Void

*Dependencies*: This class depends on the MonoBehaviour inherited script to run in a Unity engine environment.