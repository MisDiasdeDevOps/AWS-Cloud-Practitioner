
# Introduccion a la Terminal



Índice

1. Introduccion a la Terminal en Linux
2. La consola
3. Diferentes tipos de shell
4. Ejecución de la consola
5. Elevación de privilegios


#
#
 # La consola de Linux

La interfaz de línea de comandos, o CLI ****—por sus siglas en inglés command-line interface—****, es un método de comunicación entre usuario y máquina que acepta instrucciones del usuario a través de líneas de texto (siguiendo unas determinadas reglas de sintaxis que puedan ser interpretadas por el sistema operativo).
> ****La herramienta que posibilita la función de interfaz de usuario se la denomina shell.****

Aplicado en el ámbito de la interfaz de línea de comandos, estaríamos hablando de una shell CLI o intérprete de comandos.


# Tipos de shell

En Linux tenemos una multitud de shells o intérpretes diferentes. El más conocido de todos probablemente es Bash, debido a que es el que suele venir por defecto en la gran mayoría de distribuciones GNU/Linux, pero también destacan otros como Bourne Shell (sh), Korn Shell (ksh) o C Shell (csh), los cuales vamos a conocer.

# Bourne Shell

Lleva el nombre de su creador en los Laboratorios Bell, Steve Bourne. Fue la primera shell utilizada para el sistema operativo Unix y ha superado en gran parte la funcionalidad de muchas de las shells más recientes. Todas las versiones de Linux Unix permiten a los usuarios cambiar a la original Bourne Shell, conocida simplemente como "sh", si así lo desean. 
Sin embargo, hay que tener en cuenta que al hacerlo, se renuncia a funcionalidades como el completado de nombres de archivo y el historial de comandos que los depósitos posteriores han añadido.

# C/TC Shell

El C Shell fue desarrollado posteriormente al Bourne Shell y está pensado en facilitar el control del sistema al programador en lenguaje C. La razón de esto es que su sintaxis, como vamos a apreciar, es muy similar a la de este lenguaje.

Conocido popularmente también como csh, está presente en otros SO, por ejemplo, en Mac OS. Posee una evolución, conocida como tcsh que incorpora funcionalidades avanzadas y mayores atajos de teclado.


# Korn Shell

Esta también fue escrita por un programador en los Laboratorios Bell, David Korn. Intenta combinar las características de la C Shell, TC Shell y Bourne Shell en un solo paquete. 

También incluye la capacidad para crear nuevos comandos de shell para los desarrolladores cuando surja la necesidad.

Posee funciones avanzadas para manejar archivos de comandos que la colocan a la par de lenguajes de programación especializados, como AWK y Perl.

# Bourne-Again Shell (BASH)

La Bourne-Again Shell es una versión actualizada de la Bourne Shell original. Es una shell utilizada ampliamente en la comunidad de código abierto.
Su sintaxis es similar a la utilizada por la Bourne Shell, incorporando funcionalidades más avanzadas que se encuentran en las shells C, TC y Korn.

Entre las funcionalidades adicionales que carecía Bourne, está la capacidad para completar nombres de archivos pulsando la tecla TAB, la capacidad de recordar un historial de comandos recientes y la capacidad de ejecutar múltiples programas en segundo plano a la vez.

#
#
#



# Consola de Linux: Ejecución en inicio

Si bien cada distribución de Linux tiene su manera particular de acceder a la consola, cuando el SO se inicia en los niveles 1, 2, 3 y 4 nos llevará por defecto a la consola.

# Consola de Linux: Ejecución desde GUI

Si en cambio nuestro SO inicia en nivel 5 (con GUI), para poder utilizar la terminal tenemos diferentes opciones. Estas varían de acuerdo a la distribución instalada.

En el caso de Ubuntu, tenemos dos opciones:

● La primera de ellas es lanzando un TTY, o espacio de trabajo sin entorno gráfico. Podemos ejecutar 7 terminales al mismo tiempo de esta forma. De la 1 a la 6, ninguna tiene interfaz gráfica. Para cambiar de TTY en Linux debemos usar el atajo de teclado Control+Alt más la tecla —de F1 al F7— del TTY que queramos ejecutar.

● La segunda opción es encontrar una app dedicada que se ejecuta en una ventana, dentro del panel de aplicaciones de nuestra distro. En el caso de Ubuntu, por ejemplo, podemos encontrar esta terminal dentro del cajón de programas del entorno gráfico GNOME.

#

# Los privilegios del superusuario root

Por lo general, los sistemas operativos contemplan el uso de solo un usuario, el cual tiene permisos de administrador. En Linux las cosas se manejan de una forma particular, se separa la cuenta de usuario común de la de superusuario y es eso lo que conocemos como root. Esta cuenta posee todos los privilegios y permisos para realizar acciones sobre el sistema.

Para la ejecución de algunos comandos debemos ingresar dicho acceso (clave de root). Sin embargo, se debe tener un conocimiento sobre las acciones que se realizan, ya que una acción realizada de manera errónea podría ocasionar daños importantes en el sistema. El uso de instrucciones con privilegios de superusuario pueden ser
sumamente útiles, pero totalmente devastadoras si desconocemos las consecuencias de su uso en el sistema. 

Veamos el método para elevar nuestros privilegios.

Suponiendo que iniciamos sesión como un usuario “común”, denominado “gino” y queremos reiniciar un servicio (cron), vamos a obtener lo siguiente:

![Screenshot_480](https://user-images.githubusercontent.com/96561825/170152506-0b8c0034-eca8-4341-a0bd-7aaa04f4bc6b.png)


Para evitar el error, debemos usar el comando sudo, previo al comando que queremos ejecutar. Nos pedirá la contraseña de root y se ejecutará como tal de manera satisfactoria.

![Screenshot_481](https://user-images.githubusercontent.com/96561825/170152519-df1d51ef-3b4b-4184-a95f-5f1b3f4c455f.png)


#
#
#





See you on [Day 12](day12.md).
