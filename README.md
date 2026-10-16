Práctica 6: Servidor Web Nginx con Docker Compose

Asignatura: Electiva 2

Autor: Franciel

📌 Descripción del Proyecto

Este repositorio contiene la configuración e infraestructura como código necesaria para desplegar un servidor web Nginx localmente mediante Docker Compose.

El proyecto demuestra el uso de volúmenes persistentes y de solo lectura (bind mounts), vinculando un directorio local con los archivos estáticos dentro del contenedor Nginx sin necesidad de reconstruir la imagen.

📂 Estructura del Directorio

.
├── src/
│   └── index.html          # Página web estática principal
├── docker-compose.yml      # Declaración del servicio, puertos y volúmenes
├── .gitignore              # Archivos y carpetas excluidas del control de versiones
└── README.md               # Documentación del proyecto


## Tecnologías Utilizadas

Docker & Docker Compose: Orquestación y contenedorización del servicio.

Nginx (nginx:alpine): Servidor HTTP ligero y de alto rendimiento.

HTML5: Archivo base de visualización web.

Git & GitHub: Control de versiones y publicación del repositorio.

## Despliegue y Ejecución

Prerrequisitos

Tener instalado Docker Desktop (con WSL 2 habilitado en Windows).

Tener instalado Git.

Pasos para levantar el servicio

## Clonar el repositorio:

git clone https://github.com/francielgod/nginx-docker-practica6-Electiva2.git
cd nginx-docker-practica6-Electiva2


Iniciar el contenedor en segundo plano:

docker compose up -d


Verificar el estado del contenedor:

docker compose ps


Acceder a la aplicación:
Abre un navegador web e ingresa a:

http://localhost:8080


🛑 Detener el Servicio

Para detener y remover los contenedores y redes asociadas creadas por Docker Compose:

docker compose down
