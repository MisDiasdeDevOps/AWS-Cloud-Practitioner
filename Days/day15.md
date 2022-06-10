


# Implementación de un load balancer
#
#


## Escenario de trabajo


![Screenshot_78](https://user-images.githubusercontent.com/96561825/173112869-06205fc2-b3fd-4b67-8545-13b1e679d79c.png)


#
### Server, instancias o back end del load balancer

Vamos a armar, primero, en nuestra VPC, dos instancias con Ubuntu Server. 

En cada una de ellas se va a deployar un ejemplo de codigo.

Existirá redundancia de dos instancias, pero va a ser la función del balanceador dirigir a los usuarios a cada instancia.

#

### Grupos de seguridad y load balancer

Los grupos de seguridad van a mantener limitados los ingresos a nuestras instancias, permitiendo el ingreso solamente del puerto 80 a través del load balancer.

Este último es nuestro director de orquesta, va a estar constantemente chequeando en qué situación se encuentran nuestros servicios de cada instancia y va a redirigir y organizar el ingreso de los usuarios. Recibe el tráfico directamente desde el Internet de los usuarios y los envía a la instancia más liberada.





# 

## Beneficios de utilizar esta arquitectura


#### ● Bajo costo.

#### ● Continuidad de nuestra app si hubiera algún problema con una instancia.

#### ● Un gateway de seguridad para dejar ingresar solamente a determinados usuarios y puertos.

#### ● Balanceo de carga y mejor uso de los recursos.

#### ● Permite una escalabilidad muy sencilla de aplicar nuestra app.





#
#
#
#
#




See you on [Day16](day16.md)

















