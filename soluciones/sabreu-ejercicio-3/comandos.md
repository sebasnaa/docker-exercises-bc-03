## Ejercicio 3

1. **Generar la imagen del proyecto.**

    ```bash
    docker build -t nginx-custom:1.0 .
    ```

2. **Listar las imágenes y asegurarse de que lo tienes en tu local.**

    ```bash
    docker images
    ```

3. **Generar tu `docker-compose` con la capacidad de desplegar el contenedor y dar servicio (dejo a tu elección el puerto 😏)**

    ```yaml
    version: '3.8'

    services:
      nginx:
        image: nginx-custom:1.0
        container_name: mi_nginx_container
        ports:
          - "80:80"
        restart: always
    ```

    **Para ejecutar solo la imagen sin `docker-compose.yml`**

    ```bash
    docker run -d -p 80:80 --name nginx-sebas nginx-custom:1.0
    ```

4. **Testear que te da servicio usando el navegador y sacar una captura de pantalla.**

5. **Modificar el archivo `html/index.html` para que aparezca tu nombre, por ejemplo:**

    ```html
    <html>
    <head>
        <title>Mi Página</title>
    </head>
    <body>
        <h1>Hola, soy [tu nombre]</h1>
    </body>
    </html>
    ```
