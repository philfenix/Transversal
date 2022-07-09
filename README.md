# Transversal
mascotas

instalacion para ejecutar el programa

1 -Instala Django

pip install django
2 -Instala oracle db

pip install cx_oracle
3 -Instala Crispy Forms

pip install django-crispy-forms

4 -Acceder a sqlplus y crear usuario

alter session set "_ORACLE_SCRIPT"=true; 

create user django identified by django;

grant connect, resource to django;
alter user django default tablespace users quota unlimited on users;

ejecutar pillow ( pip install pillow )

5 - Ejecutar migraciones.

python manage.py migrate
python manage.py makemigrations

("python manage.py makemigrations") al parecer no es necesario

6- Crear superusuario

python manage.py createsuperuser

7- Inicia proyecto

python manage.py runserver

