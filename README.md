# Login-GroceryCrud

Tiene la funcionalidad de Login/Logout basado en el proyecto de GroceryCrud.

> Estas modificaciones estan basadas en  [WIKI](https://github.com/portapipe/Login-GroceryCrud/wiki) para su referencia
> Oficial [Official Website](https://portapipe.github.io/Login-GroceryCrud/) 

![alt tag](https://github.com/portapipe/Login-GroceryCrud/blob/master/login_page.png?raw=true)

## Requerimientos
- Apache httpd-2.4.6
- CentOS Linux release 7.6.1810 (Core) 
- MySQL
- PHP 7.2.24
- CodeIgniter

## Como configurar  

### Paso #1 - Aplicación 
Para ello es necesario copiar los siguientes archivos a su proyecto:

- application/controllers/Login.php
- application/models/Login_model.php
- application/views/login.php
- application/views/admin_page.php

### Paso #2 -  Configurar el manejo de la sesión del usuario a nivel de base de datos

 Para ello se debe modificar el archivo de configuración global config.php

 - /application/config/config.php

Es necesario cambiar las siguientes variables,  

- $config['base_url'] = 'http://34.217.90.120/gmscrudbeta/';   //  Cambiar la URL por la de su proyecto
- $config['sess_driver'] = 'database';  // debe ser database
- $config['sess_save_path'] = 'ci_sessions'; //  debe ser ci_sessions

### Paso #3 -  Configuración del  acceso a la base de datos

 Para ello se debe modificar el archivo de configuración de la conexión de la base de datos: database.php

 Y cambiar los parametros correctos

 - /application/config/database.php

 	- 'hostname' => 'localhost',
	- 'username' => 'gmscrud',
	- 'password' => 'gmscrudd4t4b4s3',
	- 'database' => 'gmscrud',
	- 'dbdriver' => 'mysqli',


