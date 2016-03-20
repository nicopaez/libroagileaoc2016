# _Continuous Discovery_: Validación de ideas para el Backlog

Por Alejandro Faguaga, @afaguaga

## Palabras clave

Dual track scrum, inception, discovery, productos con impacto, business value, UX

## Intención

En general en los proyectos ágiles, la figura del _Product Owner_ es la que trae nuevos requerimientos o necesidades del negocio. A veces como simples ideas o requerimientos de alto nivel, y otras -con suerte- en forma de _User Stories_. Sobre ésto le pide al equipo técnico que analice y estime el esfuerzo de desarrollo de dicha funcionalidad.

En este contexto, no sólo dependemos en primera instancia del conocimiento y buen criterio del _Product Owner_ para detectar las necesidades reales de los usuarios, sino también, de su capacidad para explicitar y clarificar correctamente esas ideas al equipo de desarrollo, y luego además dependemos del buen entendimiento e interpretación del equipo sobre las ideas que el _Product Owner_ pone sobre la mesa.

Esto comúnmente puede generar ítems del _Product Backlog_ definidos de manera pobre o poco claros que pueden atentar contra las reuniones de planificación de los _Sprints_, haciéndolas tediosas o muy extensas. Incluso puede afectar la velocidad del equipo, que termina analizando, refinando y entendiendo las funcionalidades en paralelo con el desarrollo del Sprint.

El resultado de esta situación por lo general es la pérdida de tiempo y el re trabajo debido a que estos ítems no han sido completamente validados a tiempo. A priori pareciera que hay demasiadas variables en juego en esta cadena de gestación y concepción de nuevas funcionalidades a ser desarrolladas, y que dicha cadena está compuesta por eslabones endebles que pueden romperse en cualquier momento.

Todo lo anterior nos da la percepción de que en muchos proyectos la precisión y la correctitud del _Backlog_ dependerá en gran parte de la fortuna.

## Motivación

Si partimos del supuesto que la suerte está de nuestro lado, o que las capacidades del _Product Owner_ hacen que sus pedidos coincidan con los requerimientos del usuario, en verdad aún quedaría mucho camino por recorrer. Cuando el equipo de desarrollo empiece a analizar lo que hay que hacer y el esfuerzo necesario para llevarlo a cabo, en reiteradas oportunidades podríamos caer en cuenta que lo que pide el negocio es inviable desde el punto de vista técnico, o que demandaría un esfuerzo prohibitivo para sus expectativas y/o posibilidades.

Y podría haber una variable más… Aún cuando la solución se pueda implementar desde el punto de vista técnico, el equipo de desarrollo y el _Product Owner_ puede que no tengan en cuenta la usabilidad o la experiencia del usuario respecto de esa solución (ya sea por falta de tiempo o de conocimientos en el área de UX).

Constantemente, requerimientos válidos, e implementados con soluciones técnicamente apropiadas y correctas, podrían no alcanzar el objetivo final de satisfacer la necesidad del usuario, ya que este mismo podría no encontrar dicha solución como “usable” o ventajosa respecto de su situación actual.

## Descripción

Hay que romper con la idea que el Product Owner trae los requerimientos y el equipo de desarrollo es un ente que ejecuta en función de ese _input_ funcional una solución técnica, que la gente de UX validará desde el punto de vista del usuario final. En definitiva hay que romper esa cadena o secuencialidad en la interacción de los equipos o perfiles. Y una buena forma de cambiar esto es hacer que el Product Owner, algún representante del Equipo de Desarrollo y un representante de UX trabajen de forma colaborativa y conjunta desde la concepción misma de los requerimientos o User Stories.

Se forma así un equipo con las 3 “patas” que trabajará sobre ideas, validando de manera conjunta que: las funcionalidades que conformen el Product Backlog cubran la necesidad funcional del negocio (Product Owner); la solución planteada sea factible técnicamente (Desarrollo) y la experiencia de usuario en dicha funcionalidad sea tenida en cuenta (UX). Este proceso se realiza de manera continua y en paralelo con el desarrollo de los Sprints y se denomina _Continuous Discovery_ [Cagan 2012a] o como lo llama Jeff Patton, _Dual Track Scrum_ [Cagan 2012b]. Justamente porque plantea un _track_ o _thread_ de “Descubrimiento” (Discovery) de ítems del Backlog en paralelo con el _Delivery_ de funcionalidad que se va desarrollando en los Sprints. Personalmente, prefiero el término _Continuous Discovery_, porque eso nos abstrae de Scrum, ya que este tipo de técnicas funcionan muy bien con prácticas como _Kanban_ y otras también.

UX, Desarrollo y Producto se complementan para pensar cómo cubrir las necesidades del negocio juntos, aportando cada uno su experiencia y asegurando que la funcionalidad planteada será la mejor posible teniendo en cuenta los 3 puntos de vista. Si se detecta que la solución planteada originalmente no es factible técnicamente o no es usable, se ahorra mucho tiempo y además permite plantear alternativas de manera temprana.

Así el track de Discovery se preocupa exclusivamente de generar PBIs (_Product Backlog Items_) validados y el track de Delivery se enfoca en generar software funcionando basado en ese Backlog validado, e implementarlo lo antes posible en producción.

