
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
# ls (Listar directorios y archivos)

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
# mkdir (Crea directorios)

El comando mkdir te permitirá crear un directorio con el nombre y la ruta que especifiques. Si no le indicas ninguna ruta, por defecto, te creará la carpeta dentro del directorio de trabajo en el que te encuentres.

![Screenshot_406](https://user-images.githubusercontent.com/96561825/170119257-a7aab17e-9895-4bd0-a7a8-4458aaf9b6cb.png)

Cas contrario, le podemos indicar que nos cree un directorio con un path definido dentro de dir1.

![Screenshot_407](https://user-images.githubusercontent.com/96561825/170119380-7c0ea647-f350-4e15-9cd1-ce8d750c38eb.png)
#

# rmdir (Borra directorios)

El comando rmdir te permite eliminar el directorio que le especifiques. Para poder utilizar este comando, el directorio a borrar debe estar vacío.

![Screenshot_408](https://user-images.githubusercontent.com/96561825/170119724-6df95d05-f6a8-47fb-adba-97d58ce4c0d1.png)

El de arriba es el uso más simple del comando, sin indicar ruta.

Podemos también borrar un directorio con un path definido.

![Screenshot_409](https://user-images.githubusercontent.com/96561825/170119834-8fac1e2a-0405-4508-b137-f435de790bb4.png)
#
# rm (Borra directorios no vacíos y archivos)

El comando rm te permite eliminar archivos sueltos y directorios que no se encuentren vacíos.

![Screenshot_410](https://user-images.githubusercontent.com/96561825/170120010-23c5a130-cdc6-496c-8e1d-74391e9ef389.png)

El de arriba es el uso más simple del comando, sin indicar ruta.
Eliminamos 1 archivo específico dentro de dir1.

![Screenshot_411](https://user-images.githubusercontent.com/96561825/170120125-2f92daa3-3f27-4161-93e2-f03f17f84d3a.png)

Con el modificador -r eliminamos el directorio dir2 y recursivamente, todo su contenido. Es un comando a utilizar con mucha precaución.
#
#cp (Copia archivos y directorios)

Usando el comando cp, serás capaz de copiar archivos y directorios, así como ubicarlos en otras rutas, definiendo origen primero y luego destino 

![Screenshot_412](https://user-images.githubusercontent.com/96561825/170120326-6438d7ab-e257-4c96-afae-e21b9e8dbfca.png)


El de arriba es el uso más simple del comando, sin indicar ruta.
Copiamos en este caso archivo3.txt, hacia dir1 y lo nombramos archivo1.txt

![Screenshot_413](https://user-images.githubusercontent.com/96561825/170120338-1be1ea92-a258-4cdb-b004-036da8c0eaa4.png)

Con el modificador -r en este caso copiamos el directorio dir3 en uno llamado dir2, el mismo comando lo creo.
#
#mv (Mueve archivos y directorios)

El comando mv te servirá para mover archivos desde la consola. 
La sintaxis es muy sencilla, solamente deberás especificar la ubicación de inicio, incluyendo el nombre del archivo y la ubicación de destino.

![Screenshot_414](https://user-images.githubusercontent.com/96561825/170130997-5d9bacde-c926-408e-a469-6c7c69b7d86a.png)

Movimos un archivo de dir1 a dir3, conservando su nombre  original.

![Screenshot_415](https://user-images.githubusercontent.com/96561825/170131018-16a43d94-119d-4d22-9ab3-2eb342744681.png)

En este caso usamos el comando mv para renombrar un archivo, ya que las rutas definidas son las mismas.
#

#cat (Leer y modificar archivos)

El comando cat es uno de los comandos más utilizados cuando se trata de manejar archivos de texto (en formato .txt) desde la terminal.
Entre sus múltiples opciones, está la posibilidad de crear un archivo, imprimir por pantalla su contenido.

![Screenshot_416](https://user-images.githubusercontent.com/96561825/170132054-ef98d498-462a-4457-9588-550c546e14f2.png)

Esto nos abrirá el archivo1.txt, permitiendo editarlo. Con la combinación CTRL+D terminaremos la edición y se guardará el contenido.

![Screenshot_417](https://user-images.githubusercontent.com/96561825/170132067-0112b87f-86e2-4b6c-be44-d31e9222e8aa.png)

Invocando el comando sin “>”, nos mostrará por pantalla el contenido del mismo. Se puede usar con el modificador -n, para numerar las líneas y con el
-b, con el propósito de no mostrar las líneas en blanco.
#
#more (Leer archivos)
El comando more es otro comando útil para imprimir por pantalla el contenido de un archivo de texto. Esencialmente es igual que el comando cat, con la diferencia que este comando página el contenido, y es más adecuado cuando para leer archivos largos.
![Screenshot_418](https://user-images.githubusercontent.com/96561825/170132323-ee2aa09f-bf85-403e-8afa-27c66cb5f502.png)


Nos paginará el archivo en cuestión, de tal manera que en sus últimas líneas lo veremos así:
![Screenshot_421](https://user-images.githubusercontent.com/96561825/170132332-a79f2368-817a-4a4f-8cd6-5f23af97166a.png)
#

# nano (Editor de textos en la terminal)

En la parte inferior se muestran las diferentes combinaciones de teclas que se necesitarán a la hora de trabajar con archivos.
CTRL+R: Combinación para indicarle un archivo de texto a Nano para que lo abra y muestre su contenido por la consola.
CTRL+V: Estando dentro de Nano y con el archivo abierto en la consola, esta combinación sirve para avanzar a la página siguiente.
CTRL+Y: Sirve para retroceder a la página anterior.
CTRL+W: Sirve para introducir un carácter o grupo de caracteres y buscar en el texto cualquier letra o palabra que coincida con el parámetro de búsqueda.
CTRL+X: Para cerrar el archivo una vez que lo hayas terminado de visualizar en la consola. Eso cerrará el editor de texto Nano y volverá a aparecer el prompt de Bash por consola.

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


