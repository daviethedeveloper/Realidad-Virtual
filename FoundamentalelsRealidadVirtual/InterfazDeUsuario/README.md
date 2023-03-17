# InterfazDeUsuario

## Unity using the XR Toolkit provided:

<br>
<br>

* Set up the Plane for the player to step on - Remember to to reset this to (0, 0, 0)

* Start by making a canvas. To do this, right-click on the hierarchy and go to UI, then select Canvas

<br>
<p align="center"><img src="UI-Images/Screenshot%202023-03-16%20173412.png" alt="Logo" > </p>


<br>
<br>

* Reposition the XR Right and face it towards the ideal position wanted

<br>
<p align="center"><img src="UI-Images/2023-03-16%20(17).png" alt="Logo" > </p>


<br>
<br>

* The Canvas comes with an event system, which you need to put at the top of the hierarchy

<br>
<p align="center"><img src="UI-Images/2023-03-16%20(18).png" alt="Logo" > </p>



<br>
<br>

* The Canvas has components attached, with Screen Space Overlay being the render mode it is on at the moment. Double-click on the Canvas to see a giant canvas and on the corner, you can see the actual world

<br>
<p align="center"><img src="UI-Images/Screenshot%202023-03-16%20173623.png" alt="Logo" > </p>


<br>
<br>

* If you run it now, you won't be able to see the canvas in VR. There are two other options: Screen Space Camera and World Space
* To use the Screen Space Camera option, you will see the canvas but it will be stuck to the camera and will follow wherever the player looks

<br>

* To use the World Space option, you will require an event camera. Drag in the event camera and scale it down to an appropriate size. Adjust the scale, with x and y being the same values to avoid stretching the text and buttons

<br>
<p align="center"><img src="UI-Images/Screenshot%202023-03-16%20173713.png" alt="Logo" > </p>

<br>
<br>

* Adjust the height and width of the canvas on the rect transform
* To interact with UI, inside the canvas make sure that the Tracked Device Raycaster - in the event system that came with the canvas - is set to use the XRI UI Input module, which will allow the raycast from the hand nodes controllers to interact with the canvas

<br>
<p align="center"><img src="UI-Images/Screenshot%202023-03-16%20190945.png" alt="Logo" > </p>
<p align="center"><img src="UI-Images/Screenshot%202023-03-16%20191100.png" alt="Logo" > </p>

<br>
<br>


* As a child component, create a background image to this canvas - adjust the scale by holding CTRL + ALT on the keyboard and the bottom left option click on it 

<br>
<p align="center"><img src="UI-Images/Screenshot%202023-03-16%20175142.png" alt="Logo" > </p>
<p align="center"><img src="UI-Images/2023-03-16%20(19).png" alt="Logo" > </p>
<p align="center"><img src="UI-Images/2023-03-16%20(20).png" alt="Logo" > </p>

<br>
<br>

* Now, as a child, add a text box and scale it to an appropriate size. The text might be facing the wrong way, so scale the font with the font size for the text size

* Also add a button and a slider as a child node of the canvas. The button will have an on-click event for any action, and the slider will have an on-change event

<br>
<p align="center"><img src="UI-Images/2023-03-16%20(21).png" alt="Logo" > </p>
<p align="center"><img src="UI-Images/2023-03-16%20(22).png" alt="Logo" > </p>



<br>
<br>

* The Raycast Mask on the XR Ray Interactor for both hands needs to be set to only UI. The invalid Gradient to Zero alpha, the raycast will only show if it is on the canvas in the UI

<br>
<p align="center"><img src="UI-Images/2023-03-16%20(24).png" alt="Logo" > </p>
<p align="center"><img src="UI-Images/2023-03-16%20(25).png" alt="Logo" > </p>

<br>
<br>

* Make sure that the event system has a XR UI Input Module 

<br>
<p align="center"><img src="UI-Images/Screenshot%202023-03-16%20191100.png" alt="Logo" > </p>


<br>
<br>

* Congrats, now you can see your results

<br>
<p align="center"><img src="UI-Images/2023-03-16%20(26).png" alt="Logo" > </p>
