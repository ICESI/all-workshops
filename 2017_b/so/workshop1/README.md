### Taller 1
**Universidad ICESI**  
**Curso:** Sistemas Operativos  
**Docente:** Daniel Barragán C.  
**Tema:** Comandos de Linux, Estructura de directorio, Virtualización  
**Correo:** daniel.barragan at correo.icesi.edu.co


### Objetivos
* Conocer y emplear comandos de Linux para la realización de tareas administrativas

### Prerrequisitos
* Virtualbox o WMWare
* Máquina virtual con sistema operativo CentOS7

### Descripción
El primer taller del curso sistemas operativos trata sobre el sistema operativo Linux, la estructura de sus directorios y virtualización 

### Actividades

1. Explique la función de los directorios en la raíz de sistema operativo Linux-CentOS.
Proporcione ejemplos de los archivos que se encuentran en cada directorio (explique al menos un
archivo por directorio).

| Directorio | Función |
|------|------|
| bin | Este directorio es un directorio estático, almacena todos los ejecutables de usuario parecidos a los archivos .exe |
| sbin | Al igual que bin contiene los programas ejecutables que solo son ejecutables por el root user |
| boot | Contiene los archivos de configuración de arranque necesarios para que el kernel pueda iniciar su funcionamiento |
| dev | Contiene todos los dispositivos en forma de archivos |
| proc | Este directorio contiene la información sobre el estado del sistema y sus procesos |
| var | Contiene los archivos con información del sistema. Archivos de registros y bases de datos |
| etc | Contiene archivos de configuración que no contiene binarios |
| home | Directorio personal para cada usuario |
| initrd | Este directorio se emplea cuando se va a iniciar un arranque personalizado |
| lib | Contiene las librerías necesarias para la ejecución de binarios |
| media | Directorio temporal para dispositivos removibles |
| opt | Este directorio es opcional contiene aplicaciones  externas |
| root | Directorio de super usuario, solo el usuario root puede emplearlo |
| srv | Contiene servicios especificos de datos del servidor |
| sys | Contiene archivos del sistema |
| tmp | Contiene los archivos temporales creados por el sistema y por los usuarios |
| usr | Aplicaciones y archivos a los que puede acceder la mayoría de los usuarios |
| mnt | Corresponde a los sistemas de archivos montados manualmente en el disco duro |


| Directorio   | Archivo ejemplo | Descripción del contenido del directorio  |
|------|------|------|
| bin | dmesg | Imprime o controla el mensaje de buffer del kernel |
| sbin | fasthalt | Detiene el sistema sin revisar los discos |
| boot | map | Contiene la ubicación del kernel |
| dev | lp0| Primer puerto paralelo corresponde a dispositivos como impresoras, escaners, entre otros |
| proc | devices | Lista los drivers de los dispositivos que estan actualmente corriendo en el kernel |
| var | db | Banco de almacenamiento de datos |
| etc | autoconf | Se crean scripts para configurar los paquetes de código fuente |
| home | ccm | Carpeta con diagramas sdl de la clase |
| initrd | /dev/initrd | Actúa como subdirectorio para iniciar la RAM |
| lib | modules/'kernel-version' | Contiene todos los módulos del kernel |
| media | cdrecorder | CD writer |
| opt | Kylix | Paquete externo, software que no está instalado por defecto |
| root | anaconda-ks.cfg | Archivo de configuración en el usuario root |
| srv | wwww | Relaciona archivos de un servidor web al sistema |
| sys | Contiene archivos del sistema |
| tmp | hannie.txt | Archivo de texto |
| usr | src | Subdirectorio de Linux que contiene las fuentes del Kernel y documentación |
| mnt | mount /dev/cdrom /mnt/cdrom | Monta un archivo en un cdrom accediendo al directorio de archivos contenidos en cdrom |


2. En una tabla como se muestra a continuación escriba 10 comandos de Linux no visto en clase. Puede incluir comandos que funcionan una vez han sido instalados con yum

| Comando   | Usuario | Descripción   |
|------|------|------|
| find -name .sh | root | Busca archivos dado un directorio |
| man | root | Proporciona documentación online de todas las opciones posibles de un comando |
| kill | root | Corta procesos que no son relevantes o que no responden |
| alias | root | Deja signar nombre a comandos |
| free | root | Proporciona información de memoria | 
| fortune | root | Adivina tu suerte | 
| htop | cualquiera | para observar los procesos que se estan ejecutando y administrarlos |
| youtube-dl url-to-video | cualquiera | Descarga videos de youtube mediante su url |
| touch testfile.txt | Permite crear archivos como mkdir crea directorios |
| command & | Ejecuta comandos sin mostrar todo su proceso, solo errores y algunas notificaciones (commands in background) |


3. ¿Cuál es la utilidad del comando printenv en Linux?, Investigue acerca de la creación de variables de ambiente en Linux y como hacerlas permanentes. Cree una variable de ambiente, hágala permanente y muestre evidencias del funcionamiento.
El comando printenv despliega en pantallalas variables de ambiente, se puede especifcar con un parametro en cuyo caso solo despliegará el valor de la variable requerida. 
Para hacerla permanente se accede a etc/environment desde el usuario root y luego con el comando vi y llamando al mismo directorio (vi /etc/environment) se  agrega la variable.

### Nota

El informe debe ser entregado en formato README.md y debe ser subido a un repositorio de github. El repositorio de github debe ser un fork de https://github.com/ICESI-Training/so-workshop1 y para la entrega deberá hacer un Pull Request (PR) respetando la estructura definida. El código fuente y la url de github deben incluirse en el informe.  

![][1]
![][2]
![][3]

## Referencias

* https://github.com/ICESI/so-commands/tree/master/centos7
* https://cmdchallenge.com  
* https://www.gutenberg.org
* https://computernewage.com/2015/06/14/el-arbol-de-directorios-de-linux-al-detalle-que-contiene-cada-carpeta/
* https://help.ubuntu.com/kubuntu/desktopguide/es/directories-file-systems.html
* http://www.thegeekstuff.com/2010/09/linux-file-system-structure/?utm_source=tuicool
* https://www.tecmint.com/20-funny-commands-of-linux-or-linux-is-fun-in-terminal/
* http://www.tldp.org/LDP/Linux-Filesystem-Hierarchy/html/index.html
* https://www.tecmint.com/20-advanced-commands-for-middle-level-linux-users/
* https://www.lifewire.com/linux-terminal-commands-rock-your-world-2201165

[1]: Captura.png
[2]: Captura2.png
[3]: Captura3.png
