### Taller 1
**Universidad ICESI**  
**Curso:** Sistemas Distribuidos  
**Docente:** Daniel Barragán C.  
**Tema:** Automatización de infraestructura (Vagrant+Chef)  
**Correo:** daniel.barragan at correo.icesi.edu.co

### Objetivos
* Realizar de forma autónoma el aprovisionamiento automático de infraestructura
* Diagnosticar y ejecutar de forma autónoma las acciones necesarias para lograr infraestructuras estables
* Ejecutar pruebas automáticas sobre infraestructuras aprovisionadas automáticamente

### Prerrequisitos
* Vagrant
* VirtualBox
* Box del sistema operativo CentOS7

### Descripción
Deberá realizar el aprovisionamiento automático de un servidor web emplean la herramienta vagrant y dos tipos de aprovisionamiento: tipo shell y tipo chef-solo. El servidor web una vez desplegado deberá desplegar una pagina web al ingresar a la dirección del servidor en el puerto 80. Adicione pruebas unitarias a la infraestructura por medio de la herramienta kitchen.

### Actividades

1. Consigne los archivos empleados para el aprovisionamiento (Vagrantfile, recetas de chef, scripts de shell, archivos HTML). Incluya la configuración automática de una interfaz de red tipo privada y tipo puente en el Vagrantfile. Adicione comentarios a los archivos explicando cada paso. Incluya capturas de pantalla del funcionamiento de lo solicitado

2. Realice las pruebas descritas en el directorio: https://github.com/ICESI/ds-vagrant/tree/master/centos7/07_kitchen . Incluya capturas de pantalla del funcionamiento de lo solicitado

3. Adapte las fuentes del punto 1 para funcionar con vagrant y chef. Consigne los archivos empleados. Incluya capturas de pantalla del funcionamiento de lo solicitado

### Referencias
* https://docs.chef.io/  
* https://github.com/ICESI/ds-vagrant
