
# Ejercitación: Amazon S3


Índice

1. Objetivos

2. Crear el primer bucket de S3

3. Cargar un objeto en el bucket

4. Descargar un objeto

5. Eliminar los objetos y el bucket



#

# Objetivos

# Crear el primer Crear el primer buecket S3

Para crear un bucket necesitamos


1. Desde el portal de AWS Educate abrir la consola de AWS, navegar al menú de servicios y seleccionar S3.

2. Elegir “Create bucket” (Crear bucket).

3. En “Bucket name” (nombre del bucket), escribir un nombre compatible con DNS para el bucket. El nombre del bucket debe:

● Ser único en todo Amazon S3.

● Tener entre 3 y 63 caracteres.

● No contener caracteres en mayúsculas.

● Comenzar por una letra minúscula o un número.



4. En “Region” (Región), elegir la región de AWS en la que deseamos que se encuentre el bucket.

5. En “Configuración del bucket”, para bloquear el acceso público, se deben mantener establecidos los valores predeterminados.

6. Finalmente, elegir “Create bucket” (Crear bucket).

#
#


# Cargar un objeto


## Cargar un objeto

Después de crear un bucket en Amazon S3, podremos cargar un objeto en el mismo.

Un objeto puede ser cualquier clase de archivo: un archivo de texto, una fotografía, un video, etc.

Para cargar un objeto a un bucket se deben realizar los siguientes pasos: 

1. Abrir la consola de AWS mediante el portal de AWS y nos dirigimos al servicio de S3.

2. En la lista “Buckets”, seleccionar el nombre del bucket en el que deseemos cargar el objeto.

3. En la pestaña “Objects” (Objetos) del bucket, elegir “Upload” (Cargar).

4. En “Files and folders” (Archivos y carpetas), elegir “Add files” (Añadir archivos).

5. Seleccionar un archivo que cargar y luego “Open” (Abrir).

6. Seleccionar “Upload”.

#
#

# Descargar

## Descargar 4 un objeto

1. Abrimos la consola de AWS mediante el portal de AWS y nos dirigimos al servicio de S3. 

2. En la lista “Buckets” (Buckets), elegimos el nombre del bucket que contiene el objeto que deseemos descargar.

3. Podemos descargar un objeto de un bucket de S3 de cualquiera de las siguientes maneras:


● Seleccionamos el nombre del objeto que queramos descargar. En la sección de la página “Overview” (Información general), seleccionamos el objeto y, en el menú
“Actions” (Acciones), elegimos “Download” (Descargar) —o “Download as” (Descargar como) en caso de que deseemos descargar el objeto en una carpeta concreta—.

● Elegimos el objeto que deseamos descargar y, a continuación, en el menú “Object actions” (Acciones de objeto), seleccionamos “Download” (Descargar) —o
“Download as” (Descargar como) en caso de que deseemos descargar el objeto en una carpeta concreta—.

● En caso de que deseemos descargar una versión específica del objeto, seleccionamos su nombre y elegimos la pestaña “Versions” (Versiones) y, a continuación, en el menú “Actions” (Acciones) presionamos “Download” (Descargar) —o “Download as” (Descargar como) en caso de que desee descargar el objeto en una carpeta concreta—.

#
#

# Eliminar los 5 objetos y el bucket


Si planeamos eliminar el bucket, primero debemos vaciarlo para eliminar todos los objetos. Para hacerlo: 

1) En la lista “Buckets”, elegimos el bucket que deseemos vaciar y, a continuación, presionamos en ‘’Vaciar’’.

2) Para confirmar que deseamos vaciar el bucket y eliminar todos los objetos que contiene, en “Bucket vacío”, escribimos el nombre del bucket.

3) Para vaciar el bucket y eliminar todos los objetos que contiene, elegimos ‘’Vaciar’’ y se abrirá una página “Vaciar bucket”. 

4) Para volver a la lista de buckets, seleccionamos ‘’Salir’’.


#
También podemos elegir un objeto específico a eliminar sin vaciar todos los objetos del bucket. Para eso:

1) En la lista “Buckets”, seleccionamos el nombre del bucket que contiene el objeto que deseamos eliminar. 

2) Seleccionamos la casilla de verificación situada a la izquierda de los nombres de los objetos que deseamos eliminar. 

3) Elegimos “Actions” (Acciones) y después “Delete” (Eliminar) en la lista de opciones que aparece; o también podemos elegir “Delete” (Eliminar) en las opciones de arriba a la derecha.
















#
#
#
#
#



See you on [Day 9](day09.md).
