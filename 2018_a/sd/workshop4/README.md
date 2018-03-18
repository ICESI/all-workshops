### Taller 4
**Universidad ICESI**  
**Curso:** Sistemas Distribuidos  
**Docente:** Daniel Barragán C.  
**Tema:** Descubrimiento de Servicio  
**Correo:** daniel.barragan at correo.icesi.edu.co

### Objetivos
* Comprender los conceptos y componentes básicos del descubrimiento de servicio
* Desplegar infraestructura de soporte a descubrimiento de servicio

### Prerrequisitos
* Vagrant
* VirtualBox
* Box del sistema operativo CentOS7

### Descripción
Deberá realizar el aprovisionamiento automático de un ambiente de descubrimiento de servicio con la tecnología consul. Incluya en su infraestructura los siguientes nodos: dos clientes ejecutando el cliente de descubrimiento de servicio,  un balanceador de carga para los clientes, un servidor de descubrimiento de servicio (opcional en cluster con balanceador), un servidor DHCP, un servidor DNS.

Tenga en cuenta las siguientes consideraciones:
* El servidor de descubrimiento de servicio tendrá una IP fija y una URL almacenada en el servidor DNS.
* Los clientes de descubrimiento de servicio recibirán una IP del servidor DHCP, la cual emplearán como entrada para la ejecución del agente.
* El cliente de descubrimiento de servicio deberá ejecutarse como un servicio del sistema.
* El balanceador debe ejecutar consul-template para actualizar dinámicamente su configuración.

### Actividades

1. Despliegue en los clientes el mismo microservicio y muestre a través de capturas de pantalla como el balanceador redirecciona las peticiones a cada uno de ellos.
2. Detenga uno de los microservicios y muestre como el balanceador continua redireccionando las peticiones unicamente al microservicio activo.
3. Despliegue un nuevo cliente y muestre como este sin ningun tipo intervención es usado por el balanceador.

### Referencias
* https://www.consul.io/  
* http://www.admintome.com/blog/installing-consul-on-ubuntu/  
* https://superuser.com/questions/968561/how-to-get-the-machine-ip-address-in-a-systemd-service-file
