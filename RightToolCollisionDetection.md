# Summary for RightToolCollisionDetection.cs


Class Name: RightToolCollisionDetection
Purpose: The purpose of this class is to detect collisions and trigger events when a right tool gets close to the cornea. It also takes care of cutting and replacing the outputCloth.

Public Methods:

* public void OnCollisionEnter(Collision collision): Called when the RightToolCollisionDetection enters a collision with another object. Sets the "touching" field to the name of the collided gameobject.
* public void OnCollisionStay(Collision collision): Called when the RightToolCollisionDetection continues to collide with another object. Updates the "touching" field to the name of the collided gameobject.
* public void OnTriggerEnter(Collider other): Called when the RightToolCollisionDetection enters a trigger volume of a gameobject. Sets the corresponding boolean flag (up/down/left/right) to true if the tag is "CatUp", "CatDown", "CatLeft" or "CatRight" respectively.
* public void OnTriggerStay(Collider other): Called when the RightToolCollisionDetection continues to be inside a trigger volume of a gameobject and updates the "Inside" field to name of the collided gameobject. It also checks if the forceps are close enough to cut the outputCloth (if possible) and sets the "isAttached" flag to true if they are.
* public void OnTriggerExit(Collider other): Called when the RightToolCollisionDetection exits a trigger volume of a gameobject. Sets the corresponding boolean flag (up/down/left/right) to false if the tag is "CatUp", "CatDown", "CatLeft" or "CatRight" respectively.
* public IEnumerator R_CutDelay(): Called after a button press to delay the cutting process for 6 seconds. Updates the "CanCut" flag to false while waiting, and sets it back to true when the delay is over.
* public IEnumerator DestroyDelay(): Called to destroy the outputCloth after a delay of 2 seconds.

Dependencies: The RightToolCollisionDetection requires the HapticPlugin script to be present in the scene, as well as a reference to the cccPlay script and the IsInsideEyeBall script. It also depends on the Animator component being present on the parentCloth gameobject.