# Guardián de un equipo con múltiples asignaciones. {#guardi-n-de-un-equipo-con-m-ltiples-asignaciones}

Por Tomás Christie, @tommychristie## Palabras clave {#palabras-clave}

Scrum, mantenimiento, desarrollo, multi-proyecto## Intención {#intenci-n}

La intención de esta técnica es aislar al equipo de las interrupciones, permitiéndoles desarrollar tranquilos.## Motivación {#motivaci-n}

En equipos pequeños que atienden múltiples proyectos en forma simultánea, los integrantes suelen sufrir interrupciones permanentemente. Se pierde el foco, existe un costo altísimo de cambio de contexto y puede traer desmotivación. En general estas interrupciones son por fallas en los sistemas, que requieren de atención inmediata por parte de alguno de los integrantes del equipo, o más de uno.## Descripción {#descripci-n}

Se presenta típicamente en los casos de equipos pequeños que tienen una gran cantidad de proyectos, en todas las etapas del ciclo de vida. En estos casos suele suceder que las tareas de mantenimiento correctivo entran fácilmente en conflicto con los nuevos desarrollos, al punto que en algunos casos se vuelve muy difícil planificar.

Este conflicto típicamente lleva a que se le dedique poco tiempo a realizar las tareas de mantenimiento y a que los problemas se solucionan con “parches”, sin resolver realmente el problema de fondo. Irremediablemente, los parches se empiezan a acumular, parche sobre parche.

Esta situación hace que la calidad del software se vuelva progresivamente peor, llevando a que se generen cada vez más incidencias de mantenimiento correctivo, más interrupciones, menos foco por parte del equipo y más insatisfacción (tanto del cliente como del equipo).

Se propone tener a alguien que sea el guardián del equipo y que se encargue de que el resto del equipo no sufra interrupciones (o la menor cantidad posible). En una primera etapa a este guardián lo podríamos llamar “Bombero”, ya que mayormente atenderá urgencias, estará “apagando incendios”.

Como suele ser una tarea estresante, el equipo de desarrollo establece algún orden cíclico que incluya a todos. Luego, por sorteo (o alguna otra manera que el equipo decida), se selecciona al primer Bombero. Cada desarrollador tiene este rol por una semana, o el tiempo que el equipo considere conveniente. Personalmente, creo que es importante que sea un tiempo balanceado. Es decir, lo suficientemente corto como para que no sobrecargue al Bombero de turno (ya que es una tarea demandante) y lo suficientemente larga como para que los demás logren descansar del rol.

Cualquier pedido de acción que esté por fuera de la planificación, debe ser atendido por el Bombero. Esto en general debería responder a la resolución de bugs “urgentes”, del tipo “necesitamos facturar y no funciona tal o cual cosa”.

Algunas ventajas que vienen por añadidura:

*   Distribución del conocimiento. El Bombero, al tener que resolver problemas de cualquier sistema, a la fuerza debe interiorizarse con cada sistema a medida que requiera atención.
*   Proporciona tiempos de respuesta más rápidos ante bugs de los sistemas.
*   Durante un período breve de tiempo, sólo uno sufre el constante cambio de contexto y luego tiene tranquilidad por un período proporcionalmente largo.

En general este estado de “bombardeo de bugs al equipo” es inicialmente fuerte y hace que el Bombero esté constantemente apagando incendios. Después de algún tiempo, esta situación tiende a mejorar, gracias a que la figura del Bombero tiene dedicación absoluta a estos temas y su tiempo no entra en conflicto con la planificación.

Cuando esto pasa, la figura del Bombero puede transformarse en la de un “Guardia”. De la misma manera que antes, el Guardia va rotando semana a semana. Hay dos variantes posibles para la figura del Guardia:

*   Dedicar su tiempo a tareas preventivas o de saneamiento. Por ejemplo, implementar más tests, hacer refactoring de código con optimizaciones, etc. Muy probablemente, esta variante pueda aplicarse primero, a modo de transición entre el Bombero y la segunda variante del Guardia.
*   Al Guardia se lo incluye dentro de la planificación. Realiza tareas de desarrollo al igual que el resto, con la salvedad de que es el interrumpible. Es para equipos bastante evolucionados, con software de alta calidad, donde la incidencia del mantenimiento es baja. De esta manera, el Guardia colabora con el desarrollo siendo el único que “padece” las interrupciones.

### Conclusión {#conclusi-n}

La técnica funciona muy bien. Los resultados se ven en el corto plazo. El equipo en general adquiere un estado más relajado de trabajo, sabiendo que puede poner todo su foco en el desarrollo que tiene entre manos, sin tener interrupciones constantes.

En general, las tareas de apagar incendios merma y comienzan las tareas de prevención y Guardia. Vemos que al poder dedicarle tiempo a tareas de prevención, la calidad del software tiende a subir y las incidencias de bugs caen. ¡Se ingresa en un círculo virtuoso!