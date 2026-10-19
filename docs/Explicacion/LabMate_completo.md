# LabMate

## La idea
LabMate es un asistente de inteligencia artificial que funciona en local, es decir, dentro de nuestros propios ordenadores y sin enviar nuestros datos a empresas externas. La idea es abrirlo desde la terminal, dentro de la carpeta de trabajo de un proyecto, y poder hablar con él como con una IA conversacional, pero una que conoce de verdad lo que hay en esa carpeta.

Los tres lo imaginamos de formas distintas, pero parecidas. Aritz lo ve como un compañero que sabe más que tú y te acompaña en todo, pero te deja hacer tu trabajo. Alex lo ve como una herramienta dentro del repositorio, parecida a Claude Code, a la que le preguntas cómo va el tablero, cuál fue el último commit o por dónde se quedó cada uno. Oscar lo describe como una IA para trabajar en proyectos de forma local. Lo que tienen en común las tres ideas es que LabMate vive junto al proyecto y ayuda a trabajar en él.

## Qué problema queremos resolver
Hoy, cuando alguien se atasca con un proyecto, acaba copiando y pegando código en una IA externa. Eso hace perder tiempo, obliga a explicar todo cada vez y supone enviar nuestro trabajo a servicios de fuera. Además, las IA generales no están pensadas para quien programa o administra sistemas, y a veces dan respuestas equivocadas o se inventan cosas, lo que lleva a tomar malas decisiones.

LabMate quiere resolver eso con una IA privada, que conozca el proyecto y no cobre una mensualidad. Pensamos en estudiantes y desarrolladores como Alex, Oscar y Aritz, que trabajan en proyectos con muchos archivos.

## Cómo se usaría
Un ejemplo de Alex: abres LabMate en la terminal y le preguntas qué te toca hacer hoy. LabMate responde que ayer no terminaste un trabajo y que tienes cambios sin subir, y te recomienda acabarlos antes de empezar la siguiente tarea del tablero.

Otro ejemplo, de Oscar y Aritz: un proyecto con muchos archivos empieza a fallar. En vez de copiar el código a una IA de fuera, le indicas la carpeta a LabMate. Él mira los archivos, te dice dónde puede estar el error y hacia dónde tirar. Si el usuario le da permiso, puede incluso ayudar a arreglarlo.

## Qué tiene que hacer bien
Entre las tres respuestas aparecen siempre las mismas capacidades:
- Consultar los archivos de la carpeta y saber qué hay ahora mismo en el proyecto.
- Resumir documentos.
- Guardar notas o recuerdos del proyecto para no empezar de cero en cada chat.
- No inventar. Si no sabe algo o no entiende la pregunta, tiene que decirlo y pedir más información.

## Reglas de privacidad y permisos
Los tres insistimos en la privacidad. LabMate funciona en local y no manda nada fuera. Las contraseñas, claves y otros datos sensibles no deben salir del ordenador ni llegar a la IA.

También coincidimos en que al principio solo debe leer. Editar archivos o ejecutar cosas es algo que se deja para más adelante y siempre con permiso explícito del usuario, como pasar de "lector" a "editor".

## Dónde pensamos distinto
- **Qué puede leer.** Alex y Oscar prefieren limitarlo a la carpeta del proyecto. Aritz piensa que, siendo local, podría consultar todo el ordenador para ayudar más.
- **Dónde funciona.** Alex quiere repartir el modelo entre varios ordenadores: el servidor guarda y coordina, y los portátiles juntan su CPU y su RAM. Oscar y Aritz piensan sobre todo en un solo equipo, el más potente, y les preocupan la RAM y la VRAM.
- **Cómo se prueba.** Alex propone probar LabMate sobre su propio repositorio. Oscar, cargar un proyecto de prueba. Aritz, hacer pruebas a mano: meter errores a propósito y ver si LabMate los encuentra, subiendo la dificultad poco a poco.

## Riesgos
- Aritz recuerda que el proyecto es muy ambicioso y el tiempo, limitado. Hay que ir al día y comunicarnos si cambia la idea.
- Alex avisa de que juntar equipos distintos casi no se hace, y de que el wifi del centro puede limitar el rendimiento.
- Oscar insiste en no olvidar nunca la privacidad.

## Cómo nos repartimos
Cada uno aporta lo que mejor sabe. Alex conoce IA locales y tiene varios modelos en su PC. Oscar es el único de DAM y ya montó un miniPC como bot de trading. Aritz aporta ideas, pensamiento abstracto y organización, y quiere coordinar el concepto y el diseño. Trabajamos unas 3 horas por persona y semana.

## Qué haremos primero
Para no pasarnos de ambiciosos, la primera versión será pequeña: un solo ordenador, en modo solo lectura, sobre la carpeta de un proyecto. Podrá consultar archivos, resumir y guardar notas. Lo demás, como arreglar cosas él solo, repartir el modelo entre varios equipos o una interfaz más bonita, se deja para más adelante. Esta propuesta falta confirmarla entre los tres.