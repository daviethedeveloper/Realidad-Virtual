# Configuracion


## Importación de XR a Unity

Guía de instrucciones: Configuración de Unity para el desarrollo de Oculus Quest

<br>


* Open Unity and click on File > Build Settings

<br>

<p align="center"><img src="Configuracion-Images/a_1_step.png" alt="Logo" > </p>

<br>
<br>



* Change the platform to Android

* Follow the link provided and use the Build settings suggested by Oculus for Unity

* Change the Texture Compression to ASTC

* Open Player Settings

<br>

<p align="center"><img src="Configuracion-Images/a_2_step.png" alt="Logo" > </p>

<br>
<br>



* Click on the "XR Plugin Management" button at the bottom left

<p align="center"><img src="Configuracion-Images/a_3_step.png" alt="Logo" > </p>

<br>
<br>



* Click "Install" for Unity's new XR plugin system

<br>

<p align="center"><img src="Configuracion-Images/a_4_step.png" alt="Logo" > </p>

<br>
<br>



* Check the Oculus toggle under the Plugin-in providers for Android

* Click on the Oculus toggle and keep all default settings

<br>

<p align="center"><img src="Configuracion-Images/a_5_step.png" alt="Logo" > </p>

<br>

<p align="center"><img src="Configuracion-Images/a_6_step.png" alt="Logo" > </p>

<br>
<br>



* You can see that this Plug in can be built for both quest and quest 2

<br>

<p align="center"><img src="Configuracion-Images/a_7_step.png" alt="Logo" > </p>

<br>
<br>



* Under Player settings, enter your unique company name for "Company Name"

* Follow Unity's suggestions for other settings

<br>

<p align="center"><img src="Configuracion-Images/a_3_step.png" alt="Logo" > </p>

<br>
<br>



* Choose "Linear" for Color Space

<br>

<p align="center"><img src="Configuracion-Images/a_8_step.png" alt="Logo" > </p>

<br>
<br>


* Ensure that OPENGLES3 is the only Graphics API in Graphics APIs

* Check the "Default package name" toggle and enter your unique package

<br>

<p align="center"><img src="Configuracion-Images/a_9_step.png" alt="Logo" > </p>

<br>
<br>


* Set the Minimum API Level to min 23 Android 6.0 Marshmallow

* Set the Target API Level to Automatic (Highest Installed)

* Set the Install Location to Automatic

<br>

<p align="center"><img src="Configuracion-Images/install_location.png" alt="Logo" > </p>

<br>
<br>

* Check "Multi-threaded Rendering"

* Under Active Input Handling, select "Both"

<br>

<p align="center"><img src="Configuracion-Images/active_both.png" alt="Logo" > </p>
<p align="center"><img src="Configuracion-Images/active_both_2.png" alt="Logo" > </p>


<br>
<br>



* Go to the "Quality" tab under project settings

* Create a new Quality level for Oculus Quest named "Quest"

* Uncheck all the other settings

* Enable the Quest setting for the Android platform

* For PC, go with Ultra

* Set the Pixel Light Count to 1

* Disable Soft Particles

* Select "Per Texture" for Anisotropic Textures

* Select "4x" for Anti Aliasing

* Be sure that "Realtime Reflection Probes" and "Billboards Face Camera" are selected

* Follow the link provided and import Unity's XR Interaction Toolkit

<br>

<p align="center"><img src="Configuracion-Images/a_10_step.png" alt="Logo" > </p>


<br>
<br>

* Go to File > Project Settings

* Choose "Package Manager" and enable "Preview Packages"

<br>

<p align="center"><img src="Configuracion-Images/a_11_step.png" alt="Logo" > </p>

<p align="center"><img src="Configuracion-Images/a_12_step.png" alt="Logo" > </p>

<br>
<br>


* Click on Window > Package Manager

* Choose "Unity Registry"

* Under "XR Interaction Toolkit", click on "Install"

* Check the warning about the new input system from Unity, if you get one

<br>

