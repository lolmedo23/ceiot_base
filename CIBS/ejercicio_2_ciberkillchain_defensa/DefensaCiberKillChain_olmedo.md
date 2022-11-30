Ejercicio Defensa CiberKillChain - Ataque
=====================================
### Alumno

	 Olmedo Lucas Eduardo

### Enunciado

Desarrolla la defensa en función del ataque planteado en orden inverso


Resolución
==========

### Defensa planteada para el caso en que un atacante obtiene las contraseñas de un usuario del comunicador. 
==============================================================================================================


Al detectar accesos que no son realizados por el usuario se propone cambiar la contraseña de acceso asociada a su comunicador y aplicacion. 


###  7- Actions on Objectives
Como medida de prevencion se plantea capacitar a los clientes sobre como debe cambiar una contraseña en caso de necesitarlo y poner advertencias para que los clientes no caigan en algun engaño donde brinden sus contraseñas ante un ataque de phishing o smishing. 
Toda la informacion que se transmite entre el dispositivo y la red debe utilizar TLS para evitar la obtencion de datos mediante la lectura de paquetes.

###  6- Command & Control
Sugerir a los usuarios utilizar redes con contraseñas y cifrado seguro
Se plantea un aviso hacia un correo electronico o telefono cada vez que un usuario se loguea a una aplicacion. De esta forma se dificulta que un atacante pueda ingresar a la aplicacion sin ser detectado, favoreciendo a una deteccion temprana para casos en que alguien distinto al usuario este accediendo a controlar o monitorizar su dispositivo.
Otra accion a tomar para la deteccion de un atacante deshabilitando la alarma de una casa o un local, es implementar en la aplicacion un mensaje de alerta informando que se desactivo la alarma en todas las aplicaciones instaladas asociadas a ese comunicador. 

###  5-Installation
Se plantea activar doble factor de autenticacion para que el atacante no solo tenga que obtener las contraseñas

###  4-Exploitation
Implementar aviso al detectar un nuevo logueo en un nuevo dispositivo y confirmacion para permitir el acceso.

###  3-Delivery 
Mantener publicados los canales oficiales de comunicacion hacia los clientes. Concientizar a los clientes del phishing/smishing.

###  2- Weaponization 
Implementar TLS en las comunicaciones del controlador.
Mantener informados a los clientes de las cuentas oficiales, detectar cuentas falsas que dicen ser de la empresa y reportarlas. 

###  1- Reconnaissance
En el manual dar informacion necesaria pero no informar detalles de implementacion del producto. 
No publicar documentos con arquitecturas o informacion especifica sobre el funcionamiento del producto. 


### Defensa planteada para el caso en que un atacante obtenga contraseñas para administrar el sistema de AWS
==============================================================================================================

###  7- Actions on Objectives
Controlar periodicamente los permisos de los usuarios y acciones ejecutadas en la cuenta para detectar cualquier accion fuera de lo previsto por la empresa, por ejemplo deshabilitar grupos de alarmas.
Se propone utilizar servicios de AWS para pruebas de seguridad. 
Control de usuarios y accesos a la cuenta de AWS detectando anomalias en el uso de los servicios. 

###  6- Command & Control
Accesos especiales para datos almacenados. Almacenamiento de los datos criticos fuera de la nube con control de acceso diferenciado de forma que quede registro de quien accede y si modifica datos. 

###  5-Installation
Cada usuario debe tener los permisos minimos, necesarios y sectorizados para realizar su tarea, esto permite que en caso de que un empleado publique su contraseña (intencional o no) el impacto en el sistema sea menor a que tenga todos los permisos de administrador. Implementar algun metodo para que ninguna persona sola pueda cambiar los permisos de una cuenta, es decir que para cambiar los permisos sean necesario que lo habilite mas de una persona. 

###  4-Exploitation 
En caso de detectar cualquier anomalia, sera necesario mediante alguna cuenta de administrador general bloquear todos los accesos. Analizar que servicios pudieron ser afectados, en caso de estar comprometidos los datos como contraseñas de los usuarios de los controladores de alarmas, sera necesario solicitar a los clientes que cambien las contraseñas para prevenir ataques. 
Es necesario analizar el estado y comportamiento de todos los sistemas para verificar su correcto funcionamiento, en caso de detectar problemas se debera buscar la solucion y de ser necesario suspender el servicio temporalmente e informar a los clientes. 
Si se detecta que se filtro una contraseña de AWS a los empleados o cualquier anormalidad, sera necesario cambiar todas las contraseñas por prevencion. 

###  3-Delivery 
Es necesario capacitar a los empleados permanentemente para evitar ser victimas de phishing.

###  2- Weaponization 
Utilizar contraseñas temporales, al cambiar cada x tiempo las contraseñas reduce el tiempo en que un atacante pueda utilizarlas en caso de ser robadas.

###  1- Reconnaissance
En el manual dar informacion necesaria pero no informar detalles de implementacion del producto. 
No publicar documentos con arquitecturas o informacion especifica sobre el funcionamiento del producto. 


