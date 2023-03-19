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



* En la configuración del reproductor, ingrese el nombre único de su empresa para " Nombre de la empresa "

* Siga las sugerencias de Unity para otras configuraciones

<br>

<p align ="center"><img src="Configuracion-Images/a_3_step.png" alt="Logo" > </p>

<br>
<br>



* Elija "Lineal" para Espacio de color

<br>

<p align ="center"><img src="Configuracion-Images/a_8_step.png" alt="Logo" > </p>

<br>
<br>


* Asegúrese de que OPENGLES3 sea la única API de gráficos en las API de gráficos

* Marque la opción "Nombre del paquete predeterminado" e ingrese su paquete único

<br>

<p align="center"><img src="Configuracion-Images/a_9_step.png" alt="Logo" > </p>

<br>
<br>


* Establezca el nivel mínimo de API en min 23 Android 6.0 Marshmallow

* Establezca el nivel de la API de destino en Automático (el más alto instalado)

* Establecer la ubicación de instalación en automático

<br>

<p align="center"><img src="Configuracion-Images/install_location.png" alt="Logo" > </p>

<br>
<br>

* Marque "Representación de subprocesos múltiples"

* En Gestión de entrada activa, seleccione "Ambos"

<br>

<p align="center"><img src="Configuracion-Images/active_both.png" alt="Logo" > </p>
<p align="center"><img src="Configuracion-Images/active_both_2.png" alt="Logo" > </p>


<br>
<br>



* Vaya a la pestaña "Calidad" en la configuración del proyecto

* Crear un nuevo nivel de calidad para Oculus Quest llamado "Quest"

* Desmarque todas las demás configuraciones

* Habilite la configuración de Quest para la plataforma Android

* Para PC, vaya con Ultra

* Establezca el recuento de píxeles de luz en 1

* Deshabilitar partículas blandas

* Seleccione "Por textura" para texturas anisotrópicas

* Seleccione "4x" para Anti Aliasing

* Asegúrese de que "Realtime Reflection Probes" y "Billboards Face Camera" estén seleccionados

* Siga el enlace proporcionado e importe el kit de herramientas de interacción XR de Unity

<br>

<p align="center"><img src="Configuracion-Images/a_10_step.png" alt="Logo" > </p>


<br>
<br>

* Vaya a Archivo > Configuración del proyecto

* Elija "Administrador de paquetes" y habilite "Vista previa de paquetes"

<br>

<p align ="center"><img src="Configuracion-Images/a_11_step.png" alt="Logo" > </p>

<p align="center"><img src="Configuracion-Images/a_12_step.png" alt="Logo" > </p>

<br>
<br>


* Haga clic en Ventana > Administrador de paquetes

* Elija " Registro de la unidad "

* En "XR Interaction Toolkit", haga clic en " Instalar "

* Verifique la advertencia sobre el nuevo sistema de entrada de Unity, si obtiene uno

<br>

<p align="center"><img src="Configuracion-Images/a_13_step.png" alt="Logo" > </p>
<p align="center"><img src="Configuracion-Images/a_14_step.png" alt="Logo" > </p>
<p align="center"><img src="Configuracion-Images/a_15_step.png" alt="Logo" > </p>

< br >
< br >

Felicitaciones, tu proyecto de Unity ahora está configurado para el desarrollo de Oculus Quest.


<br>
<br>
<br>

## Instrucciones para configurar XR Rig para Unity:

<br>

* Agregar origen xr a la jerarquía 

<br>

<p align="center"><img src="Configuracion-Images/add_xr_origin.png" alt="Logo" > </p>

<br>
<br>



* Crea un plano y agrega textura

<br>

<p align="center"><img src="Configuracion-Images/create_plane.png" alt="Logo" > </p>

<br>
<br>



* En el script de XR Rig, configure el campo "Modo de origen de seguimiento" como " Piso "

<br>

<p align ="center"><img src="Configuracion-Images/track_floor.png" alt="Logo" > </p>

