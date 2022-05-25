

# Glosario de comandos


A continuación, veremos algunos de los cmdlets más útiles y más comunes que estaremos usando en Windows Powershell.


# 25 comandos básicos de Windows PowerShell


#

## ****Cmdlet          =       Descripción****

****Set-Location****  = Establece la ubicación de trabajo actual en una ubicación específica.

****Get-Content**** = Obtiene el contenido del elemento en la ubicación especificada.

****Add-Content**** = Agrega contenido a los elementos especificados, por ejemplo, agregar palabras a un archivo.

****Set-Content**** = Escribe o reemplaza el contenido de un elemento con contenido nuevo.

****Copy-Item**** = Copia un elemento de una ubicación a otra.

****Remove-Item**** = Elimina los elementos especificados.

****Move-Item**** = Mueve un elemento de una ubicación a otra.

****Set-Item**** = Cambia el valor de un elemento al valor especificado en el comando.

****New-Item**** = Crea un nuevo elemento.

****Start-Job**** = Inicia un trabajo en segundo plano de Windows PowerShell.

****Compare-Object**** = Compara dos conjuntos de objetos.

****Group-Object**** = Agrupa objetos que contengan el mismo valor en propiedades especificadas

****Invoke-Webrequesbt**** = Obtiene contenido de una página web en Internet.

****Measure-Object**** = Calcula los valores de propiedad de determinados tipos de objetos, puede realizar tres tipos de mediciones según los parámetros del comando.

****Resolve-Path**** = Resuelve los caracteres comodín en una ruta y muestra el contenido.

****Resume-Job**** = Reinicia un trabajo suspendido.

****Set-Variable**** = Establece el valor de una variable. Crea la variable si no existe una con el nombre solicitado.

****Show-Command**** = Muestra comandos de Windows PowerShell en una ventana de comandos gráfica.

****Sort-Object**** = Ordena los objetos por valores de propiedad.

****Start-Service**** = Inicia uno o más servicios detenidos.

****Start-Process**** = Inicia uno o más procesos en la computadora local.

****Suspend-Job**** = Detiene temporalmente un trabajo.

****Wait-Job**** = Espera a que los trabajos en segundo plano de Windows PowerShell se completen antes de mostrar el símbolo de sistema.

****Where-Object**** = Selecciona los objetos del conjunto de objetos que se le pasan.

****Write-Output**** = Envía el objeto especificado al siguiente comando en la canalización. Si es el último comando en la canalización, el objeto se mostrará en consola.

#
#
#
#
#
#


# Ejemplos de uso

* Set-Location : Establece la ubicación actual.


