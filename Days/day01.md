

***BootCamp DevOps Engineer***


***CREACION y SECURACION de tu CUENTA***



***Desafío 1 AWS - Semana 1 –***

***Creación de Cuenta - MFA –***

***Alarma de Gastos-***

***Profesores Gino Rojo  Gastón Baravalle -***





Iniciamos con la creacion deuna cuenta en AWS.



Paso 1: Nos dirigimos al portal de Azure ubicado en https://aws.amazon.com/es/,  iniciamos sesion.



![image](https://user-images.githubusercontent.com/105083569/167222906-21606f34-9bc3-4777-96c7-cf09e1c83672.png)



Seremos  dirigidos a la página de iniciar sesión o a la de crear cuenta.  No se deben  preocupar  por la selección entre «Root y IAM user».  Lo veremos más tarde. 
Ahora solamente  hacer clic en «Create a new AWS account» y vas a ver la pantalla siguiente.

![image](https://user-images.githubusercontent.com/105083569/167224315-551c4fff-f732-471d-9265-24b0ad2e9822.png)

 
Despues veremos la siguiente pantalla. 
 
![image](https://user-images.githubusercontent.com/105083569/167224330-4ec9bbd4-fb20-4929-b479-9d2420487b53.png)

Completamos los datos y nios pide verificar el email, continuamos
 
![image](https://user-images.githubusercontent.com/105083569/167224365-2a15fb49-cc33-440b-9abb-cd9bcba0b1ed.png)

Vamos a nuestro correo para verificar el codigo, 
 
![image](https://user-images.githubusercontent.com/105083569/167224390-1cb9cfaa-c566-469f-abbb-4aa493d94ede.png)
 
ahora debemos proporcionar este dato en la pagina principal

![image](https://user-images.githubusercontent.com/105083569/167224407-bfc7d9c1-e97c-4532-ada9-f546cc4161cb.png)

Y pasamos al siguiente paso  donde registramos en AWS con contraseña , 

![image](https://user-images.githubusercontent.com/105083569/167224423-9c000ec2-622f-4e93-8f5f-c0fbaf102eb7.png)

Prestar atencion a las exigencias de la contraseña 

![image](https://user-images.githubusercontent.com/105083569/167224438-e4a7d391-5c12-4628-befe-27a5f2b33f8f.png)

Continuamos completando con los datos requeridos

![image](https://user-images.githubusercontent.com/105083569/167224455-98392ae1-2b17-4e5a-904b-7717416991ab.png)

Completamos y seguimos completando

![image](https://user-images.githubusercontent.com/105083569/167224472-444f1e3c-0cc7-4696-8b0a-b8e9b279df82.png)
 
Seguimos 

![image](https://user-images.githubusercontent.com/105083569/167224491-f2171a40-4b21-437a-ab6e-ca66881c0e13.png)

***Aclaracion Importante:*** 

****Debido a que ya tengo una cuenta creada bajo otra denominacion y para que no haya problemas de solapamiento y/o  conflicto  con la tarjeta,   ya que solo poseo una sola tarjeta,  aquí suspendo el proceso de la registracion.*** 

***Fin de esta proceso.***

#
#
#
#
#
-------------------------
#
#
#
#
#




***Securizar la cuenta***

-

Paso 2:  Securizar la cuenta .  Como una buena práctica debemos  inmediatamente después de iniciar sesión es  securizar nuestra cuenta de AWS. 

![image](https://user-images.githubusercontent.com/105083569/167224571-bf25470a-4555-46e8-9bb9-2b700875c6bf.png)

En la barra de búsqueda, escribimos IAM 
 
![image](https://user-images.githubusercontent.com/105083569/167224584-6289611f-85ac-4c73-846d-adb2325e430b.png)

y seleccionamos el resultado que aparece.

![image](https://user-images.githubusercontent.com/105083569/167224601-43cc6643-a156-435e-a313-1e8d11502255.png)
 
Activamos MFA –multi factor autentificacion , en la pantalla de IAM, haz click en «ACTIVAR MFA» 

![image](https://user-images.githubusercontent.com/105083569/167224626-3f23bb82-c1e2-4a96-b0c5-2b790664af81.png)

En la pantalla que nos aparece, apretamos “ DISPOSITIVIO MFA VIRTUAL” 

![image](https://user-images.githubusercontent.com/105083569/167224644-0eb8463e-511f-417b-b3c4-5038e305c254.png)
 
A posteriorla  la aplicación de autenticación de Google nos muestra el código QR que escanearámos en nuestro celular ..
Para ello debemos tener instalado el programa Google Authenticator o similar .

![image](https://user-images.githubusercontent.com/105083569/167224659-7943a243-a5c9-4bf6-8fad-e4d5a7d43363.png)
 
Entonces, la aplicación nos dara una nueva clave cada unos segundos. Introduzca las 2
claves generadas en secuencia por el autenticator en su móvil y pulse siguiente.



Al concluir,  deberíamos  lograr ver la siguiente pantalla:

![image](https://user-images.githubusercontent.com/105083569/167224691-204be275-54bd-4507-8458-b10cfdb49613.png)

#
#
#
-------------
#
#
#
 
***Create IAM user***

Primero, hablemos de los usuarios en cuestión de AWS.
Acabamos de crear e iniciar sesión en nuestra cuenta, digamos nuestra organización. Allí podemos crear diferentes usuarios, de diferentes grupos, con diferentes permisos. 
Supongamos que tiene 1 administrador, 3 desarrolladores, 1 operaciones de desarrollo y un administrador. Todos estos usuarios estarán asociados a la cuenta que acabamos de crear e ingresó como root. Entonces, asegurémonos de que el acceso y los permisos funcionan. 
Tenemos grupos, tenemos usuarios, roles y políticas. Podemos verlo a la izquierda de la pantalla. Creemos un nuevo grupo de administradores, con derechos de administrador completos. 
Vayamos a grupos y hagamos clic en Crear nuevo grupo. Demos el nombre del grupo «admins», y luego veremos el siguiente paso que consiste en adjuntar políticas al grupo. 

![image](https://user-images.githubusercontent.com/105083569/167224738-21a776ba-7194-48b9-a2cf-bea9a7c78bc4.png)

---


Aquí la elección del tipo de acceso es importante. Tenemos dos opciones:
● Acceso programático es un tipo de acceso desde la interfaz de línea de comandos de AWS utilizado por los desarrolladores. Por ejemplo, para insertar código en AWS o ejecutar otros comandos relacionados con la programación.
● Acceso a la consola de administración de AWS es básicamente un tipo de acceso para usuarios que solo acceden a la consola que estamos usando en este momento para monitorear o administrar.
Entonces, después de elegir el tipo de acceso (en este caso, solo acceso a la consola), debemos elegir una contraseña para el usuario y continuar. La siguiente pantalla nos dará la oportunidad de asignar al usuario a un grupo. Vamos a asignarlo a nuestro grupo de administradores.

![image](https://user-images.githubusercontent.com/105083569/167224763-b2b8095c-8bf1-46e1-a964-b25a1dc8ea1b.png)




Creamos un usuario

![image](https://user-images.githubusercontent.com/105083569/167225448-9ef6cbcb-642a-499f-aa20-75819e5d64f6.png)
 
Le damos permisos

![image](https://user-images.githubusercontent.com/105083569/167225464-9b3b7607-742c-4814-9c2f-4b721b80a01a.png)

Si todo esta correcto obtendremos la siguiente pantalla.

![image](https://user-images.githubusercontent.com/105083569/167225480-daab7d48-cc5a-46f0-8f7d-3d5139448b6b.png)

Cuando usamos el botón de abajo «Descargar.csv» todos los detalles de la tabla se van a descargar. Incluso el enlace de login.

![image](https://user-images.githubusercontent.com/105083569/167225502-6f0db255-5a90-43fe-ac65-32da663a8ea1.png)

Usuario creado exitosamente.
 
![image](https://user-images.githubusercontent.com/105083569/167225511-05b3c546-4c05-428c-b919-1c728fa28c56.png)

Como acabamos de crear nuestra cuenta, que ya tiene autenticación de dos factores, no hay necesidad de “Aplicar una politica de contraseña IAM”,  no se tiene que hacer este paso.

![image](https://user-images.githubusercontent.com/105083569/167225528-93d0a08f-4dad-40f6-a7d7-dc3e192061bc.png)

 
 
 
 
 
 
#
#
#
#
#
#
 -------------------
#
#
#
#
#

***CREAR UN PRESUPUESTO*** 

Iniciamos sesión en la consola como el usuario root (porque es el único que tiene acceso a la información de facturación). Luego en la barra de búsqueda de la consola de administración de AWS, escribimos «Facturacion » y elija en el resultado que aparece “Budget”

![image](https://user-images.githubusercontent.com/105083569/167225558-3c171f4b-4266-4677-8fde-ecd3ca4ce839.png)
 
Creamos nuestro propio presupuesto.

![image](https://user-images.githubusercontent.com/105083569/167225576-1a43af1c-111d-4717-a1f0-d1044edabd42.png)

Definimos el presupuesto.

![image](https://user-images.githubusercontent.com/105083569/167225594-af8e4d6a-9ed0-482b-9723-838a3e233fb6.png)


Lo definimos mensualmente y con un importe de 5 dolares .

![image](https://user-images.githubusercontent.com/105083569/167225604-a1062bd9-bf60-4d79-8bca-d9f0fa9fa3f8.png)
 
Siguiente

![image](https://user-images.githubusercontent.com/105083569/167225621-ee350839-fe7e-44d3-8920-160777b213fa.png)


Aquí aclaramos que nuestro presupuesto mensual es de 5 dolares , y cada vez que superemos los 2.50 dolares recibiremos un correo notificandonos.
 
 ![image](https://user-images.githubusercontent.com/105083569/167225635-2d154411-2b26-44b5-af28-49c4bb727565.png)
 
Aquí operamos la alerta del 50% 

![image](https://user-images.githubusercontent.com/105083569/167225651-77b7e1bd-1fda-4898-a4af-ed9e984b5dae.png)

Aquí tenemos una informacion detallada de nuestro presupuesto y como lo vamos a manejar.
 
![image](https://user-images.githubusercontent.com/105083569/167225663-20a65622-ed37-4b98-b588-656fa73d0839.png)



Finalmente tenemos una cuenta segura en AWS que está lista para  propósitos de prueba, investigación y aprendizaje
Fin.
![image](https://user-images.githubusercontent.com/105083569/167225676-68e716d8-f863-4c62-b2c7-f88694607b22.png)













