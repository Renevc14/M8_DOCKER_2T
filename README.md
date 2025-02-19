## DOCUMENTACIÓN DE LA PRUEBA
Se realiza un HTML básico con la información de mi CV.
![Descripción de la imagen](images/CV.png)
### 2. Imagen Docker
Ejecutar el siguiente comando en la terminal:
```sh
docker build -t mi-cv-vilela-imagen .
```
![Descripción de la imagen](images/dockerImage.png)
![Descripción de la imagen](images/3.png)
### 3. Docker Hub
```sh
docker tag mi-cv-vilela-imagen renevc/mi-cv-vilela-imagen
docker push renevc/mi-cv-vilela-imagen
```
![Descripción de la imagen](images/4.png)
![Descripción de la imagen](images/5.png)
### 4. Docker Compose

![Descripción de la imagen](images/6.png)
### 5. Despliegue
```sh
docker-compose up -d
```
La página web estará disponible en: [http://localhost:8585](http://localhost:8585)
![Descripción de la imagen](images/7.png)
![Descripción de la imagen](images/8.png)

### Verificar el Estado del Contenedor
```sh
docker ps
```

### Detener el Servicio
```sh
docker-compose down
```

## Notas
- Si realizas cambios en `index.html`, recuerda reconstruir y volver a subir la imagen a Docker Hub.
- Puedes ver los logs con:
```sh
docker logs <ID_DEL_CONTENEDOR>
```

🚀 Proyecto listo para ser ejecutado con Docker y Docker Compose.