## Ejercicio 3

1. **Crear los archivos Dockerfile en cada proyecto.**

2. **Ejecutar los comandos necesarios para generar las imágenes.**

    ```bash
    docker build -t api-sebas:1.0 .
    docker build -t ui-sebas:1.0 .
    ```

3. **Ejecutar las imágenes.**

    ```bash
    docker run -d -p 3000:3000 --name api api-sebas:1.0
    docker run -d -p 5173:5173 --name ui ui-sebas:1.0
    ```