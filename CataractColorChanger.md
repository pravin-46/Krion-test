# Summary for CataractColorChanger.cs

 Class Name: CataractColorChanger

 Purpose: Controls the color changes of the cataract in the eye exam process.

 Public Methods:
  void Awake()

 - Initializes a public variable "Instance" to refer to this object, which is used to access the methods of this class more easily.

- In the Start(), it finds and assigns an animator component for the current game object.

void Update()

- This method runs continuously during gameplay until the user leaves or exits through a screen.

 - It uses the if-else statement to check whether there is a contact with any collidable objects currently.
    For example, when you touch the cataract geometry. If this condition is true, it calls Timer() method which can animate the color change based on the elapsed time between frames.

void Animate()

- This method uses if-else statements to control how the colors of the stages are changed. The first step is to set the boolian variables S1(true), s2(false), s3(false), s4(false), and s5(false). If a conditional statement is activated, the stage state changes.

 -  public void GetComponent<Animation>() is used to get the animation component, in case you need any animations later.