# Summary for ToolSwitchL.cs


Tool Switch L Class:
=====

Purpose:
--------
This script is used to switch between different tools in the toolbox. It allows a user to select a tool and activate it by pressing a specific key on their keyboard or by setting the "To*" boolean flags to true. The script contains a public method called "SetTool" which takes a string parameter representing the desired tool, and sets the corresponding boolean flag to true.

Class Variables:
--------------
* Tools: A List of GameObjects that represent the tools in the toolbox.
* ToPhaco: A boolean flag indicating whether Phaco needle or chopper is active.
* ToSlitBlade: A boolean flag indicating whether Slit blade is active.
* ToLanceBlade: A boolean flag indicating whether Lance blade is active.
* ToColibriForceps: A boolean flag indicating whether Colibri forceps are active.

Class Methods:
-------------
### Start()
This method is called when the script component is enabled or when the game starts. It initializes the "Tools" list by finding all children objects with a tag of "Tools".

### Update()
This method is called once per frame in the Unity Engine update loop. It checks for key presses (P, S, L, or C) and sets the corresponding boolean flag to true if the corresponding tool is pressed. It also iterates over all the tools in the "Tools" list and activates/deactivates them based on the boolean flags.

### SetTool(string tool)
This method takes a string parameter representing the desired tool, and sets the corresponding boolean flag to true. It then updates the UI to reflect the change in active tool.

Dependencies:
--------------
* UnityEngine namespace is required for accessing various Unity Engine features (e.g., Input, KeyCode).
* UnityEngine.UI namespace is required for updating the UI elements.