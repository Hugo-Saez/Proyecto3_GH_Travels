# Proyecto3_GH_Travels

## 3º Actividad semanal Aplicando BackEnd.

Ya disponemos maquetada la aplicación pero nos falta añadir iteracción a nuestra web, para ello vamos a permitir a los usuarios registrarse y loguearse, para ello modificaremos el menú para incluir dos nuevas opciones registro y login.

Nuestra página de registro simplemente nos pedirá un alias o login de nombre de usuario un correo electrónico, y por ultimo un password y una comprobación del password
![alt_text](https://github.com/GeeksHubsAcademy/Actividad_3/blob/master/register.jpg)

En la página de login pedirá el nombre de usuario o el email y el password.
![alt_text](https://github.com/GeeksHubsAcademy/Actividad_3/blob/master/login.jpg)

---

### Condiciones.

* La web debe estar montado sobre un servidor node y Express el enrutado se deberá gestionar mediante Express.
* Respecto a la página de registro se deberá tener en cuenta las siguientes condiciones:
  * Se deberá comprobar que el password se introduzca en los dos campos igual en caso de no ser así deberá mostrar un mensaje que nos índique que no son iguales.
  * Una vez comprobado la clave se deberá encriptar debemos generar una funcion que realize dicha tarea.
* Respecto a la página de login cuando se pulse "NO RECUERDAS TU CONTRASEÑA" debe aparecer un mensaje indicándonos que introduzcamos el email para recupera la contraseña.
* Se deberá crear una Base de Datos que dispondrá de una tabla con los siguients campos:
  * id -> Integer, autonumérico, not null y clave principal.
  * usuario -> varchar(45) not null
  * email -> varchar(45) not null
  * password -> varchar(80) not null 
  * hash -> varchar(80) null
* Se deberá detectar la visita a otra página y devolver un mensaje de error para indiar que la página que busca no se encuentra.
* El nombre de usuario debe almacenarse en el localStorage del navegador

---

### Característias.
* Se utilizará NPM para la instalación de dependencias.
* El proyecto debe estar subido en un contendor en vagrant, y debe cumplir las siguientes condiciones:
  * Debe disponer de un vagrantfile y un archivo .sh donde se encuentren todos los scripts necesarios para construir el contenedor y nuestra aplicacion se autoejecute.
  * El contendor debe tener abierto el puerto 80 y apuntara internamente al puerto 3000 donde tenemos apuntado nuestro servidor de node.js
  * El contendor debe disponer un mysql instalado con la tabla descrita anteriormente.
* Dentro del package.json debemos disponer la tarea production debe llamar al módulo forever y arrancar la maquina.


"#Proyecto3_GH_Travels" 
index.html is the default apache2 server index, once npm is running,
webpage should load corrctly.
