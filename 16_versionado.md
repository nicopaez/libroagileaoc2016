# Versionado de código, configuración y ambientes

Por Nicolás Paez, @inicopaez

## Palabras clave

Devops, versionado, entrega continua

## Intención

¿Cómo organizar el versionado de artefactos de software en un contexto de entrega continua?

## Motivación

Desde una perspectiva de entrega continua toda aplicación es **código** ejecutándose en un determinado **ambiente** con una determinada **configuración**. Algunos fanáticos podrían insistir en que los datos son también parte de la aplicación, pero este es un punto que puede resultar muy polémico y por ello se dejará de lado en esta ocasión. Entonces tenemos:

código + configuración + ambiente

Por ambiente entendemos como mínimo una máquina (física o virtual) con un cierto sistema operativo con determinado software de base, por ejemplo: un servidor de aplicaciones o un servidor web. En la actualidad existen diversas herramientas que permiten especificar los ambientes en forma de código (Chef, Puppet, Ansible, etc). Entonces con una vuelta de rosca más tenemos:

código de la aplicación + configuración de la aplicación + código que describe el ambiente de la aplicación.

Finalmente como nuestra aplicación deberá evolucionar a lo largo del tiempo, agregaremos a nuestra lista un paquete de código adicional que describa cómo instalar/desplegar nuestra aplicación, con su correspondiente configuración, en su correspondiente ambiente. Pasando en limpio, podemos decir que toda aplicación se compone entonces de 3 artefactos:

*   El código fuente.
*   La configuración.
*   Los scripts de despliegue.

En un contexto de entrega continua es necesario gestionar y versionar cada uno de estos 3 artefactos. La pregunta es entonces cómo hacerlo.

## Descripción

Estos tres artefactos tienen un frecuencia de cambio distinta: el código fuente suele estar en constante modificación, mientras que los scripts de despliegue suelen ser mucho más estables y en algunos casos no recibir cambios por semanas o meses. La frecuencia de cambio de la configuración de la aplicación se encuentra en un punto intermedio, no está en constante cambio pero tampoco es tan estable como los scripts de despliegue.

Por otro lado, dependiendo del contexto organizacional, pueden definirse distintas políticas de acceso a estos artefactos. En algunas organizaciones es muy común que el equipo de desarrolladores no tenga permisos para acceder a los parámetros de configuración del ambiente productivo. También suele ocurrir que los scripts de despliegue de la aplicación sean administrados por personas ajenas al equipo de desarrolladores (usualmente personas del área de operaciones).

Estas dos cuestiones, frecuencia de cambio y permisos de acceso, son las que nos motivan a separar estos tres artefactos del proyecto en diferentes repositorios.

El primer repositorio es el que almacena el código fuente de la aplicación. Dependiendo de la complejidad del proyecto, puede haber más de un repositorio para el código fuente. Un caso típico de esto son las arquitecturas basadas en microservicios, donde cada microservicio suele tener su propio repositorio.

El segundo repositorio es el que almacena la configuración de la aplicación. Este repositorio tiene típicamente un branch por ambiente (por ejemplo: desarrollo, testing, producción) ya que la configuración de la aplicación suele variar de un ambiente a otro. Hay que destacar que estos branches nunca se mezclan, sino que evolucionan a la par. Cuando la aplicación requiere de un nuevo parámetro de configuración, el mismo debe ser agregado simultáneamente a cada uno de los branches con el valor correspondiente al ambiente asociado.

Finalmente el tercer repositorio es el que contiene los scripts de despliegue. Dependiendo de la infraestructura del proyecto pueden ser simplemente scripts de Bash o de alguna herramientas específica como Ansible, Puppet o similar.