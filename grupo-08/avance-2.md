# Grupo 8: Avance 2

Repo: 9p9yh5ztwz-wq/Estaci-n-ambiental. Proyecto: estación ambiental IoT con Arduino UNO y ESP32-S3. Integrantes: Antonia Ávila, Agustín Jiménez y Claudio Parada. Todo el trabajo se subió el 26 de octubre.

| Criterio | Nota | Observación |
|---|---|---|
| Resolución parcial problema ODS | 5.0 | Hay un sistema que funciona de punta a punta: DHT11, MQ-9 y DSM501A leen en el Arduino, un LED responde al umbral de humedad y los datos llegan por UART al ESP32, que los muestra en una página web local. El README reconoce que el MQ-9 y el DSM501A aún no están calibrados. No nombra ningún ODS ni plantea el problema que resuelve, y no hay pruebas ni mediciones registradas. |
| Proceso de iteración | 3.5 | Hay fotos del montaje y la documentación menciona que algunas lecturas siguen en validación. No hay carpetas de iteraciones ni de testing con contenido, ni versiones comparadas, ni problemas y soluciones escritos. Los commits son todos del mismo día. |
| Código documentado | 6.0 | El código del Arduino (315 líneas) tiene pines comentados, constantes con nombre (`UMBRAL_HUMEDAD`, `MQ_PIN`, `LED_PIN`), una interrupción de timer para el DSM501A y no usa `delay()`. El del ESP32 (930 líneas) valida las tramas recibidas. El README explica librerías, variables, funciones y el formato de la trama CSV. |
| Diagramas de circuito | 4.2 | Los pines del README coinciden con el código (D4, A0, D7, D8, D10 y D11 en el Arduino; GPIO 17 y 18 en el ESP32), e incluye el divisor de voltaje para pasar de 5 V a 3,3 V. Todo está descrito en texto y con dibujos ASCII, sin un diagrama hecho en Wokwi, Fritzing o KiCad. |
| Nota Sección 4 antes de penalización | 4.3 | |
| Nota Sección 5 antes de penalización | 5.1 | |
| Penalización por entrega tardía | -0.5 | Se descuenta 0.5 puntos a cada sección (1.0 punto en total). |
| Nota Sección 4 | 3.8 | |
| Nota Sección 5 | 4.6 | |

Fortalezas: sistema integrado con dos placas, tres sensores y un actuador, comunicación UART con divisor de voltaje bien pensado, código extenso con validación de datos y un README muy completo con pines y formato de datos.

Mejorar para Avance 3: subir el código en su formato propio (`.ino` o el lenguaje que usen) y no sin extensión, nombrar el ODS y el problema que atiende, hacer un diagrama de circuito en Wokwi, Fritzing o KiCad, calibrar el MQ-9 y el DSM501A y registrar las pruebas, y dejar por escrito las iteraciones con fechas y antes/después.

## Comentarios

Tienen un prototipo bastante completo: tres sensores, un actuador, dos placas conectadas y una página web, con un README que explica los pines y el formato de los datos. El código está ordenado y los pines del texto coinciden con él. Lo que más les baja la nota es que no hay un diagrama de circuito dibujado, que no se dice qué ODS ni qué problema atiende la estación, y que no hay registro de iteraciones ni de pruebas. Para el Avance 3 suban el esquema, calibren los sensores y documenten los cambios que fueron haciendo. El código debe subirse en un archivo `.ino` o en el lenguaje que usen, no sin extensión, para que conserve el formato adecuado. Se descontaron 0.5 puntos en cada sección (1.0 punto en total) por entrega tardía. Esto se debe a que entregaron fuera de plazo.
