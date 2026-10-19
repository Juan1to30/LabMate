# Propuesta de stack tecnológico de LabMate

## 1. Objetivo

El objetivo es seleccionar tecnologías que permitan desarrollar LabMate como un asistente de IA local para consultar documentación, interpretar registros de un laboratorio Linux, ayudar a diagnosticar incidencias y guardar el historial de las soluciones aplicadas.

La selección prioriza el uso de herramientas abiertas, la ejecución local, la facilidad de mantenimiento, la seguridad y la posibilidad de desarrollar el proyecto progresivamente durante el curso.

## 2. Tecnologías propuestas

**Sistema operativo:** Ubuntu Server Linux, utilizado como entorno principal del laboratorio de pruebas.

**Lenguaje de programación:** Python, por su facilidad de integración con herramientas de administración de sistemas y modelos de inteligencia artificial.

**Backend y API:** FastAPI, para gestionar las peticiones del panel web y comunicar los diferentes componentes.

**Inteligencia artificial local:** Ollama como opción inicial para ejecutar modelos localmente. El modelo definitivo se seleccionará después de evaluar los recursos de hardware, la velocidad y la calidad de las respuestas.

**Base de datos:** SQLite para almacenar las incidencias, las notas del proyecto y los resultados de las pruebas iniciales.

**Interfaz web:** HTML, CSS y JavaScript para desarrollar un panel sencillo de consulta y visualización.

**Despliegue:** Docker y Docker Compose para facilitar la instalación y reproducción de los servicios cuando la arquitectura esté definida.

**Control de versiones y organización:** Git y GitHub para mantener el código, documentar decisiones y gestionar el backlog mediante Issues.

## 3. Justificación

Python y FastAPI permiten desarrollar un backend modular sin introducir una complejidad excesiva. Ollama ofrece una vía para evaluar modelos locales, mientras que SQLite resulta suficiente para las primeras pruebas y el almacenamiento de información estructurada.

La combinación de Ubuntu Server y un servicio web de ejemplo permitirá trabajar con registros y configuraciones reales en un entorno controlado. Docker Compose podrá facilitar la reproducción del sistema una vez definidos sus componentes.

## 4. Seguridad

LabMate comenzará con funciones de consulta y análisis. Las acciones que puedan modificar el sistema deberán estar restringidas, requerir confirmación humana y probarse en una máquina aislada. Se aplicarán permisos mínimos y se evitará conceder acceso indiscriminado a archivos, credenciales o comandos del sistema.

## 5. Decisiones pendientes

Antes de cerrar el stack definitivo, será necesario comprobar los recursos disponibles, elegir y probar el modelo local, concretar el mecanismo de acceso a los registros y decidir qué componentes se ejecutarán en contenedores.

Esta propuesta es una base de trabajo para el Sprint 1 y podrá revisarse durante el desarrollo.