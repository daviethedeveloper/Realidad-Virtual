# Configuración


## Importación de XR a Unity

Guía de instrucciones: Configuración de Unity para el desarrollo de Oculus Quest

<br>


* Abre Unity y haz click en File > Build Settings

<br>

<p align="center"><img src="Configuracion-Images/a_1_step.png" alt="Logo" > </p>

<br>
<br>



* Cambia la plataforma a Android

* Sigue el enlace dado y usa la configuración de compilación sugerida por Oculus para Unity

* Cambia la compresión de textura a ASTC

* Abre la configuración del jugador (Player Settings), parte inferior izquierda

<br>

<p align="center"><img src="Configuracion-Images/a_2_step.png" alt="Logo" > </p>

<br>
<br>



* Haz click en el botón "XR Plugin Management" que está último en la lista de la izquierda

<p align="center"><img src="Configuracion-Images/a_3_step.png" alt="Logo" > </p>

<br>
<br>



* Haz click en "Install XR Plugin Management" para el nuevo sistema de complementos XR de Unity

<br>

<p align="center"><img src="Configuracion-Images/a_4_step.png" alt="Logo" > </p>

<br>
<br>


* Ve a la pestaña de Android (Ícono)

* Marca la casilla "Oculus" en "Plugin-in Providers"

* Haz click en el interruptor de Oculus y mantén todas las configuraciones predeterminadas

<br>

<p align ="center"><img src="Configuracion-Images/a_5_step.png" alt="Logo" > </p>

<br>

<p align ="center"><img src="Configuracion-Images/a_6_step.png" alt="Logo" > </p>

<br>
<br>



* Puede ver que este complemento se puede crear tanto para quest como para quest 2

<br>

<p align ="center"><img src="Configuracion-Images/a_7_step.png" alt="Logo" > </p>

<br>
<br>



* En la configuración "Player", ingresa un nombre único para tu "Company"

* Sigue las sugerencias de Unity para las otras configuraciones

<br>

<p align ="center"><img src="Configuracion-Images/a_3_step.png" alt="Logo" > </p>

<br>
<br>



* Elije "Linear" para "Color Space"

<br>

<p align ="center"><img src="Configuracion-Images/a_8_step.png" alt="Logo" > </p>

<br>
<br>


* Asegúrate de que OPENGLES3 sea la única API de gráficos en las API graficas

* Marca la opción "Default package name" e ingresa el paquete único

<br>

<p align="center"><img src="Configuracion-Images/a_9_step.png" alt="Logo" > </p>

<br>
<br>


* Establece el nivel mínimo de API en 23 "Android 6.0 Marshmallow"

* Establece el nivel de la API de destino en Automático (el más alto instalado)

* Establece la ubicación de instalación en automático

<br>

<p align="center"><img src="Configuracion-Images/install_location.png" alt="Logo" > </p>

<br>
<br>

* Marca "Multi-threaded rendering"

* En Gestión de entrada activa, seleccione "Both"

<br>

<p align="center"><img src="Configuracion-Images/active_both.png" alt="Logo" > </p>
<p align="center"><img src="Configuracion-Images/active_both_2.png" alt="Logo" > </p>


<br>
<br>



* Ve a la pestaña "Quality" en la configuración del proyecto

* Crea un nuevo nivel de calidad para Oculus Quest llamado "Quest"

* Desmarca todas las demás configuraciones

* Habilita la configuración de Quest para la plataforma Android

* Para PC escoje Ultra

* Establece el "Pixel Light Count en 1

* Desmarca "Soft Particles"

* Seleccione "Per Texture" para texturas anisotrópicas

* Seleccione "4x" para Anti Aliasing

* Asegúrate de que "Realtime Reflection Probes" y "Billboards Face Camera" estén seleccionados

* Sigue el enlace proporcionado e importa el kit de herramientas de interacción XR de Unity

<br>

<p align="center"><img src="Configuracion-Images/a_10_step.png" alt="Logo" > </p>


<br>
<br>

* Ve a File > Project Settings

* Elije "Package Manager" macra "Enable Preview Packages"

<br>

<p align ="center"><img src="Configuracion-Images/a_11_step.png" alt="Logo" > </p>

<p align="center"><img src="Configuracion-Images/a_12_step.png" alt="Logo" > </p>

<br>
<br>


* Haz click en la ventana "Package Manager"

* Elije "Unity Recorder"

* En "XR Interaction Toolkit", haz click en " Install "

* Verifica la advertencia sobre el nuevo sistema de entrada de Unity.

<br>

