Ejercicio Defensa CiberKillChain - Ataque
=====================================
### Alumno

	 Olmedo Lucas Eduardo

### Enunciado

Desarrolla la defensa en función del ataque planteado en orden inverso


Resolución
==========

### Defensa planteada para el caso en que un atacante obtiene las contraseñas de un usuario del comunicador. 

Como medida de prevencion se plantea capacitar a los clientes sobre como debe cambiar una contraseña en caso de necesitarlo y poner advertencias para que los clientes no caigan en algun engaño donde brinden sus contraseñas.
Se plantea activar doble factor de autenticacion y un aviso hacia un correo electronico o telefono cada vez que un usuario se loguea a una aplicacion. De esta forma se dificulta que un atacante pueda ingresar a la aplicacion y se favorece a una deteccion temprana para casos en que alguien distinto al usuario este accediendo a controlar o monitorizar su dispositivo. 
Al detectar accesos que no son realizados por el usuario se propone cambiar la contraseña de acceso asociada a su comunicador y aplicacion. 
Otra accion a tomar para la deteccion de un atacante deshabilitando la alarma de una casa o un local, es implementar en la aplicacion un mensaje de alerta informando que se desactivo la alarma en todas las aplicaciones instaladas asociadas a ese comunicador. 
Toda la informacion que se transmite entre el dispositivo y la red debe utilizar TLS para evitar la obtencion de datos mediante la lectura de paquetes.

### Defensa planteada para el caso en que un atacante obtenga contraseñas para administrar el sistema de AWS

Controlar periodicamente los permisos de los usuarios y acciones ejecutadas en la cuenta para detectar cualquier accion fuera de lo previsto por la empresa.
Se propone utilizar servicios de AWS para prueas de seguridad. 
En caso de detectar cualquier anomalia, sera necesario mediante alguna cuenta de administrador general bloquear todos los accesos. Analizar que servicios pudieron ser afectados, en caso de estar comprometidos los datos como contraseñas de los usuarios de los controladores de alarmas, sera necesario solicitar a los clientes que cambien las contraseñas para prevenir ataques. 
Es necesario analizar el estado y comportamiento de todos los sistemas para verificar su correcto funcionamiento, en caso de detectar problemas se debera buscar la solucion y de ser necesario suspender el servicio temporalmente e informar a los clientes. 
Si se detecta que se filtro una contraseña de AWS a los empleados o cualquier anormalidad, sera necesario cambiar todas las contraseñas por prevencion. 
Se plantea que los empleados tengan permisos limitados y sectorizados, esto permite que en caso de que un empleado publique su contraseña (intencional o no) el impacto en el sistema sea menor a que tenga todos los permisos de administrador. 
Es necesario capacitar a los empleados permanentemente para evitar ser victimas de pishing.



