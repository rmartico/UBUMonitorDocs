Anexos. Estructura de ficheros
==============================

A continuación se detalla la estructura de ficheros típica de UBUMonitor.

Contenido inicial 
-----------------

Si se instala la versión portable, al descomprimir se crea un directorio:

* ``UBUMonitor.v2.6.3-stable-Win64-Portable`` en Windows 64 bits.
* ``UBUMonitor.v2.6.3-stable-Win32-Portable`` en Windows 32 bits.
* ``UBUMonitor.v2.6.3-stable-Linux64-Portable`` en GNU/Linux 64 bits.

En el directorio creado, tendremos el siguiente contenido en Windows (el contenido con 32 bits es equivalente):

.. figure:: images/contenido_instalacion_portable_64bits.png
  :width: 350
  :alt: Contenido en Windows.
  :align: center
  
  Contenido en una instalación portable en Windows (para 64 bits)
  
Mientras que en GNU/Linux tendremos el siguiente contenido:

.. figure:: images/contenido_instalacion_portable_linux64bits.png
  :width: 350
  :alt: Contenido en GNU/Linux.
  :align: center
  
  Contenido en una instalación portable en GNU/Linux (para 64 bits)
  
Si se instala la versión Java ejecutable con ``.jar`` tendremos el siguiente contenido:

.. figure:: images/ejecutable_jar.png
  :width: 300
  :alt: Ejecutable jar.
  :align: center
  
  Contenido en la instalación con ejecutable Java .jar
  
Estructura de ficheros y directorios
------------------------------------

Una vez iniciada la aplicación, descargados algunos cursos y cambiando la configuración por defecto, nos encontraremos con los siguientes directorios y ficheros adicionales (e.g. en Windows).

.. figure:: images/estructura_ficheros.png
  :width: 300
  :alt: Login
  :align: center
  
  Estructura de ficheros
  
El fichero ``config.properties`` almacena las opciones de inicio personalizadas por el usuario (e.g. *Recordar usuario*, *Recordar host*, etc.)
  
Por otro lado se crean los siguietes directorios:

* *cache*: contiene la caché local de los ficheros con los datos de los cursos descargados. 
* *configuration*: almacena la configuración de la aplicación para el host, usuario y asignatura particular.
* *log*: directorio donde se generan los ficheros registo o log de ejecución de la aplicación. Estos ficheros contienen los registros de ejecución y errores que se producen internamente en la aplicación. Son útiles para renviarlos a los desarrolladores para corregir los posibles errores o *bugs* que se produzcan en la aplicación.

El directorio ``cache`` se organiza en un primer nivel por *host* y en un segundo nivel por usuario. En ese directorio se guarda un fichero por cada asignatura descargada (e.g. *Psychology in Cinema (Art and Media)-62*). El directorio ``configuration`` se organiza de igual forma.
  
Esta estructura de directorios permite acceder a distintos servidores Moodle desde UBUMonitor, evitando colisiones en el caso de coincidencia de nombres de usuario o de curso.

**MUY IMPORTANTE**: las versiones portables incluyen un directorio con su propia distribución JRE (e.g. ``zulu8.42.0.23-ca-fx-jre8.0.232-win_x64``, ``zulu8.44.0.13-ca-fx-jre8.0.242-linux_x64``, etc.). Dicho directorio **no debe modificarse**.