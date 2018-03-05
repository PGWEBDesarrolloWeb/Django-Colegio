# Django-Colegio
Desarrollado usando django 1.11 y python 2.7. Colegio es una aplicacion sencilla que permite administrar los cursos que imparte una institucion.
Para su correcto funcionamiento en imprescindible la creacion de un virtualenv, luego ejecutar el comando startproject con el nombre colegio_grobespa.
Recuerde crear el super usuario con el cual ingresara al administrador, se recomienda usar: python manage.py createsuperuser. user 'pedro' password 'REVELACION'.
La base de datos esta gestionada bajo postgresql, debe crear una nueva base de datos(desde pgadmin3), luego debe seleccionar la opcion restore y elegir el archivo adjunto .sql con esto la base estara creada.
En este punto de la instalacion por ahora no es necesario correr ningun comando startapp,todas las aplicaciones estan debidamente registradas en el archivo settings.py, luego de crear la base recuerde ejecutar los comandos makemigrations y migrate, con ello validara los modelos y la base entrara en funcionamiento.
Luego de ello debe instalar las siguientes dependencias usando el comando pip install:
*pip install bootstrapp-admin
*pip install django-bootstrap4
*pip install django-smart-selects
*pip install django-jquery
*pip install django-tables2
La aplicacion permite el ingreso, modificacion, consulta y eliminacion de datos de los siguientes modelos:
*Profesor
*Alumno
*Curso
*Especialidad
*Prueba
Cabe destacar los siguientes aspectos de la aplicacion:
El modelo Prueba contiene la calificacion de cada alumno referente a cada prueba de cada curso.
El modelo Especialidad define la especialidad de la cual proviene el curso impartido. Ejemplo: Especialidad=Programacion, Curso= Python Para Principiantes.
Un profesor puede ser asignado a uno o mas cursos.
Un estudiante puede estar inscrito en uno o mas cursos.
Prontamente seguiremos en el desarrollo de la aplicacion para mejorar el aspecto del frontend.
Reporte un bug o error al correo contacto@pgweb.com.ve
