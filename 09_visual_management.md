# Introducción a Visual Management
Por Soledad Pinter, @solepinter

## Palabras clave
Visual management, kanban, tableros.

## Intención
¿Cómo visualizar el estado de las tareas en curso? ¿Qué información es importante compartir con el equipo? ¿Cómo la compartimos?

## Motivación
Cuando trabajamos en equipo, necesitamos conocer los diferentes estados de las tareas en las que está trabajando cada integrante. También necesitamos visualizar información valiosa e importante para todo el equipo y muchas veces no sabemos cómo, ni cuál.

## Descripción
El visual management es un conjunto de técnicas de visualización para administrar información, en particular en este capítulo será en contexto del seguimiento de un proyecto.

Aquí encontrarás una lista de ideas que se pueden realizar para que los equipos cuenten con la información que necesitan visible cerca de su área de trabajo. Se trata principalmente del uso de láminas con diagramas UML, frases clave del proyecto en el que trabajan y láminas con gráficas acerca de temas importantes,como por ejemplo: decisiones de diseño, arquitectura, infraestructura. Todo eso, en las paredes visibles a todo el equipo. Y con colores que permitan visualizar rápidamente lo que es relevante.

### Radiadores de Información

El término Radiadores de Información (_Information Radiators_) fue usado por primera vez en contextos Ágiles por Alistair Cockburn. Él se refería en particular a los _Taskboards_, Charts and Continuous Integration Build Health Indicator.

Todo tipo de recurso que puede ayudar al equipo a mejorar su colaboración y su comunicación los llamamos “Radiadores de Información”; en adelante “RI”. Son aquellos artefactos capaces de transmitir toda la información con solo pasar y mirarlos rápidamente. ¿Qué información irradian? Aquella específica que nosotros queremos que transmita.

La información será leída y tenida en cuenta por aquellos miembros del equipo cuando la necesiten. Lo importante es tenerla a mano y todo el tiempo disponible.

Además, tener información disponible y visible a todos, facilita la transparencia y la autoorganización.

Algunos consejos para lograr buenos RI. Éstos deben ser:

**_Accesibles._** Deben estar ubicados en un lugar cercano al equipo, para que pueda ser visible por todos. Si lo ubicamos lejos o difícil de visualizar, pronto dejará de ser útil.

**_Simples._** La información debe ser precisa, fácil de entender y sobre todo fácil de mantener actualizada.

**_Personalizados._** Es importante que el equipo le encuentre sentido al RI, sino no lo van a cuidar, utilizar y con el tiempo lo van a dejar de usar.

A continuación enumeramos algunos RI que son fáciles de implementar rápidamente y ayudan a una mejor organización, coordinación y colaboración del equipo.

### Tableros Kanban

Este es el tablero más famoso y utilizado en los equipos. Con el podemos visualizar el flujo del proceso y el estado de cada una de las tareas dentro del mismo.

Para identificar las tareas en el tablero utilizamos tarjetas, una por cada tarea. Por ejemplo se podrían utilizar notas autoadhesivas para cada tarea. Lo importante es que las tareas se irán moviendo entre las columnas.

La versión más simple para comenzar, es un tablero de tres columnas de izquierda a derecha: Para hacer, En Curso y Terminado. En la primera columna: “Para Hacer”, colocamos todas aquellas tareas que identificamos y aún no comenzamos. Las ubicamos priorizadas dentro de esta columna: las primeras o más importantes arriba, y hacia abajo las de menor prioridad.

En la columna ‘en curso’, ubicamos las tareas que actualmente se están trabajando. Y en la tercer columna ‘Terminado’ se ubican aquellas tareas que ya han sido finalizadas.

Kanban apunta a reflejar todo tu proceso sobre el tablero, para ello necesitamos conocer todos los pasos para concretar una tarea. De esta manera, entendiendo de manera holística el flujo de trabajo, podemos aventurarnos a superar la versión básica de 3 columnas y organizar el tablero en nuevas columnas, reflejando en ellas cada etapa que genera valor dentro del proceso completo.

De esta manera podremos detectar fácilmente:

*   Los cuellos de botella: aquellos pasos del proceso donde las tareas se retrasan o bloquean más a menudo.
*   Limitación del trabajo en curso: no comenzar una nueva tarea hasta no terminar la actual. Disminuyendo así el tiempo basura entre cambios de múltiples tareas.

![kanban.jpg](assets/9.1.png)

_**Figura 9.1**.Tablero Kanban_

Una vez ya implementados, y luego de las primeras experiencias, se pueden aplicar estas sugerencias en el Tablero Kanban Avanzado:

