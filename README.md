# Arquitectura-de-Software
En este repositorio abarcaremos la gran mayoria de temas relacionados con arquitectura de software y daremos algunos ejemplos de estos paradigmas aplicados en proyectos de programacion.

## ¿Que es arquitectura de software? 
No hay una definicion especifica para este tema, pero si se puede intentar dividir en conceptos mas pequeños para lograr entenderlo de mejor manera.
**1)Estructura**
-Es lo que me permite como organizar cada parte del sistema y como se complementan entre si.
**2)Razonar**
-La Arquitectura de software sirve para poder discutir y razonzar a cerca  del sistema que se esta queriendo implementar.En este cao sirve para que el queipo de desarrollo pueda disctuir  sobre los requerimientos de su sistema, como va a funcionar y que patrones o elementos implementar.

![architecture](https://github.com/Luiscvj/Arquitectura-de-Software/assets/130381389/b4b79e1b-836e-44cf-bb88-faa562b883ce)

Ademas de esto tambien se  puede entender como la capacidad para tomar **desiciones de diseño**  importantes que permiten organizar el software y promover los **atributos de calidad** deseados, que en otras palabras como arquitecto se decide que tipo de patron usar segun los requerimientos de mi aplicacion para buscar  la mayor calidad  en la misma , como :
**-Escalabilidad**
**-Seguridad**
**-Desplegabilidad**


 ## ¿Que son los patrones de diseño?
*Son  soluciones habituales a problemas comunes  en el diseño de software , es decir cada uno es como un plano que se puede personalizar para resolver un problema de diseño particular del codigo.
## ¿Que son los Patrones de Arquitectura?
Son soluciones  generales  de ingenieria de software que se repiten a menudo  definiendo  la aplicacion desde el nivel mas grande y permiten los siguientes beneficios:
**1)Cambios iniciales en el diseño.**
**2)Sistemas optimizados.**
**3)Puente de comunicacion.**
Es decir me da el lineamiento para empezar a definir la estructura de mi aplicacion.

**Ejemplo**

### Arquitectura en tres capas 

Es un patron arquitectonico que consta de las siguientes capas:

**Presentacion:** Tiene la tares de generar las vistas y de interactuar directamente con el usuario.
**Negocio:** Tiene la responsabilidad  de implementar la lógica  de negocio, como implementar operaciones, calculos,validaciones, etc.
**Datos:**  Tiene la repsonsabilidad  de interactuar con la base de datos.

A medida que el usaurio interactue con este patron a traves de la capa de presentacion, el sistema si o si, requerira comunicarse con las demas capas para suplir la necesidad del cliente.Por lo tanto si una capa falla, fallan todas .Ademas si se decide cambiar el patron arquitectonico tiempo despues de finalizada la aplicacion seguramente se tendra que reestructurar toda la software construido.


Sin embargo ambos conceptos se pueden llegar a confundir , pero es necesario saber diferenciarlos de la siguiente manera.Los **Patrones Arquitectonicos** son patrones que se dan para soluciones generales relacionadas a la estructura y organizacion de un sistema ,  y los **Patornes de diseño** vienen para solucionar problemas dentro de los patrones arquitectonicos, los cuales se basan mas en como estructurar el codigo en si , y generalamente se dan a niveles de objetos y clases.


## ¿Que son los estilos arquitectonicos?

Los estilos arquitectónicos son enfoques generales y amplios para la organización y la estructura de un sistema de software. Estos enfoques establecen principios generales para diseñar la arquitectura, como la relación entre componentes, la forma en que se distribuyen y comunican, y la organización general del sistema.

*Pueden haber muchos estilos arquitectonicos y todos dependen  de la necesidad a suplir.

**Arquitectura centra en datos:** Tiene un fuerte enfoque en la gestion y almacenamiento de datos . En este estilo se tiene a los datos como nucleo y una gestion centralizadda de los mismos.

**Arquitectura centrada en flujo de datos:** Centrado en el flujo y la modificabilidad de los datos.

## ¿Cual es la relacion  entre Estilos arquitectonicos, Patron Arquitectonico, y Patron de diseño?

La relacion entre cada uno de estos conceptos se ve de la siguiente manera:
*El estilo arquitectonico sirve como base para implementar los patrones arquitectonicos.
*Los Patrones arquitectonicos se implementa al usar uno o mas patrones de diseño.
*Los Patrones de Diseño son los patrones mas especificos y se centra en resolver  como las clases se crean, como se estructuras, etc.


## Patrones de diseño.


**Singleton:** Me permite generar instancias unicas por el periodo de tiempo solicitado y tengan un punto de acceso global.Esto me permite ahorrar memoria en mis servidores  ya que si 100.000 usuarios quieren solicitar una lista de paises, van a utilizar unicamente una instancia de la entidad paises  sin tener que generar una por cada usuario.Una de las claves de este patron es crear el constuctor de la clase en **private** .Su beneficio es la administracion de la memoria, y su desventaja es que no s epuede usar siempre.

**Factory:** Es un patron de diseño que me permite obtener instancias segun un identificador, todo esto a traves de una interfaz.

**Abstract Factory:** Tengo una super fabrica de fabricas, es decir si quiero un objeto tengo que decirle primero que fabrica y loego a esa instancia de fabrica le indicio que objeto traer














 

