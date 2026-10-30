# Grupo 12: Avance 2

Repo: dpoupinr/proyecto_final_TEI201 (rama dpoupinr-patch-1). Proyecto: llenado automático de estanques con flotador P35, ESP32 y relé para zonas rurales. Integrantes: Mateo Candela, Claudio Martínez y Diego Poupin. El README y las vistas 3D se subieron el 26 y 27 de octubre, y el código el 29 de octubre.

| Criterio | Nota | Observación |
|---|---|---|
| Resolución parcial problema ODS | 3.5 | El problema y el ODS 6 están bien planteados, y hay código con la lógica completa de llenado. No hay fotos del montaje ni pruebas. El README describe notificaciones al celular y estadísticas de consumo que el código no incluye. |
| Proceso de iteración | 2.0 | Las carpetas `iteraciones/` y `testing/` siguen como plantilla, sin historial, problemas ni evidencias. |
| Código documentado | 6.0 | Cabecera con conexiones y lógica, pines y parámetros explicados, y una máquina de estados con antirrebote y descanso del motor. Baja porque se subió pegado en `software/src/README.md` y no como archivo `.ino`, y porque no incluye WiFi ni app. |
| Diagramas de circuito | 2.0 | No hay esquema en Wokwi, Fritzing ni KiCad. Hay un modelo 3D de la caja en Tinkercad y fotos de apuntes con especificaciones de componentes, pero las conexiones solo aparecen en la cabecera del código. |
| Nota Sección 4 antes de penalización | 2.8 | |
| Nota Sección 5 antes de penalización | 4.0 | |
| Penalización por entrega tardía | -0.5 | Se descuenta 0.5 puntos a cada sección (1.0 punto en total). |
| Nota Sección 4 | 2.3 | |
| Nota Sección 5 | 3.5 | |

Fortalezas: problema real bien explicado, código ordenado y comentado con una lógica pensada para proteger la bomba, y vistas del diseño 3D de la caja.

Mejorar para Avance 3: subir el código como `.ino`, armar el circuito y mostrarlo con fotos, hacer el esquema en Wokwi, Fritzing o KiCad con los pines del código, documentar cada iteración con sus problemas y soluciones, y hacer pruebas con usuarios. Lo que el README promete (avisos al celular y estadísticas) debe estar en el código o quitarse del alcance.

## Comentarios

El grupo plantea muy bien el problema de los estanques que rebalsan y escribió un código claro, con una lógica pensada para no dañar la bomba. Lo que más les baja la nota es que no hay evidencia de que el circuito esté armado ni probado, no hay esquema del circuito y no se documentó ninguna iteración. El código se subió como texto dentro de un README, y debe ir en un archivo `.ino` para que tenga el formato adecuado. Para el Avance 3 construyan el circuito, súbanlo con fotos y esquema, y documenten las pruebas. Se descontaron 0.5 puntos en cada sección (1.0 punto en total) por entrega tardía. Esto se debe a que el código se subió el 29 de octubre y las vistas 3D el 27, fuera de plazo.
