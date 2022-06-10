# Associate Cloud Engineer


Guía para el examen de certificación

Un Associate Cloud Engineer se encarga de implementar y proteger la infraestructura y las aplicaciones, supervisar las operaciones de varios proyectos y mantener las soluciones empresariales a fin de garantizar que cumplan con las métricas de rendimiento. 
#
Esta persona tiene experiencia con nubes públicas y soluciones locales. También sabe cómo usar Google Cloud Console y la interfaz de línea de comandos para realizar tareas comunes en la plataforma a fin de mantener y escalar una o más soluciones implementadas que aprovechen las funcionalidades de servicios administrados por Google o el usuario en Google Cloud.

#
#

# Sección 1.Configura un entorno de solución de nube

### 1.1	Configurar proyectos y cuentas de nube. Las actividades incluyen lo siguiente:

•	Crear una jerarquía de recursos

•	Aplicar políticas de la organización a la jerarquía de recursos

•	Otorgar funciones de IAM a los miembros dentro de un proyecto

•	Administrar usuarios y grupos en Cloud ldentity (de manera manual o automatizada)
•	Habilitación de las API en proyectos

•	Aprovisionar y configurar productos en Google Cloud's operations suite

### 1.2	Administrar la configuración de facturación. Las actividades incluyen lo siguiente:

•	Creación de una o más cuentas de facturación

•	Vinculación de proyectos a una cuenta de facturación

•	Establecimiento de presupuestos y alertas de facturación

•	Configura exportaciones de facturación

### 1.3	Instalación y configuración de la interfaz de línea de comandos {CLI), en particular el SDK de Cloud (p. ej., instalación del proyecto predeterminado).

#
#

# Sección 2. Planifica y configura una solución en la nube

### 2.1	Planificación y estimación del uso de productos de Google Cloud con la calculadora de precios

### 2.2	Planificar y configurar los recursos de procesamiento. Se incluyen las siguientes consideraciones:

•	Selección de las opciones de procesamiento apropiadas para una carga de trabajo determinada (p. ej., Compute Engine, Google Kubernetes Engine, Cloud Run y Cloud Functions)

•	Uso de VM interrumpibles y tipos personalizados de máquinas cuando corresponda

### 2.3	Planificar y configurar opciones de almacenamiento de datos. Se incluyen las siguientes consideraciones:

•	Elección del producto (p. ej., Cloud SQL, Firestore, Cloud Spanner o Cloud Bigtable)

•	Elegir opciones de almacenamiento (p. ej., Disco persistente zonal, disco persistente regional balanceado, Estándar, Nearline, Coldline, Archive)

### 2.4	Planificar y configurar recursos de red. Se incluyen las siguientes tareas:

•	Diferenciación de las opciones de balanceo de cargas

•	Identificación de las ubicaciones de recursos en una red para conocer la disponibilidad

•	Configuración de Cloud DNS

#
#

# Sección 3. Implementa una solución en la nube


### 3.1	Implementar y utilizar recursos de Compute Engine. Se incluyen las siguientes tareas:

•	Iniciación de una instancia de procesamiento con Cloud Console y el SDK de Cloud (gcloud) (p. ej., asignar discos, política de disponibilidad o claves SSH)

•	Creación de un grupo de instancias administrado y con ajuste de escala automático mediante una plantilla de instancias

•	Generar o subir una Llave SSH personalizada para las instancias

•	Instala y configura el agente de Cloud Monitoring y Logging

•	Evaluación de las cuotas de procesamiento y solicitud de aumentos

### 3.2	Implementación de recursos de Google Kubernetes Engine. Se incluyen las siguientes tareas:

•	Instalar y configurar la interfaz de línea de comandos (CU) para Kubernetes (kubectl)

•	Implementa un clúster de Google Kubernetes Engine con diferentes opciones de configuración, como AutoPilot, clústeres regionales, clústeres privados, etcétera.

•	Implementa una aplicación en contenedores en Google Kubernetes Engine

•	Configurar la supervisión y el registro de la aplicación de Google Kubernetes Engine

### 3.3	Implementa los recursos de Cloud Run y Cloud Functions. Se incluyen las siguientes tareas, cuando corresponda:

•	Implementación de una aplicación y actualización de la configuración de escalamiento, versiones y división de tráfico

•	Implementación de una aplicación que reciba eventos de Google Cloud (p. ej., eventos de Cloud Pub/Sub o eventos de notificación de cambio de objeto de Cloud Storage)

### 3.4	Implementa y utiliza soluciones de datos. Se incluyen las siguientes tareas:

•	Inicialización de sistemas de datos con productos (p. ej., Cloud SQL, Firestore, BigQuery, Cloud Spanner, Pub/Sub, Cloud Bigtable, Dataproc, Dataflow, Cloud Storage)

•	Carga de datos (p. ej., carga mediante la línea de comandos, transferencia por medio de API, importación y exportación, carga de datos desde Cloud Storage o transmisión de datos a Cloud Pub/Sub)

### 3.5	Implementa recursos de herramientas de redes. Se incluyen las siguientes tareas:

•	Creación de una VPC con subredes (p. ej.,VPC en modo personalizado o VPC compartida)

•	Lanzamiento de una instancia de Compute Engine con configuración de redes personalizada (p. ej.,dirección IP solo interna, acceso privado a Google, dirección IP externa y privada estáticas, y etiquetas de red)

•	Crear reglas de firewall de entrada y salida para una VPC (p. ej., subredes de IP, etiquetas y cuentas de servicio)

•	Creación de una VPN entre una VPC de Google y una red externa usando la VPN de Cloud

•	Creación de un balanceador de cargas para distribuir el tráfico de red de aplicaciones en una aplicación (p. ej., balanceador de cargas de HTTP(S) global, balanceador de cargas de proxy de SSL global, balanceador de cargas de proxy de TCP global, balanceador de cargas de redes regional o balanceador de cargas interno regional)

