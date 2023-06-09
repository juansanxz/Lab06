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
Ir ahora, al apartado de configuración, y en configuraciones de aplicación, se debe crear una nueva cadena de conexión:
<img src="https://user-images.githubusercontent.com/123812331/224489106-242bc78b-bc5b-406c-9c7e-689ae1d55b03.png" width="50%" height="50%"/> 
Llenamos los campo solicitados con lo indicado en la guía del laboratorio. Finalmente, guardamos los cambios:
<img src="https://user-images.githubusercontent.com/123812331/224489238-302cb94f-e5ef-4c84-a53a-1be9bcfddda6.png" width="50%" height="50%"/> 
Luego en el proyecto seleccionamos pipeline:
<img src="https://user-images.githubusercontent.com/123812766/224489704-d4b6c988-c65b-4838-a13a-7523899f51f2.png" width="50%" height="50%"/> 
Y elegimos MyShuttleBuild:
<img src="https://user-images.githubusercontent.com/123812766/224489760-dbbf7803-abc5-4ea6-ade6-ec20b8c4ceb3.png" width="50%" height="50%"/> 
Para editarlo:
<img src="https://user-images.githubusercontent.com/123812766/224490031-d8b8eb7c-ff60-4a4c-8def-743aa45dc468.png" width="50%" height="50%"/> 
Seleccionamos maven para proceder a elegir queue:
<img src="https://user-images.githubusercontent.com/123812766/224490143-c724c899-ba87-4815-ba15-33100861ccfa.png" width="50%" height="50%"/> 
Y run:
<img src="https://user-images.githubusercontent.com/123812766/224490205-d5f50233-300d-4349-bd3e-bcd6c1647e14.png" width="50%" height="50%"/>
Nos salió el siguiente error, para solucionarlo vamos a rellenar la encuesta que está en el link:
<img src="https://user-images.githubusercontent.com/123812766/224490333-5090ba88-6794-4bf3-9c4f-cdd162c8fc6c.png" width="50%" height="50%"/>
Una vez que nos hayan resuelto el problema y se vuelva a correr se evidencia algo así:
<img src="https://user-images.githubusercontent.com/123812766/225180093-9a3107f3-60ec-4e99-a957-e3afc2e95260.png" width="50%" height="50%"/>
Ahora en Releases:
<img src="https://user-images.githubusercontent.com/123812766/225180361-0c9d95d8-bbca-4a95-ac70-4530006519a1.png" width="50%" height="50%"/>
Editamos el de MyShuttleRelease para verificar que el Artifact esté apuntando al artefacto Build:
<img src="https://user-images.githubusercontent.com/123812766/225182480-1b143bd1-0446-409e-b91e-7c52504385aa.png" width="50%" height="50%"/>
Después vamos al apartado de tasks y llenamos la información solicitada y seleccionamos save:
<img src="https://user-images.githubusercontent.com/123812766/225196461-96762429-9a06-49fe-95de-9aede58b0d0a.png" width="50%" height="50%"/>
<img src="https://user-images.githubusercontent.com/123812766/225196595-39e235c5-c038-46ba-a24b-6f3f80a6690e.png" width="50%" height="50%"/>
Se crea un release:
<img src="https://user-images.githubusercontent.com/123812766/225198424-8070e329-21cc-4024-a681-a04fe3c94641.png" width="50%" height="50%"/>
Finalmente, una vez el realease se cargue, ingresando a la app web creada:
<img src="https://user-images.githubusercontent.com/123812766/225199620-127cb28f-365a-4157-9ada-4d9286cb89c3.png" width="50%" height="50%"/>
Con las credenciales otorgadas:
<img src="https://user-images.githubusercontent.com/123812766/225199798-f8560cc7-8349-4c74-bddd-356263d4d95d.png" width="50%" height="50%"/>

