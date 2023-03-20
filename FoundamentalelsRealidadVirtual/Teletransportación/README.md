# Teletransportación


## Implement teleportation into your Unity project using the XR Toolkit:


<br>

* Open Unity and load the project you are working on
* Click on the XR Rig in the scene and add the Locomotion System - Drag and Drop the XR Origin 
* Click on the XR Rig in the Scene and add the Teleportation Provider component

<p align="center"><img src="Teleportation_Images/2023-03-19%20(1).png" alt="Logotipo"></p>


<br>
<br>
<br>

* Under Camera Offset, right-click and create an empty game object called "Right Hand Parent"
* Drag the Right Hand Controller under the Right Hand Parent
* Make sure to reset the transforms for the Right Hand Parent and Right Hand Controller


<p align="center"><img src="Teleportation_Images/Screenshot%202023-03-19%20195421.png" alt="Logotipo"></p>
<p align="center"><img src="Teleportation_Images/Screenshot%202023-03-19%20195539.png" alt="Logotipo"></p>
<p align="center"><img src="Teleportation_Images/2023-03-19%20(2).png" alt="Logotipo"></p>



<br>
<br>
<br>

* Change the name of the Right Hand Controller to "Right Hand Teleport Controller"
* Create another empty game object under the Right Hand Parent and call it "Right Hand Base Controller"

<p align="center"><img src="Teleportation_Images/2023-03-19%20(3).png" alt="Logotipo"></p>
<p align="center"><img src="Teleportation_Images/2023-03-19%20(4).png" alt="Logotipo"></p>



<br>
<br>
<br>

* Add an XR Controller Action-Based component to the Right Hand Base Controller
* For the base controller, add an XR Direct Interactor and a Sphere Collider

<p align="center"><img src="Teleportation_Images/2023-03-19%20(5).png" alt="Logotipo"></p>


<br>
<br>
<br>

* Click on the Right Hand Teleport Controller and under XR Ray Interactor, set the Line type from straight to projectile curve

<p align="center"><img src="Teleportation_Images/2023-03-19%20(6).png" alt="Logotipo"></p>


<br>
<br>
<br>

* Uncheck the XR Ray Interactor to hide the raycaster when not teleporting
* Go to XR Interactors Line Visual and change the valid color to green

<p align="center"><img src="Teleportation_Images/2023-03-19%20(7).png" alt="Logotipo"></p>
<p align="center"><img src="Teleportation_Images/2023-03-19%20(8).png" alt="Logotipo"></p>



<br>
<br>
<br>


* Scroll up to the XR Controller and change the Select Action to "RightHand/TeleportSelect"

<p align="center"><img src="Teleportation_Images/2023-03-19%20(23).png" alt="Logotipo"></p>
<p align="center"><img src="Teleportation_Images/2023-03-19%20(24).png" alt="Logotipo"></p>


<br>
<br>
<br>


* Open towards the Default Input Actions and check for the Right Hand Binding Actions

<p align="center"><img src="Teleportation_Images/2023-03-19%20(10).png" alt="Logotipo"></p>

<br>
<br>
<br>


* Check XRI RightHand Locomotion - Teleport Select - Check the Binding actions associated with this



<p align="center"><img src="Teleportation_Images/2023-03-19%20(11).png" alt="Logotipo"></p>



<br>
<br>
<br>


* Click on Teleport Mode Activate to check the binding action

<p align="center"><img src="Teleportation_Images/2023-03-19%20(12).png" alt="Logotipo"></p>


<br>
<br>
<br>


* Click on Teleport Mode Cancel to check the binding action

<p align="center"><img src="Teleportation_Images/2023-03-19%20(13).png" alt="Logotipo"></p>


<br>
<br>
<br>


* Attach the 'Action Based Controller Manager' to Parent Hand Controller - This script will allow the switch between base controller action and teleport action controller

<p align="center"><img src="Teleportation_Images/2023-03-19%20(14).png" alt="Logotipo"></p>


<br>
<br>
<br>

* Attach the correct binding actions to the Parent Hand Controller 

<p align="center"><img src="Teleportation_Images/2023-03-19%20(15).png" alt="Logotipo"></p>

<p align="center"><img src="Teleportation_Images/2023-03-19%20(16).png" alt="Logotipo"></p>



<br>
<br>
<br>


* This is the result of attaching the appropiate binding actions

<p align="center"><img src="Teleportation_Images/Screenshot%202023-03-19%20212616.png" alt="Logotipo"></p>


<br>
<br>
<br>


* Attach the Teleportation Area Script to the Floor where the Player will spawn on

<p align="center"><img src="Teleportation_Images/2023-03-19%20(17).png" alt="Logotipo"></p>


<br>
<br>
<br>

* Drag and drop the Box Collider into the 'Colliders'

<p align="center"><img src="Teleportation_Images/2023-03-19%20(18).png" alt="Logotipo"></p>



<br>
<br>
<br>



* Create a new Teleport area mask and make sure that the Floor 'Layer' is 'Teleport'. 

<p align="center"><img src="Teleportation_Images/2023-03-19%20(19).png" alt="Logotipo"></p>


<br>
<br>
<br>


* The 'Interaction Layer Mask' under Teleportation Area set to 'Teleport'

<p align="center"><img src="Teleportation_Images/2023-03-19%20(20).png" alt="Logotipo"></p>
<p align="center"><img src="Teleportation_Images/2023-03-19%20(21).png" alt="Logotipo"></p>


<br>
<br>
<br>











