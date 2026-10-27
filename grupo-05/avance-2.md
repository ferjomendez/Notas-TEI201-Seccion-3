# Grupo 5: Avance 2

Repo: mrtn-fl/proyecto_final_TEI201_GRUPO5. Proyecto: COStop, alarma doméstica de monóxido de carbono. Integrantes: Benjamín Bidegain, Martín Flores, Vicente Pincheira y Thomas Von Fabeck. Casi todo el trabajo se subió el 26 de octubre y el repo sigue recibiendo commits.

| Criterio | Nota | Observación |
|---|---|---|
| Resolución parcial problema ODS | 4.8 | El README plantea bien el problema (intoxicaciones por CO en el sur de Chile, adultos mayores y niños) y el firmware implementa una alarma con umbrales, histéresis y confirmación de lecturas. Falta evidencia de funcionamiento (capturas del monitor serial, Wokwi, fotos o video), pruebas con CO real o con usuarios y los próximos pasos. |
| Proceso de iteración | 2.5 | Las carpetas `iteraciones/` y `testing/` son la plantilla sin llenar y hay un solo commit de código. Solo hay indicios de cambios menores en la documentación (DHT22 a DHT11, botón BOOT provisorio, tiempo de calentamiento). No hay versiones comparadas ni problemas y soluciones propios. |
| Código documentado | 5.5 | Un sketch de 162 líneas con variables descriptivas, constantes comentadas, funciones separadas (`leerMQ`, `revisarBoton` con antirrebote) y una máquina de estados. La librería DHT está documentada. Los comentarios son breves, falta una cabecera y las versiones de librerías quedaron como `v[x]`. |
| Diagramas de circuito | 2.0 | No hay diagrama de conexiones: `hardware/esquemas` es plantilla. Los dos diagramas de flujo de software (estados y nivel) están bien hechos, pero no reemplazan el esquema eléctrico. |
| Nota Sección 4 antes de penalización | 3.7 | |
| Nota Sección 5 antes de penalización | 3.8 | |
| Penalización por entrega tardía | -0.5 | Se descuenta 0.5 puntos a cada sección (1.0 punto en total). |
| Nota Sección 4 | 3.2 | |
| Nota Sección 5 | 3.3 | |

Fortalezas: problema bien fundamentado con datos, firmware con decisiones técnicas sólidas (histéresis, confirmación de lecturas, detección de falla del sensor) y documentación de software extensa.

Mejorar para Avance 3: entregar el diagrama de conexiones con los pines del código, documentar las iteraciones propias, aportar evidencia de funcionamiento y datos de calibración del MQ-7, y repartir los commits entre los integrantes (todos son de una sola cuenta) subiéndolos de forma progresiva.

## Comentarios

El problema está bien fundamentado y el código es ordenado y tiene buenas decisiones técnicas. Lo que más les baja la nota es que no hay diagrama de circuito ni registro de iteraciones y pruebas: las carpetas de iteraciones y testing siguen con la plantilla. Casi todo el repositorio se subió el 26 de octubre, y todos los commits son de una sola persona. Para el Avance 3 suban el esquema con los pines, documenten los cambios que sí hicieron (como pasar de DHT22 a DHT11) y muestren evidencia del sistema funcionando. Se descontaron 0.5 puntos en cada sección (1.0 punto en total) por entrega tardía. Esto se debe a que entregaron fuera de plazo.
