
# Amazon S3

## Índice


### 1. Introducción
### 2. Conceptos principales

#

# Introducción

Amazon Simple Storage Service (Amazon S3) es un servicio de almacenamiento para Internet. Está diseñado para facilitar la informática de escalada web. Tiene una
interfaz de servicios web simple que podemos utilizar para almacenar y recuperar cualquier cantidad de datos, en cualquier momento y desde cualquier parte de la web.
Ofrece a cualquier desarrollador acceso a la misma infraestructura de almacenamiento de datos económica, fácilmente escalable, fiable, segura y rápida
que utiliza Amazon para mantener su propia red global de sitios web. Este servicio tiene como fin maximizar los beneficios de escalar.


Ventajas de utilizar Amazon S3

Amazon S3 se ha desarrollado de forma deliberada con un conjunto mínimo de características que se centran en la simplicidad y robustez.
Sus ventajas son:

● Creación de buckets: podemos crear y nombrar un bucket que almacena datos. Los buckets son los contenedores fundamentales en Amazon S3 para el almacenamiento de datos.

● Almacenamiento de datos en buckets: tenemos la posibilidad de almacenar una cantidad ilimitada de datos en un bucket. Cargamos la cantidad de objetos que deseamos en un bucket de Amazon S3. Cada objeto puede contener hasta 5 TB de datos. Cada objeto se almacena y recupera con una clave única asignada por el desarrollador.

● Descarga de datos: permite descargar nuestros datos, o que otros lo hagan.

● Permisos: permite brindar o denegar acceso a otras personas que desean cargar o descargar datos en nuestro bucket de Amazon S3. También podemos conceder permisos para cargar y descargar a tres tipos de usuarios. Los mecanismos de autenticación pueden ayudar a proteger los datos del acceso no autorizado.

● Interfaces estándar: permite utilizar las interfaces REST y SOAP basadas en estándares diseñados para trabajar con cualquier conjunto de herramientas de desarrollo de Internet.



#
#
 
 # Conceptos principales
 
 S3 bucket
 
 Un bucket es un contenedor para objetos almacenados en Amazon S3, es decir, cada objeto está almacenado en un bucket. Por ejemplo, si el objeto denominado photos/puppy.jpg se almacena en el bucket awsexamplebucket1 en la región EE. UU. oeste (Oregón), es direccionable mediante la URL: https://awsexamplebucket1.s3.us-west-2.amazonaws.com/photos/puppy.jpg.
 
 
Los buckets sirven a diversos fines:

● Organizan el espacio de nombres de Amazon S3 al más alto nivel.

● Identifican la cuenta responsable para los cargos de almacenamiento y transferencia de datos.

● Juegan un papel en el control de acceso. 

● Sirven como la unidad de agregación para informes de uso.


#
## Objetos

Los objetos son las entidades fundamentales almacenadas en Amazon S3. Se componen de datos de objetos y metadatos. Los metadatos son conjuntos de pares nombre-valor que describen el objeto. Los objetos incluyen algunos metadatos predeterminados, como la fecha de la última modificación y los metadatos HTTP estándar, como Content-Type. También podemos especificar metadatos personalizados en el momento en que se almacena el objeto. Un objeto se identifica de forma exclusiva dentro de un bucket con una clave (nombre) y un ID de versión.



#
## Claves

Una clave es el identificador único de un objeto dentro de un bucket. Cada objeto de un bucket tiene una clave. La combinación de un bucket, clave e ID de versión identifican de forma única cada objeto. Por lo tanto, se puede pensar en Amazon S3 como una asignación de datos básica entre "bucket + clave + versión" y el objeto en sí.



Se puede acceder a cada objeto de Amazon S3 de forma exclusiva a través de la combinación de punto de enlace de servicio web, nombre delbucket, clave y —de forma opcional— una versión. Por ejemplo, lo podemos ver en la siguiente URL: https://doc.s3.amazonaws.com/2021-03-01/AmazonS3.wsdl, donde "doc" es el nombre del bucket y "2021-03-01/AmazonS3.wsdl" es la clave.

#

## Regiones

Podemos elegir la región geográfica de AWS donde Amazon S3 almacenará los buckets que creamos. Esta elección puede optimizar la latencia, minimizar los costos o cumplir con requisitos legales. Los objetos almacenados en una región nunca la abandonan, a menos que se transfieran expresamente a otra región. Por ejemplo, los
objetos almacenados en la región UE (Irlanda) nunca salen de ella.

#
## Identity and Access Management

Utilicemos AWS Identity and Access Management (IAM) para administrar el acceso a nuestros recursos de Amazon S3. Por ejemplo, podemos usar IAM con Amazon S3 para
controlar el tipo de acceso que tiene un usuario o un grupo de usuarios a partes concretas de un bucket de Amazon S3 que es propiedad de nuestra cuenta de AWS.


#
#


# Operaciones


A continuación, compartimos las operaciones más comunes que ejecutaremos a través de la API:


• Crear un bucket: además, podemos nombrarlo para almacenar los objetos.

• Escribir un objeto: crear o sobrescribirlo para almacenar datos. Cuando escribimos un objeto, debemos especificar una clave única en el espacio de nombres del bucket. En esa instancia es cuando debemos especificar cualquier control de acceso que deseamos aplicar en el objeto. 

• Leer un objeto: releamos los datos, se pueden descargar a través de HTTP.

• Eliminar un objeto: podemos eliminar algunos de sus datos. 

• Enumerar claves: indiquemos las claves incluidas en uno de los buckets. Podemos filtrar la lista de claves en función de un prefijo.


#















Fin

#
#
#
#
#


See you on [Day 10](day10.md).
