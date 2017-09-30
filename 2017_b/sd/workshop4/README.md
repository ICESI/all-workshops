### Taller 4
**Universidad ICESI**  
**Curso:** Sistemas Distribuidos  
**Docente:** Daniel Barragán C.  
**Tema:** Introducción a Docker Compose  
**Correo:** daniel.barragan at correo.icesi.edu.co

### Objetivos
* Realizar de forma autónoma el aprovisionamiento automático de infraestructura
* Diagnosticar y ejecutar de forma autónoma las acciones necesarias para lograr infraestructuras estables

### Prerrequisitos
* Docker
* Docker-Compose
* Contenedores: consul, consul-template, registrator, load balancer (nginx, haproxy)

### Descripción
Deberá realizar el aprovisionamiento de un ambiente compuesto por los siguientes elementos:
un servidor web con capacidad de escalar a N instancias (puede	emplear	apache+php o crear	un servicio web con el	lenguaje de su preferencia), un balanceador de carga para redireccionar las peticiones a los servidores web.

Tenga en cuenta:
* Para el aprovisionamiento deberá usar docker-compose
* Emplear una herramienta de descubrimiento de servicio (zookeper, consul, etcd) que permita
registrar automáticamente las nuevas instancias de servidores web. Las tecnologías de descubrimiento de servicio se componen de agentes y un servidor ó clúster de servidores. Los
agentes envían información al clúster acerca de los servicios que se ejecutan en las instancias. El servidor registran los servicios que son anunciados por los agentes para ser consultados por los clientes ú otros servicios
* Para evitar ejecutar mas de un servicio por contenedor (agente de consul y servicio web) emplee la aplicación dockerizada registrator (ó una tecnología similar) para registrar los nuevos contenedores ante el servidor de descubrimiento de servicio
* Para actualizar la configuración de los archivos de configuración del balanceador de carga y reiniciar el servicio emplee la aplicación consul-template. Consul-template consulta al servidor de consul el estado de los servicios y ante un cambio en ellos, a partir de plantillas, crea nuevamente los archivos de configuración.

### Actividades
1. Identifique en forma general los componentes que hacen parte de la infraestructura
2. Escriba el archivo docker-compose y los Dockerfile necesarios para realiar el despligue de la infraestructura y aprovisionamiento, incluya comentarios donde explique las líneas del archivo docker-compose y Dockerfile empleados
3. Incluya en el informe
 * Comandos para desplegar la infraestructura
 * Incluya evidencias gráficas que muestran el funcionamiento de lo solicitado

### Nota
El informe debe ser entregado en formato README.md y debe ser subido a un repositorio de github. El repositorio de github debe ser un fork de https://github.com/ICESI-Training/sd-workshop4 y para la entrega deberá hacer un Pull Request (PR) respetando la estructura definida. El código fuente y la url de github deben incluirse en el informe.  

https://livewyer.io/blog/2015/02/05/service-discovery-docker-containers-using-consul-and-registrator/  
https://picodotdev.github.io/blog-bitix/2017/01/registro-y-descubrimiento-de-servicios-con-spring-cloud-y-consul/
