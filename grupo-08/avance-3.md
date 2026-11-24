# Grupo 8: Avance 3

Repo: aavilal8822-png/estacion-ambiental (en el Avance 2 era 9p9yh5ztwz-wq/Estaci-n-ambiental). Integrantes: Antonia Ávila, Agustín Jiménez y Claudio Parada.

| Criterio | Nota | Observación |
|---|---|---|
| Captura de datos | 5.0 | `firmware/main.ino` lee el DHT11, el MQ-9 y el DSM501A y manda por HTTPS con reconexión y 60 s de calentamiento. Solo funcionan la temperatura y la humedad, porque el MQ-9 marca siempre 0 V y el DSM501A siempre 100 %. |
| Repositorio de datos | 6.5 | `server.js` guarda cada lectura en PostgreSQL con validación y API key, y la API entrega el histórico. Está limitada a 500 filas y no se puede filtrar por fecha. |
| Dashboard y visualización | 6.0 | El dashboard en Railway usa Chart.js con selector de variable, tabla y actualización cada 5 s. Es básico, sin estadísticas ni alertas, y dos de las cuatro series salen planas. |
| Generación de información | 4.5 | En `testing/informe.md` hay promedios, mínimos y máximos, y reconocen las fallas de los sensores. El sistema no tiene umbrales ni alertas, y no se conecta con el problema de comparar sectores de Santiago. |
| Calidad del código | 6.0 | El firmware está comentado, con constantes y sin credenciales, y el backend está limpio y valida las entradas. Queda un "DIAGNOSTICO API" temporal en `server.js`. |
| Nota Software (30%) | 5.6 | |
| Esquemático y BOM (Hardware) | 6.0 | El PDF del esquemático tiene el ESP32-S3 y los tres sensores, y `conexiones.md` tiene los pines y los divisores, que coinciden con el firmware. El BOM tiene cantidades, precios, proveedores con link y total. La caja tiene un asterisco sin explicación. |
| Estructura del repositorio | 6.0 | Están las carpetas `firmware/`, `hardware/`, `diseno-3d/`, `testing/` y `public/`, y el README es completo. Hay enlaces rotos a `protocolo_pruebas.md` y `testing.md`, e `informe.md` apunta a una carpeta `datos/` que no existe. |
| Respaldo completo | 6.5 | Están el código, el esquemático, los .f3d, los STL, los renders, los planos, el BOM, las fotos, las pruebas con CSV, el informe y la presentación. Casi todos los commits dicen "Add files via upload". |
| Nota GitHub (5%) | 6.3 | |

Fortalezas: sistema completo en la nube armado en poco tiempo y un repo nuevo mucho más completo, con esquemático, BOM y 3D.

Mejorar para la entrega final: hacer funcionar el MQ-9 y el DSM501A, agregar umbrales y alertas ligados al problema, y arreglar los enlaces rotos del README.

## Comentarios

Armaron el sistema completo en poco tiempo, con el ESP32 mandando a la nube, PostgreSQL y el dashboard en Railway, y el repo nuevo está mucho más completo. Lo que más baja es que el MQ-9 y el DSM501A no están midiendo, así que dos de las cuatro variables no aportan nada, y no hay alertas ni umbrales. Para la entrega final revisen esos dos sensores, agreguen umbrales relacionados con el problema y arreglen los enlaces rotos del README. Casi todos los commits están en una sola cuenta, así que traten de que cada uno suba su parte.
