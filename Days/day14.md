
# Realización de un ejemplo en Bash


Índice


1. Preparación del entorno
2. Codificación del script
3. Ejecución del script


# Nos preparamos

Para este ejemplo debemos tener en ejecución alguna de las máquinas virtuales de clase 2. Adicionalmente, debemos instalar un paquete nuevo, llamado “cowsay”, con las siguientes sentencias:

xxx
![Screenshot_483](https://user-images.githubusercontent.com/96561825/170154079-ef198600-d188-44ec-80a5-4a3d60531ef3.png)


# A codear
Creamos una carpeta en nuestro equipo y nos posicionamos en ella con las instrucciones:

xxx
![Screenshot_484](https://user-images.githubusercontent.com/96561825/170154094-cb6070d3-8db6-465b-afd5-328c3dce3a47.png)

Creamos un nuevo archivo llamado lista_verduras y lo completamos con 4 verduras aleatoriamente. Usamos el comando “cat”, finalizamos la edición del archivo con CTRL+D.

xxx
![Screenshot_485](https://user-images.githubusercontent.com/96561825/170154099-1c327d1d-54d5-4668-84dc-2b1cd656da2e.png)

Creamos otro archivo llamado lista_frutas y lo completamos con 4 frutas aleatoriamente.

Usamos nuevamente el comando “cat”, finalizamos la edición del archivo con CTRL+D.

xxxx
![Screenshot_486](https://user-images.githubusercontent.com/96561825/170154107-ed2b77a7-67d3-4730-a4d8-eacc703c2681.png)

Verificamos la creación de ambas listas con cat.

xxxx
![Screenshot_487](https://user-images.githubusercontent.com/96561825/170154115-a7b16a69-ca9a-44f8-b5c5-7a54079a8d11.png)


Vamos a crear un nuevo archivo, que será nuestro script, pero no vamos a usar cat sino el comando nano.

xxx

Se abrirá el editor nano, con un documento en blanco, en el escribimos las siguientes líneas:

xxx
![Screenshot_488](https://user-images.githubusercontent.com/96561825/170154124-53f7c93b-5cf8-4db5-b4c3-9302798f8709.png)

El propósito del script es listar los archivos y pasar dicho output a cowsay. Salimos de nano con CTRL+X, le contestamos que queremos salvar los cambios y dejamos el nombre de archivo tal cual propone.

xxxx
![Screenshot_489](https://user-images.githubusercontent.com/96561825/170154144-626b1d62-22f0-4119-a8cb-c1260649f399.png)

Ahora debemos darle permisos de ejecución a nuestro script:

xxx
![Screenshot_490](https://user-images.githubusercontent.com/96561825/170154160-81f59d72-3a3a-4766-94c0-f5be69a6c43b.png)


# A probar

Con nuestro script creado y con sus permisos correspondientes, procedemos a ejecutarlo con la sentencia (prestar atención al “.” y “/” iniciales).

xx
![Screenshot_491](https://user-images.githubusercontent.com/96561825/170154169-7d3dd191-49b5-40ad-b174-3d847c2f440f.png)


Si la ejecución fue exitosa, debemos tener un output como este:


xxxx
![Screenshot_492](https://user-images.githubusercontent.com/96561825/170154174-fc272597-7e57-47d7-a72b-455c3ec8932a.png)

















See you on [Day15](day15.md)

