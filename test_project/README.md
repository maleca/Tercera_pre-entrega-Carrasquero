Para poner en marcha este proyecto localmente en su computadora:

Configure el entorno de desarrollo de Python . Recomendamos utilizar un entorno virtual de Python.
Nota: Esto ha sido probado contra Django 3.1.2 (y puede que no funcione o sea "óptimo" para otras versiones).

Suponiendo que tiene la configuración de Python, ejecute los siguientes comandos (si está en Windows, puede usar pyo py -3en lugar de pythonpara iniciar Python):
pip3 install -r requirements.txt
python3 manage.py makemigrations
python3 manage.py migrate
python3 manage.py collectstatic
python3 manage.py test # Run the standard tests. These should all pass.
python3 manage.py createsuperuser # Create a superuser
python3 manage.py runserver
Abra un navegador http://127.0.0.1:8000/admin/ para abrir el sitio de administración
Cree algunos objetos de prueba de cada tipo.
Abra la pestaña para http://127.0.0.1:8000ver el sitio principal, con sus nuevos objetos.