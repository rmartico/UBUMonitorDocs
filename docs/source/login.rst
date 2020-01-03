Inicio de sesión
================

Una vez arrancada la aplicación se mostrará la pantalla de inicio de sesión. La ventana muestra en la parte superior la versión actual del producto y permite seleccionar el idioma de preferencia para la aplicación. 

.. figure:: images/Login.png
  :width: 400
  :alt: Login
  :align: center
  
  Inicio de sesión seguro
  
A continuación se deben introducir las credenciales de usuario (login) y su contraseña en Moodle. 

*MUY IMPORTANTE:* la aplicación *NUNCA* almacena de forma persistente, ni renvía a otros servidores, el password del usuario por motivos de seguridad.

En el campo host se debe indicar la URL de la página web de la plataforma Moodle elegida. A la hora de introducir el host, se debe incluir su URL, incluyendo el protocolo de acceso. 

Por ejemplo, para acceder al servidor Moodle de la UBU (UBUVirtual) se pondrá literalmente: 

``https://ubuvirtual.ubu.es``

Se recomienda siempre acceder a servidores seguros (con https://) para garantizar que el envío de información va encriptado.

Sin embargo, UBUMonitor permite acceder a cualquier servidor Moodle que valide usuarios de la forma login/password. Si el servidor al que se accede NO es seguro y no encripta la comunicación (con ``http://`` en lugar de ``https://``), se muestra con un icono y tooltip adicional un aviso al usuario. Se recomienda utilizar esta opción con prudencia y solo en accesos a un servidor local.

.. figure:: images/Login_no_seguro.png
  :width: 400
  :alt: Login no seguro
  :align: center
  
  Inicio de sesión no seguro
  
Por comodidad, se da la opción de *Recordar usuario* y *Recordar host*, evitando tener que volver a rellenar los campos en siguientes accesos. Esa información se guarda en un fichero ``config.properties`` en el directorio actual, si marcamos una o ambas opciones. El botón *Borrar* permite eliminar el texto de los tres campos.

Después de introducir las credenciales pulsamos el botón de *Entrar*. Si los datos son válidos cargará la siguiente pantalla y 
si no, mostrará un mensaje de error. 

En caso de error se recomienda comprobar en este orden:

#. Que la conexión de red está activa.
#. Que el login/password/host se han tecleado correctamente. 
#. Que el servidor actual está activo, accediendo directamente con un navegador.

Si los problemas persisten contactar con los autores de la aplicación para notificar el error.
  
  