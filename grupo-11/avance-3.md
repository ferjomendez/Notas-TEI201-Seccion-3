# Grupo 11: Avance 3

Repo: benito-diaz/Sensor-UV-colegios. Integrantes: Maximiliano Cornejo, Benito Díaz y Benjamín Retamal.

| Criterio | Nota | Observación |
|---|---|---|
| Captura de datos | 6.5 | `main.ino` promedia 64 muestras cada 0,5 s, pide 4 lecturas seguidas para cambiar de nivel y manda a la nube cada 10 s desde otra tarea. La prueba larga dio 96,9 % de captura. Falta calibrar contra MeteoChile y el cero marca 0,52. |
| Repositorio de datos | 7.0 | PostgreSQL en Aiven con un servidor Express en Railway, validación de rangos y consultas parametrizadas. El histórico se consulta y se exporta a CSV, y comprobaron que los datos quedan guardados al apagar el equipo. |
| Dashboard y visualización | 7.0 | El panel en Railway muestra el valor con el color de la OMS, la alerta, un gráfico con franjas en 1 h, 6 h, 24 h y 7 días, los máximos diarios, una tabla y la descarga CSV. |
| Generación de información | 6.5 | Muestra el nivel OMS con una recomendación para el colegio, alerta con UV 6 o más, el máximo del día, los minutos por nivel y avisos por Telegram. Como las pruebas fueron sin sol, no se vieron valores altos reales. |
| Calidad del código | 6.5 | `main.ino` y `server.js` están ordenados en funciones y comentados, y `software/README.md` documenta las rutas. La tabla de calibración es la típica del sensor y no la verificaron. |
| Nota Software (30%) | 6.7 | |
| Esquemático y BOM (Hardware) | 6.0 | El esquema v3 tiene el ESP32, el sensor, el semáforo, el LiPo Rider, la batería y el panel solar, y los pines coinciden con `main.ino`. Dice "D32 sin uso", pero el código usa D32 para alimentar el sensor. El BOM tiene 15 ítems, pero no tiene costo total y varios precios dicen "sin boleta". |
| Estructura del repositorio | 7.0 | Carpetas claras con README en cada una, y el README principal ya tiene integrantes, problema, ODS, componentes, instrucciones y link al panel. |
| Respaldo completo | 6.5 | Están el código, el esquemático, tres .f3d, los STL, los planos, los renders, las fotos, los datos, los reportes y la presentación, además de las evidencias que faltaban. `reporte_final/` solo tiene README y quedan pendientes el video y las fotos de pruebas con usuarios. |
| Nota GitHub (5%) | 6.8 | |

Fortalezas: panel en la nube muy completo, datos reales guardados y un reporte de testing honesto.

Mejorar para la entrega final: calibrar al sol contra MeteoChile, hacer las pruebas con usuarios, poner el costo total en el BOM y corregir D32 en el esquema.

## Comentarios

Muy buen avance. El panel en la nube está muy completo y el reporte de testing es honesto, incluido lo del GND suelto. Además entregaron todo a tiempo y con las evidencias que faltaban. Para la entrega final calibren el sensor al sol contra MeteoChile, hagan las pruebas con usuarios, pongan el costo total en el BOM y corrijan lo de D32 en el esquema. Sobre la IA, les recomiendo que no dejen que Claude quede como co-autor en los commits (el `Co-Authored-By`), porque se ve mal. Como el uso de IA está declarado en FUENTES.md, no tienen ningún problema.
