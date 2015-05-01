# Django

##Comandos utiles
Crear superusuario para acceder a localhost:8000/admin
>./manage.py createsuperuser

Arranca el servidor por defecto en localhost:8000
``` ./manage.py runserver```

Campos para los modelos
>https://docs.djangoproject.com/en/1.8/ref/models/fields/#durationfield

Windows:

1. Descargar Visual Studio 2013 || 2015
2. Instalar con la opcion: ```Web developer tools```
3. Descargar de http://pytools.codeplex.com/releases 
el archivo ```PTVS 2.2 RC VS 2013.msi o 2015```
4.  Instalar python 2.7 ??
5. Nuevo Projecto django
6. Seleccionar -> Virtual Environment
7. Project -> Django sync DB
8. Crear nuevo SuperUsuario
9. Run


##Snipets
###Vistas
Crear vista
app/views.py
```python
from django.http import HttpResponse
def vista(request):
	return HttpRequest("Hola Mundo")
```

Enlazar url con la vista
project/urls.py
```python
url(r'^url/para/la/vista/', 'app.views.vista'),
url(r'^principal/, 'musicos.views.principal'),
```

