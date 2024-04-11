# Administrador de Tareas con Flask

## Descripción
Este proyecto es una aplicación web simple creada con Flask que permite a los usuarios administrar una lista de tareas. Los usuarios pueden agregar nuevas tareas, editar tareas existentes y eliminar tareas. La aplicación utiliza SQLAlchemy para interactuar con una base de datos SQLite para almacenar las tareas.

## Funcionalidades
- Agregar nueva tarea
- Editar tarea existente
- Eliminar tarea
- Ver lista de tareas

## Estructura del Proyecto
- `app.py`: Este archivo contiene la lógica principal de la aplicación. Aquí se definen las rutas y las funciones que manejan las solicitudes del cliente.
- `templates/`: Este directorio contiene las plantillas HTML utilizadas para renderizar las páginas web.
- `static/`: Este directorio contiene archivos estáticos como CSS, JavaScript e imágenes.

## Funciones Principales en `app.py`
- `index()`: Esta función maneja la ruta principal `/` y muestra la lista de tareas en la página principal.
- `add_task()`: Esta función maneja la ruta `/add` y permite a los usuarios agregar una nueva tarea a la lista.
- `edit_task(id)`: Esta función maneja la ruta `/edit/<id>` y permite a los usuarios editar una tarea existente.
- `delete_task(id)`: Esta función maneja la ruta `/delete/<id>` y permite a los usuarios eliminar una tarea existente.
- Otros métodos y funciones: En `app.py` también pueden incluirse otras funciones auxiliares que manejan la interacción con la base de datos, la validación de datos, etc.

## Descripción de Funciones
- `index()`: Esta función consulta todas las tareas de la base de datos utilizando SQLAlchemy y las pasa a la plantilla `index.html` para ser renderizadas.
- `add_task()`: Esta función verifica si se envió un formulario con los datos de una nueva tarea, la agrega a la base de datos y redirige al usuario de vuelta a la página principal.
- `edit_task(id)`: Esta función obtiene la tarea correspondiente al `id` proporcionado, permite al usuario editar sus detalles y actualiza la base de datos con los nuevos datos.
- `delete_task(id)`: Esta función elimina la tarea correspondiente al `id` proporcionado de la base de datos.

## Requisitos previos
- Python 3.x
- pip

## Instalación
1. Clona el repositorio o descarga el código fuente.
2. Navega hasta el directorio del proyecto.
3. Crea un entorno virtual:
   python3 -m venv venv
4. Activa el entorno virtual:
   - En Windows:
     venv\Scripts\activate
   - En macOS/Linux:
     source venv/bin/activate

5. Instala las dependencias:
   pip install -r requirements.txt

## Uso
1. Ejecuta la aplicación:
   python app.py
2. Abre tu navegador web y ve a `http://localhost:5000` para acceder a la aplicación.

## Créditos
Este proyecto fue creado por Yissell Camila Arciniegas.
