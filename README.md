# Laika Radar

**Huellas que alcanzaron las estrellas.**

Página web de **Laika**, la pechera inteligente para mascotas: muestra la ubicación en tiempo real en un radar y permite activar el buzzer y la luz de la pechera para encontrarla.

Proyecto de San Diego Bilingual High School para la Competencia LUVÁ 2026.

## Cómo funciona

- **Pechera:** IdeaBoard (CRCibernetica) + GPS NEO-6M + buzzer + NeoPixel, programada en CircuitPython.
- **Datos:** la pechera escribe su posición en Firebase Realtime Database (`/laika/estado`) y lee las órdenes de la web (`/laika/comando`).
- **Web:** esta página lee Firebase cada 3 segundos, dibuja a Laika en el radar con sus huellas y envía las órdenes de buzzer, modo búsqueda y color de la luz.

Sin datos de la pechera, el botón **Volver a demo** muestra una Laika simulada.
