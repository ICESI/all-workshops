### Taller 3
**Universidad ICESI**  
**Curso:** Sistemas Distribuidos  
**Docente:** Daniel Barragán C.  
**Tema:** Cluster de RabbitMQ
**Correo:** daniel.barragan at correo.icesi.edu.co

### Objetivos
* Comprender los conceptos y componentes básicos de la comunicación por colas de mensajes
* Desplegar infraestructura de soporte a colas de mensajería

### Prerrequisitos
* Vagrant
* VirtualBox
* Box del sistema operativo CentOS7

### Descripción
Deberá realizar el aprovisionamiento automático de un cluster de RabbitMQ. Incluya en su infraestructura al menos 3 nodos.

### Actividades

1. Implemente un programa productor y un programa consumidor que haga uso del cluster de mensajería. No active el modo de alta disponibilidad en el cluster (HA). Realice las siguientes pruebas:

  * Demuestre que un mensaje enviado desde el productor puede ser recuperado por el consumidor
  * Demuestre que si elimine el nodo donde reside el mensaje enviado por el productor, este no puede ser recuperado por el consumidor.

  Proporcione evidencias de lo solicitado, incluya capturas de pantalla del estado de la cola de mensajes para cada caso.

2. Implemente un programa productor y un programa consumidor que haga uso del cluster de mensajería. Active el modo de alta disponibilidad en el cluster (HA). Realice las siguientes pruebas:  

  * Demuestre que un mensaje enviado desde el productor puede ser recuperado por el consumidor
  * Demuestre que si elimine uno de los nodos donde reside el mensaje enviado por el productor, este puede ser recuperado por el consumidor.

  Proporcione evidencias de lo solicitado, incluya capturas de pantalla del estado de la cola de mensajes para cada caso.

3. Repita el paso 2 empleando un balanceador de carga por delante del cluster de RabbitMQ.

### Referencias
* https://sensuapp.org/  
* https://www.rabbitmq.com
