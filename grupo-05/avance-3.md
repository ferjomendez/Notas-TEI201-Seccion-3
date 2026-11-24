# Grupo 5: Avance 3

Repo: mrtn-fl/proyecto_final_TEI201_GRUPO5. Integrantes: Benjamín Bidegain, Martín Flores, Vicente Pincheira y Thomas Von Fabeck.

| Criterio | Nota | Observación |
|---|---|---|
| Captura de datos | 6.5 | `costop.ino` lee el MQ-7 y el DHT11 cada 2 s, registra cada 10 s y tiene reconexión de WiFi y respaldo en LittleFS. Hay 100 lecturas reales en `testing/datos/`. La frecuencia no está justificada con el problema. |
| Repositorio de datos | 7.0 | PostgreSQL en Aiven con una API Express en Railway, el esquema en `schema.sql` con índice y restricciones, histórico en `/api/lecturas` y exportación CSV. |
| Dashboard y visualización | 4.5 | No hay dashboard con gráficas. Lo que hay son endpoints JSON, sobre todo `/api/resumen` con el último valor, el promedio y el máximo de 24 h, y el monitor serie. |
| Generación de información | 6.0 | La alarma de cuatro estados con histéresis, el aviso por Telegram y el resumen de 24 h responden directo al problema. Los umbrales siguen en valores del ADC (2000 y 3000) y no en ppm, pero lo declaran en el README. |
| Calidad del código | 6.5 | `costop.ino` y `server.js` están bien comentados, con funciones separadas y los secretos en `secrets.h` y `.env.example`. Queda un bloque de diagnóstico de WiFi y `iteracion_3/v3_codigo.ino` duplica el firmware. |
| Nota Software (30%) | 6.1 | |
| Esquemático y BOM (Hardware) | 4.0 | No hay esquemático y `hardware/esquemas/` sigue como plantilla. Lo que salva la nota es la tabla de conexiones con los pines correctos y un BOM muy completo, con cantidades, especificación, costos y total. |
| Estructura del repositorio | 6.5 | Carpetas claras y README con descripción, integrantes, problema, componentes, instalación y link al servidor. Quedan plantillas en `hardware/esquemas`, `hardware/fotos` y `reporte_final`, y el README enlaza un `protocolo_pruebas.md` que no existe. |
| Respaldo completo | 6.0 | Están el firmware, el servidor, el .f3d, los planos, los renders, el BOM, el testing con 4 usuarios, las iteraciones y la presentación. Faltan el esquemático y las fotos del prototipo. |
| Nota GitHub (5%) | 6.3 | |

Fortalezas: cadena de datos completa (ESP32, API, PostgreSQL y Telegram), código bien comentado y BOM muy detallado.

Mejorar para la entrega final: hacer el esquemático con la placa y los pines reales, armar un dashboard con gráficas sobre la API y detallar en FUENTES.md qué hizo la IA.

## Comentarios

La parte de datos les quedó muy bien, con el ESP32, la API, PostgreSQL en la nube y Telegram funcionando, y el código está bien comentado. Hay dos cosas que bajan harto la nota. No hay esquemático, solo la tabla de pines, y tampoco hay un dashboard con gráficas, porque los datos solo se ven como JSON. Para la entrega final hagan el esquema en Wokwi, Fritzing o KiCad con la placa y los pines reales, y armen una página simple con un gráfico del CO en el tiempo sobre la API que ya tienen. Detallen también en FUENTES.md qué partes hicieron con Claude.
