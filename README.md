#	Login con Laravel y Next js

##  Interfaces:
### Login
<p aling="center"><img src="/README/1.png"></p>

### Registro
<p aling="center"><img src="/README/2.png"></p>

### Panel Home
<p aling="center"><img src="/README/3.png"></p>

##	Versiones:
*	**Laravel:** 10.13.1
*	**Next js:** 


#   Requisitos necesarios:
*   Node js
*   Composer
*   Xampp/Wamp

#	Proceso:
###	Creando la APP
`laravel new example-app`
###	Ingresando a la APP
`cd example-app`
###	Consultando la versión de laravel
`php artisan --version`
###	Iniciando los servidores:
####    Back-end
`php artisan serve`
####    Front-end
`npm run dev`


#   Uso de otras tecnologías:
##  Breeze
### Instalando
`composer require laravel/breeze --dev`
##  API de autenticación:
### Instalando
`php artisan breeze:install api`
### Configurando
En la carpeta **\app\Providers** <br>
En el archivo `AppServiceProvider.php` agregar en la función **boot** y su respectiva ruta:
`Schema::defaultStringLength(191);` 

##  Encender el servidor (XAMPP / WAMP)
###  Ejecutando las Migraciones:
`php artisan migrate`
Automáticamente creara las tablas 

##  Creación del Front:
Creando una carpeta `frontLoginNextjs` con cualquier nombre en cualquier lugar, después ingresar a la carpeta creada y clonar el repositorio de [breeze](https://github.com/laravel/breeze-next):
`git clone https://github.com/laravel/breeze-next.git`
##  Instalando las dependencias:
Ingresar a la carpeta `frontLoginNextjs\breeze-next`
Ejecutar el comando: `npm install`
Correr el Front-end: `npm run dev`