<br>
<br>



* Expanda el XR Rig y verá el desplazamiento de la cámara, los controladores de mano izquierda y derecha

<br>

<p align="center"><img src="Configuracion-Images/heir_xr_origin.png" alt="Logo" > </p>

<br>
<br>



* Para configurar XR Rig para el nuevo sistema de entrada, vaya a Activos > Muestras > XRI Toolkit > XXX > Acciones de entrada predeterminadas

<br>

<p align="center"><img src="Configuracion-Images/find_XRI_strass.png" alt="Logo" > </p>

<br>
<br>



* Haga clic en "XRI Default Left Controller" y haga clic en "Add to ActionBasedController Default"

* Haga lo mismo para el "Controlador derecho predeterminado de XRI"

<br>

<p align="center"><img src="Configuracion-Images/add_left_controller.png" alt="Logo" > </p>
<p align="center"><img src="Configuracion-Images/add_right_controller.png" alt="Logo" > </p>


<br>
<br>


* Vaya a Editar > Configuración del proyecto y vaya a Administrador de ajustes preestablecidos

* Cambiar el nombre de "Left" a " LeftHandController " y "Right" a " RightHandController "

<br>

<p align="center"><img src="Configuracion-Images/preset_manager_LR.png" alt="Logo" > </p>

<br>
<br>


* Elimine el XR Rig y agréguelo nuevamente

* Asegúrese de restablecer su transformación

* Verifique que los controladores manuales usen las referencias correctas, como LeftHandController usando "Left" y RightHandController usando referencias de acción "Right".

<br>

<p align="center"><img src="Configuracion-Images/left_map_yes.png" alt="Logo" > </p>
<p align="center"><img src="Configuracion-Images/right_map_yes.png" alt="Logo" > </p>

<br>
<br>


* Crea dos cubos como manos

<br>

<p align="center"><img src="Configuracion-Images/final_picture.png" alt="Logo" > </p>

<br>
<br>

* Ahora, estás listo para ver Unity

<br>
<br>
<br>


## Ver escena construida en VR


Para ver la nueva escena de realidad virtual en su visor Oculus mediante Oculus Link o SideQuest , puede seguir estos pasos:

<br>
<br>
<br>

### Uso de Oculus Link:

* Asegúrate de que tu Oculus Quest esté conectado a tu PC con un cable USB-C y de que hayas habilitado el modo Oculus Link en tus auriculares.

* Abra la aplicación Oculus para PC en su computadora y haga clic en la pestaña Dispositivos.

* Asegúrate de que tu Oculus Quest esté conectado y que aparezca en la pestaña Dispositivos.

* Inicie la escena de realidad virtual que creó en Unity y haga clic en Archivo > Configuración de compilación.

* Seleccione la plataforma como PC, luego haga clic en Build and Run.

* Una vez creada la escena, debería aparecer la ventana de Oculus Link en su PC. Ponte el visor Oculus Quest y selecciona la opción Oculus Link en el menú Quest.

* Su escena de realidad virtual ahora debería estar visible en su Oculus Quest y puede navegar a través de ella usando los controladores.

<br>
<br>
<br>

### Uso de SideQuest :

* Conecta tu Oculus Quest a tu PC con un cable USB-C.

* Abra SideQuest en su computadora y asegúrese de que la aplicación reconozca su Oculus Quest.

* Haga clic en el botón Instalar APK en SideQuest y seleccione el archivo APK que desea instalar.

* Espere a que se complete la instalación y luego desconecte su Oculus Quest de su PC.

* Colóquese el visor Oculus Quest y vaya a la sección Fuentes desconocidas de la biblioteca.

* Seleccione la aplicación que acaba de instalar y debería iniciar la escena de realidad virtual que creó en Unity.

* ¡Felicidades! Ahora ha visto con éxito su nueva escena de realidad virtual en su visor Oculus usando Oculus Link o SideQuest .

