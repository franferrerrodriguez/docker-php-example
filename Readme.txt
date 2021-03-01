
# Creamos una imagen (Ejecutamos desde el directorio de nuestro docker)
docker build -t my-php-app .

# Listamos las imagenes actuales
docker images

# Levantamos una instancia contenedor de la imagen my-php-app
docker run -d -p 8080:80 my-php-app

# Listamos los contenedores levantados
docker ps

# Paramos la ejecución del contenedor
docker rm idcontenedor

# Listamos los contenedores (incl. los parados)
docker ps -a

# Eliminamos el contenador (tiene que estar parado)
docker rm idcontenedor

# Eliminamos la imagen
docker rmi idimagen

# Eliminamos la imagen forzando
docker rmi --force idimagen
