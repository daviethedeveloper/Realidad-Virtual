# InterfazDeUsuario

## Unity using the XR Toolkit provided:

* Start by making a canvas. To do this, right-click on the hierarchy and go to UI, then select Canvas

* Reposition the XR Right and face it towards the ideal position wanted

* The Canvas comes with an event system, which you need to put at the top of the hierarchy


* The Canvas has components attached, with Screen Space Overlay being the render mode it is on at the moment. Double-click on the Canvas to see a giant canvas and on the corner, you can see the actual world


* If you run it now, you won't be able to see the canvas in VR. There are two other options: Screen Space Camera and World Space

* To use the Screen Space Camera option, you will see the canvas but it will be stuck to the camera and will follow wherever the player looks

* To use the World Space option, you will require an event camera. Drag in the event camera and scale it down to an appropriate size. Adjust the scale, with x and y being the same values to avoid stretching the text and buttons

* Adjust the height and width of the canvas on the rect transform

* Now, as a child, add a text box and scale it to an appropriate size. The text might be facing the wrong way, so scale the font with the font size for the text size

* Also add a button and a slider as a child node of the canvas. The button will have an on-click event for any action, and the slider will have an on-change event

* To interact with these things, inside the canvas make sure that the Tracked Device Raycaster - in the event system that came with the canvas - is set to use the XRI UI Input module, which will allow the raycast from the hand nodes controllers to interact with the canvas

* The Raycast Mask on the XR Ray Interactor for both hands needs to be set to only UI. The invalid Gradient to Zero alpha, the raycast will only show if it is on the canvas in the UI

