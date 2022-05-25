
# Administrador de tareas vs. Explorador de procesos

##  Process Explorer

### Serie Systernals
#





El Administrador de Tareas de Windows, también conocido como Administrador de Tareas es una característica del sistema operativo Windows, que es una de las utilidades más importantes y poderosas. Puede administrar las tareas, aplicaciones y servicios que se ejecutan y también puede matarlas/terminarlas. También es una herramienta de monitoreo, que puede ser usada para monitorear el uso del disco duro, la memoria, la CPU y la red. Matar una aplicación que no responde o que se comporta mal es una de las características más utilizadas del Administrador de Tareas. Además, a partir de Windows 8, el Administrador de tareas también cuenta con la función de inicio, que gestiona las aplicaciones de inicio desde donde se pueden habilitar/deshabilitar las aplicaciones que están configuradas para ejecutarse cuando se inicia la ventana.

Sin embargo, existe una aplicación disponible que también puede utilizarse como alternativa al Task Manger, diseñada para usuarios avanzados y que se llama Process Explorer. Process Explorer forma parte de las herramientas de diagnóstico de la familia Sysinternals que distribuye gratuitamente Microsoft. Process Explorer es la herramienta más utilizada entre ellas.

Process Explorer puede darle mucha más información y control sobre todas las aplicaciones, procesos y servicios que se están ejecutando en su ordenador y también incluye todas las características que tiene el Administrador de Tareas. El Explorador de Procesos puede rastrear una aplicación hasta el último archivo DLL que esté usando.

****Process Explorer se ejecuta sin instalación, simplemente tienes que ejecutar un archivo muy pequeño haciéndolo portátil. En esta guía, compararemos el Administrador de Tareas con el Explorador de Procesos si desea usar el Explorador de Procesos, esta guía le ayudará.****


El Administrador de tareas puede ser utilizado por un usuario para saber qué aplicaciones, procesos, servicios se están ejecutando y también para controlar su prioridad y el número de procesadores que pueden utilizar (afinidad) También puede proporcionarle información sobre el uso de la CPU, la memoria y la red de su ordenador – ya que el Administrador de tareas está diseñado para uso doméstico y básico, no ayudará en la depuración y no proporciona un análisis extenso y detallado sobre los procesos en ejecución.

Process Explorer te da toda la información de una manera muy detallada y ordenada con muchas características extras también. 


Algunas se mencionan a continuación, pero no son casi todas las características que están allí en la interfaz del Explorador de Procesos.

Si quieres probar las características que aparecen a continuación también, te recomendamos que descargues el Explorador de Procesos (muy pequeño en tamaño, 1,2 MB para ser exactos) y lo mantengas funcionando a través de la guía.


#
#
# Interfaz de usuario avanzada

El administrador de tareas se ha mantenido prácticamente igual en términos de interfaz de usuario. Un usuario puede encontrar especialmente confusas las pestañas de proceso si está buscando un único proceso objetivo para supervisar o matar o para ver qué aplicación lo está utilizando. Todos los procesos se verían igual a un ojo menos experto en tecnología.

El Explorador de Procesos es una clara victoria en este caso. Separa con cuidado y precisión los procesos centrales del sistema en color rosa y sus propios procesos iniciados manualmente en color azul. Todos los procesos tendrían su icono asociado junto a ellos y su descripción también.

Además, su vista de árbol organiza los procesos de tal manera que se puede conocer fácilmente el proceso padre de un proceso objetivo en el que se está ejecutando.

Los gráficos de monitorización de la CPU, la GPU, la red y el disco también se pueden ver en la parte superior y se pueden ampliar si se hace clic en ellos.

![Screenshot_493](https://user-images.githubusercontent.com/96561825/170158003-282307c8-7d25-4e64-9d55-da8320377000.png)





#
#
# Desbloquear archivos y carpetas

El Explorador de Procesos también es una gran herramienta para la resolución de problemas. Si no puede eliminar un archivo/carpeta aunque haya cerrado todos los programas, puede ayudarle a rastrear el proceso y/o los manejadores DLL que siguen bloqueando innecesariamente el archivo/carpeta. Entonces podrás eliminarlos.

Para ello, simplemente abra Process Explorer y haga clic en el icono Binoculares en la parte superior. Teclea en el nombre del archivo/carpeta y haz clic en Search .





![Screenshot_494](https://user-images.githubusercontent.com/96561825/170158032-859377c7-85f7-489d-b37b-5849e5270081.png)






Seleccione cada proceso en los resultados y ciérrelos volviendo a la ventana del Explorador de Procesos, luego Haga clic con el botón derecho del ratón en el proceso del manejador objetivo y haga clic en Cerrar Manejar/Matar Proceso.





![Screenshot_495](https://user-images.githubusercontent.com/96561825/170158075-5726e1b4-63dd-4670-93f0-9418b6aa5736.png)






#
#
# Información detallada/Análisis


En la ventana Process Explorer , haga doble clic en el proceso para ver su información detallada.En la ventana de propiedades, puede ver su ubicación, el directorio temporal actual, la ubicación de inicio automático (si está configurado para ejecutarse automáticamente), el uso detallado de los recursos informáticos agrupados en red, el uso del disco y la CPU y mucho más.






![Screenshot_496](https://user-images.githubusercontent.com/96561825/170158137-d1c2a2f4-6f6f-4897-8018-c563e97ce952.png)








#
#
# Proceso de la aplicación de rastreo

Si desea rastrear un proceso, y su archivo asociado, simplemente arrastre el icono de la cruz a la aplicación y le mostrará todos los procesos relacionados/ asociados.






![Screenshot_497](https://user-images.githubusercontent.com/96561825/170158204-fd95372f-791e-4647-b7a2-179f09493e1d.png)








#
#
# Comprobación del proceso / Total de virus

El Explorador de Procesos puede escanear el proceso en línea, y también puede buscar virus en el proceso.



![Screenshot_498](https://user-images.githubusercontent.com/96561825/170158239-c3ecee17-ab54-475b-bc30-d3a01f43d643.png)

#
#
# Accesibilidad / Atajos

El Administrador de Tareas está incorporado en Windows y hay varias formas de acceder a él, como los siguientes atajos de teclado.

Pulsar y Mantener Ctrl tecla + Mayúsculas tecla + Esc

Presionar y Mantener Tecla Ctrl + Tecla Alt + Suprimir Luego hacer clic en Iniciar el Administrador de tareas .

Haga clic con el botón derecho en la barra de tareas y haga clic en Iniciar el Administrador de tareas .

Presione y mantenga presionada la tecla Windows y presione X . Pulsa Administrador de tareas . (Sólo en Windows 8 y posteriores)

También se puede acceder al Explorador de Procesos de la misma manera si se reemplaza. Para reemplazar el Administrador de Tareas por el Explorador de Procesos, Abra el Explorador de Procesos . Haga clic en en Opciones en la barra de menú y haga clic en Reemplazar el Administrador de Tareas .



![Screenshot_499](https://user-images.githubusercontent.com/96561825/170158321-a6ee1949-86cc-4ec9-98b8-8c99402cbea2.png)



Ahora podrá ejecutar el Explorador de Procesos de la misma manera que ejecutaría el Administrador de Tareas.Así que como puedes ver, esto no fue una gran competencia ya que Process Explorer es claramente más poderoso que el administrador de tareas.












#
#
#
#




See you on [Day17](day17.md)
