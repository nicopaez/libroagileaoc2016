# Revisión Triangular de Documentos

Por Natalia Baeza, @Naty3Baeza y Virginia Brassesco, @virbrassesco## Palabras clave {#palabras-clave}

Revisión por pares, aprendizaje colaborativo, _feedback_, edición, documentación## Intención {#intenci-n}

Se presenta un patrón de revisión de documentos para tratar de evitar:

*   Ambigüedades.
*   Uso de vocabulario inapropiado.
*   Redundancias.
*   Textos innecesariamente extensos.
*   Errores ortográficos.
*   Estética general inadecuada para el contexto del documento bajo revisión.
*   Uso de documentación obsoleta.

Este patrón facilita:

*   El aprendizaje y maduración del tema a tratar.
*   La comunicación entre las personas involucradas en la elaboración de documentos.
*   Lla transmisión de conocimiento.
*   La elaboración misma del documento.
*   El mantenimiento de base de conocimientos documental.## Motivación {#motivaci-n}

Este patrón resulta útil cuando un documento, público o privado, debe ser elaborado y se requiera _feedback_ para mejorar la calidad del contenido, la redacción y la presentación del mismo.

También puede usarse cuando se desee evaluar y/o ampliar el conocimiento de una persona sobre un tema dado.## Descripción {#descripci-n}

Bajo el paradigma Ágil, el código funcionando tiene más valor que la documentación como se puede leer en el [manifiesto ágil]. En general hacemos documentos que refieren a algún producto de software. Sin embargo suele emerger la idea de que éste quedará obsoleto ante algún cambio en el producto, o que escribirlo nos haría perder tiempo productivo, y por eso la documentación no es prioritaria. Pero, ¿qué ocurre cuando el documento es el objetivo de nuestro trabajo, el producto final?

Muchas veces ciertos documentos deben poseer una estructura específica que podría introducir ruido al que intenta comprender una idea. Podría ocurrir que el autor principal no sea experto del dominio o su lenguaje nativo no sea el usado en el documento y, por ende, le podría faltar vocabulario específico.

Algo que solemos olvidar es que los textos deben ser comprensibles no sólo para su redactor, sino para el público al que están orientados.

Recordemos además que no a todos les gusta escribir y no siempre todos los que contamos con el conocimiento vamos a tener voluntad de trasladarlo a un texto publicable. Para que esta tarea no resulte tediosa, trabajar colaborativamente y tener una metodología que nos guíe puede ser el puntapié inicial.

Partiendo de la bien conocida idea de revisión de pares [Crespo-Villena 2005], aplicada a la elaboración de textos, se propone un patrón de revisión triangular como estrategia de aprendizaje y así lograr mejores documentos que faciliten la tarea de compartir conocimiento.

Aspectos que matizan al patrón:

*   _Roles y tareas:_ Identificar las funciones de los actores participantes con su tipo de revisión asociada; separar revisiones conceptuales de las ortográficas y gramaticales.
*   _Expertise:_ Acceder a “diversidad” de personas que estén calificadas para hacer tu revisión.
*   _Workflow:_ Contar con un método práctico para seguir el estado del documento.
*   _Soporte a la comunicación:_ Herramientas que faciliten la visualización de cambios y el estado de la revisión.

### Roles {#roles}

Son tres (así naciendo la idea de triángulo), el _autor_, el _revisor_ y el _editor_.

El _autor_ es quien sabe del tema y quiere exponerlo al mundo, entiende bien de qué se trata y cuál es el alcance del documento. Identificó la necesidad de escribir sobre ello y tiene la voluntad de hacerlo.

El _revisor_ es el experto, sabe más o igual del tema que el autor y es capaz de decidir si el autor se está expresando bien sobre aquello que quiere contar. Conoce sobre el vocabulario del dominio y los detalles de qué es bueno decir y qué no, para cada caso.

La pregunta es, ¿por qué no lo escribió él al documento?

Todo documento surge por una necesidad, pues si no hay necesidad no hay motivos para hacerlo ya que no le aporta valor a nadie. Esa necesidad fue identificada por el autor, quien es el que conoce la intención de plasmar el tema en un documento.

El _editor_ es quien se encarga de darle formato y revisar ortográfica y gramaticalmente el texto. Esto es tan importante como el contenido. Nadie quiere leer un documento con errores de ortografía, mal redactado o donde los colores cansan la vista. Por otro lado, puede ser interesante y hasta necesario en ciertas ocasiones, saber a quién pertenece el documento, introduciendo en él algún símbolo que lo identifique: el autor, la compañía o el nombre del producto (sea comercial o no). El editor debe revisar también que el documento tenga la información necesaria para la publicación, sea agradable a la vista, y “que cuente bien la historia”.

### Tareas, ¿Quién se ocupa de qué? {#tareas-qui-n-se-ocupa-de-qu}

