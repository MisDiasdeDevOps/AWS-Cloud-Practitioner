

# Creando una cuenta en Amazon AWS y Creando una Instancia en Windows.
# 
Lo primero que deberemos tener es una cuenta en Amazon AWS. Amazon nos permite crear una cuenta que dispone de una capa gratuita de servicios y que para nuestro ejemplo será más que suficiente.

Para crear la cuenta podemos hacerlo desde el siguiente enlace. Amazon nos pedirá una serie de información básica para poder crear la cuenta, entre ellos estarán los datos de una tarjeta de crédito. El hecho de que nos pida los datos de una tarjeta no es porque nos vayan a cobrar de inicio, es porque si en algún momento excedemos el uso de servicios de la capa gratuita, tendremos que pagarlos.

El resto de información es el formulario típico de registro de cualquier servicio.


#
## Creando nuestra instancia.

Para ello deberemos acceder al panel de administración y bien desde la pestaña de
Servicios (que aparece en la parte superior izquierda) o bien desde el propio buscador,
deberemos buscar EC2. Que tiene un aspecto similar a esto:

Desde aquí podremos iniciar el proceso de creación de instancia pulsando el botón «Launch
Instance», que nos guiará por un proceso de siete pasos:

#

## 1. Selección de la AMI.

Las AMI son las Amazon Machine Images, y no son más que una serie de plantillas predefinidas que contienen distintas configuraciones de sistemas operativos, aplicaciones...

Es importante recordar que queremos hacer uso de la capa gratuita, por eso es importante que o seleccionemos en el buscador de AMIs (lateral izquierdo) la opción «Free tier only» para que nos muestre solo estas o que nos aseguremos que la AMI elegida muestra la siguiente etiqueta en su descripción «Free tier eligible».

En nuestro caso y para este ejemplo seleccionaremos una «Windows Server 2012 Base, 2016 o 2019 “ que se encontrara disponible en la capa gratuita de nuestra cuenta


#

## 2. Elegir el tipo de instancia.

Como pueden ver en el listado que se presenta, existe una amplia variedad para seleccionar el tipo de instancias, en nuestro caso (por mantenernos en la capa gratuita) seleccionaremos la t2.micro (free tier elegible).

## 3. Configurando los detalles de la instancia.

por el momento, como el objetivo es únicamente levantar la instancia, no entraremos en más detalle. Avanzamos a siguiente.

## 4. Añadir almacenamiento.

Amazon nos permite añadir hasta 30Gb en la capa gratuita, aunque por defecto la instancia tiene seleccionados 8Gb. Para el ejemplo en el que estamos, esos 8Gb son más que suficientes. Siguiente.

## 5. Añadir etiquetas.

Se trata de un par clave valor, que nos permitirá añadir etiquetas de atributos a la hora de crear la instancia. Por lo general recomiendo como mínimo añadir la de nombre (name). Pueden nombrarla como deseen.

## 6. Configuración de los grupos de seguridad.

Por defecto Amazon nos propone habilitar una RDP , al ser Windows, utilizara Remote Desktop Protocol.


## 7. Revisión y lanzamiento.

En este punto se nos muestra un resumen de la instancia y su configuración, el siguiente paso sería lanzar la instancia «Launch«. En este momento se nos mostrará un mensaje para seleccionar las claves (crearlas, usar existentes o proceder sin ellas), la recomendación, evitar la opción de proceder sin ellas, ya que podemos estar dejando la puerta abierta a futuros ataques.





### ATENCION : Descargar el par de LLAVES DE ACCESO, en un lugar seguro , no se olviden de este paso, si no guardan las llaves, después no podremos convertirlas en clave de acceso (Usuario y Contrasela) de sus intancias y servidores, y será necesario crear la instancia nuevamente.

### Nota : el archivo de llaves de acceso tiene una extensión .pem, asi lo distinguirán.



#
#
#
#
#





See you on [Day 12](day12.md).
