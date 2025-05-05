# Summary for ChopperPivotRayCast.cs


Class Name: ChopperPivotRayCast
Purpose: This class is responsible for casting rays from the "Chopper" gameobject and checking for collisions with various objects in the scene, including the "IOL Lens Parent", the "Cataract Geo", and the "Parts(Clone)" object. The class also contains functionality for rotating the gameobjects based on user input.

Public Methods:

1. Start(): This method is called when the script is attached to a gameobject, setting initial variables such as the position of the chopper raycaster and its offset from the center of the gameobject.
2. Update(): This method is called every frame, casting a ray in a specific direction and checking for collisions with various objects in the scene. If there are any collisions, the class will rotate the relevant gameobjects based on user input.
3. TextureToTexture2D(texture): This method is used to convert a Texture object into a Texture2D object, which can be used to access the pixel data of the texture. This method is called when the script detects a collision with the "Parts Clone" gameobject.

Dependencies: The class depends on various UnityEngine components such as MonoBehaviour, GameObject, Vector3, and Material. It also depends on user input to determine the direction of the ray and the speed at which the chopper gameobject should be rotated.