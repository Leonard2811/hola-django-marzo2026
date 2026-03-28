# 🌍 Hola Mundo Django

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/)
[![Django](https://img.shields.io/badge/Django-4.2+-green.svg)](https://www.djangoproject.com/)
[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

Un proyecto simple y educativo de Django que demuestra la creación de un sitio web básico con páginas de inicio y acerca de. Perfecto para principiantes que quieren aprender los fundamentos de Django.

## ✨ Características

- 🏠 Página de inicio con mensaje de bienvenida
- ℹ️ Página "Acerca de" con información del proyecto
- 📱 Diseño responsivo con Bootstrap
- 🗂️ Estructura modular con apps de Django
- 🗃️ Base de datos SQLite integrada
- 🚀 Servidor de desarrollo fácil de usar

## 🛠️ Tecnologías Utilizadas

- **Backend**: Django 4.2+
- **Frontend**: HTML5, CSS3, Bootstrap 5
- **Base de Datos**: SQLite3
- **Lenguaje**: Python 3.8+
- **Entorno Virtual**: venv

## 📋 Requisitos Previos

Antes de comenzar, asegúrate de tener instalado:

- Python 3.8 o superior
- pip (gestor de paquetes de Python)
- Git (opcional, para clonar el repositorio)

## 🚀 Instalación y Configuración

Sigue estos pasos para configurar el proyecto en tu máquina local:

### 1. Clona el Repositorio

```bash
git clone https://github.com/tu-usuario/hola-mundo-django.git
cd hola-mundo-django
```

### 2. Crea un Entorno Virtual

```bash
python -m venv .venv
```

### 3. Activa el Entorno Virtual

**En Windows:**
```bash
.venv\Scripts\activate
```

**En macOS/Linux:**
```bash
source .venv/bin/activate
```

### 4. Instala las Dependencias

```bash
pip install -r requirements.txt
```

### 5. Realiza las Migraciones de la Base de Datos

```bash
python manage.py migrate
```

### 6. Ejecuta el Servidor de Desarrollo

```bash
python manage.py runserver
```

¡Listo! El servidor estará corriendo en `http://127.0.0.1:8000/`

## 📖 Uso

Una vez que el servidor esté ejecutándose, puedes acceder a las siguientes páginas:

- **Página de Inicio**: [http://127.0.0.1:8000/](http://127.0.0.1:8000/)
  - Muestra un mensaje de bienvenida y una breve descripción del proyecto.

- **Página Acerca de**: [http://127.0.0.1:8000/about/](http://127.0.0.1:8000/about/)
  - Proporciona información detallada sobre el proyecto y sus características.

## 📁 Estructura del Proyecto

```
hola_mundo_django/
├── db.sqlite3                    # Base de datos SQLite
├── manage.py                     # Script de gestión de Django
├── requirements.txt              # Dependencias del proyecto
├── base_proyect/                 # Configuración principal del proyecto
│   ├── __init__.py
│   ├── asgi.py                   # Configuración ASGI
│   ├── settings.py               # Configuración de Django
│   ├── urls.py                   # URLs principales del proyecto
│   ├── wsgi.py                   # Configuración WSGI
│   └── __pycache__/              # Archivos compilados
├── pages/                        # App de páginas
│   ├── __init__.py
│   ├── admin.py                  # Configuración del admin
│   ├── apps.py                   # Configuración de la app
│   ├── models.py                 # Modelos de datos
│   ├── tests.py                  # Tests de la app
│   ├── urls.py                   # URLs de la app
│   ├── views.py                  # Vistas de la app
│   ├── __pycache__/              # Archivos compilados
│   └── migrations/               # Migraciones de la base de datos
│       ├── __init__.py
│       └── __pycache__/
└── templates/                    # Plantillas HTML
    ├── _base.html                # Plantilla base
    ├── home.html                 # Página de inicio
    └── about.html                # Página acerca de
```

## 🔧 Configuración Adicional

### Variables de Entorno

Para entornos de producción, considera configurar variables de entorno para:

- `SECRET_KEY`: Clave secreta de Django
- `DEBUG`: Modo de depuración (False en producción)
- `ALLOWED_HOSTS`: Hosts permitidos

### Personalización

Puedes personalizar el proyecto editando:

- `base_proyect/settings.py`: Configuración general
- `templates/*.html`: Apariencia de las páginas
- `pages/views.py`: Lógica de las vistas

## 🧪 Tests

Para ejecutar los tests incluidos:

```bash
python manage.py test
```

## 📦 Despliegue

Para desplegar en producción:

1. Configura un servidor web (Apache/Nginx)
2. Usa un servidor WSGI (Gunicorn/uWSGI)
3. Configura una base de datos más robusta (PostgreSQL/MySQL)
4. Establece variables de entorno apropiadas
5. Ejecuta migraciones y collectstatic

## 🤝 Contribución

¡Las contribuciones son bienvenidas! Para contribuir:

1. Fork el proyecto
2. Crea una rama para tu feature (`git checkout -b feature/AmazingFeature`)
3. Commit tus cambios (`git commit -m 'Add some AmazingFeature'`)
4. Push a la rama (`git push origin feature/AmazingFeature`)
5. Abre un Pull Request

## 📝 Licencia

Este proyecto está bajo la Licencia MIT. Ver el archivo [LICENSE](LICENSE) para más detalles.

## 👨‍💻 Autor

**Tu Nombre**
- GitHub: [@tu-usuario](https://github.com/tu-usuario)
- Email: tu-email@example.com

## 🙏 Agradecimientos

- Django Project por el excelente framework
- Bootstrap por los componentes CSS
- Comunidad de Python por el soporte continuo

---

⭐ Si te gusta este proyecto, ¡dale una estrella en GitHub!

*Última actualización: Marzo 2026*