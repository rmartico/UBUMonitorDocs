Visualización de registros
==========================

Opciones de los registros
-------------------------

Al pulsar la pestaña de Registros aparece varias opciones de filtrado en la zona inferior de la pantalla principal.

.. figure:: images/OpcionesRegistros.png
  :width: 600
  :alt: Filtro de registros
  :align: center
  
  Filtro de registros
  
* **Cambiar escala máxima sugerida**: permite modificar la escala máxima del eje Y. Se actualiza el valor al cambiar los componentes y/o eventos seleccionados o las otras opciones. Aporta información útil también al mostrar que existe un usuario con esa escala.
* **Agrupar por**: agrupa los registros en diferentes formas

   * Horas
   * AM/PM
   * Días
   * Días de la semana
   * Semanas 
   * Meses
   * Trimestres
   * Años
   * Todos
   
* **Fecha de referencia inicial**: la fecha de inicio orientativo que se muestra al agrupar. Inicialmente toma el valor de la configuración de la asignatura en Moodle.
* **Fecha de referencia final**:  fecha límite orientativa que se muestra al agrupar. Inicialmente se toma como fecha fin el mínimo de la fecha actual y la fecha de fin de curso si existe.

Hay que tener en cuenta que la fecha de referencia  incial y final no toman todos los datos al realizar las agrupaciones. Por ejemplo al agrupar por meses y una fecha inicial del 17/06/2019 a 24/06/2019 no mostrará los registros entre esos dos días, si no que mostrara todas las de junio.

También las agrupaciones por **Horas**, **AM/PM** y **Días de la semana** no usa el selector de fechas, por lo tanto se deshabilitan.

En la zona izquierda inferior se muestran las posibles pestañas de selección de elementos sobre los que generar las gráficas: **Componentes**, **Eventos**, **Secciones** o **Módulos de curso**. Se permite selección múltiple sobre todos ellos.

Componentes
-----------

Lista los registros del curso en función del **Componente** que sea. Incluye las actividades y recursos típicos en Moodle. Solo se visualizan componentes que hayan generado los usuarios matriculados en el curso actualmente.

.. figure:: images/ListaComponentes.png
  :width: 300
  :alt: Lista de componentes
  :align: center
  
  Lista de componentes
  
Eventos
-------

Lista los registros del curso en función del **Componente y Evento** que sea. Se muestran solo los componentes y eventos generados por los usuarios actuales matriculados en el curso. Básicamente desglosa los tipos de eventos que se producen sobre los componentes.

.. figure:: images/ListaEventos.png
  :width: 300
  :alt: Lista de eventos
  :align: center
  
  Lista de eventos
  
Sección
-------

Muestra la estructura de secciones en la que se encuentra organizado el curso. En la prácticas, se corresponden habitualmente con temas o semanas. Inicialmente se muestran solo las secciones visibles pero seleccionando **Con ocultos**, se muestran todas.

.. figure:: images/ListaSecciones.png
  :width: 300
  :alt: Lista de secciones
  :align: center
  
  Lista de secciones
  
Módulos de curso
----------------

Muestra el conjunto completo de módulos de curso, incluyendo todos recursos y actividades que se han creado en el curso. Se muestran ordenados tal y como se encuentran colocados en la asignatura. Inicialmente se muestran solo los módulos visibles pero seleccionando **Con ocultos**, se muestran todos.  

.. figure:: images/ListaModulos.png
  :width: 300
  :alt: Lista de módulos
  :align: center
  
  Lista de módulos

Gráfico de barras apiladas
--------------------------

Para todos los tipos de subpestañas (Componentes, Eventos, Secciones y Módulos de curso) la gráfica que se usa para mostrar los registros del curso son barras apiladas. Muestra en barras cada uno de los usuarios seleccionados con los componentes y/o eventos apilados con diferentes colores cada uno. También se apilan las líneas que indican el valor medio de los usuarios filtrados en ese momento.

.. figure:: images/GraficoBarrasApiladas.png
  :width: 600
  :alt: Grafico de Barras Apiladas
  :align: center
  
  Gráfico BarrasApiladas
  
  
Gráfico de HeatMap
------------------

De igual forma, para todas las subpestañas, si seleccionamos la vista **HeatMap**, se muestra un "mapa de calor" para los usuarios seleccionados. El mapa de calor colorea desde rojo hacia verde, de menor a mayor intensidad, en relación al número de accesos del usuario a los elementos seleccionados en la pestaña de **Registros** y con la selección de filtro de la zona inferior. 

.. figure:: images/GraficoHeatMap.png
  :width: 600
  :alt: Grafico de HeatMap
  :align: center
  
  Gráfico de HeatMap
  
Si presionamos en el gráfico sobre la leyenda superior en un intervalo, por ejemplo en  el valor cero, se resaltan en el gráfico dichos valores situados en dicho intervalo, facilitando por ejemplo, la detección de alumnos en riesgo de abandono o en otras situaciones.
 
.. figure:: images/GraficoHeatMapResaltandoValor.png
  :width: 600
  :alt: Grafico de HeatMap
  :align: center
  
  Gráfico de HeatMap resaltando intervalo seleccionado
  
Por otro lado, al hacer click sobre cualquier zona del gráfico, se resalta el alumno correspondiente en el listado de alumnos, facilitando su identificación.