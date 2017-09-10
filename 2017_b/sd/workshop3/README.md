### Taller 3
**Universidad ICESI**  
**Curso:** Sistemas Distribuidos  
**Docente:** Daniel Barragán C.  
**Tema:** Introducción a Docker
**Correo:** daniel.barragan at correo.icesi.edu.co

### Objetivos
* Realizar de forma autónoma el aprovisionamiento automático de infraestructura
* Diagnosticar y ejecutar de forma autónoma las acciones necesarias para lograr infraestructuras estables

### Prerrequisitos
* Docker
* Imagen de Python 3.6 de dockerhub
* Repositorio de paquetes local de pip

### Descripción
Deberá	realizar	el	aprovisionamiento	de	un	ambiente	compuesto	por	los	siguientes	elementos: un	servidor	web	(puede	emplear	apache+php o crear	un servicio web con el	lenguaje de su preferencia) y un servidor de base de datos (postgresql, mysql ó mariadb). Se	debe probar	el	funcionamiento	de la conexión entre los servicios web y base de datos a través	de	una	aplicación	web	que realice	 consultas a la	 base	 de	 datos

### Actividades

1. Realice el despliegue de un repositorio de paquetes de pip
2. Escriba un archivo Dockerfile donde realice el despliegue de la aplicación proporcionada. Las instalaciones de los paquetes pip y dependencias deberán realizarse a partir de repositorios de paquetes locales, incluya comentarios donde explique las líneas del archivo Dockerfile
3. Incluya los comandos para:
 * Construir la imagen del contenedor
 * Ejecutar el contenedor.
 * Incluya evidencias gráficas que muestran el funcionamiento de lo solicitado

### Nota

El informe debe ser entregado en formato README.md y debe ser subido a un repositorio de github. El repositorio de github debe ser un fork de https://github.com/ICESI-Training/sd-workshop3 y para la entrega deberá hacer un Pull Request (PR) respetando la estructura definida. El código fuente y la url de github deben incluirse en el informe.  

### Referencias
* https://www.docker.com/  
* https://github.com/ICESI/ds-docker
* https://aboutsimon.com/blog/2012/02/24/Create-a-local-PyPI-mirror.html
