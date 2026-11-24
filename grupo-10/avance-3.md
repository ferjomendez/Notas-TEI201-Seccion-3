# Grupo 10: Avance 3

Repo: isiparrab/sensor_ruido_clases. Integrantes: Matilda Steiner, Isidora Parra, Isidora Vidal y Florencia Gutiérrez.

| Criterio | Nota | Observación |
|---|---|---|
| Captura de datos | 7.0 | El KY-038 se mide en ventanas de 50 ms, se promedia cada 10 s y se manda por HTTPS desde otro núcleo. La frecuencia está justificada y en la prueba de 1 hora informan 332 mediciones y 4 cortes. |
| Repositorio de datos | 7.0 | PostgreSQL en Aiven con tablas de lecturas y asistencias, índices y hora de Chile. El histórico se consulta por calendario y se exporta a CSV. |
| Dashboard y visualización | 7.0 | La página en vivo tiene semáforo, gráfico y acceso para la profesora, y el registro diario tiene calendario, gráfico cada 5 minutos y tabla de pedidos. |
| Generación de información | 7.0 | Calculan el porcentaje de tiempo en cada color, los pedidos de ayuda, la espera promedio, la hora de más ruido y el ruido de los 10 minutos antes de cada pedido. Los umbrales los calibraron en la sala. |
| Calidad del código | 6.5 | Los sketches y el servidor están bien comentados y ordenados. Quedó el `central.ino` antiguo junto al nuevo. |
| Nota Software (30%) | 6.9 | |
| Esquemático y BOM (Hardware) | 6.5 | El esquemático v3 tiene los dos módulos, el KY-038, los actuadores y el botón con batería. El LED del semáforo tiene R y G cruzados, porque el esquema dice R en 27 y G en 26 y el código lo tiene al revés. El BOM tiene un total de 42.790 CLP, pero el pulsador y la carcasa no tienen precio. |
| Estructura del repositorio | 7.0 | Carpetas ordenadas con README en cada una y un README principal muy completo, con inicio rápido y link a la página en vivo. |
| Respaldo completo | 7.0 | Está todo (código, esquemático, BOM, .f3d, planos, renders, fotos, testing con datos, presentación e iteraciones), con commits descriptivos. |
| Nota GitHub (5%) | 7.0 | |

Fortalezas: sistema completo con indicadores pensados para la sala y un repositorio muy bien organizado.

Mejorar para la entrega final: corregir R y G del semáforo en el esquemático, ponerle precio al pulsador y la carcasa, y sacar o marcar como antiguo `central.ino`.

## Comentarios

Excelente trabajo, es de los mejores del curso. El sistema funciona completo y los indicadores están pensados para la sala, como la espera promedio o el ruido antes de cada pedido de ayuda. Además corrigieron todo lo que les pedí en el Avance 2. Solo arreglen R y G del semáforo en el esquemático y borren o marquen como antiguo `central.ino`. Sobre la IA, Claude aparece como contributor del repo y como co-autor en varios commits. Les recomiendo que no dejen que la IA haga el co-authored, porque se ve mal. Como el uso de IA está declarado en FUENTES.md, no tienen ningún problema.

muchas felicidades en serio por todo, me duele contarles que por temas medicos no estoy comiendo azuar jajaja, pero mi polola y hermano aprecieron los brownies antes del control de Opti JAJSAJS. Sigan asi, cualquier cosa siempre me pueden escribir.
