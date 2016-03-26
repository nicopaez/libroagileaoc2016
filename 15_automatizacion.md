# Automatización a través de Git hooks
Por Fernando Di Bartolo, @fdibartolo

## Palabras clave
desarrollo de software, git, automatización, entrega continua

## Intención
Minimizar el error humano a través de la automatización de ciertas rutinarias tareas de un desarrollador de software.

## Motivación
Somos humanos, y por ello, cometemos errores. Por otra parte, en la ingeniería de software, se menciona el hecho de que cuanto más tarde se descubre un _defecto_, mayor es el esfuerzo necesario para solucionarlo. Dicho esto, desde la perspectiva del desarrollador de software, si damos por sentado que vamos a introducir errores, defectos, y/o violación de estándares, ¿qué podemos hacer para detectarlos lo suficientemente temprano como para que corregirlos sea trivial?

A esta altura y por los años que corren, la respuesta a la pregunta de arriba podría ser: “escribe tus pruebas unitarias, escribe tus pruebas de integración, escribe tus pruebas de interfaz gráfica, bla bla bla”. Claramente yo apoyo esta moción (sujeto al contexto del proyecto en cuestión), pero aun así, y lo he visto, no todos los miembros de un equipo de desarrollo tienen la misma disciplina de correr dichas pruebas antes de enviar sus cambios al repositorio, o bien, solo corren aquellas que “teóricamente” están asociadas a su cambio en el código. Entonces, nuevamente, ¿qué podemos hacer?

## Descripción
La idea planteada aquí no es bala de plata para cualquier implementación, ni tampoco la única. Sin ir más lejos, existen herramientas que incluso facilitan lo que estoy a punto de describir, pero la intención es plantear las bases, más aún cuando nuestro contexto nos limita a poder hacer uso de aquellas herramientas (por ejemplo, si trabajamos con un cliente que ya tiene su set de herramientas predefinido; o bien que por políticas internas, las herramientas que podríamos usar no están permitidas).

Los _git hooks_ (ganchos) son pequeños _scripts_ que nos permiten ejecutar acciones en ciertos puntos del flujo de trabajo. Estas acciones podrían ser por ejemplo:

*   Generar un nuevo objeto _commit._
*   Sincronizar código propio con un repositorio remoto.
*   Hacer un _merge_ de dos ramas del repositorio.

En pos de mantener la simpleza, aquí mencionaremos solo 3 _hooks_, aunque la lista es larga como indica Scott Chacon en su libro “Pro Git”, [Chacon 2009].

Entonces, en líneas generales, un desarrollador debe:

1.  Cumplir con estándares de codificación.
2.  Ejecutar la(s) suite(s) de pruebas localmente, contemos o no con un servidor de integración continua.
3.  Desplegar código a un servidor/entorno de prueba.

Veamos cuáles _git hooks_ nos ayudan a lograr que estas tareas rutinarias se ejecuten en el momento adecuado y de manera automática, sin riesgo de error humano (errores tales como olvido o mala lectura del resultado por falta de atención).

1.  Nos encontramos escribiendo código y guardando los cambios a través del comando git add. Estamos listos para hacer un _commit_. Deberíamos ahora ejecutar manualmente la herramienta para asegurar que nuestros cambios no violan ningún estándar, pero frecuentemente, es algo que olvidamos y que terminamos chequeando _post-mortem_. He aquí un git hook al rescate: **pre-commit**. Creamos un archivo con ese mismo nombre dentro de _[repo]/.git/hooks_, con su correspondiente permiso de ejecución. Dentro del mismo, programamos aquello mismo que veníamos corriendo a mano, que dependiendo del lenguaje de programación en cuestión, será usando librerías tales como Rubocop, JsLint o CodeAnalysis. Una particularidad con este _hook_ es que, llegado el caso que algún estándar no se cumpla y quisiéramos por ello rechazar el _commit_, solo tenemos que hacer que el _script_ retorne un valor distinto de cero.
2.  Tenemos ahora un conjunto de _commits_ listos para empujarlos a un repositorio remoto. Si no lo hicimos antes, deberíamos ejecutar manualmente nuestro conjunto de pruebas, y nuevamente, solo lo hacemos cuando nos acordamos. El hook que ahora nos puede ayudar es el **pre-push**. Así como hicimos antes, creamos un archivo con el mismo nombre del _hook_ (pre-push) y en el mismo lugar físico ([repo]/.git/hooks). Escribimos dentro de él aquel o aquellos comandos que corren nuestras pruebas. Ante una prueba fallida, haremos nuevamente que el _script_ retorne un valor distinto de cero, y el _push_ será rechazado. Como habrán notado, todos aquellos _hooks_ cuyo nombre comience con **pre-**, se ejecutan un instante antes de la acción en cuestión, con lo cual, haciendo que el _script_ retorne un valor distinto de cero, impedimos que la acción se lleve a cabo.
3.  Por último, necesitamos desplegar código a un entorno de pruebas, y esto puede requerir varios pasos: actualizar esquema de base de datos, minimizar javascripts y/o hojas de estilo, etc. Tareas rutinarias, algunas fácil de saltear, por lo cual, ¡automaticemos! Suponiendo que desplegar implica empujar código a un repositorio remoto (por ejemplo, de la forma que funciona Heroku), podemos hacer uso del hook **post-receive.** En este caso, a diferencia de los 2 primeros, debemos crear el archivo en el repositorio remoto, no en el que tenemos localmente. Una vez que empujemos código via git push desde nuestro repositorio local hacia el remoto, el _script_ correrá en el servidor, aunque tendremos la posibilidad de ver el log de ejecución desde nuestra máquina, en tiempo real.

### En resumen
No todos los pasos o procesos que automatizamos en el contexto de un proyecto, funcionan tal cual en otro. De la misma manera, la automatización está limitada por la creatividad del desarrollador; lo importante es hacer una buena lectura del contexto y aplicarla con criterio.