Preguntas frecuentes
====================

**¿Puedo cambiar o borrar datos accidentalmente en mis cursos al usar UBUMonitor?**

No. Esta aplicación solo lee datos del servidor y **NO modifica ningún dato**, por lo tanto NO hay ningún riesgo en su uso.

**¿Puedo ejecutar UBUMonitor sin conexión a red?**

No. Actualmente como mínimo siempre es necesario validarse inicialmente contra el host o servidor Moodle a través de la red. Una vez validado, si no se quieren actualizar datos, se podría trabajar sin red. 

**¿Puedo tener instaladas varias versiones de UBUMonitor en el mismo equipo?**

Sí. Se pueden tener tantas instalaciones como se quiera, puesto que cada una va en su directorio, sin afectar a las otras versiones. 

**¿Puedo borrar la caché de datos?**

Sí. Simplemente podemos borrar manualmente desde el sistema operativo el directorio caché. Por el momento no existe una opción para realizar esto desde la aplicación.

**¿Cómo puedo desinstalar UBUMonitor?**

Simplemente borrando el directorio donde esté instalada la aplicación. Hay que tener en cuenta que se eliminan TODOS los ficheros locales y los datos descargados, pero no tiene ningún efecto sobre los datos originales del servidor.

**¿Estamos utilizando algún dato al que no deberíamos tener acceso legalmente en Moodle?**

No. UBUMonitor solo lee los datos para los que tiene permiso el usuario actual. Todos los datos utilizados son los mismos de los que se dispone en Moodle. UBUMonitor simplemente extrae, limpia y ordena esos datos para facilitar su filtrado y mejorar su visualización.

**¿Si ejecuto UBUMonitor en un equipo de terceros, debería desinstalar la aplicación al finalizar?**

Solo es necesario si se han utilizado las opciones de **exportación**. Si se exportan gráficos en formato ``.png`` o los datos en formato ``.csv`` debemos ser conscientes de que esos datos **NO están encriptados**. En tal caso, es aconsejable borrar el directorio de UBUMonitor. 

**¿Puedo ejecutar UBUMonitor desde un stick USB?**

Sí siempre y cuando se utilice una versión portable, o bien se tenga instalado Java 8 en el equipo donde se conecta el stick USB.

**Con algunas asignaturas se genera un error al cargar los datos.**

Si no tenemos rol de profesor, no tendremos permisos suficientes para leer los datos y UBUMonitor genera un error. Compruebe que realmente es profesor de dicho curso.

**La aplicación funciona, pero no escalar y redimensiona  correctamente los gráficos ¿por qué?**

Comprobar que se está ejecutando la aplicación con una versión Java 8 que incluya las bibliotecas JavaFX. Para comprobar la versión actual, se puede abrir una consola del sistema operativo y ejecutar $> java -version. Se mostrará el número actual de versión instalada. Con versiones superiores se ha detectado que la visualización de gráficos no es correcta. Recordemos que las versiones libres (e.g. OpenJDK) tampoco funcionarán al no incluir JavaFX.