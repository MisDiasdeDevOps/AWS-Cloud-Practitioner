


# Configuración y Mantenimiento del sistema.

Retomando los conceptos:

# “La automatización de la infraestructura consiste en el uso de sistemas de software para crear instrucciones y procesos repetibles a fin de reemplazar o reducir la interacción humana con los sistemas de TI.”
#
Plantea una visión muy amplia, ya que tiene que abarcar los diversos rubros de las empresas que poseen su área de sistema, según el tipo de organización en la que trabajamos es el grado de automatización con el que nos vamos a encontrar en la infraestructura de TI. 

Uno de los Roles del equipo de trabajo del área de sistemas es el DEVOPS Engineering, encargado de automatizar los procesos del área de Development y Operations. Su función es hacer más amigable y eficiente la relación entre estos dos equipos de trabajo. 
#
# 1- Infraestructura y servicios.
Primeramente tenemos que analizar los dispositivos tenemos en nuestra red de IT. Si contamos con servidores legacy o servicios contratados por un cloud providers.

De las dos opciones anteriores lo que tenemos que tener en cuenta es el sistema operativo con el que trabajan. (MAC, Linux, Windows) 

De los cloud providers más conocidos contamos con:
-AWS.
-Google Cloud.
-Microsoft Azure.

Para la elección se evalúan los costos y la oferta de servicios que disponen, esta última es cada vez más robusta y completa. (Load balancing, backup, clustering, security, etc).


# 2- Manejo del Código.
Partimos desde donde alojamos nuestro código de trabajo si somos programadores, por excelencia el gestor de versionado e integrador de código más utilizado es GIT.
Los alojamientos de estos repositorios más conocidos en la nube son GitLab, Github, Bitbucket, Gitea, etc.

En estos se almacenan nuestro código de las aplicaciones que pueden estar en lenguajes de programación diversos según lo que necesitemos: 
Python, JS, JAVA, .NET,etc.
Deployar nuestro código también lo podemos automatizar con CI/CD (refiere a las prácticas combinadas de integración continua y entrega continua.​​​)
-Jenkins.
-GitActions.
-JetBrains.

# 3- Contenedores.
Los contenedores se están convirtiendo en el modelo de empaquetado de software del producto que desarrollamos. Virtualización de ambientes de trabajo compatibles transportables, totalmente configurados para que nuestro código funcione en todos los equipos.
-Docker

Cuando manejamos muchos contenedores, tenemos que migrar a un cluster de contenedores, dirigidos por los orquestadores de contenedores.
-Kubernetes.
-Docker Swarn.
   
# 4- Ambientes de trabajo.
Luego nuestro cluster hay que tener en cuenta en cual ambiente está.

En cada ambiente se trabajan con distintas tecnologías según el grado de exposición del producto. Automatizando estos procesos vamos a tener más eficiencia, transparencia, facilidad de replicación y recuperación.
-Ansible.
-Chef.
-Puppet.
-Terraform.


# 5- Monitores de red.
Es muy importante tener la supervisión de nuestros dispositivos que hay en nuestra red y de los servicios, y programar alertas en caso de que suceda algún cambio.
-Nagios.
-Prometheus.
-Icinga2.
-DataDog.


# 6- Lenguajes de Scripting.
Necesitamos trabajar en estrecha colaboración con los desarrolladores y el administrador del sistema para automatizar tareas de los operadores y desarrolladores.(backups, cron jobs, system monitoring).
Según el sistema operativo:
-Bash.
-Powershell.

Lenguajes de scripting independientes del SO:
Python.
-Ruby.
-Go.

El más popular es Python, ya que posee muchas librerías, es de fácil lectura y aprendizaje.

# Conclusión.
Estas tecnologías expuestas para automatizar la infraestructura TI no son todas las que están en el mercado, sino una visión general de lo que hoy son las más populares. Hay que tener en cuenta que cada día se están desarrollando nuevas herramientas y metodologías de trabajo para cada para cada empresa, como también empresas que brindan el servicio de automatización outsourcing de la organización. Siempre hay que tomar la decisión en base a la necesidad, recursos disponibles y experiencia que cuenta la empresa.