Adicionalmente, no solo queremos obtener soluciones validadas y realizables, sino que además queremos asegurarnos lo antes posible que realmente estamos cubriendo la necesidad del usuario final, y la mejor manera de lograr esto es obteniendo su feedback de manera rápida y ajustando en función de la retroalimentación recibida.

Continuous Discovery se basa en que en general, aproximadamente el 50% de las ideas propuestas para ser desarrolladas en un proyecto de desarrollo son erróneas o no cubren las necesidades reales de los usuarios.

Para esto la técnica lleva al extremo el concepto de _Fail Fast_, generando prototipos ejecutables para permitir probar la funcionalidad rápidamente y detectar si estamos en el camino correcto o no.

Hay muchas maneras de implementar esto. Puede ser a través de _A/B Testing_, prototipos operativos, funcionalidades que puedan ser activadas o desactivadas mediante un “_switch_”, _Mock Objects_, entre otros.

Independientemente de la forma, lo importante aquí es permitirle al usuario probar la funcionalidad y obtener su feedback lo antes posible.

Hace unos años tuve la oportunidad de trabajar en un equipo Scrum desarrollando una aplicación web de viajes, y aplicábamos varias técnicas. Por un lado se armaba un prototipo ejecutable, con objetos _mock_ que simulaban la lógica de negocios y el acceso a datos y una pantalla de UI con validaciones y el aspecto visual que queríamos que tenga la página. Esto se instalaba en _tablets_ o teléfonos móviles y luego salíamos y pedíamos a la gente en la calle que use la aplicación y nos diera _feedback_ directo, en ese mismo instante.

También armábamos laboratorios de pruebas, donde traíamos a usuarios específicos, les dábamos instrucciones para que ejecuten una funcionalidad, mientras observábamos y tomábamos nota de los problemas que surgían al momento de usar la aplicación.

En otras oportunidades nos sentábamos al lado y los guiábamos para que usen la funcionalidad desde una computadora y les íbamos pidiendo _feedback_ al respecto.

Hay muchas formas, pero lo importante más allá de cómo se obtiene el _feedback_, es lo que uno hace luego con ello.

¿Cómo se relaciona el track de _Continuous Discovery_ con las conocidas sesiones de refinamiento (_backlog_ _refinement sessions_)[Cohn 2015]? La realidad es que se complementan. El _Continuous_ _Discovery_ generalmente es previo, ya que tiene que ver con la creación y validación de ideas que luego se podrán o no transformar en PBIs. Y una vez que empieza el _Discovery_ no termina nunca, con lo cual en algún momento, cuando empezamos a hacer refinamiento, vamos a tener las dos actividades en paralelo.

Lo interesante del _Discovery_ es que de alguna manera "filtra" y valida los PBIs que luego serán refinados como parte del track de _Delivery_, es decir, si hacemos bien el _Discovery_, deberíamos tener PBIs a refinar pre-validados y de "mejor calidad" en cuanto a valor agregado para el producto, y adicionalmente no deberíamos tener PBIs que al refinarlos nos demos cuenta que son técnicamente inviables, o que aportan poco valor.

Ahora bien, la pregunta es, ¿toda "idea" debe pasar por una fase de Discovery antes de ser refinado en las _refinement sessions_? Eso depende del proyecto, del equipo, del contexto. A veces el equipo que lleva adelante el Discovery es cuello de botella, entonces hay que elegir. Lo ideal sería que, en la medida de lo posible, todo requerimiento o característica crítica de nuestro producto pasará por una instancia de Discovery previo a ingresar al _Product Backlog_ y ser refinada, y las _features_ menos relevantes quizás puedan ir directo a las sesiones regulares de refinamiento.

La dedicación del equipo de Discovery también dependerá del contexto y las posibilidades, teniendo en cuenta siempre que el tiempo y esfuerzo dedicado a esta tarea ayudará a evitar que ideas o funcionalidades que no son útiles sean analizadas en detalle o incluso desarrolladas más adelante (en el _track_ de _Delivery_), con lo cual es tiempo bien invertido.

### Conclusión

Un efecto colateral y muy positivo de la práctica de _Continuous Discovery_ tiene que ver con la situación que se presenta continuamente en equipos ágiles, que terminan haciendo una especie de “mini cascada” dentro del marco de Scrum. El Product Owner trabaja en los “requerimientos”, que son pasados a los diseñadores, quienes generan los artefactos visuales que finalmente son pasados al equipo de desarrollo para construir y testear la funcionalidad. _Continuous Discovery_ no se basa en cada rol entregando artefactos a los demás roles sino que se enfoca en tener al Product Owner, un desarrollador y un diseñador trabajando juntos, hombro a hombro en la validación de los PBIs.

Las ideas que no son bienvenidas por el usuario, se descartan automáticamente y las que son bien recibidas se ajustan en base al feedback obtenido y se convertirán en User Stories que pasarán a formar parte del Backlog. Desde este punto el Product Owner no tendrá más que priorizar dicha funcionalidad, pero ya con el pleno convencimiento que tiene entre manos una funcionalidad que será útil para el usuario, usable y factible desde el punto de vista técnico, con una UI pre probada y validada y con el simple costo de haber tenidos un par de reuniones e invertido algo de tiempo en un prototipo.

Pero es muy importante no “casarse” con ninguna idea por más buena que pueda parecer a priori y si vemos que no funciona como esperábamos, descartarla automáticamente.