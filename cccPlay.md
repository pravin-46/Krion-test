# Summary for cccPlay.cs

  Class Name: cccPlay

 Purpose: The class handles the animations and interactions of the spheres in the game, including dragging and swapping. It also includes functionality to control the sliders, which regulate the speed and strength of the movements.

 Public Methods:

     Method Name: Start()
     Parameters: none
     Description: The method is called when the script is initialized. In this case, it initializes all 12 sphere objects as Inactive except for one, which is set to active. It also sets up animations for each sphere and initial values of sliders.

     Method Name: Update()
     Parameters: none
     Description: The method updates the position of the spheres depending on their tags, which correspond to the animation parameters. For example, when a sphere with tag "Sphere01" enters this object's collider, it plays an animation and sets another sphere with tag "Sphere02" as active.

     Method Name: OnTriggerEnter(Collider other)
     Parameters: Collider other
     Description: When a collision occurs between the object and another object that has a sensor, this method is called which updates the properties of the spheres in the game based on their tags. It also initiates animations and swaps them with each other for different levels.

       Dependencies: HapticPlugin, UnityEngine, Animator, GameObject