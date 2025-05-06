# 🌐 Web Personal - Portafolio en Django

Este es un proyecto de sitio web personal creado con **Python** y **Django**, que funciona como un portafolio online. Contiene varias secciones como:

- 🏠 **Portada**
- 🙋‍♀️ **Sobre mí**
- 💼 **Portfolio**
- 📬 **Contacto**

Está diseñado con plantillas **HTML** personalizadas y usa una base de datos **SQLite3** para manejar los datos.

---

## 🚀 Tecnologías utilizadas

- **Python 3**
- **Django**
- **HTML / CSS**
- **SQLite3**
- **Visual Studio Code**

---

## 🛠️ Cómo ejecutar este proyecto en local

1. Clona este repositorio:
    ```bash
    git clone https://github.com/Mai-de-jerez/sitio_web_django.git
    cd sitio_web_django
    ```

2. Crea y activa un entorno virtual (opcional pero recomendado):
    ```bash
    python -m venv venv
    source venv/bin/activate    # en Linux/Mac
    venv\Scripts\activate       # en Windows
    ```

3. Instala las dependencias:
    ```bash
    pip install -r requirements.txt
    ```

4. Ejecuta el servidor de desarrollo:
    ```bash
    python manage.py runserver
    ```

5. Abre tu navegador y entra a:
    ```
    http://127.0.0.1:8000/
    ```

---

## 📁 Estructura general del proyecto
```
webpersonal/                 
│
├── manage.py               
├── db.sqlite3              
├── requirements.txt       
├── README.md                
├── webpersonal/            
│   ├── __init__.py          
│   ├── settings.py         
│   ├── urls.py              
│   ├── wsgi.py              
│   └── asgi.py              
│
├── portfolio/                
│   ├── migrations/
│   │   ├── __init__.py
│   │   ├── 0001_initial.py
│   │   └── 0002_alter_projects_options_project_link_and_more.py
│   │
│   ├── templates/          
│   │   └── portfolio/
│   │            └── portfolio.html
│   ├── init.py             
│   ├── admin.py             
│   ├── apps.py           
│   ├── models.py
│   ├── tests.py
│   └── views.py
│
├── core/
│   ├── migrations/
│   │    └── __init__.py
│   ├── static/
│   │    └── core/
│   │           ├── css/
│   │           │    └── clean-blog.min.css
│   │           ├── img/
│   │           │    ├── about-bg.jpg
│   │           │    ├── contact-bg.jpg
│   │           │    ├── home-bg.jpg
│   │           │    ├── mai.jpg
│   │           │    └── portfolio-bg.jpg
│   │           ├── js/
│   │           │    ├── clean-blog.js
│   │           │    ├── clean-blog.min.js
│   │           │    ├── contact_me.js
│   │           │    ├── contact_me.min.js
│   │           │    ├── jqBootstrapValidation.js
│   │           │    └── jqBootstrapValidation.min.js
│   │           │
│   │           └── vendor/
│   │                ├── boostrap/
│   │                │       ├── css/...
│   │                │       └── js/...
│   │                ├── font-awesome/
│   │                │    ├── css/...
│   │                │    ├── fonts/...
│   │                │    ├── less/...
│   │                │    └── scss/...
│   │                └── jquery/...
│   ├── templates/
│   │    └── core/
│   │          ├── about.html
│   │          ├── base.html        
│   │          ├── contact.html
│   │          └── home.html
│   │              
│   ├── init.py             
│   ├── admin.py             
│   ├── apps.py           
│   ├── models.py
│   ├── tests.py
│   └── views.py
│    
│     
│   
└── media/               
    └── projects/
            ├── cierre.jpg
            └── envase.jpg
```

---

### Descripción de las aplicaciones:

- **`webpersonal/`**: App principal que contiene los archivos de configuración de Django, como `settings.py`, `urls.py` y otros archivos de configuración del proyecto.

- **`portfolio/`**: Una app que maneja la parte de los proyectos, donde se almacenan los detalles de cada proyecto, como nombre, descripción, y link.

- **`core/`**: Contiene archivos comunes y reutilizables, como plantillas HTML, archivos estáticos (CSS, JS) y otras configuraciones generales del sitio.

- **`media/`**: Carpeta donde se almacenan los archivos subidos por el usuario, como imágenes de los proyectos.

---

### 1. Crear un superusuario (usuario administrador)

Para acceder al panel de administración, primero necesitas crear un superusuario. Abre una terminal y navega a la carpeta de tu proyecto Django, luego ejecuta el siguiente comando:

```bash
python manage.py createsuperuser
```
### 2. Ejecuta el servidor de desarrollo

Si aún no lo has hecho, ejecuta el servidor de desarrollo con:

```bash
python manage.py runserver
```
### 3. Accede al panel de administración

Abre tu navegador y ve a la URL:

```url
http://127.0.0.1:8000/admin/
```

### 4. Añadir proyectos

- En el panel de administración, busca y haz clic en la sección **"Proyectos"**.
- Haz clic en **"Añadir"** en la parte superior derecha para crear un nuevo proyecto.
- Completa los campos (nombre, descripción, enlaces, imágenes, etc.) y guarda los cambios.


### 5. Ver los proyectos en el sitio web

- Después de agregar los proyectos desde el panel de administración, se mostrarán automáticamente en la sección **Proyectos** de tu portafolio online.

---

## 📩 Contacto

Creado por **[María del Carmen Martín Rodríguez]**  
GitHub: [https://github.com/Mai-de-jerez/sitio_web_django](https://github.com/tu_usuario)