<p align="center"><img src="Configuracion-Images/a_13_step.png" alt="Logo" > </p>
<p align="center"><img src="Configuracion-Images/a_14_step.png" alt="Logo" > </p>
<p align="center"><img src="Configuracion-Images/a_15_step.png" alt="Logo" > </p>

<br>
<br>

Congratulations, your Unity project is now configured for Oculus Quest development!


<br>
<br>
<br>

## Instructions for Setting up XR Rig for Unity:

<br>

* Add xr origin to heirarchy 

<br>

<p align="center"><img src="Configuracion-Images/add_xr_origin" alt="Logo" > </p>

<br>
<br>



* Create a plane and add texture

<br>

<p align="center"><img src="Configuracion-Images/create_plane.png" alt="Logo" > </p>

<br>
<br>



* In the XR Rig script, set the "Tracking Origin Mode" field as "Floor"

<br>

<p align="center"><img src="Configuracion-Images/track_floor.png" alt="Logo" > </p>

<br>
<br>



* Expand the XR Rig and you will see Camera offset, Left and Right Hand controllers

<br>

<p align="center"><img src="Configuracion-Images/heir_xr_origin.png" alt="Logo" > </p>

<br>
<br>



* To set up the XR Rig for the new input system, go to Assets > Samples > XRI Toolkit > X.X.X  > Default Input Actions

<br>

<p align="center"><img src="Configuracion-Images/find_XRI_strass.png" alt="Logo" > </p>

<br>
<br>



* Click on "XRI Default Left Controller" and click on "Add to ActionBasedController Default"

* Do the same for the "XRI Default Right Controller"

<br>

<p align="center"><img src="Configuracion-Images/add_left_controller.png" alt="Logo" > </p>
<p align="center"><img src="Configuracion-Images/add_right_controller.png" alt="Logo" > </p>


<br>
<br>


* Go to Edit > Project Settings and go to Preset Manager

* Rename "Left" to "LeftHandController" and "Right" to "RightHandController"

<br>

<p align="center"><img src="Configuracion-Images/preset_manager_LR.png" alt="Logo" > </p>

<br>
<br>


* Delete the XR Rig and add it again

* Make sure to reset its transform

* Check that the hand controllers use the correct references, such as LeftHandController using "Left" and RightHandController using "Right" action references

<br>

<p align="center"><img src="Configuracion-Images/left_map_yes.png" alt="Logo" > </p>
<p align="center"><img src="Configuracion-Images/right_map_yes.png" alt="Logo" > </p>

<br>
<br>


* Create two cubes as hands

<br>

<p align="center"><img src="Configuracion-Images/final_picture.png" alt="Logo" > </p>

<br>
<br>

* Now, you are ready to view Unity

<br>
<br>
<br>


## Ver escena construida en VR


To view the new VR scene on your Oculus headset using either Oculus Link or SideQuest, you can follow these steps:

<br>
<br>
<br>

### Using Oculus Link:

* Make sure your Oculus Quest is connected to your PC with a USB-C cable and that you have enabled Oculus Link mode on your headset.

* Open the Oculus PC app on your computer and click on the Devices tab.

* Make sure your Oculus Quest is connected and that it shows up under the Devices tab.

* Launch the VR scene you created in Unity and click on File > Build Settings.

* Select the platform as PC, then click on Build and Run.

* After the scene is built, the Oculus Link window should appear on your PC. Put on your Oculus Quest headset and select the Oculus Link option in the Quest menu.

* Your VR scene should now be visible on your Oculus Quest and you can navigate through it using the controllers.

<br>
<br>
<br>

### Using SideQuest:

* Connect your Oculus Quest to your PC with a USB-C cable.

* Open SideQuest on your computer and make sure your Oculus Quest is recognized by the app.

* Click on the Install APK button in SideQuest and select the APK file you want to install.

* Wait for the installation to complete and then disconnect your Oculus Quest from your PC.

* Put on your Oculus Quest headset and navigate to the Unknown Sources section of the library.

* Select the app you just installed and it should launch the VR scene you created in Unity.

* Congratulations! You have now successfully viewed your new VR scene on your Oculus headset using either Oculus Link or SideQuest.
