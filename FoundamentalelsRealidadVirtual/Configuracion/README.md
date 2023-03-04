# Configuracion


## Importación de XR a Unity

Guía de instrucciones: Configuración de Unity para el desarrollo de Oculus Quest

This guide provides step-by-step instructions on how to configure Unity for Oculus Quest development. Follow the instructions in order to ensure that your Unity project is set up correctly.
Open Unity and click on File > Build Settings.
Change the platform to Android.
Go to the link attached to this lecture and follow the Build settings suggested from Oculus for Unity.
Change the Texture Compression to ASTC.
Open Player Settings.
On the left bottom, click on XR Plugin Management.
Press Install for Unity's new XR plugin system.
Check Oculus toggle under the Plugin-in providers for Android.
Click on Oculus toggle here.
Keep all the default settings.
Under Player for other settings, give your unique company name for Company Name.
Follow the suggestions Unity gives for other settings.
Choose linear color space for Color Space.
Make sure to have OPENGLES3 as the only Graphics API in Graphics APIs.
Check the Default package name toggle and enter your unique package.
Set the Minimum API Level to min 23 Android 6.0 Marshmallow.
Set the Target API Level to Automatic (Highest Installed).
Set the Install Location to Automatic.
Check Multi-threaded Rendering.
Under Active Input Handling, select Both.
Go to the quality tab under project settings.
Create a new Quality level for Oculus Quest named Quest.
Uncheck all the other settings.
Enable the Quest setting for the Android platform.
For PC, go with Ultra.
Set the Pixel Light Count as 1.
Disable Soft Particles.
Select Per Texture in Anisotropic Textures.
Select 4x in Anti Aliasing.
Be sure that Realtime Reflections Probes and Billboards Face Camera are selected.
Go to the link attached to this lecture and import Unity's XR Interaction Toolkit.
Go to File > Project Settings.
Choose Package Manager and Enable Preview Packages.
Click on Window > Package Manager.
Choose Unity Registry.
Under XR Interaction Toolkit, click on install.
Check the warning about the new input system from Unity, if you get one.
Congratulations, your Unity project is now configured for Oculus Quest development!
[XR Setup]
Instructions to set up XR Rig for Unity:
Create a plane add texture 
In the XR Rig script, set the Tracking Origin Mode field as Floor.
Expand the XR Rig and you will see Camera offset, Left and Right Hand controllers.
To set up the XR Rig for the new input system, go to Assets > Samples > XRI Toolkit > 1.0.0 pre 4 > Default Input Actions.
Click on XRI Default Left Controller and click on Add to ActionBasedController Default.
Do the same for the XRI Default Right Controller.
Go to Edit > Project Settings and go to Preset Manager.
Rename Left to LeftHandController and Right to RightHandController.
Delete the XR Rig and add it again.
Make sure to reset its transform.
Check that the hand controllers use the right references such as LeftHand Controller uses Left and RightHand Controller uses right action references.
Create a new gameobject called Input Action Manager.
Add an Input Action Manager Script to it.
In the Action Assets list under it, write 1 to it and drag and drop the XRI Default Input actions to Element 0.
Create two cubes as hands 
Now, you are ready to view Unity scenes in VR.


## Ver escena construida en VR

To set up a Unity project for development APK files for Oculus Quest, follow these steps:
Enable Developer Mode for your Oculus Quest by going to https://dashboard.oculus.com/ and logging in with the Facebook account that you use to log in to your Oculus Quest. Create an Organization if you don’t have one. Then, enable developer mode using the mobile Oculus app, and toggle Developer Mode On.
Download Oculus ADB drivers from the link provided in the lecture and install them on your PC if you're using Windows. Skip this step if you're using Mac or Linux.
Open Unity and click on File > Build Settings. Add the Home Scene that you want to build and test.
Connect your Oculus Quest to your PC with a USB-C cable, and make sure that it is visible in Build Settings > Run Device.
Click on Build and Run, and give a name to your first APK file. Unity will build and install the APK automatically.
To install the APK file without Unity Editor, use SideQuest. Install SideQuest to your PC, and connect your Oculus Quest to it. Click on Games and Apps, and locate the APK file you want to install. After choosing the APK file, you can see the status of the installation.
Congratulations! You are now ready to develop APK files for Oculus Quest in Unity.
