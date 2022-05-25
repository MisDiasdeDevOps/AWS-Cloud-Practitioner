


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

e) En el método de particionado de disco, seleccionamos “guiado - utilizar todo el disco” y elegimos el único disco en la lista. En la opción siguiente, le indicamos que como esquema de particionado vamos a colocar “Todos los ficheros en una partición”. Finalmente le indicamos “Finalizar particionado y escribir cambios en el disco”.

f) El proceso de instalación comenzará, es vital tener conectividad de Internet porque se descargan paquetes adicionales. En un momento se nos preguntará por el país de réplica, seleccionamos nuestro país de residencia

g) Debemos llegar a un menú de selección de programas, ahí podemos elegir entre usar interfaz gráfica o solo texto, nuestra idea es utilizar esta última. Para ello, debemos desmarcar la opción de “Entorno de escritorio Debian”. Debería quedarnos así:


xxxxxxxxxxx

h)Después de unos minutos, le indicamos que queremos instalar GRUB y seleccionamos el único dispositivo en la lista —normalmente /dev/sda—. Luego de esto el proceso nos pedirá reiniciar y, finalmente, se iniciará el SO. Deberíamos llegar a la siguiente pantalla:

xxxxxxxxx


i) Como login utilizaremos nuestro nombre de usuario y contraseña. Podemos también usar como usuario “root” y la contraseña de superusuario asignada.





****6)**** Ahora procederemos a instalar el servidor Web Apache, para ello, ejecutaremos las siguientes sentencias:

En caso de estar logueados como el usuario creado, debemos cambiar a root para poder tener permisos de instalación.


xxxxxxxxxxxxxxx




En caso de estar logueados como root:


xxxxxxxxxxxxxx


Para poder probar que nuestro servidor web está instalado y corriendo, debemos averiguar la IP de nuestra VM, ejecutando la sentencia:


xxxxxxxxxxxxxx

Esta nos devolverá una lista de los adaptadores de red que tenemos en nuestro sistema, sus direcciones IP y MAC address. La de nuestro interés es la 2, para este ejemplo es la 192.168.0.74.



xxxxxxxxxxxxxxx

Con esta dirección, en nuestro equipo, abrimos en el navegador de Internet nuestra dirección IP (siguiendo nuestro ejemplo sería: http://192.168.0.74). Allí debemos obtener la pantalla de inicio de Apache.

xxxxxxxxxxxxxxxxxxxxxx


#
#
#

# Ejercicio 2

De forma individual ejecutamos los siguientes pasos:

Sin cerrar nuestra máquina virtual, lo que vamos a hacer es conectarnos vía SSH a la máquina virtual. Para ello, prepararemos nuestro entorno de trabajo con dos pasos previos:

* Habilitaremos el servidor SSH en nuestra VM, ejecutando las siguientes instrucciones:
En caso de estar logueados como el usuario creado, debemos cambiar a root para poder tener permisos de instalación:


xxxxxxxxxxx


En caso de estar logueados como root:

xxxxxxxxxxxx


* Descargamos la utilidad PuTTY desde el siguiente enlace y la instalamos:

[
](https://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html)


****1)**** Abrimos la utilidad PuTTY.

xxxxxxxxxxxxxxxx


Esta nos va a permitir conectarnos a nuestra VM. Este método de conexión es válido tanto para nuestra VM como para cualquier equipo que esté ejecutando Linux y tenga habilitado el openssh-server.


xxxxxxxxxxxxxxxx

En “Host Name”, debemos colocar la IP de nuestra VM y hacemos clic en “Open”.

Allí nos vamos a encontrar nuevamente con la pantalla de logueo y lo haremos con nuestro usuario (en principio, no podremos hacerlo con el usuario root).


xxxxxxxxxxxxxxxxxxxxxxxxx

Con toda la mesa de trabajo debatan sobre las siguientes preguntas y contesten en conjunto:

* Tanto para el ejercicio 1 como para el ejercicio 2, describan con sus palabras lo que acaban de hacer.
* Describir para qué sirve “apt-get”.
* Describir para qué sirve “su”.
* En el caso del ejercicio 1, ¿cuál fue la utilidad de instalar el paquete apache2? 
* En el caso del ejercicio 2, ¿les resultó familiar esta forma de conectarse a un equipo?





























See you on [Day18](day18.md)
