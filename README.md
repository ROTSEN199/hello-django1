# hello-django1

1- Vamos a entrar al directorio donde creamos nuestro entorno y accedemos a esa carpeta.
chacamos que nuetro equipo tenga la version de python mas reciente.
tenemos que poner el siguiente comando. (Nombre proyecto)\Scripts\activate
![image](https://user-images.githubusercontent.com/95454472/178560931-97c1aa88-6abb-4687-89f5-68226418d18f.png)
2- vamos a instalar Django dentro de python con este comando > python -m pip install django~=4.0.0 
![image](https://user-images.githubusercontent.com/95454472/178563933-dc8d3c52-3471-461e-95b1-3936c387132e.png)
3- crearemos el esqueleto de nuestra aplicacion con el siguiente comando > django-admin startproject (IntegradoraPV) //nombre del proyecto.
![image](https://user-images.githubusercontent.com/95454472/178566194-4603d214-085a-4114-85fb-b5903e2464d5.png)
4- ingresamos a la carpeta que se creo con el nombre que le pusimos al esqueleto.
![image](https://user-images.githubusercontent.com/95454472/178566533-0d13d4a3-5a4f-42b4-9e6f-d245addeebd9.png)
5- migramos los datos que tenemos del esqueleto con el comando: > python manage.py migrate
![image](https://user-images.githubusercontent.com/95454472/178567058-b29b3a36-9b1c-4065-8625-fcb3bdf75ad6.png)
6- se nos genrara la siguueinte estrutura de documentos.
![image](https://user-images.githubusercontent.com/95454472/178576593-09b45b98-610d-489d-8f09-c8e4fd9651ba.png)
7- Ejecutar la instrucción en la terminal > python3 manage.py startapp catstudent
![image](https://user-images.githubusercontent.com/95454472/178577177-d9ecd138-e486-443e-ba96-63bd51bfcf3e.png)
8- Abriremos nuetra carpeta de todo el pryecto con visual estudios y nos parecera algo como esto.
![image](https://user-images.githubusercontent.com/95454472/178577556-1a057cff-577f-48e9-8e90-4bfbb1e5b8aa.png)
9- Modifique catstudent/views.py para que coincida con el siguiente código. de esta manera.
![image](https://user-images.githubusercontent.com/95454472/178578253-a2491bf3-1c75-4720-be7e-cadbc4639295.png)
10- Cree un archivo, catstudent/urls.py, con el contenido a continuación de esta forma.
![image](https://user-images.githubusercontent.com/95454472/178578445-2f627908-de85-4096-baba-dd3fc96952d7.png)
11-agregamos las siguientes lineas de codigo.
![image](https://user-images.githubusercontent.com/95454472/178578802-99d067eb-d8f3-4ca9-b895-4e0ac0dd806a.png)
12- Abra IntegrdoraPV/urls.py y modifícalo para que coincida con el siguiente código.
![image](https://user-images.githubusercontent.com/95454472/178579163-45b0078e-37b1-4be6-8fde-dea41019cb41.png)
13- Registrar la aplicación
Abre el fichero de ajustes del proyecto myapliweb/myapliweb/settings.py y encuentra la definición de la lista INSTALLED_APPS. Añade a continuación una nueva línea al final de la lista, como se muestra en negrilla abajo.
![image](https://user-images.githubusercontent.com/95454472/178579874-52d15f00-5dab-4afc-8713-4030a77daef6.png)
14- Especificaciòn de la base de datos
Usaremos la base de datos SQLite para este ejemplo, porque no esperamos que se requiera un montón de accesos concurrentes en una base de datos de demostración, y también ¡porque no requiere trabajo adicional para ponerla en marcha! Puedes ver cómo está configurada en settings.py (más información también se incluye abajo):
![image](https://user-images.githubusercontent.com/95454472/178580417-15fdf008-a74f-4832-bca2-813a67db8ba2.png)
![image](https://user-images.githubusercontent.com/95454472/178580495-753d88b1-4529-4a92-ad2d-dd40ea4c4c4b.png)
15-El fichero settings.py se usa para configurar muchos otros ajustes, pero en este punto probablemente sólo querrás cambiar la TIME_ZONE — ésta debería ser igual a una cadena de la Lista de base de datos tz de time zones.
![image](https://user-images.githubusercontent.com/95454472/178580654-111928db-2fab-4b20-8b2a-0847fdcb3183.png)
16- Salvar los archivos y ejecutar la aplicación >python3 manage.py runserver
Ingresa la URL http://127.0.0.1:8000/student
![image](https://user-images.githubusercontent.com/95454472/178580874-1f7f86e3-9c64-4d04-bd1b-faebd9b25adc.png)



