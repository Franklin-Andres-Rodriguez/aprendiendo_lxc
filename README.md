> _[!NOTE]_

## LXC Installation and Configuration Guide for Lubuntu␍

### Step 1: Update System Packages␍
Open a terminal and update the package list:
sudo apt update

### instala el entorno de LXC junto con las plantillas necesarias para que puedas crear y gestionar contenedores en tu sistema.
sudo apt install lxc lxc-templates

### Verificar si el computador es apto para la instalacion
lxc-checkconfig

### Crea un contenedor
sudo lxc-create -n my-container -t ubuntu

### Inicia un contenedor
sudo lxc-start -n my-container

### ejecuta sin mantener la sesión de la terminal activa. 
sudo lxc-start -n my-container -d

###  conectarte a un contenedor en ejecución 
sudo lxc-attach -n my-container

### Parar el contenedor
sudo lxc-stop -n my-container

###  lista todos los contenedores presentes en tu sistema.
sudo lxc-ls --fancy
