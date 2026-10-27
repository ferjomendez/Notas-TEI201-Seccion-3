# Grupo 2: Avance 2

Repo: joaco-eng/Proyecto-tei. Proyecto: sistema detector de nivel anormal en sumidero. Último commit: 18 de octubre. El README no lista integrantes.

| Criterio | Nota | Observación |
|---|---|---|
| Resolución parcial problema ODS | 4.0 | Hay un prototipo funcional: ESP32 con sensor ultrasónico, umbral de 8 cm con confirmación de 5 s, alerta con LED y página web de monitoreo. El repo no nombra ningún ODS ni explica el problema, y no hay evidencia de funcionamiento (capturas, video o pruebas con agua) ni próximos pasos. |
| Proceso de iteración | 4.0 | El historial muestra iteración real el 18 de octubre: monitor web, conexión WiFi, corrección de la redirección desde https y un portal cautivo de configuración. No hay documentación de pruebas, de problemas y soluciones, ni comparación antes y después. |
| Código documentado | 6.0 | El `.ino` está organizado en secciones, con cabecera de pines y endpoints, constantes comentadas (`UMBRAL_ALERTA`, `TIEMPO_CONFIRMACION`) y uso de `millis()` sin bloqueo. Las funciones de WiFi y del portal tienen pocos comentarios y falta explicar la conversión de `pulseIn` a centímetros. |
| Diagramas de circuito | 2.0 | No hay diagrama ni imagen. Solo existe una tabla de pines en el README (TRIG 5, ECHO 4, LED 6 con 220 Ω) que coincide con el código. |
| Nota Sección 4 antes de penalización | 4.0 | |
| Nota Sección 5 antes de penalización | 4.0 | |
| Penalización por entrega tardía | -0.5 | Se descuenta 0.5 puntos a cada sección (1.0 punto en total). |
| Nota Sección 4 | 3.5 | |
| Nota Sección 5 | 3.5 | |

Fortalezas: firmware funcional y bien organizado con una máquina de estados clara, portal cautivo sin claves en el código y un historial de commits descriptivo.

Mejorar para Avance 3: agregar un diagrama de conexiones en Wokwi o Fritzing con los pines, documentar los cambios, problemas y decisiones (por qué 8 cm y 5 s), incluir evidencia de pruebas, nombrar el ODS y el problema, y listar a los integrantes en el README.

## Comentarios

El código está bien armado y el historial muestra que fueron mejorando el sistema, con WiFi, portal de configuración y monitor web. Lo que falta es la documentación: no hay diagrama de circuito, ni registro de pruebas, ni se dice qué ODS atiende el proyecto. La tabla de pines coincide con el código, pero no reemplaza un diagrama. Para el Avance 3 suban el esquema con el sensor y todos los pines, y dejen por escrito las pruebas y las decisiones técnicas. Se descontaron 0.5 puntos en cada sección (1.0 punto en total) por entrega tardía. Esto se debe a que entregaron fuera de plazo.
