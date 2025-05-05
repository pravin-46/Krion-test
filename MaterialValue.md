# Summary for MaterialValue.cs


Class Name: MaterialValue

Purpose: This class represents a value that can be used to dynamically change the ZWrite property of a material. It allows developers to set the Z Write property in the Unity Inspector and updates the material's ZWrite when the script is enabled or disabled.

Public Methods:

* Start
    * Description: This method is called before the first frame update, and it initializes the material and sets the value of the ZWrite property.
    * Parameters: None
    * Returns: Nothing
* Update
    * Description: This method is called once per frame, and it does nothing in this case since there is no relevant logic to execute here.
    * Parameters: None
    * Returns: Nothing

Dependencies:

* UnityEngine.Material (used for the material property)
* System.Collections.Generic.Dictionary&lt;string, object&gt; (used for storing and retrieving the ZWrite value)