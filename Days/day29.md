# Aqui encontraran una lista de los Comandos mas importantes y Utiles para realizar los desafios del Bootcamp, tanto de los Desafios como del material de Alumni.

Comenzemos.

## 1. Get-Help 

Si eres nuevo en PowerShell, puedes tener problemas; y en tales situaciones, Get-Help se convierte en tu salvador. Proporciona la información necesaria sobre cmdlets,
comandos, funciones, scripts y flujos de trabajo de PowerShell.

Además, es fácil: necesitas escribir Get-Help seguido del comando, del cual, buscas los detalles. Por ejemplo, puedes obtener información sobre el uso de “Get-Process”, usando:Get-Help Get-Process


![Screenshot_5](https://user-images.githubusercontent.com/96561825/172929076-83f3144b-cdb0-4d7c-81b5-05a3f36cacde.png)




## 2. Get-Command

Windows PowerShell permite descubrir sus comandos y características mediante Get-Command. Muestra la lista de comandos de una función específica o para un propósito específico basado en tu parámetro de búsqueda.

Solo necesitas escribir Get-Command seguido de tu consulta de búsqueda en PowerShell.

Por ejemplo,
Get-Command *-service*

muestra comandos que llevan “-service” en su nombre. Recuerda utilizar los asteriscos en ambos lados de la consulta porque es un comodín que ayuda a buscar lo desconocido.

Comando Get-Command en PowerShell

![Screenshot_6](https://user-images.githubusercontent.com/96561825/172929132-ca1fcced-a006-432b-a130-90c32b0cf3c9.png)




## 3. Invoke-Command

Cuando desees ejecutar un comando o un script de PowerShell, local o remotamente en una o varias computadoras, “Invoke-Command” es tu amigo. Es fácil de usar y te ayuda a controlar las computadoras por lotes.

Deberás escribir Invoke-Command seguido del comando o la secuencia de comandos con su ruta completa. Por ejemplo, puedes ejecutar un comando “Get-EventLog” usando:

Invoke-Command -ScriptBlock {Get-EventLog system -Newest 50}

o en una computadora remota “Server01” usando:

Invoke-Command -ScriptBlock {Get-EventLog system -Newest 50} -ComputerName Server01 

En el ejemplo anterior: “Server01” representa el nombre de la PC remota o la dirección IP.

“Get-EventLog system -Newest 50” es el comando que desea ejecutar.



## 4. Invoke-Expression

Invoke-Expression proporciona una forma de ejecutar un script desde Windows PowerShell, además puede ejecutar una función por una variable. Si estás proporcionando una expresión o una cadena como entrada, este comando primero la evalúa, luego la ejecuta, pero también funciona localmente, a diferencia del comando
anterior.

Invoke-Expression c:\scripts\prueba.ps1

Debes escribir Invoke-Expression seguido de un comando o una expresión. Por ejemplo, puedes asignar una variable “$Comando” con una cadena que indique el comando
“Get-Process“. El siguiente comando ejecuta “Get-Process” como un comando en tu computadora local.

$Comando="Get-Process"
Invoke-Expression $Comando


![Screenshot_7](https://user-images.githubusercontent.com/96561825/172929156-10625e55-32fc-430f-baf3-a07ea24753eb.png)



## 5. Invoke-WebRequest

Puede descargar, iniciar sesión y buscar información sobre sitios web y servicios web mientras trabajas en Windows PowerShell utilizando Invoke-WebRequest.
Debe usar Invoke-WebRequest seguido de sus parámetros. Por ejemplo, puedes obtener los enlaces en una página web dada usando el siguiente comando: (Invoke-WebRequest -Uri "https://esgeeks.com").Links.Href

![Screenshot_8](https://user-images.githubusercontent.com/96561825/172929174-48553f84-1fab-4121-9f12-daad357c984a.png)


## 6. Set-ExecutionPolicy 

Aunque la creación y ejecución de scripts (que tienen la extensión “ps1“) en Windows PowerShell es posible; existen restricciones por motivos de seguridad. Así que puedes cambiar el nivel de seguridad utilizando el comando Set-ExecutionPolicy.
Puedes escribir Set-ExecutionPolicy seguido de uno de los cuatro niveles de seguridad: 

Restricted, Remote Signed, All Signed, o Unrestricted. Por ejemplo, puedes asignar el estado de política restringida usando:
Set-ExecutionPolicy -ExecutionPolicy Restricted


![Screenshot_9](https://user-images.githubusercontent.com/96561825/172929194-43f4534d-9151-4c13-ac19-4d9cecdd856c.png)



## 7. Get-Item 

Si buscas información sobre un elemento en cualquier ubicación determinada, por ejemplo, un archivo de tu disco duro, Get-Item es la mejor manera de conseguirlo en Windows PowerShell. Debes saber que no obtienes el contenido del elemento, como archivos y subdirectorios en un directorio determinado, a menos que lo especifiques explícitamente.

Debes escribir Get-Item seguido de una ruta o una cadena junto con sus parámetros, si corresponde. Por ejemplo, puedes usar todos los elementos (archivos o carpetas) que comiencen con “M” en el directorio actual, así:Get-Item M*


![Screenshot_10](https://user-images.githubusercontent.com/96561825/172929258-028a6bc5-dfb6-4cff-a275-86a811c88eda.png)




## 8. Copy-Item 

Si necesitas copiar archivos y directorios en tu disco de almacenamiento o entradas y claves de registro, puedes usar Copy-Item. Funciona de manera similar al comando “cp” que tenemos en el Símbolo del sistema, pero es mucho mejor.

También puede utilizar el comando Copy-Item para copiar y cambiar el nombre de los elementos en el mismo comando; proporcionando un nuevo nombre como destino. Por
ejemplo, puedes copiar y renombrar “Geek.htm” a “Geeks.txt”, usando: Copy-Item "Geek.htm" -Destination "D:\BLOG\Geeks.txt"


## 9. Remove-Item

Si deseas eliminar elementos como archivos, carpetas, funciones, claves de registro y variables, Remove-Item es el comando ideal. Lo que me pareció interesante es que proporciona parámetros para incluir y excluir elementos.

Puedes utilizar el comando Remove-Item para eliminar elementos de ubicaciones específicas mediante parámetros. Por ejemplo, puedes eliminar el archivo “Geek.txt” con el comando: Remove-Item "C:\Users\Alex\Desktop\Geek.txt"

## 10. Get-Content

Cuando necesitas ver el contenido de un archivo de texto en un lugar específico, puedes abrir y leerlo en un editor de código/texto como Notepad++. 

En Windows PowerShell, puedes usar Get-Content para recuperar el contenido sin abrir el archivo.

Por ejemplo, puedes recuperar 50 líneas de contenido de “Geek.txt”, así: Get-Content "C:\Users\Alex\Desktop\Geek.txt" -TotalCount 50


## 11. Set-Content

Puedes guardar texto en archivos usando Set-Content, similar al comando “echo” del Bash Shell. En combinación con Get-Content, también puedes recuperar el contenido de un archivo y copiarlo en otro archivo usando este comando.

Por ejemplo, puedes usar Set-Content para escribir o reemplazar el contenido de un archivo con contenido nuevo. Además, puedes agruparlo con el ejemplo del comando anterior para guardar su salida en un nuevo archivo llamado “EsGeeks.txt”, usando: Get-Content "C:\Users\Alex\Desktop\Geek.txt" -TotalCount 50 | Set-Content
"C:\Users\Alex\Desktop\EsGeeks.txt"


## 12. Get-Variable

Si estás buscando usar variables en Windows PowerShell, el comando Get-Variable te ayuda a visualizar los valores de las variables. Los muestra en forma de tabla y permite incluir, excluir y usar comodines.

Puedes usar este comando escribiendo Get-Variable seguido de sus opciones y parámetros. Por ejemplo, se puede recuperar el valor de una variable llamada “Var” usando
el siguiente código:

$Var="Get-Process"
Get-Variable -Name "Var"



## 13. Set-Variable

Puedes asignar, cambiar o restablecer el valor de una variable usando el comando Set-Variable. Como atajo, también puedes establecer una variable simple usando el
formato {$NombreVar = ValorVar}, algo como $var = “Descripción”.

Puedes usar el comando Set-Variable seguido de sus parámetros para establecer una variable. Por ejemplo, podemos establecer el valor para una variable llamada “var” usando el comando: Set-Variable -Name "var" -Value "Descipción"


![Screenshot_11](https://user-images.githubusercontent.com/96561825/172929288-7897f95d-6069-47af-b9b8-d02cdf18dec7.png)



## 14. Get-Process

Usualmente usamos el Administrador de tareas para encontrar los procesos en ejecución de nuestra computadora. En Windows PowerShell, cualquier usuario puede usar Get-Process para obtener la lista de los procesos que se están ejecutando actualmente.

Puedes escribir el comando Get-Process junto con tu consulta de búsqueda. Por ejemplo, si necesitas información sobre los procesos con el nombre “explore”, puedes escribir lo siguiente: (ten en cuenta los asteriscos) Get-Process *explore*

## 15. Start-Process

Windows PowerShell facilita el inicio de uno o más procesos en tu computadora. Descubrí que este comando es útil en las aplicaciones de scripting, ya que es uno de los comandos imprescindibles que necesitarás para automatizar una tarea.

Puedes escribir Start-Process seguido de sus parámetros para usar el comando. Por ejemplo, puedes iniciar el Bloc de notas escribiendo lo siguiente: Start-Process -FilePath "notepad" -Verb runAs


## 16. Stop-Process

Puedes detener instancias específicas o todas las instancias de un proceso que se ejecuta en tu computadora utilizando su nombre o PID (ID de proceso), gracias al comando Stop-Process. Lo que lo hace atractivo es que puede detectar un proceso detenido o no, e incluso puede detener los procesos que el usuario actual no posee ni inicia.

Puedes escribir el comando Stop-Process seguido de sus parámetros para detener los procesos dados. Por ejemplo, puedes detener todos los procesos de Bloc de notas usando el comando: Stop-Process -Name "notepad"



## 17. Get-Service

Cuando necesites información sobre servicios específicos (en ejecución o detenidos) en tu computadora, puedes usar Get-Service. Muestra los servicios instalados en tu sistema y proporciona opciones para filtrarlos, incluirlos y excluirlos.

Si deseas utilizar este comando, puedes escribir Get-Service seguido de sus parámetros.

Por ejemplo, escribe lo siguiente para obtener los servicios “en ejecución” de tu sistema: Get-Service | Where-Object {$_.Status -eq "Running"}


![Screenshot_12](https://user-images.githubusercontent.com/96561825/172929308-01edda59-3324-4bcd-a82a-63fb95e09717.png)



## 18. Start-Service

Si deseas iniciar un servicio en tu computadora, el comando Start-Service puede ayudarte a hacer lo mismo desde Windows PowerShell. Descubrí que es lo suficientemente potente como para iniciar un servicio, incluso si ese servicio está desactivado en tu computadora.

Debes especificar el nombre del servicio mientras usas el comando Start-Service. Por ejemplo, el siguiente comando inicia el servicio “Búsqueda de Windows” en tu computadora local: Start-Service -Name "WSearch" 


## 19. Stop-Service

Si deseas detener la ejecución de servicios en tu computadora, el comando Stop-Service será útil. Debes especificar el nombre del servicio junto con Stop-Service. Por ejemplo, escribe lo siguiente para detener el servicio “Búsqueda de Windows” en tu computadora: Stop-Service -Name "WSearch"


## 20. ConvertTo-HTML 

PowerShell puede proporcionar información asombrosa sobre tu sistema. Sin embargo, lo presenta principalmente en un formato ‘indigerible’, por eso puedes usar ConvertTo-HTML para crear y formatear un informe y analizarlo o enviarlo a alguien.

Puedes usar ConvertTo-HTML junto con la salida de otro comando usando pipes (|). Por ejemplo, el siguiente comando muestra la lista de todos los servicios, y su estado, en forma de un informe web, que se almacena en el archivo “Servicios.htm”: Get-Service | ConvertTo-HTML -Property Name, Status > C:\Users\Gino\Desktop\Servicios.htm


fin

#
#
#
#
#





See you on [Day 30](day30.md)
