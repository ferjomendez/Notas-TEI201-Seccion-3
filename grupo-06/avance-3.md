# Grupo 6: Avance 3

Repo: mkind06/sensor_fugas_TEI201-. Integrantes: Andrés García, Mathias Kind, Macarena Kuperman y Pablo Miranda.

| Criterio | Nota | Observación |
|---|---|---|
| Captura de datos | 5.5 | `RiegoMonitor_WiFi.ino` cuenta pulsos por interrupción con antirrebote y publica un JSON por segundo, y explican el filtro por el ruido de la bomba. El sensor 1 dejó de funcionar por una falla en la placa soldada, así que no lograron capturar los dos sensores a la vez. |
| Repositorio de datos | 5.0 | Los datos quedan en la pestaña del navegador y se descargan con el botón de CSV, sin base de datos ni nube. En el repo están `lecturas_preajuste.csv` y `testeo_verde.csv`, que es sintético. |
| Dashboard y visualización | 7.0 | El dashboard lo sirve la misma ESP32 por WiFi y hay una copia en GitHub Pages. Tiene semáforo, indicadores, gráficos de caudal y de diferencia con varias ventanas de tiempo, tiempo por estado, eventos y CSV. Está muy completo. |
| Generación de información | 6.5 | Calculan la diferencia porcentual, el agua perdida en litros, el tiempo en cada estado y un registro de eventos, con umbrales de 10 % y 25 %. No detecta un sensor caído y la diferencia real no se pudo validar con ambos sensores. |
| Calidad del código | 6.5 | El firmware tiene cabecera, constantes con unidades, pines claros y no usa librerías externas. El dashboard está repetido en el .ino y en tres HTML. |
| Nota Software (30%) | 6.1 | |
| Esquemático y BOM (Hardware) | 6.5 | `esquematico_v3` tiene símbolos reales, los divisores, la resistencia de 330 Ω y la bomba con fuente aparte, y los pines coinciden con el firmware. El BOM tiene 12 ítems con cantidad, proveedor, costo unitario y un total de 72.790 CLP. El S1 quedó en GPIO 8 por un diagnóstico que no resultó. |
| Estructura del repositorio | 7.0 | Carpetas claras con README en cada una y un README principal completo, con integrantes, problema, arquitectura, instrucciones, link al dashboard y un estado honesto del proyecto. |
| Respaldo completo | 6.5 | Están el código, el esquemático, el .f3d, el STEP, los planos, los renders, las fotos, la presentación, el protocolo y los resultados. Faltan evidencias reales de la demo (un CSV físico o un video con la placa) y casi todo se subió el mismo día de la presentación. |
| Nota GitHub (5%) | 6.8 | |

Fortalezas: dashboard de los mejores del curso, documentación excelente y honestidad sobre lo que falló.

Mejorar para la entrega final: arreglar el divisor del sensor 1, guardar los datos en una base en la nube y dejar un CSV real con ambos sensores.

## Comentarios

La documentación está excelente y el dashboard es de los mejores del curso. También valoro harto que digan con honestidad que el sensor 1 falló y que el modo demo es simulado. Lo que más baja es el almacenamiento, porque los datos solo quedan en el navegador. Para la entrega final arreglen el divisor del sensor 1, guarden los datos en una base en la nube y dejen un CSV real con ambos sensores. Sobre la IA, Claude sigue apareciendo como contributor del repo y como co-autor en varios commits. Les recomiendo que no dejen que la IA haga el co-authored, porque se ve mal. Como el uso de IA está declarado en FUENTES.md, no tienen ningún problema.
