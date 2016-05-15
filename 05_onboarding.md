# Técnicas de OnBoarding para la gestión de conocimiento

Por Vanesa Savino, @VaneSavino

## Palabras claves

Transferencia de conocimiento, Coaching, Roles variables.

## Intención

¿Cómo trasmitir el conocimiento a los nuevos miembros de un equipo?

## Motivación

Con la llegada de un nuevo miembro a un equipo nos encontramos con el dilema de transmitirle conocimiento relacionado con nuestro proyecto. Además de las pruebas automatizadas de código, en muchos casos hay que brindar información conocida por los expertos del negocio.

Los métodos expuestos a continuación intentan que los expertos puedan dividir su trabajo entre la formación de los nuevos integrantes y sus tareas habituales.

## Descripción

Las ocho prácticas que aquí se mencionan surgieron de la necesidad de reorganizar un equipo de desarrollo. Sólo permanecieron dos miembros del equipo original: un desarrollador y el analista funcional/tester que llevaban trabajando tres y siete años, respectivamente, en el proyecto. El desarrollador fue designado como líder del equipo y al mismo tiempo ingresaron tres nuevos desarrolladores, uno de ellos con experiencia previa y dos más que iniciaban su carrera en sistemas.

Al principio el caos era tal, que el líder siempre estaba atrasado con su trabajo, y justamente era quien resolvía los temas más urgentes o importantes.

Pasada la etapa de adaptación, de tres meses aproximadamente, los desarrolladores observaron que el líder continuaba sobrecargado y decidieron proponer algunos métodos para distribuir el conocimiento, aliviar la presión del líder y al mismo tiempo, sentirse confiados al realizar un requerimiento complejo.

La aplicación de los métodos fue un proceso iterativo. Algunos métodos fueron creados dentro del equipo y otros adaptados de la bibliografía.

A continuación se muestra un listado con la organización de los mismos:

*   Regla de la mano izquierda.
*   _Coaching._
*   Más que programación en parejas.
*   El héroe nuestro de cada semana.
*   Resolución que hace eco.
*   Repositorio de conocimiento compartido.
*   Capacitación.
    *   Clases particulares.
    *   Tarde de películas.
*   Diseño colaborativo.
    *   Adaptación de Kata arquitectura.
    *   Reunión de diseño más informal.

### Regla de la mano izquierda

Este método previene que el experto sea consultado todo el tiempo, escalando las dudas por intermediarios, hasta agotar las instancias y consultarle directamente. Además contribuye a que el conocimiento fluya a través del grupo y no esté centralizado en el experto.

Cuando surge una duda, el primero a ser consultado es nuestro compañero de la izquierda. Si la duda se puede resolver, no se escala más. De lo contrario nuestro compañero se la transmite a su compañero de la izquierda, y así sucesivamente hasta llegar al experto. En este caso el experto explica la solución para todo el equipo.

### Coaching

Este método tiene por objetivo que el desarrollador se sienta seguro al introducirse en un tema complejo ya que su trabajo está respaldado por los conocimientos brindados por el experto.

Cuando un miembro del equipo necesita resolver una tarea que requiere del conocimiento del especialista, solicita su asesoramiento. El especialista aporta su visión y experiencia, discutiendo juntos la forma de aproximarse a la solución con menos trabas y escollos en el camino.

### Más que programación en parejas

En programación de a pares (_pair programming_) el grupo es conformado por dos programadores, pero en esta propuesta uno de los miembros es el experto que no necesariamente es un programador. A diferencia de _coaching_, el experto permanece constantemente junto al desarrollador hasta finalizar la solución.

Este método favorece la cooperación entre diferentes roles, aportando visiones que ayudan a comprender el problema o fijar conceptos.

Se arma un equipo temporal para trabajar en el código. Si el especialista programa, puede codificar las partes más complicadas de la solución y explicarle su funcionamiento al compañero. Cuando el especialista no sea técnico puede validar la solución que construyan.

Siempre que se crea conveniente, se puede solicitar la colaboración temporaria de miembros con otros roles, para que aporten otros enfoques del problema, formando un equipo de tres miembros. Un ejemplo de esta colaboración puede ser un grupo conformado por un especialista técnico y otro desarrollador que le solicitan ayuda al analista funcional para despejar una duda de negocio que surgió en medio de su tarea.

Este método puede aplicarse junto con la “regla de la mano izquierda” y armar un equipo con el compañero de la izquierda.

### El héroe nuestro de cada semana

Este método tiene un doble propósito, el primero es que cada miembro del grupo se encuentre capacitado para resolver las urgencias del sistema. El otro es que el experto pueda continuar con sus tareas y no se encargue exclusivamente de los casos urgentes, que provocan demoras en su trabajo si las interrupciones son muy frecuentes.

Del Agile Open Camp 2015 se tomó una idea interesante: un miembro del grupo va a tener el rol de "Héroe" para ocuparse de los problemas urgentes del sistema.

El rol es ocupado por cada miembro durante una semana, hasta que todos lo hayan ocupado una vez y luego se vuelve a comenzar. Para hacerlo identificable frente a los demás miembros del equipo, cada miembro puede tener un muñeco o imagen de su héroe favorito a la vista, sobre la que pegan una estrella de Sheriff para informar que están de “guardia”.

Quien desempeñe este rol continúa con sus tareas habituales; en caso de haber un problema urgente, pospone su tarea y se dedica a la resolución del problema. Dependiendo de la complejidad de la situación, un experto o cualquier otro miembro del equipo es requerido para ayudar a resolver la urgencia. Así cada miembro aprende a resolver errores críticos sintiéndose confiado bajo la tutela de alguien con conocimiento sobre el tema.

Este método puede combinarse con “_coaching_” y “más que programación en parejas” para facilitar un arreglo urgente.

