
# Comandos útiles en la terminal de Linux  (Parte 1)

Índice

1. Preparación del ambiente
2. Comandos para el manejo de archivos
3. Comandos para leer archivos de texto

#
Consolidando nuestro ambiente

Para poder seguir correctamente los ejemplos posteriores, es deseable que en su ambientes (máquina virtual o WSL) tengan replicada la siguiente estructura de carpetas y archivos.

![Screenshot_399](https://user-images.githubusercontent.com/96561825/170118416-2712d8b2-f2a5-4e47-a001-7b9fc6c5b810.png)

Para ello debemos ejecutar los siguientes comandos, en el orden dado (solo el texto que está luego del prompt o sea, luego del “$”, en color blanco):

![Screenshot_401](https://user-images.githubusercontent.com/96561825/170118634-5ffd273f-74b2-47d6-b002-7c74bc64edeb.png)
#
Listamos los directorios con la instrucción “ls -R”, debiendo obtener lo siguiente:

![Screenshot_402](https://user-images.githubusercontent.com/96561825/170118793-be0cad4f-ddad-4844-b758-6d132b9c2852.png)
#
Con el comando ls podrás listar los diferentes archivos y directorios de la carpeta de trabajo en la que te encuentres. El comando acepta multitud de opciones, algunas de las cuales veremos a continuación. 
En la imagen debajo podemos observar el uso más simple del comando ls. Si no le indicamos ninguna opción, enumerará todos los archivos y directorios que se encuentran en la carpeta de trabajo actual, sin tener en cuenta archivos ocultos.

![Screenshot_403](https://user-images.githubusercontent.com/96561825/170118943-72aaaadb-68e8-494c-94f2-63ae06c496ce.png)
#
Opción -a: Con esta opción, el comando te mostrará, en forma de lista, todo el contenido que se encuentre dentro del directorio de trabajo, incluyendo, además, archivos y carpetas ocultos. Dependiendo del shell, algunos tipos de archivos se mostrarán con colores diferentes.

![Screenshot_404](https://user-images.githubusercontent.com/96561825/170119047-5351ecf7-97df-41f2-977e-386ba642c372.png)
#
Opción -l: Esta opción es similar a “- a”, pero muestra el contenido en forma de lista e incluye información referente a cada elemento.
Es de las más utilizadas, siendo especialmente útil a la hora de conocer el propietario y los permisos de cada fichero.

![Screenshot_405](https://user-images.githubusercontent.com/96561825/170119141-49edd860-17b4-402f-b786-f6e159681e80.png)
#
El comando mkdir te permitirá crear un directorio con el nombre y la ruta que especifiques. Si no le indicas ninguna ruta, por defecto, te creará la carpeta dentro del directorio de trabajo en el que te encuentres.

![Screenshot_406](https://user-images.githubusercontent.com/96561825/170119257-a7aab17e-9895-4bd0-a7a8-4458aaf9b6cb.png)

Cas contrario, le podemos indicar que nos cree un directorio con un path definido dentro de dir1.

![Screenshot_407](https://user-images.githubusercontent.com/96561825/170119380-7c0ea647-f350-4e15-9cd1-ce8d750c38eb.png)
#
El comando rmdir te permite eliminar el directorio que le especifiques. Para poder utilizar este comando, el directorio a borrar debe estar vacío.

![Screenshot_408](https://user-images.githubusercontent.com/96561825/170119724-6df95d05-f6a8-47fb-adba-97d58ce4c0d1.png)

El de arriba es el uso más simple del comando, sin indicar ruta.

Podemos también borrar un directorio con un path definido.

![Screenshot_409](https://user-images.githubusercontent.com/96561825/170119834-8fac1e2a-0405-4508-b137-f435de790bb4.png)
#
El comando rm te permite eliminar archivos sueltos y directorios que no se encuentren vacíos.

![Screenshot_410](https://user-images.githubusercontent.com/96561825/170120010-23c5a130-cdc6-496c-8e1d-74391e9ef389.png)

El de arriba es el uso más simple del comando, sin indicar ruta.
Eliminamos 1 archivo específico dentro de dir1.

![Screenshot_411](https://user-images.githubusercontent.com/96561825/170120125-2f92daa3-3f27-4161-93e2-f03f17f84d3a.png)

Con el modificador -r eliminamos el directorio dir2 y recursivamente, todo su contenido. Es un comando a utilizar con mucha precaución.
#
Usando el comando cp, serás capaz de copiar archivos y directorios, así como ubicarlos en otras rutas, definiendo origen primero y luego destino 

![Screenshot_412](https://user-images.githubusercontent.com/96561825/170120326-6438d7ab-e257-4c96-afae-e21b9e8dbfca.png)


El de arriba es el uso más simple del comando, sin indicar ruta.
Copiamos en este caso archivo3.txt, hacia dir1 y lo nombramos archivo1.txt

![Screenshot_413](https://user-images.githubusercontent.com/96561825/170120338-1be1ea92-a258-4cdb-b004-036da8c0eaa4.png)

Con el modificador -r en este caso copiamos el directorio dir3 en uno llamado dir2, el mismo comando lo creo.
#















"#
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




See you on [Day 9](day09.md).