*   Tareas de un dia.
*   Carril de emergencia: la primera fila del tablero la usamos para colocar aquellas tareas que entran de emergencia al backlog, por ejemplo los errores en producción.
*   Tags con nombres: utilizar notas autoadhesivas o algún identificador más pequeño para señalar los nombres de los responsables en la nota autoadhesiva de cada tarea.
*   Fotos con los miembros del equipo.
*   Métricas como el Leap Time y el Cycle Time permiten conocer, ajustar y mejorar los tiempos de desarrollo y entrega de una tarea, asi como también ayudan a identificar los cuellos de botella en el proceso.

### Calendario del Equipo

Si el equipo se autoorganiza para coordinar y organizar las vacaciones y ausencias planificadas (turnos médicos, preparación de exámenes, vacaciones), alcanza con imprimir o dibujar un calendario mensual en blanco en una hoja de papel. Luego, los miembros del equipo escriben su nombre en los días que estará fuera de la oficina, Pueden acordar un símbolo o color distinto para cada tipo de ausencia planificada por estudio, vacaciones, etc. También se pueden variar los colores o símbolos para cada integrante del equipo. Y en ocasiones, para evitar colapso de información podemos tener un calendario en la misma pared por cada integrante del equipo.

Este calendario debe estar visible junto al tablero de tareas o área de trabajo del equipo para que todos puedan verlo fácilmente.

![calendario.jpg](assets/9.2.png)

_**Figura 9.2**.Calendario de Equipo_

### Criterio de Terminado (_Definition of Done_)

Cuando el equipo trabaja con historias de usuario, necesita acordar los Criterios de Terminado, más allá de los Criterios de Aceptación de cada Historia de Usuario o Item del Backlog.

Para ello, se suele colgar una lámina con estos criterios listados, para que todos puedan tenerlos presentes siempre que necesiten recordarlos.

![DoD.jpg](assets/9.3.png)

_**Figura 9.3**. Criterio de Terminado_

### Matriz de Programación de a Pares

Cuando un equipo realiza programación de a pares, es una buena práctica llevar registro de cómo lo hacemos para no repetir u olvidar alguna combinación. Para eso, dibujamos una matriz de doble entrada donde en las filas y columnas ponemos los nombres de los programadores del equipo, con esto logramos una cuadrícula de pares. Cada vez que dos miembros del equipo programaron juntos, colocan una cruz en la celda que intersecta sus nombres en fila y columna. De esta manera sabremos quiénes restan aún trabajar juntos.

![pair programming](assets/9.4.png)

_**Figura 9.4**. Matriz de Pair Programming_

### Araña de Dependencias

Es una lámina donde dibujamos todas las dependencias que identificamos como aquellas que pueden condicionar la entrega de nuestro trabajo.

En la lámina ubicamos al equipo en el centro. Alrededor de éste, simulando las patas de la araña, todas aquellas fuentes de dependencias que pueden bloquear o pueden hacer peligrar la entrega a tiempo de las tareas del equipo.

A un costado de la araña replicamos estas fuentes en forma de lista bajo el título de “Resueltas”. Luego a medida que fuimos atacando cada dependencia acomodamos junto a cada fuente las tareas que se fueron desbloqueando. Esta métrica sirve para entender qué tipo de dependencias tiene el equipo y así poder pensar en acciones para poder removerlas.

### Sprint Information

Cuando trabajamos con metodología Scrum, siempre es muy útil tener junto al tablero de tareas del equipo los datos importantes correspondientes al Sprint en curso. Sirve a modo de recordatorio a los miembros actuales y también para ayudar a nuevos integrantes.

En una hoja A4 escribimos aquellos datos que pensamos son complementarios y necesarios a la hora de transitar un sprint: Número de Sprint en curso, fecha de inicio y fecha de fin, Objetivo del Sprint.

![IMG_20160226_092039.jpg](assets/9.5.png)

_**Figura 9.5**. Sprint Information_

### Acuerdos de Trabajo

Cada equipo tiene su dinámica de trabajo. Siempre es bueno al comenzar, establecer entre todos los miembros del equipo, aquellas reglas o acuerdos que pueden ayudar a la convivencia y el desempeño del equipo. Por ejemplo: horario laboral, hora de la Daily meeting, cómo rotan la facilitación de las reuniones, a qué temperatura es aceptable el aire acondicionado y todas aquellas cosas que entre todos accedan a incorporar como "Acuerdo de trabajo".

![Acuerdos.jpg](assets/9.6.png)

_**Figura 9.6**. Acuerdos de Trabajo_
