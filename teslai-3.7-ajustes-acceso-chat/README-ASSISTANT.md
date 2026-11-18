# TeslAI Assistant · configuración

TeslAI Assistant usa la API de OpenAI desde un servidor Node.js. La clave privada nunca se coloca en `app.js`, `index.html` ni en el navegador.

## Requisitos
- Node.js 20 o superior.
- Una clave de API de OpenAI con facturación/crédito habilitado. El uso de la API se cobra por separado de una suscripción de ChatGPT.

## Ejecutar localmente
1. Abre una terminal en la carpeta del proyecto.
2. Ejecuta `npm install`.
3. Copia `.env.example` como `.env`.
4. Abre `.env` y reemplaza `pega_aqui_tu_clave_privada` por tu clave. No compartas la clave ni la subas a GitHub.
5. Ejecuta `npm start`.
6. Abre `http://localhost:3000`.

## Publicar en Render
GitHub Pages solo sirve archivos estáticos y no puede proteger la clave ni ejecutar este servidor. Para que el chatbot funcione en producción, publica el repositorio como un servicio web Node en un proveedor que ejecute el servidor (la configuración `render.yaml` prepara Render).

1. Sube el proyecto a un repositorio privado o público de GitHub, sin incluir `.env`.
2. En Render, crea un servicio nuevo desde ese repositorio y usa la configuración del archivo `render.yaml`.
3. En la configuración del servicio, agrega `OPENAI_API_KEY` como variable secreta. No la escribas en el repositorio, en el código del navegador ni en capturas.
4. Despliega el servicio. El mismo servidor sirve el sitio y la ruta `/api/chat`.

## Seguridad y límites
- El servidor limita el tamaño del mensaje, el historial enviado y las solicitudes por minuto.
- Las conversaciones se mantienen en la memoria de la pestaña; no se guardan en una base de datos.
- No se debe usar el chatbot para compartir información personal.
- El modelo puede equivocarse; verifica resultados importantes.
