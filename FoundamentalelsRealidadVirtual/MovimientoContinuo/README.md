# Movimiento Continuo

## Continuous Movement in Unity using the XR toolkit

* Open the Unity project and navigate to the XR Rig game object

* Click on the XR Rig and add the Locomotion System Script to the game object. This script will provide access to the XR Rig from the other movement scripts that will be added later

* Open the Default Input Actions folder inside the Samples folder. This is where the input actions for the XR controllers are located

* Click on the helper presets for Continuous Move and Turn and press the Add to provider default buttons for both of them. This will set up the input actions for Continuous Move and Turn

* Add the Continuous Move provider to the scene to make sure it's action-based. This provider script is connected with the joystick of our hand controllers

* Drag and drop the Locomotion System we just added onto the Continuous Move provider to connect them

* Uncheck the Right hand actions since we only want to move with our Left Hand

* Change the move speed under Continuous Providers if desired

* Set the Main Camera as the Forward Source if desired

* Add the Continuous Turn Provider Action-based to enable rotation. This provider script is connected with the joystick of our hand controllers


* Uncheck the Left Hand Move Actions reference for the Continuous Turn Provider since we only want to rotate ourselves using the right-hand joystick

* Add the Character Controller Component to the XR Rig game object. This will allow us to constrain the movement by collisions without having to deal with a rigid body


* Change the Character Controller's center Y-axis to 1 and use a smaller radius so that we can get closer to the objects

* Test the implementation by hitting play. The left joystick should enable movement and the right joystick should enable rotation. The character should collide with walls and obstacles
