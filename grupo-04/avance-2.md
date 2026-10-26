# Grupo 4: Avance 2

Repo: sophifuenzalidaa13/TEI201_Bitacora. Integrantes: Sophia Fuenzalida, Sofía Lagos, Rafaela Montero y Sofía Campos.

| Criterio | Nota | Observación |
|---|---|---|
| Resolución parcial problema ODS | 4.5 | El problema está bien planteado (fatiga al volante, dato ACHS) y el prototipo calibra 30 s y alarma si el BPM varía más de 20%. No explican por qué esa variación indica somnolencia, no hay pruebas con usuarios y la conexión con el ODS 11 es débil. |
| Proceso de iteración | 2.5 | Hay una simulación Wokwi, un plano v10 y el .ino final, pero declaran "v10" sin documentar v1 a v9. `iteraciones/` y `testing/` son plantilla y todo se subió en pocos días (19 al 21 de octubre). |
| Código documentado | 6.0 | `monitor_cardiaco_s3.ino` (363 líneas) tiene cabecera, pines, constantes descriptivas y una máquina de estados. Hay pocos comentarios dentro de las funciones y el código está en `hardware/` en vez de `software/src`. |
| Diagramas de circuito | 4.5 | Hay una captura Wokwi con un potenciómetro en lugar del sensor de pulso, lo que no se penaliza (se autorizó por falta del sensor en Wokwi). Los pines sí fallan: el buzzer está en GPIO 18 y el código usa GPIO 3. El plano v10 es mecánico, no eléctrico. |
| Nota Sección 4 | 3.5 | |
| Nota Sección 5 | 5.3 | |

Fortalezas: firmware funcional con calibración personalizada y web móvil, problema respaldado con un dato y encapsulado coherente (.f3d y plano con dimensiones).

Mejorar para Avance 3: documentar las iteraciones reales con fechas y antes/después. Probar con 5 o más usuarios y registrar BPM y falsos positivos. Subir un diagrama coherente con el .ino y ordenar el repo (código en `software/src`).
