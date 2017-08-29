# MicrosoftFaceApi-Examples
Algunos ejemplos para poner en marcha los ejemplos publicos de Microsoft relacionados con su api cognitive


Ejemplo #1

El ejemplo mas simple esta disponible en la pagina de documentacion de microsoft sin embargo he creado una cuenta en github para su descarga y puesta en funcionamiento de forma más simple.

Github: https://github.com/miguelaav/MicrosoftFaceApi-Examples

cd face-api/

Es necesario agregar en el archivo detect_faces.py las lineas 8 y 18 para agregar la api key y el endpoint

subscription_key = '0def8ac866dc4fa39b43ce49b24ef568'

uri_base = 'https://westcentralus.api.cognitive.microsoft.com/face/v1.0'

Ejecutar la aplicación

python detect_faces.py

Ejemplo #2

Este ejemplo ejecuta una aplicación web en la que se permite levantar una aplicación web en la que se puede seleccionar una fotografica, determinar la emociones e indicar si la persona esta feliz o no.

Requerimientos tener instalado:
python 2.7
pip

$ cd happy-image-tester-django/

$ pip install -r requirements.txt

Para poder ejecutar la aplicación es importante agregar la key optenida en el archivo app/views.py linea 49

client = Client.emotion('be8c823e2e584fcfbb0ca1832e159401')

Ejecutar la aplicación

$ python manage.py runserver
