# 🚀 Hola Mundo Django

[![Django Version](https://img.shields.io/badge/Django-6.0.3-green.svg)](https://www.djangoproject.com/)
[![Python Version](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/)
[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

Un proyecto de ejemplo simple para demostrar los fundamentos de Django. Este es un "Hola Mundo" básico que muestra cómo crear una aplicación web con Django, incluyendo vistas basadas en plantillas, configuración de proyecto y estructura de archivos.

## 📋 Descripción

Este proyecto es una introducción práctica a Django, el framework web de Python. Incluye una página de inicio simple que muestra un mensaje de bienvenida, demostrando conceptos clave como:

- Configuración de un proyecto Django
- Creación de aplicaciones Django
- Uso de vistas basadas en clases (TemplateView)
- Plantillas HTML
- Estructura de directorios estándar de Django

## ✨ Características

- 🏠 Página de inicio personalizable
- 📱 Diseño responsivo básico
- 🔧 Configuración de desarrollo lista para usar
- 🗄️ Base de datos SQLite integrada
- 📦 Dependencias gestionadas con pip

## 🛠️ Tecnologías Utilizadas

- **Backend**: Django 6.0.3
- **Base de Datos**: SQLite 3
- **Lenguaje**: Python 3.8+
- **Frontend**: HTML5, CSS3 (básico)

## 📦 Instalación

### Prerrequisitos

- Python 3.8 o superior instalado en tu sistema
- Git (opcional, para clonar el repositorio)

### Pasos de Instalación

1. **Clona o descarga el proyecto**
   ```bash
   git clone https://github.com/tu-usuario/hola-mundo-django.git
   cd hola-mundo-django
   ```

2. **Crea un entorno virtual** (recomendado)
   ```bash
   python -m venv venv
   # En Windows:
   venv\Scripts\activate
   # En macOS/Linux:
   source venv/bin/activate
   ```

3. **Instala las dependencias**
   ```bash
   pip install -r requirements.txt
   ```

4. **Realiza las migraciones de la base de datos**
   ```bash
   python manage.py migrate
   ```

5. **Ejecuta el servidor de desarrollo**
   ```bash
   python manage.py runserver
   ```

6. **Accede a la aplicación**
   
   Abre tu navegador web y ve a: `http://127.0.0.1:8000/`

## 🚀 Uso

### Ejecutar el servidor

```bash
python manage.py runserver
```

### Crear un superusuario (opcional, para acceder al admin)

```bash
python manage.py createsuperuser
```

Sigue las instrucciones para crear un usuario administrador.

### Acceder al panel de administración

Una vez creado el superusuario, ve a: `http://127.0.0.1:8000/admin/`

## 📁 Estructura del Proyecto

```
hola_mundo_django/
├── base_proyect/           # Configuración principal del proyecto
│   ├── __init__.py
│   ├── asgi.py
│   ├── settings.py         # Configuraciones de Django
│   ├── urls.py             # URLs principales del proyecto
│   ├── wsgi.py
│   └── __pycache__/
├── pages/                  # Aplicación Django
│   ├── __init__.py
│   ├── admin.py
│   ├── apps.py
│   ├── models.py           # Modelos de datos
│   ├── tests.py
│   ├── urls.py             # URLs de la aplicación
│   ├── views.py            # Vistas de la aplicación
│   ├── __pycache__/
│   └── migrations/         # Migraciones de base de datos
│       ├── __init__.py
│       └── __pycache__/
├── templates/              # Plantillas HTML
│   └── home.html
├── db.sqlite3              # Base de datos SQLite
├── manage.py               # Script de gestión de Django
└── requirements.txt        # Dependencias del proyecto
```

## 🔧 Configuración

### Variables de Entorno

Para producción, considera configurar estas variables:

- `DEBUG=False`
- `SECRET_KEY` (genera una nueva clave secreta)
- `ALLOWED_HOSTS` (lista de hosts permitidos)

### Base de Datos

Por defecto, usa SQLite. Para cambiar a otra base de datos, modifica `settings.py`:

```python
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.postgresql',  # o mysql, etc.
        'NAME': 'tu_base_datos',
        'USER': 'tu_usuario',
        'PASSWORD': 'tu_contraseña',
        'HOST': 'localhost',
        'PORT': '5432',
    }
}
```

## 🧪 Pruebas

Ejecuta las pruebas con:

```bash
python manage.py test
```

## 📝 Personalización

### Cambiar el contenido de la página

Edita `templates/home.html` para modificar el contenido de la página de inicio.

### Agregar nuevas páginas

1. Crea nuevas vistas en `pages/views.py`
2. Agrega URLs en `pages/urls.py`
3. Crea plantillas en `templates/`

## 🤝 Contribución

¡Las contribuciones son bienvenidas! Para contribuir:

1. Haz un fork del proyecto
2. Crea una rama para tu feature (`git checkout -b feature/nueva-funcionalidad`)
3. Commit tus cambios (`git commit -am 'Agrega nueva funcionalidad'`)
4. Push a la rama (`git push origin feature/nueva-funcionalidad`)
5. Abre un Pull Request

## 📄 Licencia

Este proyecto está bajo la Licencia MIT. Ver el archivo [LICENSE](LICENSE) para más detalles.

## 📞 Contacto

Si tienes preguntas o sugerencias, no dudes en contactarme:

- Email: tu-email@example.com
- GitHub: [tu-usuario](https://github.com/tu-usuario)

---

⭐ Si te gusta este proyecto, ¡dale una estrella en GitHub!

Hecho con ❤️ usando Django