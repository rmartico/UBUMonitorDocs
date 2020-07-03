Preguntas frecuentes
====================

**¿Puedo cambiar o borrar datos accidentalmente en mis cursos al usar UBUMonitor?**

No. Esta aplicación solo lee datos del servidor y **NO modifica ningún dato**, por lo tanto NO hay ningún riesgo en su uso.

**¿Puedo ejecutar UBUMonitor sin conexión a red?**

Sí. Desde la versión *2.6.1-stable* se permite trabajar en modo offline con las asignaturas previamente cargadas.

**¿Puedo tener instaladas varias versiones de UBUMonitor en el mismo equipo?**

Sí. Se pueden tener tantas instalaciones como se quiera, puesto que cada una va en su directorio, sin afectar a las otras versiones. 

**¿Puedo borrar la caché de datos?**

Sí. Simplemente podemos borrar manualmente desde el sistema operativo el directorio caché o bien utilizando el botón **Limpiar** disponible en la ventana de selección de curso/asignatura. 

**¿Cómo puedo desinstalar UBUMonitor?**

Simplemente borrando el directorio donde esté instalada la aplicación. Hay que tener en cuenta que se eliminan TODOS los ficheros locales y los datos descargados, pero no tiene ningún efecto sobre los datos originales del servidor.

**¿Estamos utilizando algún dato al que no deberíamos tener acceso legalmente en Moodle?**

No. UBUMonitor solo lee los datos para los que tiene permiso el usuario actual. Todos los datos utilizados son los mismos de los que se dispone en Moodle. UBUMonitor simplemente extrae, limpia y ordena esos datos para facilitar su filtrado y mejorar su visualización.

**¿Si ejecuto UBUMonitor en un equipo de terceros, debería desinstalar la aplicación al finalizar?**

Solo es necesario si se han utilizado las opciones de **exportación**. Si se exportan gráficos en formato ``.png`` o los datos en formato ``.csv`` debemos ser conscientes de que esos datos **NO están encriptados**. En tal caso, es aconsejable borrar aquellos ficheros que se hayan exportado.

**¿Puedo ejecutar UBUMonitor desde un stick USB?**

Sí siempre y cuando se utilice una versión portable, o bien se tenga instalado Java 8 con JavaFX en el equipo donde se conecta el stick USB.

**La aplicación funciona, pero no escala y redimensiona  correctamente los gráficos ¿por qué?**

Se debe comprobar que se está ejecutando la aplicación con una **versión Java 8 que incluya las bibliotecas JavaFX**. Para comprobar la versión actual, se puede abrir unaE consola del sistema operativo y ejecutar $> java -version. Se mostrará el número actual de versión instalada. Con versiones superiores (e.g. Java 11 o superior) se ha detectado que la visualización de gráficos no es correcta. Recordemos que las versiones libres (e.g. OpenJDK) tampoco funcionarán al no incluir JavaFX.