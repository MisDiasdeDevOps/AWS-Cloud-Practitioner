
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

# jq - Aspectos técnicos

JSON es un formato de datos estructurados ampliamente utilizado que se utiliza normalmente en la mayoría de las API y servicios de datos modernos. Es
particularmente popular en aplicaciones web debido a su naturaleza liviana y compatibilidad con JavaScript.

Desafortunadamente, shells como Bash no pueden interpretar y trabajar con JSON directamente . Esto significa que trabajar con JSON a través de la línea de comando puede ser engorroso y implica la manipulación de texto utilizando una combinación de herramientas como sed y grep.

Allí es donde aparece jq, un potente procesador JSON para la consola.


# jq - Sintaxis básica

jq se basa en el concepto de filtros que funcionan sobre un flujo de JSON. Cada filtro toma una entrada y emite JSON a la salida estándar.

Tomando el archivo json obtenido con curl, una ejecución sencilla de jq nos devuelve todo el contenido del JSON.

![Screenshot_435](https://user-images.githubusercontent.com/96561825/170146015-09b2f38f-ef49-4a66-b534-6be31ba730fd.png)

Como vemos, no vamos a acceder a ningún atributo en especial, ya que con el modificador ‘.’ no se lo indicamos.

# jq - Accediendo a propiedades

Para poder acceder a una propiedad específica, es necesario indicarla luego del punto, con el nombre de la misma.

![Screenshot_436](https://user-images.githubusercontent.com/96561825/170146149-f3943ba3-8296-4a50-b2ab-6c83aac030a0.png)

En este caso, accederemos a la propiedad “display_name” del Json. Si queremos acceder a varias propiedades, las separamos por coma.

![Screenshot_437](https://user-images.githubusercontent.com/96561825/170146158-c81fd6d1-e6b7-4193-8d90-a70ed43780f1.png)

De esta manera, accedemos a “display_name” y “type”.
TIP: Si alguna propiedad tuviese un espacio en su nombre, debemos envolverla con comillas dobles.

# Combinar comandos con pipelines (|)

Para poder combinar el poder de curl con el recurso y la capacidad de proceso de jq, debemos combinarlo usando pipelines.

Para ello, vamos a realizar una introducción a una de las características más interesantes que tiene la terminal.

El pipeline o tubería es una función que permite utilizar la salida de un programa como entrada en otro.

El pipeline en Linux se representa con la barra vertical |, la cual dividirá los comandos. Por ejemplo, si nosotros queremos saber la IP de nuestro equipo, lo hacemos con la instrucción

![Screenshot_439](https://user-images.githubusercontent.com/96561825/170146353-9f4c87ee-0857-4f25-9ad9-cb133a423996.png)

Lo cual nos devolverá muchísimos datos (MAC, protocolos, direcciones IPv4 e IPv6), si quisiéramos filtrar dentro de ese texto por la cadena ‘192.168’, lo deberíamos llevar a un archivo y allí buscar con grep.

![Screenshot_441](https://user-images.githubusercontent.com/96561825/170146360-a7133dd5-4898-4dfd-bea9-74961833f4a4.png)

Pero es aquí en donde aparece la magia del pipe, ya que podemos combinar ambas sentencias en una.

Para ello, primero colocamos nuestra sentencia inicial, sabiendo que tipo de salida puede tener, separamos con el pipe | y colocamos la segunda sentencia.

![Screenshot_442](https://user-images.githubusercontent.com/96561825/170146452-7a76052e-cfcb-4c3c-9fbd-120f13ea51d3.png)

Allí el grep nos indicará la línea coincidente con “192.168”; nuestro pipe podría seguir aplicándose sin límites más allá de aquellos que imponga el sistema operativo, como, por ejemplo, cantidad de procesos en ejecución.

#
# Aplicar el pipeline con curl y jq

Conociendo el uso básico del pipe, vamos a aplicarlo a la obtención de datos externos y el parseo de una propiedad específica, la cual la guardaremos en un archivo. Nuestro comando tendrá 3 partes:

![Screenshot_443](https://user-images.githubusercontent.com/96561825/170146532-c2c22684-a642-4658-9b3f-9aaf16946dbc.png)

En este caso, vemos cómo la sentencia obtiene el JSON con curl, lo procesa con jq para obtener el display_name y el type y, finalmente, lo guarda en un archivo llamado consultapipe.txt

![Screenshot_444](https://user-images.githubusercontent.com/96561825/170146630-af88967d-b36b-4323-8715-9a93768236b0.png)

Fin

#
#
#
#
#


See you on [Day 10](day10.md).
