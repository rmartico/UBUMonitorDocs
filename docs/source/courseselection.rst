Selección de curso/asignatura
=============================

En esta pantalla muestra un listado de cursos (o asignaturas) en los que está registrado el usuario actual. Se  permite seleccionar uno de ellos, para realizar la carga de datos y acceder a la siguiente pantalla. 

Cuando se elige uno de los cursos, se muestra la información de fecha de la **Última actualización local**. Esta fecha indica la última actualización de datos, realizada en dicho curso (se muestra en función del fichero local de caché).  

Si queremos forzar la actualización de datos, con el contenido actual del servidor, debemos marcar la opción de **Actualizar datos**. En caso contario se mostrarán los datos de la caché local que pudieran estar desactualizados.

Si el curso nunca ha sido cargado previamente se mostrará siempre el texto **No disponible** y se marca por defecto la opción de **Actualizar datos**.

.. figure:: images/Seleccion_de_curso.png
  :width: 400
  :alt: Login
  :align: center
  
  Selección de curso (asignatura) en primer acceso
  
Cuando se haya seleccionado un curso y pulsamos en el botón **Entrar**, si la casilla de **Actualizar datos** está seleccionada, cargará el fichero en local (si existía) o lo crea en el primer acceso y actualiza los datos (usuarios matriculados, calificaciones, registros, etc...) conectándose por red con el servidor Moodle.

Este proceso de descarga de datos del calificador y registro (o *logs*) puede **tardar varios minutos en la primera actualización** (en función del número de alumnos, tamaño del calificador y número de registros nuevos), mostrando en la parte inferior una barra de progreso indicando las etapas realizadas (carga del calificador, descarga del log y actualización del mismo). Posteriores actualizaciones serán más breves, puesto que la carga de registros es incremental, aunque el calificador siempre se actualiza por completo.

Es **MUY IMPORTANTE** que en el calificador esté visible la información de porcentaje (por defecto está visible en Moodle) para una correcta lectura y visualización posterior de las calificaciones.

Si no está marcada la opción **Actualizar datos** (previamente ya se cargó la asignatura) abre directamente el fichero de la caché local y lo carga de forma casi instantánea. Se recuerda que el fichero local se **encripta** usando la contraseña de Moodle como clave, por motivos de seguridad. 

En siguientes accesos a cursos previamente cargados, se mostrará ya la fecha de última actualización y se dará la opción de marcar o no la opción **Actualizar datos**.

.. figure:: images/Seleccion_de_curso_recargar_asignatura.png
  :width: 400
  :alt: Selección de curso recargando asignatura
  :align: center

  Acceso posterior a asignatura cargada previamente
  
Si la carga de datos ha sido correcta, se pasará a mostrar la ventana principal de la aplicación. En caso contrario, compruebe que tiene **rol de profesor** en el curso a cargar. Si el error se produce con la opción **Actualizar datos** desmarcada, compruebe que en el subdirectorio ``cache`` de su instalación de UBUMonitor no ha sufrido cambios externos o malintencionados.
  
Contraseña modificada
---------------------

En el caso de que se haya modificado la contraseña de Moodle recientemente, se muestra una ventana emergente, indicando que se ha detectado un cambio y pide la anterior contraseña, que se tuviera en la fecha señalada.

.. figure:: images/password_antiguo.png
  :width: 400
  :alt: Cambio de constraseña
  :align: center
  
  Cambio de contraseña
  
Cuando se haya introducido correctamente la contraseña antigua, el fichero en caché local se guarda con la nueva. Esto es **obligatorio**, debido a que la información **siempre se guarda encriptada**.

**MUY IMPORTANTE**: es necesario recordar la contraseña previa, para poder recuperar los datos. En caso contrario se debe borrar manualmente la caché, para forzar a cargar los cursos nuevamente. En próximas versiones se incluiría una opción para el borrado de caché desde la aplicación.