
# Cómo armar un ambiente más complejo en AWS

#
#
#

El objetivo de la clase es que conozcas cuáles son los usos reales que se van a encontrar en las empresas donde desarrollan. 

Además, aprenderás buenas prácticas al momento de elegir una arquitectura para tu aplicación y sacarle provecho a la fase 2. 

El modelo a diseñar es el siguiente:


![Screenshot_51](https://user-images.githubusercontent.com/96561825/173106520-bd7041b3-1e70-45d5-955c-22a9923feb26.png)

#
#

# Vamos a armar el ambiente en 2 clases.



## La primera Clase vamos a realizar:

### 1) Creación de las 2 instancias en la VPC.

#

## En la Segunda clase vamos realizar:

### 2) Creación del load balancer.

### 3) Configuración del tráfico y verificación del funcionamiento.


#
#

# Empecemos.

![Screenshot_52](https://user-images.githubusercontent.com/96561825/173106748-3287b7c1-1f77-4d89-949e-45fec2585ba5.png)



### 1. Creación de las instancias EC2 en la VPC.

###  1.a. Acceso a la consola de gestión AWS.

Una vez logueados en la consola de Amazon Educate, seleccionamos la opción AWS Account, aparecerá listada la materia y hacemos clic en Go to Classroom.

Seleccionamos  la opción AWS Educate Starter Account.

Presionamos el botón de acceso a AWS Console y verificamos que el browser no bloquee ventanas emergentes en este sitio.

Nos encontramos con la consola de gestión de la plataforma AWS

![Screenshot_53](https://user-images.githubusercontent.com/96561825/173106862-f376e147-0763-4a9d-958f-4df35af4d0b0.png)

![Screenshot_54](https://user-images.githubusercontent.com/96561825/173106883-4f05c533-00d4-4f14-b1cb-ce8a3b62598b.png)


En la consola de gestión de la plataforma AWS hacemos clic en EC2.



#
#

### 1.b. Crear una instancia en EC2.

Vale aclarar que este paso lo vamos a repetir para crear también la segunda instancia. 

Nos posicionamos en la parte superior derecha de la pantalla y hacemos clic en el botón Launch instances. 
![Screenshot_76](https://user-images.githubusercontent.com/96561825/173111260-3b73e322-eea5-458a-9025-c5066a7e5d6c.png)


### Elgimos Ubuntu Server 20.04 LTS.

![Screenshot_56](https://user-images.githubusercontent.com/96561825/173107295-c8c7a6f2-6756-4865-b467-9643476094d0.png)

![Screenshot_57](https://user-images.githubusercontent.com/96561825/173107321-1a36b8f9-9a6f-4ef4-9101-4fcfd5d948d6.png)



Seleccionamos el modelo de máquina Family T2.micro (capa free).

![Screenshot_58](https://user-images.githubusercontent.com/96561825/173107365-d46c90b2-d05a-469f-951f-23a0c905f8f4.png)



Hacemos clic en Next.

En la interfaz, el Step 3 lo dejamos tal cual está y apretamos Next.

En el Step 4, dejamos los discos por defecto de 8 GB, volvemos a presionar Next.

En el Step 5, hacemos lo mismo. 

![Screenshot_59](https://user-images.githubusercontent.com/96561825/173107437-b87e2631-e2ea-446c-8607-0dc2c798ca02.png)

#

COPIAMOS A QUE GRUPO DE SEGURIDAD PERTENECE

**sg-0bcec8812b56facd1**
#


En el Step 6 vamos a configurar, por ahora, un grupo de seguridad para el acceso a la instancia.

![Screenshot_60](https://user-images.githubusercontent.com/96561825/173107556-26a523bb-404b-4ace-8b8b-e0a8054962f4.png)

Lo importante es darle un nombre y una descripción que nos ayude a identificarlo y dar acceso a los protocolos:

### * SSH TCP PUERTO 22 ANYWHERE

### * HTTP TCP PUERTO 80 ANYWHERE


#

Hacemos clic en Review and Launch.

Corroboramos la configuración de la instancia y hacemos clic en Launch instances.



![Screenshot_62](https://user-images.githubusercontent.com/96561825/173107944-92050000-aac5-4f85-b703-28a618606afe.png)

Creamos un nuevo key pair, si no tenemos, y descargamos el archivo .pem.


#
#


### 1.c. Repetimos los pasos para crear la segunda instancia.

![Screenshot_63](https://user-images.githubusercontent.com/96561825/173108048-c80fd050-8c04-4a71-88fa-e5c1138e64b3.png)

![Screenshot_64](https://user-images.githubusercontent.com/96561825/173108097-a607c6bf-af97-4463-90b9-bf5872e48334.png)

Para este apartado vamos a necesitar una consola o terminal BASH para comunicarnos vía SSH. En la actualidad, hay muchos productos disponibles y depende del sistema operativo que estemos utilizando. Por el momento, dejamos a tu criterio cuál te parece  más cómodo y agradable a la vista. En este ejemplo, utilizamos windows 10 con CMDER. 

En caso de no tenerlo, se puede descargar de https://cmder.net  —recomendamos bajar la versión full que es totalmente portable—.


Copiamos el archivo de claves .pem en la carpeta raíz del cmder, solo por comodidad del ejemplo.

![Screenshot_65](https://user-images.githubusercontent.com/96561825/173108194-2f14440a-f119-433f-b73d-fd49b63b12bf.png)



Abrir la carpeta en Bash donde esta la clave

Abrimos la consola. En la parte inferior derecha abrimos un bash como administrador.

![Screenshot_66](https://user-images.githubusercontent.com/96561825/173108271-f16b0b57-fd86-4f18-82ae-9063f1ed94c5.png)

![Screenshot_67](https://user-images.githubusercontent.com/96561825/173108306-2d010229-5a10-48d6-9832-5a34ca0347da.png)

Vamos a buscar la IP de la “Instancia01” que está online.
			chmod 400 ubuntukey.pem


### >> ssh -i tuarchivo.pem ubuntu@3.221.170.223

![Screenshot_68](https://user-images.githubusercontent.com/96561825/173108407-fd7fc15e-508a-420a-a4fc-b8e0e09a67f5.png)

# 
Una vez dentro, tenemos que instalar un servidor Apache para deployar nuestro código. Con este objetivo, ponemos el siguiente comando:

### >> sudo apt update

### >> sudo apt upgrade -y

![Screenshot_69](https://user-images.githubusercontent.com/96561825/173108500-0f1afdb5-0db3-4c1b-9667-88303ff9dd52.png)

### >> sudo apt install apache2 -y


Comprobamos que el servicio esté andando. Ingresamos a un explorador y colocamos la IP de nuestra instancia y nos debe contestar: Apache2 recientemente instalado.


![Screenshot_70](https://user-images.githubusercontent.com/96561825/173108586-8f6f5ff6-2fad-4b17-b976-a9da88b14d89.png)

Luego, clonamos el repositorio de un proyecto publico de internet

![Screenshot_70](https://user-images.githubusercontent.com/96561825/173108641-9a1d3893-3919-48bd-b9c0-722ef85d11ef.png)


### >> sudo git clone 

### https://github.com/GinoLucianoRojo1993/fase2devopsbootcampeditaws

### >>sudo chmod 777 -R fase2devopsbootcampeditaws/

### >> sudo cp -rf fase2devopsbootcampeditaws/* /var/www/html/


#

Ingresamos nuevamente a la instancia a través del navegador web (repetimos este procedimiento para la segunda instancia en EC2).


![Screenshot_72](https://user-images.githubusercontent.com/96561825/173108734-a9dec13c-b549-46a8-baa8-0b86db429840.png)

![Screenshot_73](https://user-images.githubusercontent.com/96561825/173108740-338beb28-d281-4e9a-a95b-144b2f95b717.png)

#


### ¡Felicitaciones! Ya has llegado hasta acá, en la próxima clase vamos a configurar el load balancer.


#
#

![Screenshot_74](https://user-images.githubusercontent.com/96561825/173108895-0e272927-4714-4f80-96ec-cdfd8c0aca1a.png)

![Screenshot_75](https://user-images.githubusercontent.com/96561825/173108900-eca06882-2e57-4793-a7a3-f01eee4472d9.png)


#


# Actividades a realizar

1. Intentar ingresar directamente a cada instancia constatar que está corriendo nuestra aplicación. Veremos que para ingresar tenemos que cambiar nuestra url.




#
#
#
#
#





See you on [Day15](day15.md)

