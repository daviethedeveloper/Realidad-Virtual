## Teletransportacion


## Implementa la teletransportación en tu proyecto de Unity usando el kit de herramientas XR:


<br>

* Abre Unity y carga el proyecto en el que estás trabajando
* Haz click en el equipo XR en la escena y agrega el “Locomotion System”: arrastra y suelta en XR Origin
* Haz click en XR Rig en la escena y agrega el componente “Teleportation Provide”

<p align="center"><img src="Teleportation_Images/2023-03-19%20(1).png" alt="Logotipo"></p>


<br>
<br>
<br>

* En “Camera Offset”, haz click con el botón derecho y crea un objeto de juego nuevo llamado "Right Hand Parent"
* Arrastra el control de la mano derecha debajo de “Right Hand Parent”
* Asegúrate de restablecer los “transforms” para “Right Hand Parent” y “Right Hand Controller”


<p align="center"><img src="Teleportation_Images/Screenshot%202023-03-19%20195421.png" alt="Logotipo"></p>
<p align="center"><img src="Teleportation_Images/Screenshot%202023-03-19%20195539.png" alt="Logotipo"></p>
<p align="center"><img src="Teleportation_Images/2023-03-19%20(2).png" alt="Logotipo"></p>


<br>
<br>
<br>

* Cambia el nombre del control de la mano derecha a " Right Hand Teleport Controller "
* Crea otro objeto de juego nuevo debajo de “Right Hand Parent” y llámalo "Right Hand Base Controller"

<p align="center"><img src="Teleportation_Images/2023-03-19%20(3).png" alt="Logotipo"></p>
<p align="center"><img src="Teleportation_Images/2023-03-19%20(4).png" alt="Logotipo"></p>



<br>
<br>
<br>

* Agrega el componente “XR Controller Action-Based” al control base de la mano derecha
* Para el controlador base, agrega un “XR Direct Interactor” y un “Sphere Collider”

<p align="center"><img src="Teleportation_Images/2023-03-19%20(5).png" alt="Logotipo"></p>


<br>
<br>
<br>

* Haz click en “Right Hand Teleport Controlley”, y en “XR Ray Interactor” configura el tipo de línea de recta( Straight) a curva de proyectil (Projectile Curve)

<p align="center"><img src="Teleportation_Images/Screenshot%202023-03-19%20212616.png" alt="Logotipo"></p>


<br>
<br>
<br>

* Desmarca el “XR Ray Interactor” para ocultar el “raycaster” cuando no se teletransporte
* Ve a “XR Interactors Line Visual” y cambiar el color válido a verde (Green)

<p align="center"><img src="Teleportation_Images/2023-03-19%20(7).png" alt="Logotipo"></p>
<p align="center"><img src="Teleportation_Images/2023-03-19%20(8).png" alt="Logotipo"></p>



<br>
<br>
<br>


* Desplázate hacia arriba hasta “XR Controller “ y cambia “Select Action” a "RightHand/TeleportSelect""

<p align="center"><img src="Teleportation_Images/2023-03-19%20(23).png" alt="Logotipo"></p>
<p align="center"><img src="Teleportation_Images/2023-03-19%20(24).png" alt="Logotipo"></p>


<br>
<br>
<br>


* Abre “Default Input Actions” y “verifica Right Hand Binding Action”
<p align="center"><img src="Teleportation_Images/2023-03-19%20(10).png" alt="Logotipo"></p>

<br>
<br>
<br>


* Verifica XRI RightHand Locomotion - Teleport Select - Verifica las acciones de enlace (Binding) asociadas con este



<p align="center"><img src="Teleportation_Images/2023-03-19%20(11).png" alt="Logotipo"></p>



<br>
<br>
<br>


* Haz click en “Teleport Mode Activate” para verificar la acción vinculante

<p align="center"><img src="Teleportation_Images/2023-03-19%20(12).png" alt="Logotipo"></p>


<br>
<br>
<br>


* Haz click en “Teleport Mode Cancel” para verificar la acción vinculante

<p align="center"><img src="Teleportation_Images/2023-03-19%20(13).png" alt="Logotipo"></p>


<br>
<br>
<br>


* Adjunta “Action Based Controller Manager” al controlr de mano principal: este script permitirá el cambio entre la acción del control base y el control de acción de teletransporte

<p align="center"><img src="Teleportation_Images/2023-03-19%20(14).png" alt="Logotipo"></p>


<br>
<br>
<br>

* Adjunta las acciones de enlace correctas al” Parent Hand Controlle”

<p align="center"><img src="Teleportation_Images/2023-03-19%20(15).png" alt="Logotipo"></p>

<p align="center"><img src="Teleportation_Images/2023-03-19%20(16).png" alt="Logotipo"></p>


<br>
<br>
<br>


* Este es el resultado de adjuntar las acciones vinculantes correctamente

<p align="center"><img src="Teleportation_Images/Screenshot%202023-03-19%20212616.png" alt="Logotipo"></p>


<br>
<br>
<br>


* Adjunta “Teleportation Area Script” al piso donde aparecerá el jugador

<p align="center"><img src="Teleportation_Images/2023-03-19%20(17).png" alt="Logotipo"></p>


<br>
<br>
<br>

* Arrastra y suelta el “Box Collider” en los “Colliders”

<p align="center"><img src="Teleportation_Images/2023-03-19%20(18).png" alt="Logotipo"></p>



<br>
<br>
<br>



* Crea una nueva “Teleport area mask” y asegúrate de que 'Layer' del piso sea 'Teleport'.

<p align="center"><img src="Teleportation_Images/2023-03-19%20(19).png" alt="Logotipo"></p>


<br>
<br>
<br>


* La “Interaction Layer Mask” en el Área de teletransporte establecida en 'Teleport'

<p align="center"><img src="Teleportation_Images/2023-03-19%20(20).png" alt="Logotipo"></p>
<p align="center"><img src="Teleportation_Images/2023-03-19%20(21).png" alt="Logotipo"></p>


<br>
<br>
<br>



