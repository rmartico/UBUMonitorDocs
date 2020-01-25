Instalación y arranque
======================

Para descargar el programa, descargar la última versión disponible en: https://github.com/yjx0003/UBUMonitor/releases/latest.

Se mostrará una entrada similar a la siguiente (*Nota: los números de versión irán cambiando en un futuro según evolucione el producto*):

.. figure:: images/Release_Github.png
  :width: 600
  :alt: Última release en GitHub

  Descarga desde GithHub de UBUMonitor

En la zona de **Assets** se muestran los posibles ficheros a descargar para su ejecución. Solo interesan los tres primeros:

* ``UBUMonitor.v2.5.0-stable-Win32-Portable.zip``: versión portable para sistema operativo Windows 32 bits.
* ``UBUMonitor.v2.5.0-stable-Win64-Portable.zip``: versión portable para sistema operativo Windows 64 bits.
* ``UBUMonitor.v2.5.0-stable.jar``: versión multiplataforma ejecutable con Java instalado en el sistema operativo. Versión para Windows, GNU/Linux o Mac.

Se ofrecen dos versiones: 

* Versión portable (con mínima instalación) para **Windows** descomprimiendo un fichero .zip.
* Versión fichero ejecutable java (con extensión ``.jar``) para **TODAS** las plataformas.

Versión portable para Windows
-----------------------------

Si se trabaja en Windows, y no se quiere instalar Java en el equipo actual, se sugiere descargar la versión portable que corresponda, según el sistema operativo sea de 32 o 64 bits. 

Pasos para su instalación:

* Copiar el fichero descargado con sufijo ``-Portable.zip`` a un directorio a libre elección del usuario, donde tenga permisos de escritura y ejecución.
* Descomprimir el fichero con sufijo ``-Portable.zip`` correspondiente con alguna herramienta tipo WinZip, 7Zip, WinRar, etc.
* En el directorio generado al descomprimir, hacer doble click sobre el fichero ejecutable con extensión ``.exe`` (e.g. ``UBUMonitor.v2.5.0-stable-Win64.exe``)

*Nota: las versiones portables incluyen dentro del fichero ``.zip`` un JDK 8 con JavaFX, por eso ocupan más espacio.*

Versión ejecutable con Java 8
-----------------------------

Si no se trabaja en Windows, o bien no se quiere usar la versión portable, es requisito tener instalada una versión de Java 8. En particular la distribución oficial de Oracle que sí incluye las bibliotecas de JavaFX. Con versiones posteriores **NO** funcionará correctamente, así como tampoco con versiones libres (e.g. OpenJDK, AdoptOpenJDK, Amazon Correto, etc.) que no incluyan las bibliotecas de JavaFX.
 
Suponiendo que se tiene ya instalada dicha versión Java 8 (y que es la versión de Java activa) se siguen los siguientes pasos:

#. Copiar el fichero ``.jar`` a un directorio donde el usuario tenga permisos de escritura y ejecución.
#. Probar a ejecutar haciendo doble click sobre el fichero ``.jar``.  

Si Java está asociado correctamente a la extensión ``.jar`` se ejecutar la aplicación.
Si no, ejecutar desde una consola del sistema operativo, en el directorio donde se tenga el fichero ``.jar`` lo siguiente: 
   
* ``$> java -jar UBUMonitor.v2.5.0.jar``

*Nota: el número de versión puede ir cambiando.*

Si todo va correcto se iniciará la ejecución de la aplicación. En caso contrario, verificar de nuevo los pasos previos.