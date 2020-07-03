.. _errormessages:

Mensajes de error
=================

La aplicación mostrará los distintos mensajes de error, con dos formatos básicos de visualización: mensaje incrustado en ventana o diálogo modal de error. 

Mensaje en ventana
------------------

Se muestran en rojo en la parte inferior de la ventana activa. Se producen por una incorrecta introducción de datos. En la figura se muestra el error al iniciar sesión con un usuario y/o contraseña incorrectos. 

.. figure:: images/error_validacion.png
  :width: 300
  :alt: Error de usuario y/o contraseña
  :align: center
  
  Error en la validación de usuario
 
Otro ejemplo, en la siguiente figura, nos muestra el mensaje correspondiente si no hay conexión a red, informando de que no es posible la conexión al host indicado.
  
.. figure:: images/error_sin_red.png
  :width: 200
  :alt: Error de conexión a red
  :align: center
  
  Error por falta de conexión a red en validación
  
Diálogo de error
----------------

Se abre un diálogo modal con un texto descriptivo del error y la opción a desplegar de **Mostrar detalles**. En la siguiente figura vemos un ejemplo de error al perder la conexión de red a la hora de cargar una asignatura.

.. figure:: images/error_sin_red_cargando_asignatura.png
  :width: 300
  :alt: Error en conexión a red
  :align: center
  
  Error en conexión en red al cargar asignatura
  
Si seleccionamos la opción **Mostrar detalles**, se abre un cuadro de texto en la parte inferior del diálogo, con la traza del error. 

.. figure:: images/error_sin_red_cargando_asignatura_desplegada.png
  :width: 300
  :alt: Detalles del error en conexión al cargar asignatura
  :align: center
  
  Detalles del error en conexión en red al cargar asignatura
  
La información mostrada en el cuadro de texto es técnica, y aunque no es de interés para el usuario, es **MUY IMPORTANTE** remitir ese texto a los desarrolladores para la corrección de errores o bugs de la aplicación (se puede seleccionar y copiar el texto directamente).


Errores habituales
------------------

Esta nueva versión reduce los mensajes de error habituales en otras versiones, comprobando con antelación los permisos disponibles de usuario. Por lo tanto ya no se mostrarán errores por falta de permisos en el acceso a datos.

Por otro lado, cuando exista **incompatiblidad de las versiones de los cachés de datos**, ya no se muestra un mensaje de error, ni se fuerza al usuario limpiar manualmente la caché. En este caso, se accede a una **nueva caché compatible**. Sin embargo hay que tener en cuenta que **la caché estará inicialmente vacía** forzando al usuario a **recargar nuevamente los datos**.
