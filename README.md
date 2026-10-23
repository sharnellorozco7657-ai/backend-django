# Backend Django

API backend desarrollada con Django para gestionar los datos de mi aplicación.

## Tecnologías

- Python 3.x
- Django
- SQLite (base de datos local de desarrollo)

## Estructura del proyecto

```
backend-django/
├── config/            # Configuración del proyecto (settings, urls, wsgi)
├── manage.py          # Comandos de Django
├── requirements.txt   # Dependencias de Python
├── .env.example       # Ejemplo de variables de entorno
└── .gitignore
```

## Requisitos previos

- Python 3.10 o superior (marca **Add Python to PATH** al instalar)
- Git

## Instalación

### 1. Clonar el repositorio

```bash
git clone https://github.com/sharnellorozco7657-ai/backend-django.git
cd backend-django
```

### 2. Crear el entorno virtual

```bash
python -m venv venv
```

### 3. Activar el entorno virtual

Windows:

```bash
venv\Scripts\activate
```

Mac / Linux:

```bash
source venv/bin/activate
```

### 4. Instalar las dependencias

```bash
pip install -r requirements.txt
```

### 5. Configurar las variables de entorno

```bash
copy .env.example .env
```

Contenido del `.env`:

```
SECRET_KEY=pon-aqui-una-clave-secreta
DEBUG=True
```

El archivo `.env` no se sube a GitHub. Nunca compartas tus claves.

### 6. Aplicar las migraciones

```bash
python manage.py migrate
```

### 7. Ejecutar el servidor

```bash
python manage.py runserver
```

Abre en el navegador: http://127.0.0.1:8000/

## Comandos útiles

| Comando | Para qué sirve |
|---|---|
| `python manage.py runserver` | Inicia el servidor de desarrollo. |
| `python manage.py makemigrations` | Genera migraciones tras cambiar los modelos. |
| `python manage.py migrate` | Aplica las migraciones. |
| `python manage.py createsuperuser` | Crea un usuario administrador. |

## Autor

GitHub: [@sharnellorozco7657-ai](https://github.com/sharnellorozco7657-ai)

Proyecto en desarrollo.