# hola-mundo-docker


1) Para visualizar los cambios de este proyecto en un servidor real, lo que debes hacer es lanzar un commit alterando únicamente el mensaje del archivo "index.html"

2) Una vez que hagas push al repositorio remoto: https://github.com/eduardobg/hola-mundo-docker , AWS Codepipeline ejectura el build respectivo de la imagen y publicará el cambio en el siguiente repositorio de contenedores: https://hub.docker.com/repository/docker/eduardobg99/hola-docker/general . Una vez dentro de Docker Hub, podrás observar que se ha publicado una nueva versión del saludo, creando un tag con el commit que acabas de ejecutar (esto es genial porque nos ayudará a saber quien fue la persona que altero cada versión de la imagen).

Nota: Iniciar sesión en GitHub y Docker Hub para visualizar ambos repositorios.

3) Despues de publicar la nueva imagen, AWS Codebuild ejecutará un script que nos ayudará a reiniciar el contenedor en ejecución y lo forzará a tomar la nueva imagen con la ayuda de docker-compose.override

4) Ingresa a la siguiente ruta para visualizar tu cambio: http://34.207.120.254/

Saludos!
