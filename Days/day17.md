


# Objetivos

En el siguiente ejercicio vamos a crear una máquina virtual con el virtualizador VirtualBox. Una vez creada vamos a instalar el servidor web Apache y accederemos a la publicación por defecto.

## ¿Qué recibimos?

El enlace a la imagen .ISO del sistema operativo a instalar —el VirtualBox ya debe estar instalado en nuestro ordenador—.

#
#

### Instrucciones

Ejercicio 1
De forma individual ejecutamos los siguientes pasos: 

****1)**** Descargamos el siguiente archivo (son 337 MB): https://www.debian.org/distrib/netinst 

Hacemos clic en la versión AMD64:


xxxxxxxxxx
#
#

****2)**** Iniciamos VirtualBox. 

Allí vamos a crear una nueva máquina con la opción “Nueva”. En cada pantalla deberemos indicarle las siguientes opciones:
* Nombre: DebianCliente
* Sistema operativo: Linux 64 bit
* Memoria: 1024MB
* Disco Duro: Crear Disco Duro, 8 GB
* Tipo VDI, Reservado Dinámicamente

Nos debe quedar algo similar a esto:


xxxxxxxxxx


#
#

****3)**** Adicionalmente vamos a tener que modificar algunas opciones de nuestra VM, las cuales detallamos a continuación:

      a)El tipo de red, que está como “NAT”, debemos cambiarlo a “Adaptador puente (Bridge)”, de la siguiente manera:
      
      xxxxxx
      
      
     





Cuando hacemos este cambio, debemos elegir del listado la placa de red por la cual nos conectamos a Internet habitualmente.


xxxxxx


b)Debemos vincular el archivo descargado a nuestra VM para que podamos instalarlo. Seleccionamos la opción “Almacenamiento”
      
      
      xxxxx
      
      
Dentro de “Controlador IDE”, nos posicionamos sobre “Vacío” y en la parte de atributos hacemos clic en el ícono de CD y elegimos “Seleccionar un archivo de disco”. Allí se nos abrirá un explorador de archivos y debemos ir a nuestro archivo .ISO descargado.


xxxxx




Debería quedar así:


xxxxxxxxx



#
#

****4)**** Ahora vamos a iniciar nuestra VM desde el menú principal. Debe abrirse una ventana similar a la siguiente:


xxxxxx

#
#

****5)**** Las opciones recomendadas para instalar el SO son las siguientes:

****Tip: Siempre observar qué tecla se asigna como “anfitrión”. En el caso de Windows por defecto es “CTRL DERECHA”. Esta tecla nos permite salir de la máquina virtual y que el cursor/puntero vuelva al sistema operativo host.****


a) Install, idioma Spanish y la distribución de teclado que manejemos.

b) En el nombre de la máquina, colocamos “debiancliente”, sin nombre de dominio.

c) Colocamos una clave al superusuario. Es importante que no la olvidemos.

d) Luego crearemos un usuario con el nombre que queramos. También nos pedirá clave y confirmación.

e) En el método de particionado de disco, seleccionamos “guiado - utilizar todo el disco” y elegimos el único disco en la lista. En la opción siguiente, le 













See you on [Day18](day18.md)
