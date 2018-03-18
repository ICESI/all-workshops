### Taller 2
**Universidad ICESI**  
**Curso:** Sistemas Distribuidos  
**Docente:** Daniel Barragán C.  
**Tema:** Monitoreo de alertas con Sensu y RabbitMQ  
**Correo:** daniel.barragan at correo.icesi.edu.co

### Objetivos
* Realizar el aprovisionamiento automático de herramientas para el monitoreo de infraestructura
* Diagnosticar y corregir fallas en infraestructura distribuida
* Desplegar infraestructura que hace uso de colas de mensajería

### Prerrequisitos
* Vagrant
* VirtualBox
* Box del sistema operativo CentOS7

### Descripción
Deberá realizar el aprovisionamiento automático de un ambiente de monitoreo con la tecnología sensu. Incluya en su infraestructura los siguientes nodos: dos clientes, un servidor de cola de mensajes y un servidor de sensu. Emplee la capacidad de multiambientes de Vagrant para definir la infraestructura de cada nodo y su aprovisionamiento.

### Actividades

1. Consigne los archivos empleados para el aprovisionamiento (Vagrantfile, recetas de chef ó scripts de shell). Incluya capturas de pantalla del funcionamiento de lo solicitado y una breve descripción de lo observado en las capturas. Incluya una o varias capturas del dashboard de uchiwa.

2. Por cada uno de las tecnologías involucradas en el despliegue, incluya un fragmento de los logs (var/log/) y explique que indican.

### Referencias
* https://sensuapp.org/  
* https://www.rabbitmq.com