El autor y el revisor evalúan básicamente _contenido_, definen el _estilo_ de la escritura y parcialmente formato a sólo efecto de no agregar confusión en el documento por ejemplo identificando jerarquías de títulos o definiendo colores que no pueden ser de otro modo. Además, el editor debe saber exactamente a qué le está dando formato, por ende el autor debe entregar un documento con ideas claras al editor.

El rol del editor es muy distinto al del revisor. Él estará concentrado en los aspectos gramaticales, formato y estilo visual del documento. Será el encargado de dejar la versión final publicable. Si es un experto en el idioma de redacción del documento, puede aportar en mejoras del estilo de escritura.

### _Expertise_ {#expertise}

Escribir sobre un tema implica entenderlo en plenitud. Solo puedes explicarlo bien si puedes entenderlo muy bien. La revisión de un experto en etapas tempranas ayuda al aprendizaje y balance de conocimiento entre el autor y el revisor. Así el texto es finalmente construido con el conocimiento de las partes involucradas, consensuando los alcances del documento actual y decidiendo qué documentación elaborar en un siguiente ciclo de revisión.

Cuando el revisor cuenta con mayor conocimiento específico de ese dominio que el autor, se debe asegurar de que el texto final sea comprensible para el público al que está destinado.

**Si en tu equipo diario no encuentras a alguien cercano que cuente con el _expertise_ para hacer tu revisión, debes buscarlo en otro lugar, si no deberás hacerlo tú mismo y el resultado será carente de objetividad y no tendrás _feedback_.**

Pero…, ¿qué pasa si el revisor tiene menor _expertise_ que el autor? ¿Es factible?

La revisión que se pretende incorporar en este patrón tiene intención de ser vista como un método de aprendizaje para todos los que escriben en él, no sólo para el autor.

Alguien que no domine el tema en plenitud puede aportar valor. Es importante que pueda tener lugar para formular todas las preguntas necesarias y así comprender lo que está leyendo. A través de estas preguntas el autor puede detectar qué información es faltante o poco clara en el documento.

En este caso, el experto es el autor, y el revisor se introduce en un _workflow_ de revisión sobre algo pre-elaborado. Notemos que en este caso la confianza del revisor al autor para poder realizar preguntas y del autor al revisor para dar lugar a edición es fundamental. Motivemos al revisor a preguntar, pero también a reformular textos para hacerlos más comprensibles.

Este tipo de revisión conviene hacerla en etapas avanzadas del documento, cuando éste ya fue revisado en al menos una iteración por un revisor experto y el editor. Esa persona debe estar preparada para modificar un documento que trata de un tema en el que no es experta, por lo cual no debe ser elegida al azar.

Por supuesto, se puede contar con varias personas para el mismo rol: puede haber más de un autor, más de un revisor y más de un editor.

Con respecto al _expertise_ del editor, debe conocer bien las reglas del lenguaje en el que se escribe el documento. En el caso que el documento deba publicarse en un idioma diferente al usado por el autor, el editor debe contar con conocimientos expertos en ambos lenguajes, y hasta podría realizar una traducción del mismo, o crear las versiones necesarias del documento en diferentes idiomas.

Por otra parte, si el diseño del documento es muy complejo, se podría recurrir a algún diseñador que colabore agregando estilos gráficos, corrigiendo imágenes, y dando el marco acorde que identifica al documento como parte de una base de conocimiento específica.

### Comunicación fluida {#comunicaci-n-fluida}

La interacción entre las personas que redactan y editan el documento es clave, debe ser fluida. Esto no implica tener reuniones constantemente para poder redactar cada línea; aquí prima la confianza en nuestros pares, donde el grupo de revisión está enfocado a lograr un producto de calidad, construyendo y aprendiendo en el camino.

Antes de comenzar la elaboración del documento hay que elegir las herramientas que soporten esta comunicación.

Un ejemplo muy práctico es la plataforma de Google, Google Docs. Lo valioso de esto es que permite volver atrás cualquier cambio realizado e identificar el momento y el autor del cambio. Por supuesto esto no es para identificar culpables, sino para acudir a esa persona y entender el cambio si es que no está claro.

Aquí es necesario comunicarse en tiempo real. Pueden ser útiles herramientas de _chat_, o llamados telefónicos. El objetivo es visualizar la traza del cambio, aclarar las dudas de inmediato y decidir y resolver en función de ello.

### _Workflow_: Revisión iterativa en ciclos cortos {#workflow-revisi-n-iterativa-en-ciclos-cortos}

Para no caer en el cansancio o creencias de que se “pierde tiempo” en un documento, la redacción de documentos debe ser de manera iterativa, con el cubrimiento de todos los roles aportando cambios incrementales pequeños, con lo cual se requiere menos tiempo para tomar una decisión sobre ellos, y por ende son más simples de incorporar (descartar) en el documento, o bien crear nuevos documentos a partir de ellos. Además así se mantienen actualizados a lo que realmente ocurre en ese momento.

