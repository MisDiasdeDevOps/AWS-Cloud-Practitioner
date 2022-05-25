
# Acerca de los módulos de PowerShell



## ¿Qué es un módulo?

Como mencionamos antes, un módulo es un paquete que contiene objetos de PowerShell, como cmdlets, proveedores, funciones, flujos de trabajo, variables y alias. Los objetos u acciones de este paquete se pueden implementar en un script de PowerShell, una DLL compilada o una combinación de ambos. Por lo general, estos archivos se agrupan en un solo directorio. 

Las personas que escriben comandos pueden usar módulos para organizar sus comandos y compartirlos con otros. Las personas que escriben módulos pueden agregar los comandos en los módulos a sus sesiones de PowerShell y usarlos como  comandos integrados.

#

## Carga automática de los módulos


A partir de PowerShell 3.0, PowerShell importa módulos automáticamente la primera vez que ejecuta cualquier comando en un módulo instalado. Ahora pueden usar los comandos en un módulo sin ninguna configuración o configuración de perfil, por lo que no es necesario administrar los módulos después de instalarlos en su computadora. 


Los comandos de un módulo también son más fáciles de encontrar. El cmdlet Get-Command obtiene todos los comandos en todos los módulos instalados, incluso si aún no están en la sesión. Pueden encontrar un comando y usarlo sin importar la necesidad de importar el módulo primero. Solo los módulos que se almacenan en la ubicación especificada por la variable de entorno PSModulePath se importan automáticamente.


Los comandos que incluyen un carácter comodín (*) se consideran para descubrimiento, no para uso y no importan ningún módulo.

Los módulos en otras ubicaciones deben importarse ejecutando el Import-Module cmdlet.

#
#
#
#
#

















See you on [Day19](day19.md)
