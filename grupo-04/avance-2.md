# Grupo 4: Avance 2

Repo: sophifuenzalidaa13/TEI201_Bitacora (y repo anterior sophifuenzalidaa13/bitacora-dise-o). Integrantes: Sophia Fuenzalida, Sofía Lagos, Rafaela Montero y Sofía Campos.

| Criterio | Nota | Observación |
|---|---|---|
| Resolución parcial problema ODS | 4.5 | El problema está bien planteado (fatiga al volante, dato ACHS) y el prototipo calibra 30 s y alarma si el BPM varía más de 20%. No explican por qué esa variación indica somnolencia, no hay pruebas con usuarios y la conexión con el ODS 11 es débil. |
| Proceso de iteración | 5.5 | Hay una evolución visible entre el 28 de septiembre y el 19 de octubre: de una simulación inicial a un diseño 3D con componentes definidos, plano técnico v10 y código con fases de calibración y alarma. Se subió la nota considerando los dos repositorios. No hay versiones intermedias de código ni de circuito, ni pruebas con usuarios, y las carpetas de iteraciones y testing quedaron como plantilla. |
| Código documentado | 6.0 | `monitor_cardiaco_s3.ino` (363 líneas) tiene cabecera, pines, constantes descriptivas y una máquina de estados. Hay pocos comentarios dentro de las funciones y el código está en `hardware/` en vez de `software/src`. |
| Diagramas de circuito | 4.5 | Hay una captura Wokwi con un potenciómetro en lugar del sensor de pulso, lo que no se penaliza (se autorizó por falta del sensor en Wokwi). Los pines sí fallan: el buzzer está en GPIO 18 y el código usa GPIO 3. El plano v10 es mecánico, no eléctrico. |
| Nota Sección 4 | 5.0 | |
| Nota Sección 5 | 5.3 | |

Fortalezas: firmware funcional con calibración personalizada y web móvil, problema respaldado con un dato y encapsulado coherente (.f3d y plano con dimensiones).

Mejorar para Avance 3: documentar las iteraciones con fechas y antes/después, incluir el sensor real con los pines correctos, probar con 5 o más usuarios y registrar BPM y falsos positivos, y ordenar el repo (código en `software/src`).

## Comentarios

El firmware funciona y está bien estructurado, con calibración personalizada y una web para el celular. Usar un potenciómetro en lugar del sensor de pulso no les baja la nota, porque Wokwi no tenía el sensor. Sí pesa que el buzzer esté en el GPIO 18 en el diagrama y en el GPIO 3 en el código. Revisé también su repositorio anterior y la nota de iteración sube a 5.5 por la evolución entre septiembre y octubre. Aun así no hay versiones intermedias ni pruebas documentadas, y no explican por qué un cambio en el BPM indica somnolencia. Para el Avance 3 incluyan el sensor real con los pines correctos y registren las pruebas.