Es común que al elaborar un documento hagamos referencias a otros existentes ya publicados. Si se descubre un documento obsoleto, es necesario actualizarlo de inmediato resolviendo lo que esté desactualizado. Si el documento es completamente obsoleto es recomendable hacer “borrón y cuenta nueva”.

Para poder hacer un seguimiento de documentos publicados se recomienda que cada documento tenga una fecha o versión de publicación que coloque el editor final.

#### Aún así, ¿quién empieza? {#a-n-as-qui-n-empieza}

El autor es el que da el paso inicial. Manifiesta ideas lo más claramente posible y en un muy corto plazo, por ejemplo 1 día o 2, el revisor ya se hace parte del documento.

Alinea los tópicos, pide explicaciones verbales sobre los mismos (esto puede implicar una reunión inicial) y da lugar al autor con indicaciones, ideas, ayudas fuertes de cómo seguir. El resultado es un acuerdo entre ambas partes.

Si al escribir cualquier cosa del documento hay un “impedimento” se debe acudir de inmediato al revisor o viceversa (revisor a autor).

Y aquí hemos trazado un canal de ida y vuelta en la comunicación dando forma a un lado de nuestro triángulo, Figura 2.1.

**_Figura 2.1._** _Interacción autor-revisor_

En esta etapa de la revisión pueden surgir documentos anexos, secciones no previstas o nuevos documentos a generar a posteriori. Hasta aquí es claramente una revisión de pares.

En estas dos instancias, el editor cumple un rol pasivo. Se le pueden preguntar cuestiones puntuales pero aún no edita el documento.

Cuando ya hay una versión lo suficientemente madura del documento que contenga las ideas principales del mismo y que estén explicadas de forma clara para autor y revisor, se hace parte activa del _workflow_ el Editor.

Es posible que el editor no requiera ayuda del autor o revisor para realizar su tarea, pero si hay algo de fondo que se deba cambiar o alguna idea no está clara, el editor debe consultar al autor.

Aquí ya tenemos dos aristas del triángulo. Figura 2.2.

**_Figura 2.2._** _Interacción autor-editor_

Si el autor no es capaz de responder a la pregunta o no está disponible en ese momento, el editor debe acudir al revisor.

La tercer arista es más liviana (editor al revisor y viceversa) ya que quien intermedia cada revisión en el _workflow_, es el autor. Figura 2.3\.

**Figura 2.3.** Interacción editor-revisor

Este ciclo de 3 etapas, debe repetirse cuantas veces sea necesario.

Durante la generación del documento la revisión se realiza de manera cruzada e iterativa hasta tener la versión final que también es revisada por el autor previa a su publicación.

### Otros detalles {#otros-detalles}

Cada equipo de revisión debe generar su propio mecanismo para saber cuándo le toca a quién (siguiendo el _workflow_ anterior) y no pisarse en los cambios. No es recomendable que revisor, editor y/o autor hagan cambios en simultáneo sobre la misma parte del documento. Cada uno debe decir explícitamente si el documento completo o qué parte del él está lista desde su perspectiva.

Otro punto inflexible es que **aquel que decide que algo debe escribirse de otro modo, borra lo escrito y escribe su idea. No pide permiso.** Esto puede sonar agresivo pero no lo es y el resultado es favorablemente bueno, ya que quien escribe, lee y elabora su idea sin pensar en una frase o concepto que ya decidió que debía reformularse. La revisión y elaboración de la revisión es un proceso de aprendizaje. Tomo mi mejor decisión, aprendo y mejoro mi decisión en la siguiente iteración.

Por esta razón es fundamental que la herramienta de soporte de la edición, guarde las versiones y los cambios con autor y _timestamp_. De ese modo es posible tener y visualizar la traza a versiones anteriores y resolver dudas aclarando ideas nuevas.

### Conclusiones {#conclusiones}

Este patrón se propone como un mecanismo de aprendizaje extendiendo la idea de revisión de pares. Se definen 3 roles principales, cada uno con su expertise aportando valor en un proceso iterativo de revisión.

A la hora de implementarlo seamos concientes que los participantes van a ser enriquecidos en conocimiento y nos ayudará a mantener la información actualizada no solo escrita, sino también en las mentes de todos los participantes.

De este modo, se facilita la elaboración de documentos que soporten la gestión del conocimiento a partir de un documento de calidad, dividiendo y distribuyendo la revisión en pequeñas tareas y actuando de forma colaborativa. Aplicado el patrón, el producto debe lograrse en cortos períodos de tiempo dando valor y resolviendo una necesidad actual de aprendizaje y divulgación, e incrementando una base de conocimiento que intenta mantenerse actualizada.

### Agradecimientos {#agradecimientos}

Este capítulo se ha realizado utilizando este patrón de revisión triangular a través de 2 iteraciones. Agradecemos a Pablo Tortorella y Nicolás Páez, como revisor y editor respectivamente, por su colaboración en la primer iteración de revisión triangular que dio forma a este documento.