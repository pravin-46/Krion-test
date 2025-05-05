# Summary for Rotation_curve.cs

 Class Name: Rotation_curve

Purpose: The purpose of this script is to enable the object it is attached to rotate around a target object in response to user input. Specifically, it allows the object to track the mouse position and orient itself towards the target while also maintaining a fixed distance from it.

Public Methods:
1. Update () - This method is called once per frame, allowing the script to update its internal state and perform any necessary actions in response to user input.
2. Start () - Called once when the object starts, it allows the script to initialize any variables or setup required for operation.
3. OnDestroy () - This method is called when the object is destroyed, useful for cleaning up any resources used by the script during its lifetime.
4. OnTriggerEnter () - Called when this collider enters another one with our Trigger flag enabled on the other.
5. OnTriggerExit () - Called when this collider exits another one with our Trigger flag enabled on the other.
6. OnTriggerStay () - Called when this collider stays in contact with another collider that has our Trigger flag enabled for a set amount of time.
7. LateUpdate() - Called every frame but after all objects' update functions have been called. Can be used to detect collisions.
8. FixedUpdate() - Called every fixed framerate frame, if the timestep parameter of Time.fixedDeltaTime is non-zero. Used for physics calculations.
9. Awake() - This method is called when the object is first created.
10. StartCoroutine () - It starts a coroutine with the specified IEnumerator implementation. A Coroutine is a type of iterator that allows you to write iterative code, allowing for asynchronous operations.
11. StopCoroutine() - This method stops the specified coroutine, if it was started by the same game object and script.
12. Reset()- It resets the current value of all class variables to their default values.

Dependencies:

 - UnityEngine - The base unity engine namespace that contains all the unity built-in classes and functions required for the project. 
 - System.Collections - This is the namespace for the system collections, it provides data structures that allow you to store a collection of objects. For example, the list class.
  - System.Collections.Generic - It is responsible for providing generic implementations of all the collection types provided with System.Collections. It also provides a number of additional types and features that enhance the functionality of collections when used with generics.