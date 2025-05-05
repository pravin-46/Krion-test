# Summary for ToolSwitch1.cs

  Here is a detailed summary of the provided C# code:
  ```
Class Name: ToolSwitch1
 Purpose: The purpose of this class is to control the tool switch in the Flex simulation. It allows users to choose which tool they want to use by pressing different keys on their keyboard. This class provides functionality for displaying and hiding tools, enabling/disabling FlexFluidRenderer components, and checking whether a tool is enabled or not.
Public Methods:
    Method Name: Update()
    Parameters: None
    Description: This method is called once per frame and updates the state of the tool switch logic. It checks for key inputs to determine which tools are visible and which tools are not, and enables/disables FlexFluidRenderer components accordingly. 
        #region Tools Button logic
            if (Input.GetKey(KeyCode.D))
            {
               
                foreach (GameObject item in Tools)
                {
                    if (item.name == "Dispenser")
                    {
                        item.SetActive(true);
                        
                    }
                    else
                    {
                        item.SetActive(false);
                    }
                }
            }
     #endregion
  ```
This class is declared in the `NVIDIA.Flex` namespace and inherits from `MonoBehaviour`. It has several public fields, including `flexSource`, a list of `FlexFluidRenderer` components, and `Tools`, an array of `GameObject`s, which are used to store references to the game objects containing the tools. 
The class also contains two methods: `Awake()` and `Update()`. The `Awake()` method is called when the script instance is loaded and is used to initialize the variables and detect whether this is the first time an instance of the script has been activated. This instance is then stored as a singleton, so that only one instance can be active at any one time.
The `Update()` method contains all the logic for checking key inputs and using them to switch between different tools. It also enables/disables `FlexFluidRenderer` components depending on if  `HP.Buttons[0] == 1`, where HP is an instance of the `HapticPlugin` class, which handles haptic device interactions in the simulation.
  