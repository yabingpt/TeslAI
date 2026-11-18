# TeslAI 4.6 — Asistente de dos especialidades

## Enfoque del asistente
TeslAI Assistant se limita a dos áreas:
1. Física básica: cinemática, MRU, MRUA, caída libre, leyes de Newton, fuerzas, fricción, trabajo, energía y potencia mecánica.
2. Inteligencia artificial aplicada al tráfico: movilidad inteligente, flujo y densidad vehicular, sensores, cámaras, visión artificial, radar, LiDAR, semáforos adaptativos, ADAS, vehículos autónomos, frenado y prevención de accidentes.

Se retiró electricidad básica y se eliminaron las categorías independientes de matemáticas e inteligencia artificial general. Las fórmulas y operaciones matemáticas se ofrecen como herramientas dentro de los dos temas centrales.

## Estructura didáctica
Cada subtema ofrece cuatro rutas:
- Comprender el concepto.
- Consultar fórmulas y despejes.
- Ver un ejemplo resuelto.
- Resolver un problema guiado.

## Conversación compacta
Cada nuevo mensaje del usuario reemplaza el intercambio anterior (mensaje del usuario y respuesta de TeslAI), evitando que el historial crezca indefinidamente. Los menús se vuelven a presentar cuando se navega entre áreas.

## Funcionamiento
El asistente utiliza respuestas locales en JavaScript. No requiere API, servidor ni conexión a servicios externos. Para la primera carga y el almacenamiento offline del sitio, el navegador debe poder acceder a los archivos; después el service worker conserva los recursos estáticos.