![Screenshot_448](https://user-images.githubusercontent.com/96561825/170150316-17db3e71-31bc-41fd-9d42-f295a34e9fe8.png)


* Get-Content: Obtiene el contenido de un archivo de texto.

![Screenshot_450](https://user-images.githubusercontent.com/96561825/170150340-068815cb-ee62-48f4-b7ed-58fedc2a4f05.png)



* Add-Content: Añade contenido a un archivo de texto.

![Screenshot_452](https://user-images.githubusercontent.com/96561825/170150345-12d5bf5a-d16b-4307-8420-adbd2053633c.png)



* Set-Content: Modifica una línea de un archivo de texto.
 
![Screenshot_454](https://user-images.githubusercontent.com/96561825/170150356-77a6303f-82ce-4feb-889d-22cf78dd79de.png)



* Copy-Item: Copia un archivo a un directorio específico.


![Screenshot_456](https://user-images.githubusercontent.com/96561825/170150361-20e38152-e5ca-496d-864c-e955f3d8b142.png)



 * Remove-Item: Este ejemplo elimina de la carpeta actual todos los archivos que tienen una extensión de nombre de archivo .doc con la excepción de los que tengan un * 1 * en su nombre.


![Screenshot_459](https://user-images.githubusercontent.com/96561825/170150371-7f2f3dac-e8f4-4063-9fc9-d3bcddfd184d.png)



* Move-Item: Mueve un archivo a otro directorio y lo renombra.


![Screenshot_461](https://user-images.githubusercontent.com/96561825/170150378-ff131bcd-d469-498a-8cf1-24fe60b3059a.png)



* Set-Item: Este ejemplo crea un alias llamado np para el Notepad de Windows.

![Screenshot_464](https://user-images.githubusercontent.com/96561825/170150386-8fe8e61e-df6e-4e20-9d06-f8e3eae9ddc2.png)





* New-Item: Crea un archivo en el directorio actual.

![Screenshot_465](https://user-images.githubusercontent.com/96561825/170150396-88bed01d-f954-47f6-a2ea-1a5167e84e61.png)




* Start-Job: Ejecuta un script como un proceso en segundo plano.

![Screenshot_466](https://user-images.githubusercontent.com/96561825/170150407-66c79ccd-6e1c-4a14-bbcd-bbac1268a07d.png)




* Compare-Object: Compara el contenido de dos archivos: 
*
Este ejemplo compara el contenido de dos archivos, el ejemplo usa los siguientes dos archivos de texto, cada uno con un valor en una línea diferente.
verduras.txt contiene los valores: papa, zapallo, tomate.
frutas.txt contiene los valores: banana, tomate, naranja.

El resultado muestra solo las líneas que son diferentes entre los archivos. En verduras.txt usa el objeto de referencia (<=) y en frutas.txt usa el objeto de diferencia (=>). Las líneas que se encuentran en los dos archivos no son mostradas.



![Screenshot_467](https://user-images.githubusercontent.com/96561825/170150574-cdfd5e12-c522-41e9-97ab-f1da19e541f2.png)



* Group-Object: Agrupa archivos por su extensión.


![Screenshot_468](https://user-images.githubusercontent.com/96561825/170150583-689905d4-c6b8-4372-8252-61285f2c2e94.png)

![Screenshot_469](https://user-images.githubusercontent.com/96561825/170150608-982438ec-3e62-4b57-b302-8c2e8ad35e1d.png)


* Invoke-Webrequest: Muestra una página web.


![Screenshot_470](https://user-images.githubusercontent.com/96561825/170150623-5495caee-e0f4-40ef-9754-43c02fc28371.png)



* Measure-Object: este comando cuenta los archivos y carpetas del directorio actual.

![Screenshot_471](https://user-images.githubusercontent.com/96561825/170150628-4b50ad40-4fd1-465f-ac91-8ebddd005934.png)

* Resolve-Path: Muestra la ruta actual.

![Screenshot_472](https://user-images.githubusercontent.com/96561825/170150635-5e05af23-c013-4c04-987f-64fc8d7f9956.png)


* Resume-Job: Reanuda un trabajo por Nombre.


![Screenshot_473](https://user-images.githubusercontent.com/96561825/170150668-bd76e7b0-e702-4544-a83b-cf67084ab804.png)


* Set-Variable: Establece una variable y obtiene su valor.


![Screenshot_474](https://user-images.githubusercontent.com/96561825/170150679-2cae3c68-87de-464a-91ad-0898f68b9cde.png)


* Show-Command: Abre un cmdlet en una ventana de comandos.

![Screenshot_475](https://user-images.githubusercontent.com/96561825/170150685-fd111ca2-db0b-46f9-886a-9322a125fae0.png)

![Screenshot_476](https://user-images.githubusercontent.com/96561825/170150713-a89ca179-ee65-4333-849c-9f908fd5d697.png)


* Sort-Object: Ordena el directorio actual por nombre.

![Screenshot_477](https://user-images.githubusercontent.com/96561825/170150727-be355b0d-2a00-48dd-b6bc-e9a3e5fad20d.png)


* Start-Service: Inicia un servicio detenido.


![Screenshot_478](https://user-images.githubusercontent.com/96561825/170150735-801639cb-4df1-41d0-88a7-75684566de0f.png)


* Start-Process: Inicia un proceso que use valores por defecto.

![Screenshot_479](https://user-images.githubusercontent.com/96561825/170150740-382d5a8e-00bc-4dd9-8c1b-df59a8791955.png)






See you on [Day 11](day11.md).
