# TeslAI 4.5 – Chat educativo ampliado y sin conexión

Esta versión conserva la experiencia visual y la navegación guiada de TeslAI 4.4, pero amplía el chat para convertirlo en el espacio principal de consulta y aprendizaje.

## Cambios
- Biblioteca local ampliada con explicaciones estructuradas, fórmulas, variables, ejemplos, aplicaciones y límites de los modelos.
- Más subtemas en física, matemáticas, inteligencia artificial e IA aplicada al tráfico.
- La conversación ocupa mejor el espacio disponible; los mensajes, tarjetas temáticas y sugerencias tienen mayor jerarquía visual.
- Se conserva la selección por áreas, subtemas y tipo de ayuda, además de la entrada de texto libre.
- Sin API, servidor ni claves. El asistente procesa las consultas en el navegador.
- Se actualizó la versión de caché del service worker para evitar servir archivos anteriores.

## Límites
El asistente utiliza una biblioteca educativa local y reconocimiento por palabras y frases. No es un modelo generativo y no puede responder de forma fiable cualquier pregunta fuera de sus contenidos. Las respuestas de ejercicios son ejemplos didácticos; conviene verificar resultados y unidades.

## Uso
Abre `index.html` en un navegador moderno. Para instalar el service worker y disponer de caché sin conexión, sirve la carpeta desde un origen local o HTTPS y realiza una primera carga con conexión.
