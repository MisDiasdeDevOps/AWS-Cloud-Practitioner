

# Desafio Inicial : Instalar Windows 7 en una VBOX

Este desafio entregable debe cargarse con las capturas de pantalla de acuerdo a lo consignado en el drive para la correcion del tutor.

## Configurar la máquina virtual

Actualmente existen varias máquinas virtuales para Windows, Mac y Linux, tanto gratuitas como de pago. Sin embargo, en este caso utilizaremos VirtualBox por ser gratuito, multiplataforma y muy fácil de utilizar.

Así que descarga VirtualBox desde su sitio web y procede a instalarlo en tu PC o Mac. Una vez instalado, sigue los pasos a continuación para crear una nueva máquina virtual:

1. Abre VirtualBox y haz clic en la opción “Nueva”


![Screenshot_13](https://user-images.githubusercontent.com/96561825/172943248-d849d112-0e9a-4565-85d2-18320eab0ad6.png)



2. Escribe un nombre y selecciona Windows 7 (Utilizaremos una version mas desactualizada para los ejercicios , no elijan Windows 10 ) (de 32 o 64 bits) como la versión
a instalar.

![Screenshot_14](https://user-images.githubusercontent.com/96561825/172943310-f05a0d74-320a-427c-95e8-45275a6a1d51.png)

3. Indica la cantidad de memoria RAM que quieres asignar. Ten en cuenta que, de acuerdo a los requisitos de Windows 7 necesitas por lo menos 1 GB para 32 bits y 2 GB para 64 bits.


![Screenshot_15](https://user-images.githubusercontent.com/96561825/172943384-c9bd4e30-4093-48a8-8d28-0ea54e2c8373.png)


4. En la siguientes ventanas, deja la opciones por defecto: “Crear un disco duro virtual ahora” y “VDI” como tipo de archivo de disco duro.



5. Ahora puedes elegir entre “Reservado dinámicamente” o “Tamaño fijo”. Recomendamos
elegir la primera opción (por defecto)

![Screenshot_16](https://user-images.githubusercontent.com/96561825/172943666-472bd6de-8358-4d47-a1a5-4c9ea728d635.png)


6. Finalmente, asigna el tamaño del disco duro. Windows 10 necesita 16 GB (32 bits) o 32 GB (64 bits) para instalarse. Pero lo mejor es seguir la recomendación de VirtualBox y asignarle 50 GB.

¡Listo! Con esto ya tienes creada la máquina virtual.


#
# 3. Instalar Windows 10 en VirtualBox

Sigue estos pasos para instalar Windows 10 en máquina virtual:

1. Haz clic en el botón “Iniciar”

![Screenshot_17](https://user-images.githubusercontent.com/96561825/172943837-076a31df-e849-4c08-941c-f9ea42f46845.png)


2. En la ventana que se abre, haz clic en el ícono de la carpeta y luego en “Añadir”. Ahora selecciona la ISO de Windows 10 que has descargado anteriormente. Continua haciendo clic en Abrir, Seleccionar y luego en Iniciar.



![Screenshot_18](https://user-images.githubusercontent.com/96561825/172943887-509006ac-9fb4-4e6e-a836-78c6f026c243.png)


3. Ahora iniciará el instalador de Windows 10. En la primera ventana indica el idioma, formato de hora y teclado. Haz clic en Siguiente para continuar.


![Screenshot_19](https://user-images.githubusercontent.com/96561825/172944021-e7c74cfc-c19d-4ed7-a8d8-c10b13ac97df.png)

4. En la siguiente ventana, haz clic en “Instalar Ahora” ,  haciendo clic en “No tengo una clave de producto”.

![Screenshot_20](https://user-images.githubusercontent.com/96561825/172944208-097a419f-28c9-4f6a-a148-6e5e9786a85d.png)

6. Acepta el acuerdo de licencia

7. Clic en la segunda opción “Personalizada”

![Screenshot_21](https://user-images.githubusercontent.com/96561825/172944329-62b92e2c-be4c-47d3-a4d8-6d58c48d19d9.png)

8. Selecciona la unidad de disco y haz clic en “Siguiente”. También puedes crear nuevas particiones si los deseas.


![Screenshot_22](https://user-images.githubusercontent.com/96561825/172944737-c37ecd67-36c3-46c0-a541-29b7156b033d.png)

9. Espera a que se instale Windows 10. Puede tardar unos minutos y reiniciarse durante el proceso.

![Screenshot_23](https://user-images.githubusercontent.com/96561825/172944891-db1e1fc4-db7c-45b4-9dd8-5b84d3b0ce9d.png)


10. Termina de configurar tu sistema

![Screenshot_24](https://user-images.githubusercontent.com/96561825/172944930-5c76d72c-3f73-4388-a822-32895e33989f.png)

Eso es todo. Ahora puedes empezar a utilizar el sistema operativo en la máquina virtual.


![Screenshot_25](https://user-images.githubusercontent.com/96561825/172945046-c347f512-6413-431f-bcd2-7c2b22dfeebf.png)


# 4. Configuraciones adicionales


Después de la instalación, hay algunas configuraciones que creemos que son importantes y
que debes llevaras a cabo.

Nos referimos a las Guest Additions, un complemento de VirtualBox que permite que la máquina virtual se comunique con el anfitrión. Por ejemplo, mover el mouse entre la MV y tu sistema principal o compartir carpetas entre ambos. 

Sigue estos pasos para instalar las Guest Additions:

1. Haz clic en el menú “Dispositivos”

2. Selecciona «Insertar imagen de CD de las Guest Additions»

3. Abre el Explorador de archivos y ubícate en “Este equipo”

4. Clic en VirtualBox Guest Additions (que está montado como si fuera un disco)

5. Clic en VBoxWindowsAdditions.exe y procede con la instalación

![Screenshot_26](https://user-images.githubusercontent.com/96561825/172945231-1325a095-fc91-46c4-8297-85cddeba558f.png)


Adicionalmente puedes ir al menú “Dispositivos”, seleccionar Portapapeles compartido y luego “Bidireccional”. Lo mismo para Arrastrar y soltar. El primero permite compartir archivos entre la máquina virtual y tu sistema principal, mientras que el segundo permite arrastrar y soltar archivos entre ambos.

![Screenshot_27](https://user-images.githubusercontent.com/96561825/172945343-0641b655-38d1-49f1-9a97-21d0d4076eb3.png)

Para aplicar los cambios, reinicia el sistema.



#
#
#
#
#


See you on [Day 31](day31.md)