<p align="center"><img src="Configuracion-Images/a_13_step.png" alt="Logo" > </p>
<p align="center"><img src="Configuracion-Images/a_14_step.png" alt="Logo" > </p>
<p align="center"><img src="Configuracion-Images/a_15_step.png" alt="Logo" > </p>

< br >
< br >

Felicidades, tu proyecto de Unity ahora está configurado para el desarrollo de Oculus Quest.


<br>
<br>
<br>

## Instrucciones para configurar XR Rig para Unity:

<br>

* Agrega origen xr a "Hierarchy"

<br>

<p align="center"><img src="Configuracion-Images/add_xr_origin.png" alt="Logo" > </p>

<br>
<br>



* Crea un plano y agrega textura

<br>

<p align="center"><img src="Configuracion-Images/create_plane.png" alt="Logo" > </p>

<br>
<br>



* En el script de XR Rig, configura el campo "Tracking Origin Mode" como "Floor"

<br>

<p align ="center"><img src="Configuracion-Images/track_floor.png" alt="Logo" > </p>

<br>
<br>



* Expande el XR Rig y verás el desplazamiento de la cámara, los controladores de la mano izquierda y derecha

<br>

<p align="center"><img src="Configuracion-Images/heir_xr_origin.png" alt="Logo" > </p>

<br>
<br>



* Para configurar XR Rig para el nuevo input, ve a Assets > Samples > XRI Toolkit > XXX > Started Assets

<br>

<p align="center"><img src="Configuracion-Images/find_XRI_strass.png" alt="Logo" > </p>

<br>
<br>



* Haz click en "XRI Default Left Controller" y click en "Add to ActionBasedController Default"

* Haz lo mismo para el "XRI Default Right Controller"

<br>

<p align="center"><img src="Configuracion-Images/add_left_controller.png" alt="Logo" > </p>
<p align="center"><img src="Configuracion-Images/add_right_controller.png" alt="Logo" > </p>


<br>
<br>


* Ve a Edit > Project Settings y luego "Preset Manager"

* Cambia el nombre de "Left" a "LeftHandController" y "Right" a "RightHandController"

<br>

<p align="center"><img src="Configuracion-Images/preset_manager_LR.png" alt="Logo" > </p>

<br>
<br>


* Elimina el XR Rig y agrégalo nuevamente

* Asegúrate de restablecer la transformación

* Verifica que los controles manuales usen las referencias correctas, como LeftHandController usando "Left" y RightHandController usando referencias de acción "Right".

<br>

<p align="center"><img src="Configuracion-Images/left_map_yes.png" alt="Logo" > </p>
<p align="center"><img src="Configuracion-Images/right_map_yes.png" alt="Logo" > </p>

<br>
<br>


* Crea dos cubos como si fueran manos

<br>

<p align="center"><img src="Configuracion-Images/final_picture.png" alt="Logo" > </p>

<br>
<br>

* Ahora, estás listo para ver Unity

<br>
<br>
<br>


## Ver la escena construida en VR


Para ver la nueva escena de realidad virtual en su visor Oculus mediante Oculus Link o SideQuest sigue estos pasos:

<br>
<br>
<br>

### Uso de Oculus Link:

* Asegúrate de que tu Oculus Quest esté conectado a tu PC con un cable USB-C y de que hayas habilitado el modo Oculus Link en tus auriculares.

* Abre la aplicación Oculus para PC en su computadora y haga clic en la pestaña Dispositivos (Devices).

* Asegúrate de que tu Oculus Quest esté conectado y que aparezca en la pestaña Dispositivos.

* Inicia la escena de realidad virtual que creaste en Unity y haz click en File > Build configuration.

* Selecciona la plataforma como PC, luego haz click en Build and Run.

* Una vez creada la escena, debería aparecer la ventana de Oculus Link en tu PC. Ponte el visor Oculus Quest y selecciona la opción Oculus Link en el menú Quest.

* Tu escena de realidad virtual ahora debería estar visible en tu Oculus Quest y puedes navegar a través de ella usando los controladores.

<br>
<br>
<br>

### Uso de SideQuest :

* Conecta tu Oculus Quest a tu PC con un cable USB-C.

* Abre SideQuest en tu computadora y asegúrate de que la aplicación reconozca tu Oculus Quest.

* Haz click en el botón Install APK en SideQuest y selecciona el archivo APK que deseas instalar.

* Espera a que se complete la instalación y luego desconecta tu Oculus Quest de su PC.

* Colócate el visor Oculus Quest y ve a la sección unknown library sources.

* Selecciona la aplicación que acabas de instalar y se debería iniciar la escena de realidad virtual que creaste en Unity.

* ¡Felicidades! Ahora has visto con éxito tu nueva escena de realidad virtual en tu visor Oculus usando Oculus Link o SideQuest .

