#Movimiento Continuo 

## Movimiento Continuo en Unity usando el kit de herramientas XR

* Abre el proyecto Unity y navega hasta el objeto del juego XR Rig

* Haz clic en XR Rig y agrega “Locomotion System Script” al objeto del juego. Este script proporcionará acceso a “XR Rig” desde los otros scripts de movimiento que se agregarán más adelante.

* Agrega el “Locomotion System Component “al “XR Origin” - Arrastra y sueltalo en “XR Origin”
<p align="center"><img src="Moviement_Images/2023-03-16%20(27).png" alt="Logo" > </p>
<p align="center"><img src="Moviement_Images/Screenshot%202023-03-16%20200130.png" alt="Logo" > </p>



* Abre la carpeta “Default Input Actions“ dentro de la carpeta “Samples”. Aquí es donde se encuentran los diferentes inputs para los controles XR

* Aquí puedes ver el movimiento vinculado para cada acción; considéralo como un diccionario/ hashmap en código

<p align="center"><img src="Moviement_Images/2023-03-16%20(29).png" alt="Logo" > </p>




* Haz click en los ajustes preestablecidos de “Continuous Move and Turn “ y presiona los botones “Add” para establecer botones predeterminado para ambos. Esto configurará las acciones de entrada para “Continuous Move and Turn “


<p align="center"><img src="Moviement_Images/2023-03-16%20(30).png" alt="Logo" > </p>
<p align="center"><img src="Moviement_Images/2023-03-16%20(31).png" alt="Logo" > </p>


* Agrega el “Continuous Move” a la escena para asegurarte de que está basado en la acción. Este script está conectado con el joystick de nuestros controles manuales.

* Agrega el “Continuous Turn Provider Action-based “para habilitar la rotación. Este script está conectado con el joystick de nuestros controles manuales.

<p align="center"><img src="Moviement_Images/Screenshot%202023-03-16%20200350.png" alt="Logo" > </p>


* Desmarca las acciones de la mano derecha (Right hand )ya que solo queremos movernos con la mano izquierda (Left Hand)

* Cambia la velocidad de movimiento en “Continuous Providers “ si lo desea

* Establece la cámara principal (Main Camera) como “Forward Source”

* Desmarca la referencia “Left Hand Move Actions “ para el giro continuo, ya que solo queremos rotarnos con el joystick de la mano derecha.

* Arrastra y suelta el “Locomotion System “ que acabamos de agregar al movimiento continuo para conectarlos

<p align="center"><img src="Moviement_Images/Screenshot%202023-03-16%20200423.png" alt="Logo" > </p>



* Agrega el “Character Controller Component” al objeto del juego XR Rig. Esto nos permitirá restringir el movimiento por colisiones sin tener que lidiar con un cuerpo rígido

* Cambia el eje Y central del controlador de personajes a 1 y use un radio más pequeño para que podamos acercarnos a los objetos


<p align="center"><img src="Moviement_Images/2023-03-16%20(32).png" alt="Logo" > </p>




* Prueba la implementación dándole al play. El joystick izquierdo debe permitir el movimiento y el joystick derecho debe permitir la rotación. El personaje debe chocar con paredes y obstáculos.

<p align="center"><img src="Moviement_Images/2023-03-16%20(33).png" alt="Logo" > </p>

