
# EFS

## Amazon EFS

### Amazon Elastic File Storage

#### Servicios de almacenamiento Amazon EFS


En este apartado estudiaremos los conceptos del servicio Elastic File System (EFS), como:

● usa el protocolo NFS.

● es escalable.

● aumenta y reduce la capacidad de almacenamiento automáticamente.

● tiene alta disponibilidad y durabilidad.

AWS implementa y administra de manera automática la infraestructura de EFS, que se distribuye en una cantidad ilimitada de servidores, para evitar cuellos de botella en el rendimiento.

Amazon EFS proporciona capacidad de almacenamiento elástica, que escala para adaptarse a las cargas de trabajo que se ejecutan en instancias de Elastic Compute Cloud (EC2) y acceder a archivos a través de solicitudes de la API (interfaz de programación de aplicaciones).

#
#

## Amazon EFS ofrece dos tipos de clases de almacenamiento:

La clase de almacenamiento estándar se utiliza para almacenar archivos a los que se accede con frecuencia, como aplicaciones de bases de datos. (Recordemos S3
Standard, para archivos de acceso frecuente, Amazon suele mantener estos modelos en todos sus servicios.) 

La clase de almacenamiento de acceso infrecuente (IA) es una clase de almacenamiento de menor costo que está diseñada para almacenar archivos a los que se accede con poca frecuencia de manera rentable. Puede utilizar este tipo de almacenamiento con fines de archivo. (Recordemos S3 Glacier, para almacenamiento de archivos de acceso poco frecuente,como backups.) 

#
#

## EFS - Casos de uso y rendimiento 

Algunas de los usos más comunes de AWS EFS pueden ser para el almacenamiento de archivos de aplicaciones empresariales, para cargas de trabajo y aplicaciones,
incluyendo big data, o también para flujos de trabajo de procesamiento, gestión de contenido o websites.

El rendimiento del sistema va en función del tamaño del sistema de archivos, aunque soporta picos altos de lectura/escritura.

Cualquier sistema de archivos EFS creados podrá soportar picos de 100MB de lectura/escritura por segundo.

Para los sistemas de archivos superiores a 1TB, Amazon Web Services te adjudicará 100MB de más por cada TB para los picos en tu carga de trabajo.

El sistema funciona parecido a las instancias EC2, que acumulan créditos en las fases inactivas del servicio, por lo que la acumulación de créditos para los
periodos inactivos o de baja frecuencia darán pie a disponer de una mayor tasa de rendimiento cuando tenga picos de carga de trabajo.


#
#

## Repaso

● Servicio diseñado para ser altamente Escalable.

● Servicio High Available.

● Servicio Standard o IA (Infrequent Access).

Amazon EFS ● Servicio de Alto Rendimiento (Orden de los Terabytes)




#
#
#
#




See you on [Day17](day17.md)
