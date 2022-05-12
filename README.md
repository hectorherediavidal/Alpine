# Alpine



## 1- El primer paso es descargar alpine linux desde tu pagina web
  ![descarga]( https://github.com/hectorherediavidal/Alpine/blob/main/img/17.PNG "")
  <br>
  <br>


## 2- Ahora debemos crear una maquina virtual con alpine
  ![maquina]( https://github.com/hectorherediavidal/Alpine/blob/main/img/18.PNG "")
   <br>
  <br>
  
 - En las opciones de la maquina virtual podemos dejarlas en predeterminado
 <br>
 
 
 ## 3- Seleccionamos la ISO de alpine que nos hemos descargado
  ![maquina]( https://github.com/hectorherediavidal/Alpine/blob/main/img/19.PNG "")
   <br>
  <br>
  
  
 ## 4- Al iniciar la maquina nos debe aparecer esto
  ![maquina]( https://github.com/hectorherediavidal/Alpine/blob/main/img/1.PNG "")
   <br>
  <br>
  
  - Debemos iniciar sesión como root
  - Una vez que hemos entrado, usamos el comando setup-alpine.

## 5- Debemos seleccionar el idioma del teclado, en nuestro caso sera es (español)
  ![maquina]( https://github.com/hectorherediavidal/Alpine/blob/main/img/es.PNG  "")
   <br>
  <br>
  
  
## 6- En esta parte debemos seleccionar unas cuantas opciones:
  ![maquina]( https://github.com/hectorherediavidal/Alpine/blob/main/img/20.PNG  "")
  <br>
  - Elegimos localhost
  - Interfaz eth0
  - Seleccionamos iniciar con eth0
  - Seleccionamos la ip por DHCP
  - Escribimos n
  - Y finalmente debemos escribir una contraseña
  
   <br>
  <br>
  
## 7- Ahora nos pedirá que disco queremos usar:
  ![maquina]( https://github.com/hectorherediavidal/Alpine/blob/main/img/21.PNG  "")  
  <br>
  - Seleccionamos sda y despues escribimos sys
  - Nos pedira borrar el disco, escribimos "y" para hacerlo
  - Una vez que este borrado, debemos reiniciar la máquina


## 8- Debemos cambiar los siguientes ajustes en la configuración de la máquina
  ![maquina]( https://github.com/hectorherediavidal/Alpine/blob/main/img/22.PNG  "")
  <br>
  ![maquina]( https://github.com/hectorherediavidal/Alpine/blob/main/img/23.PNG  "")
  <br>
  <br>
  
  
## 9- Una vez que tengamos la maquina encendida debemos iniciar sesión como root y poner la contraseña que hemos puesto antes
<br>
A continuación debemos usar el siguiente comando:
<br>
    vi /etc/ssh/sshd_config
  
  
## 10- Una vez dentro, debemos bajar hasta la linea 32 y realizar los siguientes cambios:
![maquina]( https://github.com/hectorherediavidal/Alpine/blob/main/img/31.PNG  "")
  
  
  - Y ahora usamos el comando "service sshd restart"
  - Necesitamos ver la ip de la máquina, y podemos hacerlo con el comando "ip a".
<br>
<br>

- Ahora debemos usar GIT para conectarnos a la maquina de Alpine
<br>
<br>


## 12- Usamos el siguiente comando cambiando la ip por la ip que tengas en tu maquina de Alpine
![maquina]( https://github.com/hectorherediavidal/Alpine/blob/main/img/32.PNG  "")
<br>
<br>


## 12- Ahora debemos cambiar unos archivos, asi que usamos el siguiente comando:
  -vi /etc/apk/repositories.
<br>

![maquina]( https://github.com/hectorherediavidal/Alpine/blob/main/33.PNG "")


  - Ahora usamos el comando "apk add docker" para instalar Docker en Git.
<br>
<br>

## 13- Usamos el comando "service docker start" para iniciar Docker

  - Y ahora usamos "docker run -p 8989:80 -d nginx


## 13- Para comprobar que todo ha funcionado, vamos a lanzar un "docker run hello-world" para ver si todo ha funcionado.

![maquina]( https://github.com/hectorherediavidal/Alpine/blob/main/34.PNG "")




  
