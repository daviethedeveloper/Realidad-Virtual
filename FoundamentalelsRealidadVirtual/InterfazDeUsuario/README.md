## Interfaz De Usuario

## Unity usando el “XR Toolkit” provisto:

<br>
<br>

* Configura el plano para que el jugador lo pise - Recuerda restablecer esto a (0, 0, 0)

* Comienza por hacer un lienzo. Para hacer esto, haz clic derecho en la jerarquía y vaya a UI, luego seleccione “Canvas”

<br>

<p align="center"><img src="UI-Images/Screenshot%202023-03-16%20173412.png" alt="Logo" > </p>


<br>
<br>

* Vuelve a colocar el “XR Right” y colócalo en la posición ideal que desees

<br>

<p align="center"><img src="UI-Images/2023-03-16%20(17).png" alt="Logo" > </p>


<br>
<br>
* Canvas viene con un sistema de eventos, que debes colocar en la parte superior de la jerarquía

<br>

<p align="center"><img src="UI-Images/2023-03-16%20(18).png" alt="Logo" > </p>



<br>
<br>

* El lienzo tiene componentes adjuntos, siendo “Screen Space Overlay” el modo de representación en el que te encuentras en este momento. Haz doble clic en el lienzo para ver un lienzo gigante y en la esquina puedes ver el mundo real

<br>

<p align="center"><img src="UI-Images/Screenshot%202023-03-16%20173623.png" alt="Logo" > </p>

<br>
<br>

* Si lo ejecutas ahora, no podrás ver el lienzo en VR. Hay otras dos opciones: Screen Space Camera y World Space
* Al usar la opción Screen Space Camera, verás el lienzo pero estará pegado a la cámara y seguirá a donde mire el jugador.

<br>


* Para usar la opción World Space, necesitarás una cámara de eventos. Arrastra la cámara de eventos y reducirla a un tamaño adecuado. Ajusta la escala, siendo “x“ e “y” los mismos valores para evitar estirar el texto y los botones

<br>

<p align="center"><img src="UI-Images/Screenshot%202023-03-16%20173713.png" alt="Logo" > </p>

<br>
<br>

* Ajusta la altura y el ancho del lienzo en el “rect transform”
* Para interactuar con la interfaz de usuario, dentro del lienzo, asegúrate de que “Tracked Device Raycaster”, el sistema de eventos que vino con el lienzo (Canvas), esté configurado para usar el módulo “XRI UI Input”, que permitirá que el “raycast” de los controles manuales interactúe con el lienzo

<br>
<p align="center"><img src="UI-Images/Screenshot%202023-03-16%20190945.png" alt="Logo" > </p>
<p align="center"><img src="UI-Images/Screenshot%202023-03-16%20191100.png" alt="Logo" > </p>

<br>
<br>


* Como componente secundario, crea una imagen de fondo para este lienzo: ajusta la escala manteniendo presionadas las teclas CTRL + ALT en el teclado y haz clic en la opción inferior izquierda.

<br>
<p align="center"><img src="UI-Images/Screenshot%202023-03-16%20175142.png" alt="Logo" > </p>
<p align="center"><img src="UI-Images/2023-03-16%20(19).png" alt="Logo" > </p>
<p align="center"><img src="UI-Images/2023-03-16%20(20).png" alt="Logo" > </p>

<br>
<br>

* Ahora, como “child”, añade un cuadro de texto y escálalo a un tamaño apropiado. Es posible que el texto esté orientado de manera incorrecta, así que escala la fuente con el tamaño de fuente para el tamaño del texto

* Agrega también un “Button” y un “Slider” como un nodo secundario del lienzo. El botón tendrá un evento de one-click para cualquier acción y el control deslizante tendrá un evento on-change. 

<br>
<p align="center"><img src="UI-Images/2023-03-16%20(21).png" alt="Logo" > </p>
<p align="center"><img src="UI-Images/2023-03-16%20(22).png" alt="Logo" > </p>



<br>
<br>

* El “Raycast Mask“ en el “XR Ray Interactor “para ambas manos debe configurarseen “only UI”. El “Gradient to Zero alpha”, el “raycast” solo se mostrará si está en el lienzo en la interfaz de usuario

<br>
<p align="center"><img src="UI-Images/2023-03-16%20(24).png" alt="Logo" > </p>
<p align="center"><img src="UI-Images/2023-03-16%20(25).png" alt="Logo" > </p>

<br>
<br>

* Asegúrate de que el sistema de eventos tenga un “XR UI Input Module”

<br>
<p align="center"><img src="UI-Images/Screenshot%202023-03-16%20191100.png" alt="Logo" > </p>


<br>
<br>

* Felicidades, ahora puedes ver tus resultados

<br>
<p align="center"><img src="UI-Images/2023-03-16%20(26).png" alt="Logo" > </p>

