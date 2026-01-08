1. ¿Qué comando de consola usarías para ver todas las redes que existen actualmente en tu Docker?
docker network ls

2. Explica con tus palabras: ¿Por qué es mucho más cómodo usar una "User-defined bridge" en lugar de la red por defecto?
Porque tienen DNS automatico, es decir, si a un contenedor le asignas un nombre como "ejemplo" y desde otro haces "ping ejemplo" este resolvera la ip y tendra conexion.

3. Si uso el driver `host`, ¿puedo mapear puertos con `-p 8080:80`? ¿Por qué?
Si usas el driver "host" el contenedor usara la interfaz de red de tu ordenador, es decir, que si el contenedor tiene asignado el puerto 80 este usara le puerto 80 de tu equipo

4. Investiga: ¿Qué comando usas para ver los detalles de una red (qué contenedores están conectados, sus IPs, etc. Añade la palabra fuenterior a la respuesta.)? 
docker network inspect "el_nombre_de_la_red"