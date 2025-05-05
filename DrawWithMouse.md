# Summary for DrawWithMouse.cs


[Class Name: DrawWithMouse]
Purpose: The purpose of this class is to allow the user to draw with their mouse on a texture, allowing them to place objects and manipulate the texture.

Public Methods:

Method Name: Awake
Parameters: None
Description: This method initializes the instance variable "Instance" if it is null or destroys the gameObject if the instance variable is not null. It also creates a new material using the DrawShader and sets its texture coordinate as red.
Returns: void

Method Name: Start
Parameters: None
Description: This method initializes the snowMaterial and drawMaterial, sets the splatmap's texture coordinate as a temporary render texture, and sets the material texture to the new texture. It also resets the texture on the material and the Shader.
Returns: void

Method Name: ToStart
Parameters: None
Description: This method creates a new Shader and material using the DrawShader, sets its color as red, and sets it to the snowMaterial.
Returns: void

Method Name: Update
Parameters: None
Description: This method checks if the drawMaterial is null. If it is not, it will raycast with the mouse click and set the material's texture coordinate using the hit information. It will also debug log the hit information for testing. 
Returns: void

Method Name: DrawToShader
Parameters: RaycastHit hit (out parameter)
Description: This method sets the drawMaterial's texture in the shader to the hit info, sets a temporary texture to store the shaders output, blits the previous output and the new shaders output with the temporary texture as an input, releases the temporary texture back after use. Sets it to the splatmap and log the hit information for testing.
Returns: void

Method Name: OnGUI
Parameters: None
Description: This method draws the splatmap using GUI in scale mode and sets its size as 256x256. However, this feature is not implemented at this time since the render texture is not drawn to screen yet.
Returns: void

Method Name: ResetTexture
Parameters: None
Description: This method resets the texture on the material and the Shader by creating a new RenderTexture with 1024x1024 dimensions, 0 mipmaps, 0 depth and format ARGBFloat. It also sets it on the Material by first setting it as its new texture on the splatmap RenderTexture and then resets the shaders texture.
Returns: void