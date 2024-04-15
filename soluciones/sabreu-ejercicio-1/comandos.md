## Ejercicio 1

1. **Bajar la imagen de Nginx:latest**

    ```bash
    docker pull nginx
    ```

2. **Iniciar el contenedor con un nombre personalizado**
   
    ```bash
    docker run -d --name sabreu-nginx nginx
    ```

3. **Obtener el ID y detener un contenedor**

    ```bash
    docker ps
    docker stop <container_name/id>
    ```

4. **Mostrar los contenedores detenidos**

    ```bash
    docker ps -a
    ```

5. **Eliminar un contenedor**

    ```bash
    docker rm <container_name/id>
    ```

6. **Usar el comando para listar las imágenes**

    ```bash
    docker images
    ```

7. **Usar el comando para listar los contenedores y su estado**

    ```bash
    docker ps -a
    ```

8. **Acceder al contenedor a través de la consola y ejecutar cualquier comando**

    ```bash
    docker exec -it sabreu-nginx bin/bash
    ```

9. **Eliminar el contenedor**

    ```bash
    docker rm <container_name/id>
    ```

10. **Eliminar la imagen de vuestro registro local**

    ```bash
    docker rmi <container_name/id>
    ```