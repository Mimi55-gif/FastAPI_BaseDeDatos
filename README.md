# API de Gestión de Biblioteca con FastAPI y RDS

Este proyecto implementa una API RESTful para gestionar libros y usuarios, utilizando FastAPI y SQLModel, diseñada para ser desplegada en AWS EC2 con una base de datos administrada en Amazon RDS.

## Instalación Local

1. Clonar el repositorio:
   ```bash
   git clone <https://github.com/mateovivas453-dot/Fast-api-_-Base-de-Datos-1.git>
   cd Fastapi_BaseDeDatos
   ```

2. Crear y activar entorno virtual:
   ```bash
   python -m venv venv
   source venv/bin/activate  # Linux/Mac
   venv\Scripts\activate     # Windows
   ```

3. Instalar dependencias:
   ```bash
   pip install -r requirements.txt
   ```

4. Configurar variables de entorno:
   Crear un archivo `.env` basado en `.env.example` con tus credenciales de base de datos.

5. Ejecutar la aplicación:
   ```bash
   uvicorn app.main:app --reload
   ```

## Despliegue en AWS

La aplicación está diseñada para correr en una instancia EC2 conectándose a una instancia RDS PostgreSQL.

### Variables Requeridas:
- `DATABASE_URL`: Cadena de conexión a la base de datos RDS.

### Documentación de la API:
Una vez desplegada, la documentación interactiva estará disponible en:
`http://<IP_PUBLICA_EC2>:8000/docs`
