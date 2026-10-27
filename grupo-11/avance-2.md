# Grupo 11: Avance 2

Repo: benito-diaz/Sensor-UV-colegios. Proyecto: medidor de radiación UV con semáforo para colegios. Integrantes: Maximiliano Cornejo, Benito Díaz y Benjamín Retamal. Todo el repositorio se subió el 27 de octubre.

| Criterio | Nota | Observación |
|---|---|---|
| Resolución parcial problema ODS | 5.5 | Hay un prototipo con el sensor real: un GUVA-S12SD convierte el voltaje a índice UV, un semáforo de 5 niveles sigue la escala de la OMS y se envían avisos al celular por Telegram. La calibración usa una tabla típica del sensor sin verificar y no hay pruebas con usuarios. El README principal sigue como plantilla, sin integrantes, ODS ni problema (el problema sí aparece en la iteración 1). |
| Proceso de iteración | 6.5 | El historial de v2.0 a v2.3 tiene fechas, problemas, causas y soluciones reales: faltaba el driver CP210x, la protoboard no servía, un GND flotante daba UV 4 a oscuras y Telegram devolvía errores 429, -11 y 502. Se guardó el código de cada versión y se justifica la decisión de volver a la conexión directa. Las evidencias que citan (`testing/evidencias/01_driver_cp2102_faltante.png` y `04_prueba_protoboard.jpg`) no están en el repo. |
| Código documentado | 7.0 | `main.ino` (382 líneas) tiene cabecera con conexiones y escala de la OMS, pines y ajustes comentados, una tarea separada para WiFi y Telegram y credenciales reemplazadas por texto de ejemplo. `FUENTES.md` lista librerías con versiones y explica el uso de IA con prompts y adaptaciones. |
| Diagramas de circuito | 5.5 | `esquema_conexiones` muestra ESP32, sensor y semáforo con los pines (3V3, D34, GND, D25, D26 y D27) iguales al código. Es un diagrama dibujado y no un Wokwi, Fritzing o KiCad, y no incluye valores ni el pin D32 que el código también usa para alimentar el sensor. |
| Nota Sección 4 antes de penalización | 6.0 | |
| Nota Sección 5 antes de penalización | 6.3 | |
| Penalización por entrega tardía | -0.5 | Se descuenta 0.5 puntos a cada sección (1.0 punto en total). |
| Nota Sección 4 | 5.5 | |
| Nota Sección 5 | 5.8 | |

Fortalezas: prototipo funcional con el sensor real y avisos por Telegram, historial de iteraciones muy bien documentado con problemas y decisiones, código ordenado y una explicación honesta del uso de IA.

Mejorar para Avance 3: subir al repo las evidencias que citan, calibrar el sensor contra una referencia (por ejemplo MeteoChile), hacer pruebas con 5 o más usuarios, completar el README principal con integrantes, ODS y problema, y rehacer el esquema en Wokwi, Fritzing o KiCad.

## Comentarios

El grupo tiene un prototipo funcional con el sensor real y la mejor documentación de iteraciones del curso: cada versión cuenta qué falló, por qué y cómo se resolvió. El código está ordenado y comentado, y el esquema coincide con los pines. Lo que más les baja la nota es que faltan las evidencias que citan, las pruebas con usuarios y la calibración contra una referencia. Para el Avance 3 suban esas evidencias, completen el README principal y rehagan el esquema en una herramienta estándar. Se descontaron 0.5 puntos en cada sección (1.0 punto en total) por entrega tardía. Esto se debe a que subieron el repositorio el 27 de octubre, fuera de plazo.
