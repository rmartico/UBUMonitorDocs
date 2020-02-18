Introducción y requisitos
=========================

UBUMonitor es una *aplicación cliente de escritorio* que permite conectarse a un *servidor Moodle* para la monitorización de la actividad particular de los alumnos. Permite extraer los datos del calificador, registros (logs) y finalización de actividad de nuestras asignaturas, visualizando dichos datos de una manera más amigable para el profesor.

Requisitos de instalación
-------------------------

* Sistema operativo Windows, GNU/Linux o Mac.
* Disponer de conexión a Internet.
* Disponer de un mínimo de:

   * *250 MB libres* de disco duro para la versión portable, que incluye el Java Runtime Environment (JRE).
   * *26 MB* libre de disco si ya se tiene instalado Java 8.

Requisitos en Moodle
--------------------

* Obligatorio

   * Disponer de cuenta con **rol de profesor** en las asignaturas o cursos a los que se quiera acceder.
   * Acceder a Moodle con validación web básica a través de `http://` o `https://`. Actualmente **NO** se incluye soporte a sistemas de único registro tipo *Single Sign-on*.
   * Tener activado en el servidor Moodle el **soporte para móviles** (apps móviles). En caso de error al realizar *login* desde UBUMonitor, consulte con el administrador del servidor Moodle su posible activación.

* Opcional (para una mejor experiencia)

   * Configurar correctamente (en **Editar ajustes** del curso), en **General**, la  *Fecha de inicio del curso* y *Fecha de finalización del curso* (habilitada) en sus asignaturas. En caso contrario, la selección inicial de cursos (en las pestañas *En progreso*, *Futuros* y *Pasados*) y los filtros de fecha para los gráficos de registros **NO funcionarán correctamente**.
   * Tener **visibles los porcentajes** de la asignatura en el **calificador de Moodle**. En caso contrario **NO se podrán cargar los datos del calificador**.
   * Activar en **Editar ajustes** del curso, en el apartado **Rastreo de finalización** la opción **Habilitar rastreo del grado de finalización**. Una vez realizado ese cambio se recomienda ajustar la opción **Finalización de actividad** para cada actividad y recurso, si se quiere utilizar el gráfico correspondiente.
   * Tener **definidos grupos en la asignatura** si se quieren utilizar los filtros y gráficos particulares sobre grupos.