### Resolución que hace eco

Este método pretende unificar criterios, lo que facilita el entendimiento de los temas. También propone que se incorporen ideas generales del funcionamiento del sistema cuando se investiga en busca de comportamiento común dentro de la aplicación.

Al recibir un requerimiento para cambiar una característica en particular, se tiene que investigar si hay otras funcionalidades con similar comportamiento que requieran ser modificadas y también cambiarlas.

En una aplicación grande y de larga data, suele ocurrir que la solución a un problema ya está implementada en otro lugar, de modo que es importante asegurarse que realmente sea necesario dedicar tiempo a construirla desde cero, cuando lo más probable es que lleguemos a un código y lógica duplicados, que traerá consecuencias si el día de mañana uno de estos comportamientos se modifica y el otro no. A no repetir código!

Este método se puede combinar libremente con cualquiera de los métodos que consisten en desarrollo, ya que no interfiere con su misión.

### Repositorio de conocimiento compartido

Construir un repositorio en la nube y compartir la documentación ha desplazado al uso de otros sistemas más formales. Hoy en día existen muchas plataformas y servicios gratuitos que brindan acceso desde diferentes dispositivos, lo que facilita la distribución de la documentación.

Este método tiene por objetivo tener disponibilidad online de la documentación con todas las ventajas que eso representa, entre ellas: accesibilidad móvil, y un mecanismo más simple para creación de contenido, ya que se evita la instalación de programas específicos.

Es muy importante mantener un orden conocido por todos, para que cada miembro sepa dónde ubicar el contenido que produce o donde buscar la información que necesita. Dependiendo de la organización se pueden otorgar diferentes permisos de acceso y edición, lo que requiere una moderación del contenido que se cree colaborativamente.

### Capacitación

Se van a explicar dos maneras de comunicar información. El objetivo es incorporar conceptos a través de diferentes formatos, el más moderno, audiovisual y el tradicional con material escrito.

#### Clases particulares

Consiste en preparar clases con temas especiales y brindar material para los asistentes que ayude a la compresión del tema tratado. Es fundamental que luego el material se suba al repositorio para que pueda ser consultado en cualquier momento. Además conviene tener un modelo de contenido para implementar las charlas, dando un marco mínimo de información que deben cubrir.

#### Tarde de películas

Existen muchos videos de tutoriales online que nos enseñan desde cómo hacer el nudo de una corbata hasta como aprender a tocar la guitarra. Esta forma de enseñanza es cada vez más habitual, incluso se pueden encontrar clases de prestigiosas universidades disponibles online.

¿Por qué no aplicarlo entonces a nuestro sistema? Para partes que sufren pocas modificaciones, como la configuración de un entorno, es de mucha utilidad contar con tutoriales que muestren la configuración correcta, de esta forma se ahorra mucho tiempo de búsqueda infructuosa.

### Diseño colaborativo

Como ya se sabe la visión de grupo en sinergía supera la suma de la visión de sus miembros.

En esta instancia se propone utilizar diseño colaborativo para llegar a la solución óptima de un problema.

Dependiendo de la estructura y la cantidad de miembros del equipo se pueden hacer reuniones más informales o adaptaciones de katas de arquitecturas.  

El término kata proviene del karate y consiste en una serie de ejercicios establecidos que se realizan sólo.  Este término se aplicó al diseño de código cuando Dave Thomas creó las “Code Kata”.  

Las katas de arquitecturas se realizan en grupos, tienen reglas y roles definidos. Se acuerda un tiempo de duración para todo el ejercicio, los miembros se dividen en grupos de desarrolladores y se designa un moderador, responsable de responder todas las dudas de los equipos. Si el moderador es el líder del equipo, también se encarga de guardar las buenas prácticas de programación.

Los equipos se separan una distancia prudencial para hablar sin interferirse mutuamente. Después de finalizado el tiempo, un orador elegido por los miembros del grupo expone la solución frente al interesado. En este caso el rol del interesado puede ser ocupado por el analista funcional.

El moderador, el interesado y los restantes participantes formulan todas las preguntas necesarias para entender la propuesta. Al finalizar esta etapa todos votan al mismo tiempo la solución.

La votación se realiza con la regla del pulgar: pulgar para arriba para indicar que me gustó la propuesta. Horizontal para indicar que no me convenció del todo y pulgar para abajo para indicar que no me agradó.

Luego de la votación comienza la exposición del siguiente equipo hasta terminar, al finalizar se trabaja con la solución más votada.

Si el equipo es pequeño (3 o 4 personas) puede trabajarse más informalmente, reuniéndose frente a una pizarra y diagramando una solución. Aquellos con más conocimiento pueden proponer una solución tentativa y los demás pueden dar su _feedback_ para ver en que se puede mejorar.

Es importante a tener en cuenta el _feedback_ en ambos métodos, pues a veces la solución más brillante la aporta el miembro menos pensado.

Este métodos propician la participación de todos en la construcción de la solución, pero como la experiencia de cada miembro es diferente se pueden complementar con “_coaching_” o “más que programación en parejas” dependiendo de si es una solución más técnica o de negocio.

Los métodos expuestos tienen como eje principal compartir conocimientos, algunos han surgido por la necesidad de resolver un problema, otros han sido adaptados de la bibliografía o tomados literalmente. Estos métodos pueden aplicarse en forma iterativa e incremental; lo fundamental es lograr la comodidad del equipo y una transferencia de conocimiento efectiva.

La intención de exponerlos aquí es que sirvan de base para generar otros métodos que se adapten a cada situación particular.

El progreso que se realizó después de su implementación ha sido muy significativo; además contribuyó a crear un equipo muy sólido, con confianza en sus miembros y auto-organizado.
