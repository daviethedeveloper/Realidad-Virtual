# Teletransportación


## Implement teleportation into your Unity project using the XR Toolkit:

* Go to the hierarchy window

* Under the hierarchy window, select the XR Rig object that you want to add the teleportation system to

* Next, add the Teleportation Provider component to the XR Rig object. This component is responsible for moving the XR Rig to the desired location based on where we choose

* After adding the Teleportation Provider component, you'll notice that it requires a Locomotion System. So, drag and drop the locomotion system onto it

* Now, go to the Camera Offset object under XR Rig, and add an empty game object by right-clicking and selecting "Create Empty". Name it "Right Hand Parent" as this game object will hold the game objects associated with the right-hand controllers

* Under the Right Hand Parent, add the Right Hand Controller and make sure that the transforms are reset.
Rename the Right Hand Controller to "Right Hand Teleport Controller" as this will be the controller specifically for Teleportation

* Next, create another empty game object under the Right Hand Parent and call it "Right Hand Base Controller"

* Now, add an XR Controller Action-Based component to the Right Hand Base Controller. It comes ready with the right references because we set up the new input system before

* Add the XR Direct Interactor and a Sphere Collider to the Right Hand Base Controller

* Click on the Right Hand Teleport Controller, and under XR Ray Interactor, set the Line type from straight to projectile curve to make it look like aiming for teleportation

* Uncheck the XR Ray Interactor because we don't want a raycaster pointing toward the scene all the time, we only want it when we teleport

* Go to XR Interactors Line Visual and change the valid color to blue or any other color you prefer.
Change the Select Action to "RightHand/TeleportSelect" by choice under the XR Controller. It uses the same bindings as the Select action


* Go to the Github page that includes example projects for XR Interaction Toolkit from Unity, download and extract the example project

* In the example project, go to the WorldInteraction Demo scene, expand XRRigDemo, and you will see a similar Hand controller setup. Here we have this Action Based Controller Manager script, which handles the Teleportation mode switch very well.

* Add the Action Based Controller Manager script to your project and set it up. This script handles the teleportation mode switch

Test the teleportation system in your scene.

https://github.com/Unity-Technologies/XR-Interaction-Toolkit-Examples

https://onedrive.live.com/?authkey=%21AH5uCH91kQkqesc&id=AF7C4978DAD898DD%21121643&cid=AF7C4978DAD898DD&parId=root&parQt=sharedby&o=OneUp


