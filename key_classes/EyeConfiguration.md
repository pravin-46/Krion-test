# Summary for EyeConfiguration.cs

 Class Name: EyeConfiguration
 Purpose: This class is responsible for managing the position, rotation and scale of an eye object in a Unity scene. It provides various methods to change the eye's visual representation based on user input.
 
 Public Methods:

* `Awake()`: This method initializes the singleton instance of this class by setting the `Instance` variable.
* `Update()`: This method is called every frame and updates the eye's position, rotation and scale based on the user's input. It changes the eye's visual representation based on the user's decision.
* `ChangeProposition()`: This method changes the eye's visual representation based on a given set of vectors.

 Variables:

* `Instance`: A static variable that represents the singleton instance of this class, and is used to access the global state.
* `Eye`: A Transform component that represents the eye object in the scene.
* `RightSuperior`, `LeftSuperior`, `RightTemporal`, `LeftTemporal`: Arrays of vectors that store the coordinates, rotations and scales of eye visual representations for different options. Some are [HideInInspector] because they are not intended to be changed from the Inspector window.
* `IsLeftSuperior`, `IsRightSuperior`, `IsLeftTemporal`, `IsRightTemporal`: Bool variables that indicate if the current visual representation is of a superior or temporal orientation.

Important Methods:

* `ChangeProposition()`: This method changes the eye's visual representation based on a given set of vectors. It takes an array of 3 vectors as input and applies them to the `Eye` transform, rotating it by the specified angles in its Y axis and scaling it along the Z axis.
* `Update()`: This method updates the position, rotation, and scale of the eye object based on the user's input. It uses the `IsLeftSuperior`, `IsRightSuperior`, `IsLeftTemporal`, and `IsRightTemporal` values to decide which representation to show. Whenever a new value is given for any of these variables, it calls the `ChangeProposition()` method with the corresponding set of vectors.
* `Awake()`: This method initializes the `Instance` variable by setting it to this class instance. Then, if there exists already an instance in the scene, it destroys this game object.