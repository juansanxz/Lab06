# LABORATORIO 6 AZURE 
## Santiago Arévalo Rojas y Juan Felipe Sánchez Pérez
### Exercise 1: Creating Azure Web App and MySQL database
1. Seleccionar shell.azure.com:
<img src="img/1.png" width="30%" height="30%"/>
PowerShell:
<img src="img/2.png" width="30%" height="30%"/>  
Ingresamos a la terminal, y escribimos el siguiente comando para desplegar a un grupo de recurso:  
<img src="img/3.png" width="50%" height="50%"/>  
Para crear un plan de servicio de aplicación:
<img src="img/4.png" width="50%" height="50%"/>   
Para crear la aplicación web con nombre único:
<img src="img/5.png" width="50%" height="50%"/>  
Para crear el MySQL server con un nombre único:  
<img src="img/6a.png" width="50%" height="50%"/>  
En la sección de todos los recursos, observamos la creación de la base de datos:
<img src="img/7.png" width="50%" height="50%"/>  
Se selecciona la base de datos, y en el apartado de propiedades, se observa el nombre del servidor y Nombre de inicio de sesión del administrador del servidor.  
<img src="img/8.png" width="50%" height="50%"/>  
Ahora en el apartado de seguridad de la conexión, permitimos el acceso a los servicios de Azure y guardamos, para que puedan interactuar con las bases de datos del servidor MySQL:
<img src="img/9.png" width="50%" height="50%"/>  
Ahora en la sección de todos los recursos, seleccionamos la aplicación web, y en configuración, seleccionamos la pila de Java, con la versión 8, y con el servidor web de Jaba Apache Tomcat 9.0. Finalmente guardamos:  
<img src="https://user-images.githubusercontent.com/123812331/224488320-ac2163a0-10dc-45b0-a5ec-7123d8c8fd4b.png" width="50%" height="50%"/>   
Seleccionar introducción, y luego examinar, abriendo la página web:
<img src="https://user-images.githubusercontent.com/123812331/224488822-0720fe99-1c2e-4e11-b054-a0d2fccfc3ed.png" width="50%" height="50%"/> 
