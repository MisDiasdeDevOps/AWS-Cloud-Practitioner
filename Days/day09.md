
prueba
# Comandos útiles en la terminal de Linux (Parte 2)

Índice

1. Escenario
2. El comando Curl
3. El comando Jq
4. Combinación de uso de ambos comandos



# Obtener datos desde un web service

La terminal de Linux tiene tanta versatilidad y potencia que nos permite vincularla con un Webservice, obtener datos de allí y procesarlos con propósitos tales como agregarlo a archivos en nuestro servidor, modificarlos y republicarlos.
Las opciones son muy variadas, como, por ejemplo, obtener un JSON desde una URL externa, procesar su contenido, obtener el o los atributos que nos interesen y en función de ello, crear nuevos archivos, insertarlos en una base de datos.


![Screenshot_425](https://user-images.githubusercontent.com/96561825/170134850-398076fd-1eb6-434b-b015-c619068b4af2.png)


# curl - Aspectos técnicos
Es un comando disponible en la mayoría de los sistemas basados ​en Unix. Es una abreviatura de «Client URL». Los comandos de Curl están diseñados para funcionar como una forma de verificar la conectividad a las URL y como una gran herramienta para transferir datos. 

El comando tiene una amplia compatibilidad con los protocolos más usados, podemos verlos en la columna de abajo.
![Screenshot_426](https://user-images.githubusercontent.com/96561825/170135030-81b7fe08-5052-4dd9-9edf-3a17f7aebb9a.png)


# curl - Sintaxis básica
El uso de este modificador puede extenderse a procesar descargas:
![Screenshot_427](https://user-images.githubusercontent.com/96561825/170145409-dae984d4-58b1-46d4-9397-c320fbdb8327.png)

Descarga la iso de la URL de referencia y la nombrara ubuntu.iso
![Screenshot_428](https://user-images.githubusercontent.com/96561825/170145419-df3722e0-da62-41ff-934d-c8a6c2894d33.png)

En este caso, no renombramos el archivo de destino (con el modificador -O) y además, permitimos la continuidad de la descarga con el modificador -C.

# curl - Encabezados y verificaciones

El modificador -v nos permite verificar la conectividad hacia un sitio remoto.
![Screenshot_429](https://user-images.githubusercontent.com/96561825/170145555-12eafeda-c60c-48a7-b242-6cecbbfd9ccf.png)

Nos brindará además del contenido, datos como IP de destino, protocolos de seguridad y certificados utilizados.
![Screenshot_431](https://user-images.githubusercontent.com/96561825/170145566-8636dbd3-d5ee-46e4-94f4-a6f1f7a9bef0.png)

Y con el modificador -I, nos muestra todos los encabezados de la solicitud, tales como ruta por defecto, publicador web, etcétera.

# curl - Contenido JSON

Viendo todas las opciones brindadas, nos podemos imaginar lo útil de este comando con el propósito de obtener el contenido en formato JSON desde un endpoint que lo entregue en dicho formato, por ejemplo, la API de OpenStreetMap, la cual nos devuelve una dirección pasándole las coordenadas, con la siguiente URL: https://nominatim.openstreetmap.org/reverse.php?lat=-34.60378&lon=-58.38161&zoom=18&format=jsonv2

![Screenshot_434](https://user-images.githubusercontent.com/96561825/170145694-17fc801a-6d8e-4bed-a43c-5643beabdb39.png)


Allí estamos guardando en el archivo resultado .json lo obtenido en el web service, notemos el detalle de colocar la URL entre comillas simples o dobles.











#
#
#
#
#
##
#
#
#
##
#


See you on [Day 10](day10.md).
