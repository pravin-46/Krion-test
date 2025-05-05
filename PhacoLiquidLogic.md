# Summary for PhacoLiquidLogic.cs

Class Name: PhacoLiquidLogic
Purpose: The purpose of this class is to control the liquid used during phacoemulsification, which is a medical process for treating certain skin and other body conditions by breaking them down into small particles. 
    It has several methods that are involved in this process. One method involves checking which button was pressed and then disabling or enabling it in a specific manner.  
Dependencies: UnityEngine, FlexSourceActor.cs, HapticPlugin.cs
Public Methods:
         Method Name: Start 
          Purpose: The "Start" function initiates the values of variables associated with the Phaco Liquid Logic class. It also sets the water to appear by checking if the button was pressed.  
         Returns: void.
        Method Name: Update. 
          Purpose: The "Update" function is called every frame and uses various inputs from user through Input class (either keyboard with KeyCode.I, or JHorizontal joystick which can trigger it in one of two ways -  by pressing the key I, or when it equals 1).  
        Method Name: fluidDisAppear. 
          Purpose: The "fluidDisappear" function is used to drain the liquid from the container and then make the water disappear through this coroutine method.
        Returns: void.
