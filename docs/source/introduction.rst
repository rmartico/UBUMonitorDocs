Introducción y requisitos
=========================

UBUMonitor es una *aplicación cliente de escritorio* que permite conectarse a un *servidor Moodle* para la monitorización de la actividad particular de los alumnos. Permite extraer los datos de los registros (logs), calificador y finalización de actividad de nuestras asignaturas, visualizando dichos datos de una manera más amigable para el profesor. Adicionalmente permite monitorizar el riesgo de abandono de los alumnos matriculados.

Requisitos de instalación
-------------------------

* Sistema operativo Windows, GNU/Linux o Mac.
* Disponer de conexión a Internet.
* Disponer de un mínimo de:

   * *200 MB libres* de disco duro para la versión portable con el *launcher*, que incluye el Java Runtime Environment (JRE).
   * *30 MB* libre de disco si ya se tiene instalado Java 8 con JavaFX y se opta por utilizar directamente el fichero ejecutable ``.jar`` (opción **NO recomendada**).

Requisitos en Moodle
--------------------

* Obligatorio

   * Disponer de cuenta con **rol de profesor** en las asignaturas o cursos a los que se quiera acceder.
   * Acceder a Moodle con validación web básica a través de `http://` o `https://`. 
   * Tener activado en el servidor Moodle el **soporte para móviles** (apps móviles). En caso de error al realizar *login* desde UBUMonitor, consulte con el administrador del servidor Moodle su posible activación.

* Opcional (para una mejor experiencia)

   * Configurar correctamente en la asignatura (en **Editar ajustes** del curso en **General**), la *Fecha de inicio del curso* y además, habilitar y establecer la *Fecha de finalización del curso*. De esta forma, la selección inicial mostrará los cursos en las pestañas adecuadas (en *En progreso*, *Futuros* y *Pasados*) y funcionará correctamente la configuración por defecto de los filtros de fecha para los registros.
   
   * Tener **visibles los porcentajes** en la vista de usuario de la asignatura en el calificador de Moodle (en *Calificaciones* -> *Vista* -> *Usuario*). Para que funcione la carga de los datos del calificador, establecerlo en: *Calificaciones* -> *Configuración* -> *Ajustes de la calificación del curso* -> *Usuario* -> *Mostrar porcentaje* -> *Mostrar*.
   

   * Habilitar la **opción del rastreo de finalización de las actividades o recursos** en *Editar ajustes del curso*, en el apartado *Rastreo de finalización*. Una vez realizado ese cambio se necesita entrar en cada actividad y recurso, para personalizar su opción *Finalización de actividad*.
   
   * Tener **definidos grupos en la asignatura** si se quieren utilizar los filtros y gráficos particulares sobre grupos.

