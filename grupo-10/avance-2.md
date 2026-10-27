# Grupo 10: Avance 2

Repo: isiparrab/sensor_ruido_clases. Integrantes: Matilda Steiner, Isidora Parra, Isidora Vidal y Florencia Gutiérrez. Se re-evaluó con lo subido hasta el 26 de octubre.

| Criterio | Nota | Observación |
|---|---|---|
| Resolución parcial problema ODS | 5.5 | El README conecta el problema (crisis por ruido en niños con TEA) con los ODS 4 y 10, y ahora hay un sistema de dos módulos que funciona: un ESP32 en la pizarra con el micrófono KY-038 y un semáforo RGB, una red WiFi propia con página web en vivo, y un botón de escritorio que enciende una luz blanca. Hay fotos del prototipo y renders 3D. Faltan pruebas con usuarios: `testing/` sigue en plantilla. |
| Proceso de iteración | 5.5 | La iteración 2 tiene una tabla de cambios de v1 a v2, tres problemas con su causa y solución (dependencia del hotspot, presiones del botón perdidas, amarillo que no se veía), la calibración de umbrales de 15/1000 a 17/42, la respuesta al feedback del profesor y los pasos de la v3. Las iteraciones 1 y 3 siguen en plantilla y no hay copias del código de cada versión. |
| Código documentado | 6.5 | Tres sketches (`central.ino`, `boton_estudiante.ino` y la prueba del micrófono) con cabecera, qué hace cada módulo, historial de versiones, constantes con nombre y comentarios útiles. Las librerías y el uso de IA están en `FUENTES.md`. Las carpetas del código tienen espacios al inicio del nombre y `software/librerias` sigue como plantilla. |
| Diagramas de circuito | 5.0 | Hay una captura de Wokwi con un potenciómetro en lugar del KY-038, lo que no se penaliza, y los pines (34, 25, 26 y 27) coinciden con el código. El diagrama no incluye el RGB #2 ni el módulo del botón, que solo están en una tabla del BOM, y muestra tres LEDs separados donde el prototipo real usa un RGB. |
| Nota Sección 4 antes de penalización | 5.5 | |
| Nota Sección 5 antes de penalización | 5.8 | |
| Penalización por entrega tardía | -0.25 | Se descuenta 0.25 puntos a cada sección (0.5 puntos en total). |
| Nota Sección 4 | 5.3 | |
| Nota Sección 5 | 5.5 | |

Fortalezas: prototipo completo con dos módulos que se comunican por WiFi, iteración 2 bien documentada con problemas y soluciones, código ordenado y comentado, y diseño 3D con renders.

Mejorar para Avance 3: completar el diagrama con el RGB #2 y el módulo del botón, documentar las iteraciones 1 y 3, hacer pruebas con 5 o más usuarios y registrar los resultados, llenar `software/librerias`, y renombrar las carpetas del código sin espacios al inicio.

## Comentarios

Subieron mucho desde la primera revisión: ahora hay un prototipo que funciona, con código comentado, una iteración documentada con sus problemas y un diagrama en Wokwi cuyos pines coinciden con el código. Lo que falta es evidencia de uso real, porque no hay pruebas con usuarios, y que el diagrama incluya el botón y la segunda luz. Para el Avance 3 completen el esquema, documenten las otras iteraciones y registren las pruebas. Se descontaron 0.25 puntos en cada sección (0.5 puntos en total) por entrega tardía, pero es un descuento menor porque el grupo ya había subido trabajo desde el principio y se vio su avance.
