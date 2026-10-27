# Grupo 5: Avance 2

Repo: mrtn-fl/proyecto_final_TEI201_GRUPO5. Proyecto: COStop, alarma doméstica de monóxido de carbono. Integrantes: Benjamín Bidegain, Martín Flores, Vicente Pincheira y Thomas Von Fabeck. Se re-evaluó con lo subido hasta el 27 de octubre.

| Criterio | Nota | Observación |
|---|---|---|
| Resolución parcial problema ODS | 5.5 | El problema está bien fundamentado (intoxicaciones por CO en el sur de Chile, adultos mayores y niños) y el firmware implementa una alarma con umbrales, histéresis y confirmación de lecturas. Ahora hay además una caja diseñada en MDF con su justificación, renders y planos. Falta evidencia de funcionamiento (fotos, video, monitor serial) y pruebas con CO real o con usuarios. |
| Proceso de iteración | 5.5 | `iteraciones/README.md` cuenta la evolución de v1 a v2: de protoboard con botón BOOT y alimentación por USB a placa soldada con batería LiPo, TP4056, pulsador dedicado e interruptor. Incluye problemas, razones e impacto de cada cambio, y se guardaron `v1_codigo.ino` y `v1_esquema.jpg`. Quedan marcadores `[COMPLETAR]` y `[medir]`, no hay fotos de cada versión y el README dice que el software no cambió, aunque el código pasó de DHT22 a DHT11. |
| Código documentado | 7.0 | `codigo_esp32.ino` tiene cabecera con descripción y funcionamiento, pines y parámetros comentados, una máquina de estados clara y funciones separadas. La documentación de software explica funciones, librerías, instalación y operación, con dos diagramas de flujo. |
| Diagramas de circuito | 4.0 | Hay un diagrama en Wokwi (MQ-7, DHT22, buzzer y botón) y el esquema v1. Está hecho con una ESP32 clásica y no con la S3 Super Mini del código, no incluye el LED RGB y los pines no calzan con los GPIO del código (MQ-7 en 1, buzzer en 5, LED en 6, 8 y 9). Los planos del encapsulado son mecánicos, no eléctricos. |
| Nota Sección 4 antes de penalización | 5.5 | |
| Nota Sección 5 antes de penalización | 5.5 | |
| Penalización por entrega tardía | -0.5 | Se descuenta 0.5 puntos a cada sección (1.0 punto en total). |
| Nota Sección 4 | 5.0 | |
| Nota Sección 5 | 5.0 | |

Fortalezas: problema bien fundamentado, firmware con decisiones técnicas sólidas (histéresis, confirmación de lecturas, detección de falla del sensor), documentación de software extensa, historial de iteraciones con justificación y diseño de encapsulado completo.

Mejorar para Avance 3: rehacer el diagrama con la placa real (ESP32-S3 Super Mini), el LED RGB, la batería y el TP4056, con los pines del código. Completar los marcadores pendientes de la iteración 1, agregar fotos de cada versión, aportar evidencia de funcionamiento y datos de calibración del MQ-7, y probar con usuarios.

## Comentarios

Avanzaron bastante desde la primera revisión y se nota el esfuerzo del grupo. Ahora hay historial de iteraciones, código bien comentado, esquema, diseño 3D y una justificación de la caja, y los commits vienen de varios integrantes. Lo que más pesa en la nota es el diagrama: usa otra placa, no tiene el LED RGB y los pines no coinciden con los del código. Faltan también fotos y evidencia del sistema funcionando. Para el Avance 3 rehagan el esquema con los componentes reales y registren pruebas. Se descontaron 0.5 puntos en cada sección (1.0 punto en total) por entrega tardía. Esto se debe a que entregaron fuera de plazo.
