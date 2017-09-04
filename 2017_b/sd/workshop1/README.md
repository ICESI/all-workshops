### Taller 1
**Universidad ICESI**  
**Curso:** Sistemas Distribuidos  
**Docente:** Daniel Barragán C.  
**Tema:** Automatización de infraestructura (Vagrant+Chef)  
**Correo:** daniel.barragan at correo.icesi.edu.co

### Objetivos
* Realizar de forma autónoma el aprovisionamiento automático de infraestructura
* Diagnosticar y ejecutar de forma autónoma las acciones necesarias para lograr infraestructuras estables
* Realizar el aprovisionamiento automático de un balanceador de carga

### Prerrequisitos
* Vagrant
* Box del sistema operativo CentOS7

### Descripción
Deberá	realizar	el	aprovisionamiento	de	un	ambiente	compuesto	por	los	siguientes	elementos:	un servidor	encargado de	realizar balanceo de	carga,	dos	servidores	web	(puede	emplear	apache+php o crear	un servicio web con el	lenguaje de su preferencia). Se	debe probar	el	funcionamiento	del balanceador	a través	de	una	aplicación	web	que realice	 consultas	 a	 la	 base	 de	 datos	 a	 través	 de	 los servidores	 web (mostrar visualmente cual	servidor web atiende la	petición)

![][1]

### Actividades

1. Consigne los comandos de linux necesarios para el aprovisionamiento de los servicios solicitados. En este punto no debe incluir recetas solo se requiere que usted identifique los comandos o acciones que debe automatizar
2. Escriba el archivo Vagrantfile para realizar el aprovisionamiento, teniendo en cuenta definir:
maquinas a aprovisionar, interfaces solo anfitrión, interfaces tipo puente, declaración de cookbooks, variables necesarias para plantillas. Incluya el Vagrantfile añadiendo comentarios en cada línea encargada del aprovisionamiento de la infraestructura.

  ```ruby
  # -*- mode: ruby -*-
  # vi: set ft=ruby :

  VAGRANTFILE_API_VERSION = "2"

  Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
    config.ssh.insert_key = false
    config.vm.define :load_balancer do |lb
       #
    end
    config.vm.define :wb_server do |wb|
      #
    end
   end
  end
  ```

3. Escriba los cookbooks necesarios para realizar la instalación de los servicios solicitados. Incluya una tabla como se muestra a continuación explicando la función de cada archivo o directorio en los cookbooks. No incluya código fuente en el informe para esta sección.  

| Directorio o archivo | Descripción   |
|------|------|
| cookbooks | En este directorio se ubican ... |

4. Incluya evidencias gráficas que muestran el funcionamiento de lo solicitado

### Nota

El informe debe ser entregado en formato README.md y debe ser subido a un repositorio de github. El repositorio de github debe ser un fork de https://github.com/ICESI-Training/sd-workshop1 y para la entrega deberá hacer un Pull Request (PR) respetando la estructura definida. El código fuente y la url de github deben incluirse en el informe.  

### Referencias
* https://docs.chef.io/  
* https://github.com/ICESI/ds-vagrant

[1]: images/01_diagrama_despliegue.png
