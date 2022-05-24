

# Glosario de comandos

A continuación, veremos algunos de los cmdlets más útiles y más comunes que estaremos usando en Windows Powershell.


# 25 comandos básicos de Windows PowerShell


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


# Ejemplos de uso

* Set-Location : Establece la ubicación actual.

PS C:\> Set-Location -Path "HKLM:\"
PS HKLM:\>


* Get-Content: Obtiene el contenido de un archivo de texto.




* Add-Content: Añade contenido a un archivo de texto.




* Set-Content: Modifica una línea de un archivo de texto.
 



* Copy-Item: Copia un archivo a un directorio específico.





 * Remove-Item: Este ejemplo elimina de la carpeta actual todos los archivos que tienen una extensión de nombre de archivo .doc con la excepción de los que tengan un * 1 * en su nombre.





* Move-Item: Mueve un archivo a otro directorio y lo renombra.





* Set-Item: Este ejemplo crea un alias llamado np para el Notepad de Windows.






* New-Item: Crea un archivo en el directorio actual.





* Start-Job: Ejecuta un script como un proceso en segundo plano.





* Compare-Object: Compara el contenido de dos archivos: 
*
Este ejemplo compara el contenido de dos archivos, el ejemplo usa los siguientes dos archivos de texto, cada uno con un valor en una línea diferente.
verduras.txt contiene los valores: papa, zapallo, tomate.
frutas.txt contiene los valores: banana, tomate, naranja.

El resultado muestra solo las líneas que son diferentes entre los archivos. En verduras.txt usa el objeto de referencia (<=) y en frutas.txt usa el objeto de diferencia (=>). Las líneas que se encuentran en los dos archivos no son mostradas.






* Group-Object: Agrupa archivos por su extensión.





* Invoke-Webrequest: Muestra una página web.



* Measure-Object: este comando cuenta los archivos y carpetas del directorio actual.


* Resolve-Path: Muestra la ruta actual.


* Resume-Job: Reanuda un trabajo por Nombre.






* Set-Variable: Establece una variable y obtiene su valor.




* Show-Command: Abre un cmdlet en una ventana de comandos.


* Sort-Object: Ordena el directorio actual por nombre.



* Start-Service: Inicia un servicio detenido.





* Start-Process: Inicia un proceso que use valores por defecto.






See you on [Day 11](day11.md).
