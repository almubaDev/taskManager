# Task Manager

Task Manager es una aplicación de gestión de tareas construida con Django Framework. Proporciona un conjunto completo de operaciones CRUD (Crear, Leer, Actualizar, Eliminar) para organizar tus tareas diarias. Además, incluye etiquetas de prioridad y tipos para una mejor organización.

## Funcionalidades

- **CRUD Completo:** Gestiona tus tareas con operaciones básicas de Crear, Leer, Actualizar y Eliminar.
- **Etiquetas de Prioridad:** Asigna etiquetas de prioridad a tus tareas (Alta, Media, Baja) para destacar la importancia.
- **Etiquetas de Tipo:** Organiza tus tareas por categorías como Hogar, Trabajo, Deporte, Estudio, etc.

## Instalación

1. Clona el repositorio: `git clone https://github.com/tuusuario/task-manager.git`
2. Instala las dependencias: `pip install -r requirements.txt`
3. Realiza las migraciones: `python manage.py migrate`

### Nota
Si deseas cargar tus propias etiquetas, puedes modificar el archivo data.json antes de ejecutar `python manage.py loaddata .\data.json`, junto con ello modififica los template 'templates/task/partials/filterTag.html' haciendo coincidir el nombre de la etiqueta con el parámetros de la URL que es el pk de la etiqueta almacenada en la base de datos. Si deseas expandir la cantidad de prioridades y etiquetas tambien deberas modificar la vista 'task.views.task' para que coincida con tus necesidades.

4. Carga etiquetas y etiquetas de prioridad: `python manage.py loaddata .\data.json`
5. Inicia el servidor: `python manage.py runserver`

## Uso

1. Ejecuta la aplicación Django: `python manage.py runserver`
2. Abre tu navegador y ve a `http://localhost:8000`
3. Explora las funciones de Task Manager y gestiona tus tareas.



## Contribución

¡Contribuciones son bienvenidas! Si encuentras algún problema o tienes ideas para mejorar la aplicación, sigue estos pasos:

1. Crea un nuevo *issue* explicando el problema o la mejora.
2. Haz un *fork* del repositorio.
3. Crea una nueva rama para tu contribución: `git checkout -b feature/nueva-funcion`
4. Realiza los cambios y haz *commit*: `git commit -m "Añadir nueva función"`
5. Haz *push* a tu rama: `git push origin feature/nueva-funcion`
6. Crea un *pull request* en GitHub.

## Licencia

Este proyecto está bajo la Licencia MIT. Consulta el archivo [LICENSE](LICENSE) para más detalles.

