# Summary for Instruction_Logic.cs

Class Name: Instruction_Logic
Purpose: This class is responsible for managing the enablement of pop-up instructions. It provides a central place to control the visibility and behavior of multiple pop-up instructions.
 
Public Methods:
Method Name: PopEnable(int index)
Parameters: int index - The index of the pop-up instruction that should be enabled.
Description: This method enables the specified pop-up instruction and disables all others by setting their active state to false. The parameter "index" is used to determine which pop-up instruction should be enabled. 
When an instuction is enabled, it becomes visible and can be interacted with. When disabled, it is hidden and cannot be interacted with.
Returns: void - This method does not return any values.
Dependencies: UnityEngine.GameObject[]. The Instruction_Logic class depends on the use of GameObject[] to store pop-up instructions and enable/disable them.

