# Movimiento Continuo

## Continuous Movement in Unity using the XR toolkit

* Open the Unity project and navigate to the XR Rig game object

* Click on the XR Rig and add the Locomotion System Script to the game object. This script will provide access to the XR Rig from the other movement scripts that will be added later

* Add the Locomotion System Component to the XR Origin - Drag and Drop the the XR Origin

<p align="center"><img src="Moviement_Images/2023-03-16%20(27).png" alt="Logo" > </p>
<p align="center"><img src="Moviement_Images/Screenshot%202023-03-16%20200130.png" alt="Logo" > </p>



* Open the Default Input Actions folder inside the Samples folder. This is where the input actions for the XR controllers are located

* Here you can view the binding movement for each action - think of it as a Dictionary/Hashmap in code

<p align="center"><img src="Moviement_Images/2023-03-16%20(29).png" alt="Logo" > </p>




* Click on the helper presets for Continuous Move and Turn and press the Add to provider default buttons for both of them. This will set up the input actions for Continuous Move and Turn


<p align="center"><img src="Moviement_Images/2023-03-16%20(30).png" alt="Logo" > </p>
<p align="center"><img src="Moviement_Images/2023-03-16%20(31).png" alt="Logo" > </p>


* Add the Continuous Move provider to the scene to make sure it's action-based. This provider script is connected with the joystick of our hand controllers

* Add the Continuous Turn Provider Action-based to enable rotation. This provider script is connected with the joystick of our hand controllers

<p align="center"><img src="Moviement_Images/Screenshot%202023-03-16%20200350.png" alt="Logo" > </p>


* Uncheck the Right hand actions since we only want to move with our Left Hand

* Change the move speed under Continuous Providers if desired

* Set the Main Camera as the Forward Source

* Uncheck the Left Hand Move Actions reference for the Continuous Turn Provider since we only want to rotate ourselves using the right-hand joystick

* Drag and drop the Locomotion System we just added onto the Continuous Move provider to connect them

<p align="center"><img src="Moviement_Images/Screenshot%202023-03-16%20200423.png" alt="Logo" > </p>



* Add the Character Controller Component to the XR Rig game object. This will allow us to constrain the movement by collisions without having to deal with a rigid body

* Change the Character Controller's center Y-axis to 1 and use a smaller radius so that we can get closer to the objects


<p align="center"><img src="Moviement_Images/2023-03-16%20(32).png" alt="Logo" > </p>




* Test the implementation by hitting play. The left joystick should enable movement and the right joystick should enable rotation. The character should collide with walls and obstacles

<p align="center"><img src="Moviement_Images/2023-03-16%20(33).png" alt="Logo" > </p>
