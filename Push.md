# Summary for Push.cs

Class Name: Push
Purpose: This class is used to push a rigidbody moving left with a force of 1000f

Public Methods:

* Start () 
This method is called before the first frame update. It does not have parameters and does not return anything. It simply initializes the object.

* Update()  
This method is called once per frame and it handles adding force to the gameobject moving left with a force of 1000f. The method also checks if the MeshCollider component's convex parameter is true or false, if the mesh is not convex, the method will make it convex and then apply the force.
	
Note: The method comment //this.GetComponent<MeshCollider>().convex = true; is a redundant statement as the initial value of the convex parameter is already set to false. Therefore, the method simplistically sets the convex property of MeshCollider to false after setting it to true at the beginning without any purpose.