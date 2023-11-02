## Descripción del proyecto
El proyecto pretende definir las bases de configuración y despliegue de aplicaciones web que utilizan Laravel como framework de desarrollo y una base de datos relacional de postgreSQL.
## Guía de despliegue
Clonar el repositorio en un directorio local:
git clone https://github.com/janckos/cloud.git

Dentro del repositorio local, construir la imagen:
docker compose build

Ejecutar los servicios en modo desatendido:
docker compose up -d

Instalar dependencias del la aplicación dentro del contenedor vía Composer:
docker compose exec phpa composer update

Generar la llave de la aplicación/laravel:
docker compose exec phpa php artisan key:generate




(Colocar solo el título, esto se irá rellenando a lo largo del diplomado).
## Instrucciones para ejecutar
- Configurar en el servidor web Apache un virtual host denominado www.diplo.test
- Mediante un navegador web ingresar al siguiente enlace: www.diplo.test
## Pruebas del servicio, con ejemplos de respuesta del servicio.
Una vez que ingrese al enlace proporcionado, se mostrará la siguiente página:

<img src="firstrun.jpg" />

El contenido de esta aplicación irá cambiando a lo largo del diplomado para incorporar lo aprendido.
## Referencias al proyecto
A este momento el repositorio cuenta con el código necesario para ejecutar un proyecto base de Laravel, sin embargo, una vez aprendido los contenidos del Modulo III. Contenedores (en curso), se utilizarán las siguientes imágenes:
- [bitnami/laravel](https://hub.docker.com/r/bitnami/laravel/) Bitnami Laravel Docker Image by VMware 
- [postgres](https://hub.docker.com/_/postgres) Docker Official Image
