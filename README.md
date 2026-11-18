# TeslAI 5.1 · Asistente educativo offline

TeslAI es una experiencia educativa estática sobre dos áreas: **Física básica** e **inteligencia artificial aplicada al tráfico**. El asistente utiliza una biblioteca local de contenidos y reglas de reconocimiento; no es un modelo generativo.

## Novedades 5.1

- El chat es el espacio principal del asistente, con globos diferenciados, estados visuales y animación del personaje.
- Navegación guiada integrada en la conversación: área → subtema → concepto, fórmulas, ejemplo o problema guiado.
- Biblioteca local estructurada para 38 subtemas, cada uno con explicación, fórmulas y unidades, ejemplo desarrollado y ejercicio de práctica.
- Los problemas guiados esperan una respuesta numérica, la comparan con el resultado esperado y ofrecen retroalimentación y pistas.
- Reconocimiento de saludos, despedidas, agradecimientos, acentos omitidos y distintas expresiones de consultas.
- Contexto básico de seguimiento: preguntas como «¿y su fórmula?» pueden referirse al subtema activo.
- Conversación compacta: cada nuevo mensaje reemplaza el intercambio visible anterior, sin perder el contexto de la lección o del ejercicio actual.
- Sin API, claves, servicios de IA externos ni lógica de servidor.

## Ejecutar

Abre `index.html` en un navegador moderno. Para que la experiencia pueda instalarse y guardar sus recursos para uso posterior sin conexión, publícala primero en un alojamiento estático HTTPS y ábrela una vez con conexión. Después, el service worker conserva los archivos locales. Abrir el HTML directamente como archivo (`file://`) puede limitar el almacenamiento offline según el navegador.

## Límites

Las respuestas son predefinidas y se seleccionan mediante reglas, sinónimos y reconocimiento aproximado de términos. El asistente solo está preparado para los dos campos indicados; no puede responder preguntas arbitrarias como un modelo generativo. Los ejercicios numéricos comprueban respuestas de la biblioteca local y no sustituyen la revisión docente.

## Correcciones 5.1
- Diseño del chat reorganizado para teléfonos: área de conversación flexible, desplazamiento vertical interno, burbujas adaptables y compositor que no desborda el ancho.
- Física ampliada con densidad, unidades, vectores, masa y peso, presión, movimiento circular, momento e impulso, y las tres leyes de Newton explicadas por separado.
- Tráfico alineado con los siete módulos de aprendizaje guiado: variables macroscópicas y microscópicas, flujo, densidad vehicular, headway, ITS, sensores, control semafórico, visión, dinámica vehicular y validación de IA.
