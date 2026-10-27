# Grupo 7: Avance 2

Repo: Macarena2026/proyecto_final_TEI201. Integrantes: Macarena Aldana, Sofía Godoy y Daniela Oñate. Se re-evaluó con lo subido hasta el 26 de octubre.

| Criterio | Nota | Observación |
|---|---|---|
| Resolución parcial problema ODS | 4.5 | El problema está bien definido (obstáculos sobre el torso, cifras de Chile) y la conexión con los ODS 3 y 10 es razonable. Falta evidencia vivencial: no hay pruebas con usuarios, `testing/` está vacío y `pruebas.md` marca todo como pendiente. |
| Proceso de iteración | 4.8 | Hay dos versiones del diseño 3D y dos del circuito: la v1 incluía un TP4056 y la v2 lo quita y conecta la batería directo a la placa. Además hay un plan de pruebas en `pruebas.md`. Las carpetas `iteraciones/` siguen en plantilla, sin antes/después ni problemas resueltos escritos. |
| Código documentado | 6.0 | `main.ino` tiene constantes descriptivas (`DIST_MAX`, `PWM_MIN`, `MOTOR_PIN`), comentarios útiles, estructura clara en `setup()` y `loop()` y manejo de timeout y de error del sensor. Las librerías están documentadas con instrucciones de instalación. Falta una cabecera (autores, versión) y comentarios por bloque en `loop()`. |
| Diagramas de circuito | 5.5 | Los pines coinciden con el código (SDA 4, SCL 5 y pin 6 al transistor 2N2222). Incluye diodo, interruptor, batería, colores y leyenda, y hay dos versiones. Está dibujado a mano, faltan el valor del resistor, el modelo de placa y el voltaje de la batería, y la leyenda dice 5 V mientras el sensor y el motor van a 3,3 V. |
| Nota Sección 4 antes de penalización | 4.7 | |
| Nota Sección 5 antes de penalización | 5.8 | |
| Penalización por entrega tardía | -1.0 | Se descuenta 1.0 punto a cada sección. |
| Nota Sección 4 | 3.7 | |
| Nota Sección 5 | 4.8 | |

Fortalezas: pasaron de no tener código a un firmware coherente con el diagrama y bien documentado, con limitaciones reconocidas con honestidad y un diagrama v2 que mantiene la correspondencia de pines.

Mejorar para Avance 3: llenar `iteraciones/` con fechas, problemas y antes/después (por ejemplo por qué se quitó el TP4056), hacer pruebas con 5 o más usuarios y subir el video, rehacer el diagrama en Wokwi o Fritzing con valores y modelo de placa, convertir las fotos HEIC a JPG y agregar cabecera al `main.ino`.

## Comentarios

Subieron bastante desde la primera revisión: ahora hay código comentado, documentación de software y la segunda versión del diagrama, con los pines coincidiendo con el código. Eso mejora las notas de código y de iteración. Queda pendiente escribir las iteraciones, que siguen como plantilla, y hacer pruebas con usuarios para tener evidencia del impacto. Las dos fotos del prototipo están en formato HEIC con extensión .jpg, por lo que no se abren. Para el Avance 3 conviértanlas, corrijan la leyenda de voltaje del diagrama y registren los resultados de las pruebas. Se descontó 1.0 punto en cada sección por entrega tardía. Esto se debe a que entregaron fuera de plazo.