### 3.6	Implementa una solución con Cloud Marketplace. Se incluyen las siguientes tareas:

•	Exploración del catálogo de Cloud Marketplace y visualización de la información de las soluciones

•	Implementar una solución de Cloud Marketplace

### 3.7	Implementa recursos a través de la infraestructura como código. Se incluyen las siguientes tareas:

•	Compila infraestructura mediante plantillas de Cloud Foundation Toolkit y realiza prácticas recomendadas


•	Instala y configura Config Connector en Google Kubernetes Engine para crear, actualizar, borrar y proteger recursos

#
#
# Sección 4. Asegura la operación exitosa de una solución en la nube


### 4.1	Administración de recursos de Compute Engine. Se incluyen las siguientes tareas:

•	Administración de una única instancia de VM (p. ej., iniciar, detener, borrar o editar la configuración de una instancia)

•	Conéctate a la instancia de forma remota

•	Adjunta una GPU a una instancia nueva e instala las dependencias necesarias

•	Visualización del inventario en ejecución actual de la VM (ID de las instancias y detalles)

•	Trabajo con instantáneas (p. ej., crear una instantánea a partir de una VM, ver instantáneas o borrar una)

•	Trabajo con imágenes (p. ej.,crear una imagen a partir de una VM o una instantánea y ver o borrar imágenes)

•	Trabajo con grupos de instancias (p. ej.,establecer parámetros de ajuste de escala automático, asignar plantillas de instancia, crear una plantilla de instancia o quitar grupos de instancias)

•	Trabajo con interfaces de administración (p. ej., Cloud Console, Cloud Shell o el SDK de Cloud)

### 4.2	Administra los recursos de Google Kubernetes Engine. Se incluyen las siguientes tareas:

•	Visualización del inventario en ejecución actual del clúster (nodos, pods y servicios)

•	Explora imágenes de Docker y visualiza sus detalles en Artifact Registry

•	Trabajo con grupos de nodos (p. ej., agregar, editar o quitar un grupo de nodos)

•	Trabajo con pods (p. ej., agregar,editar o quitar pods)

•	Trabajo con servicios (p. ej., agregar, editar o quitar un servicio)
 
•	Trabajo con aplicaciones con estado (p. ej.,volúmenes persistentes o conjuntos con estado)

•	Administración de la configuración del ajuste de escala automático horizontal y vertical

•	Trabajar con interfaces de administración (p. ej., Cloud Console, Cloud Shell, SDK de Cloud o kubectl)

### 4.3	Administra recursos de Cloud Run. Se incluyen las siguientes tareas:

•	Ajuste de los parámetros de división de tráfico de la aplicación

•	Establecimiento de parámetros de escalamiento para instancias con ajuste de escala automático

•	Determina si deseas ejecutar Cloud Run (completamente administrado) o Cloud Run for Anthos

### 4.4	Administra soluciones de almacenamiento y base de datos. Se incluyen las siguientes tareas:

•	Administra y protege objetos dentro y entre buckets de Cloud Storage

•	Establecimiento de políticas de administración del ciclo de vida del objeto para los depósitos de Cloud Storage

•	Realización de consultas para obtener datos de las instancias de datos (p. ej., Cloud SQL, BigQuery, Cloud Spanner, Cloud Datastore o Cloud Bigtable)

•	Estima los costos de los recursos de almacenamiento de datos

•	Crear copias de seguridad y restablecer instancias de datos (p. ej., Cloud SQL, Datastore)

•	Revisión del estado del trabajo en Dataproc, Dataflow o BigQuery

### 4.5	Administrar recursos de herramientas de redes. Se incluyen las siguientes tareas:

•	Adición de una subred a una VPC existente

•	Expandir una subred para tener más direcciones IP

•	Reserva de direcciones IP estáticas externas o internas

•	Trabaja con Cloud DNS, Cloud NAT, los balanceadores de cargas y las reglas de firewall

### 4.6	Supervisión y registro. Se incluyen las siguientes tareas:

•	Crea alertas de Cloud Monitoring basadas en métricas de recursos

•	Crear y transferir métricas personalizadas de Cloud Monitoring (p. ej., de aplicaciones o registros)

•	Configuración de receptores de registros para exportar registros a sistemas externos (p. ej., a nivel local o en BigQuery)

•	Configura routers de registro

•	Visualización y filtrado de registros en Cloud Logging

•	Visualización de detalles de mensajes de registro específicos en Cloud Logging

•	Uso de los diagnósticos de nube a fin de investigar el problema de una aplicación (p. ej., ver datos de Cloud Trace o usar Cloud Debug para ver una aplicación en un momento determinado)

•	Visualización del estado de Google Cloud

#
#

# Sección 5. Configura el acceso y la seguridad


### 5.1	Gestiona la administración de identidades y accesos (IAM). Se incluyen las siguientes tareas:

•	Visualiza las políticas de IAM

•	Crea políticas de IAM

•	Administración de los distintos tipos de funciones y definición de funciones de IAM personalizadas (p. ej., primitivas, predefinidas y personalizadas)

### 5.2	Administrar cuentas de servicio. Se incluyen las siguientes tareas:

•	Crea cuentas de servicio

•	Usa cuentas de servicio en políticas de IAM con permisos mínimos
•	Asigna cuentas de servicio a los recursos

•	Administra la IAM de una cuenta de servicio

•	Administra el robo de identidad de cuentas de servicio

•	Crea y administra credenciales de cuenta de servicio de corta duración

### 5.3 Consulta los registros de auditoría


fin

#
#
#
#
#

Nos vemos el [Dia 3](day03.md).  



