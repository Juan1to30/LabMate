# ADR-001: Alcance inicial de LabMate

- **Estado:** propuesta, pendiente de validar por Alex, Oscar y Aritz
- **Fecha:** 2026-10-19 (Sprint 1)

## Contexto

La idea presentada era un asistente de IA local para trabajar con un proyecto. En los formularios individuales del Sprint 1 los tres coinciden en lo importante:

- Que funcione **en local** y proteja la **privacidad**.
- Que **no se invente** información.
- Que empiece **solo leyendo**, y que editar o ejecutar quede para más adelante con permiso.
- Que lo probemos nosotros mismos con errores hechos a propósito.

También hay ideas distintas:

- Alex propone repartir el modelo entre varios equipos (ThinkCentre y portátiles) en una red privada.
- Oscar y Aritz piensan en un solo equipo.
- Aritz querría que pudiera leer todo el ordenador. Alex y Oscar prefieren limitarlo a la carpeta del proyecto, y los datos sensibles se quedan en el PC.

Tenemos unas 3 horas por persona y semana, y hardware muy distinto (RTX 3080 Ti, portátil con RTX 3050, ThinkCentre sin GPU).

## Decisión propuesta

**Primera versión (MVP):** LabMate funciona en **un solo equipo**, en **modo solo lectura** y **solo sobre la carpeta del proyecto** que el usuario elige. Debe poder:

1. Consultar los archivos de la carpeta.
2. Resumir documentos.
3. Guardar notas internas del proyecto.
4. Decir "no lo sé" cuando no tenga base para responder, en lugar de inventar.

**Se pospone (Sprint 2 en adelante):**

- Repartir el modelo entre varios equipos. Es la **línea de infraestructura de ASIX**: red privada, rendimiento y límites de RAM y red.
- Que LabMate edite archivos o ejecute comandos (solo con permiso explícito).
- Leer fuera de la carpeta del proyecto.

## Motivo

- Con 9 horas semanales entre los tres, hay que cerrar primero una versión que funcione y se pueda demostrar.
- El reparto entre equipos tiene riesgo alto (wifi del centro, equipos distintos). Conviene medirlo cuando ya exista un MVP.
- Limitar el acceso a la carpeta reduce el riesgo de leer claves u otros datos sensibles.

## Consecuencias

- El MVP es más pequeño que la idea presentada: se documenta aquí el motivo del ajuste, como permite la guía del Sprint 1.
- La idea del reparto entre equipos no se descarta: pasa a ser un experimento posterior y medible.
- Si el equipo no está de acuerdo, se cambia el estado de este documento y se anota el motivo.
