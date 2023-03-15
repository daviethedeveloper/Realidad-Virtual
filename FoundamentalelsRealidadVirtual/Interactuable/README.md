# Interactuable

## Get Started With Interaction

* Add a plane to the scene and make sure gizmos are enabled

* Set up the player space to be a 6 meter by 6 meter area where the player can spawn

* Create a cube and rename it to "Table". Drag it in the forward camera direction

* Create a "Material" folder in the "Assets" folder and create a material for the table with any color you prefer

* Go to the Unity Asset Store and download the "Medical Kit" asset

* Import the downloaded package into your Unity project

* In the "Project" tab of the "Scene View", go to "Prefabs" and drag the medical kit prefab to the scene view

* Select the prefab and add a Mesh Collider and Rigid Body component. Make sure to change the collision detection mode of the Rigid Body to "Continuous Speculative"

* For the water bottle and flashlight prefabs, add an XR Ray Interactor component to both the left and right hand XR Rig. This is preset with a ray interactor that shoots out a line from the hand and checks if it can interact with anything that line hits. If it can interact, it will bring the item to the hand

* There is also a Direct Interactor that can be used, which is a sphere collision object. If there is a collider, it will be picked up. You can only choose one, but there is a possible way to make them a parent object if necessary.
The XR Ray Interactor can work with UI and teleportation. It has a preset Interaction Line Visual that turns red and white when it knows what it can pick up.

* Add the XR Grab Interactable component to the objects you want to interact with. This will contain the data for anything that can be interacted with.

* Use Layer Mask to choose which collider to interact with if there are many colliders on an object.
You can set up a custom reticle for when hovering or interacting with an object. This is a 2D sprite that maps to the surface of the object.


* For the table created in step 3, don't forget to add a Rigid Body component and set it to "Continuous".
To set up the Default Hand Controller, delete all components attached to the right hand controller in a specific order.
Add the following components: XR Controller Action Based, XR Direct Interactor, and Sphere Collider. Resize the sphere collider as necessary.


* Check both prefabs of the object under Mesh Collider. For the right hand sphere collider, check IsTrigger to allow it to go through and have a trigger interaction.


* Make sure to uncheck Anchor Control for both left and right hand XR Ray Interactor when walking and holding an object.
For movement type under XR Grab Interactable, choose between physics space, velocity tracking, kinematic, or instantaneous teleportation depending on the desired effect.


## Step-by-Step Guide Understanding XR Grab Interactable 

### Layer Mask
This allows you to choose which layers the interactable will interact with. For example, if you have a table with multiple colliders, you can choose to only interact with the top of the table and ignore the legs

### Interaction Manager
This allows you to specify which interaction manager the interactable should use. This is useful if you have multiple interaction managers in your scene

### Attach Transform
This allows you to specify a transform that the interactable will snap to when it's picked up. For example, if you have a tool that should snap to the player's hand when it's picked up, you can use this to specify the hand transform

### Interaction Layer Mask
This allows you to choose which layers the interactable can interact with. For example, if you have a gun that shouldn't be able to interact with other guns, you can use this to restrict the interaction to only certain layers.
Selecting Interactor Type - This allows you to choose which type of interactor will be used to select the interactable. The options are: Ray Interactor, Direct Interactor, and Hybrid Interactor

### Movement Type
This allows you to choose how the interactable should move when it's picked up. The options are: Kinematic, Velocity Tracking, and Instantaneous Teleport


### Throw
Throw - This allows you to specify the throw settings for the interactable. You can adjust things like the throw force, the direction of the throw, and the amount of randomness.
Haptic Feedback - This allows you to specify haptic feedback for the interactable. You can adjust the intensity and duration of the feedback

### Custom Reticle
This allows you to specify a custom reticle for the interactable. For example, if you have a gun, you could use a crosshair reticle that appears when the player is aiming.
On First Hover Enter - This allows you to specify a Unity Event that will be triggered when the player first hovers over the interactable

### On Last Hover Exit
This allows you to specify a Unity Event that will be triggered when the player stops hovering over the interactable

### On Select Entered
This allows you to specify a Unity Event that will be triggered when the player selects the interactable

### On Select Exited
This allows you to specify a Unity Event that will be triggered when the player deselects the interactable

### On Activate
This allows you to specify a Unity Event that will be triggered when the interactable is activated


Overall, the XR Grab Interactable in Unity XR Toolkit gives you a lot of flexibility when it comes to specifying how interactable objects in your scene will behave. By understanding each of the different options available, you can create complex interactions that feel natural and intuitive for the player.

