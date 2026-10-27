# Grupo 1: Avance 2

Repo: ClementeAbarzua/camara_detecta_basura_TEI201_2026. Integrantes: Clemente Abarzúa, Matías Armijo, José Tomás De la Cuadra y Santiago León.

| Criterio | Nota | Observación |
|---|---|---|
| Resolución parcial problema ODS | 5.0 | El problema está bien fundamentado con datos de Peñalolén (ODS 11 y 12) y el prototipo clasifica "hay/no hay basura" con un dataset propio. Falta evidencia de impacto: no hay usuarios ni métricas, `testing/` es plantilla y el README raíz describe una arquitectura con Raspberry Pi que no es la del prototipo (XIAO ESP32-S3). |
| Proceso de iteración | 5.0 | Hay tres iteraciones con código real (streaming AP, detección AP/WiFi y versión comentada) y un bug documentado y corregido: el modelo no concluía con baja confianza. Los README de las iteraciones 2 y 3 están intercambiados, y no hay tabla antes/después con métricas ni reportes de pruebas. |
| Código documentado | 7.0 | La versión final (`iteracion_3`) tiene secciones numeradas, docblocks, librerías identificadas y licencias. Las versiones previas casi no tienen comentarios. |
| Diagramas de circuito | 5.5 | El circuito es solo la placa y la batería, así que el diagrama pictórico alcanza para el hardware que tienen. Queda en 5.5 porque no muestra pines ni valores de los componentes. `hardware/esquemas` es plantilla. |
| Nota Sección 4 | 5.0 | |
| Nota Sección 5 | 6.3 | |

Fortalezas: el código final funciona y está comentado, la iteración es real, el dataset es propio y el trabajo se reparte entre varios autores.

Mejorar para Avance 3: corregir los README de iteración y completar métricas reales (precisión, tiempos, batería). Documentar pruebas con fotos y videos y validar en terreno. Entregar un esquema formal (Fritzing o Wokwi) que incluya el interruptor.

## Comentarios

Tienen un buen avance en el código: la versión final está ordenada, comentada y con las librerías identificadas, y el trabajo se nota repartido entre varios. Como el circuito es solo la placa y la batería, el diagrama pictórico alcanza para el hardware que tienen, aunque no muestra pines ni valores. Lo que más pesa en la nota es la falta de evidencia de impacto y de pruebas: los README de las iteraciones 2 y 3 están cambiados de lugar y no hay métricas de antes y después. Para el Avance 3 documenten pruebas con resultados medidos y, si agregan electrónica, un esquema con todos los pines.
