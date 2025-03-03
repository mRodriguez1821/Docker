# MinIO con Docker Compose

Este proyecto configura un servidor **MinIO** usando Docker Compose, proporcionando un almacenamiento de objetos compatible con S3.

## 📦 Servicios

- **MinIO**: Servicio principal de almacenamiento de objetos.
  - Expone el puerto `9000` para la API de MinIO.
  - Expone el puerto `9090` para la consola de administración.
  - Usa credenciales de acceso definidas en variables de entorno.
  - Almacena datos en un volumen persistente llamado `minio_data`.

## 🚀 Instalación y Uso

### 1️⃣ Requisitos previos
Asegúrate de tener instalado:
- [Docker](https://www.docker.com/get-started)
- [Docker Compose](https://docs.docker.com/compose/install/)

### 2️⃣ Levantar el servicio
Ejecuta el siguiente comando en la terminal:

```sh
docker-compose up -d
```

### 3️⃣ Acceder a MinIO
- **API de MinIO**: [http://localhost:9000](http://localhost:9000)
- **Consola web de MinIO**: [http://localhost:9090](http://localhost:9090)
- **Credenciales por defecto**:
  - Usuario: `username`
  - Contraseña: `administrator`

### 4️⃣ Detener el servicio
Para apagar los contenedores y eliminar la red:

```sh
docker-compose down
```

## 📌 Notas
- Se usa la imagen oficial `quay.io/minio/minio`.
- Los datos se almacenan en el volumen `minio_data` para persistencia.
- Puedes cambiar las credenciales modificando las variables de entorno en `docker-compose.yml`.

## 📄 Licencia
Este proyecto está bajo la licencia **MIT**.

