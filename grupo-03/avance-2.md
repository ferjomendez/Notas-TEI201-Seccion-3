# Grupo 3: Avance 2

Repo: JoacoAgurto/Monitoreo-electrico-eficiente-IOT-TEI201-GRUPO-03-. Integrantes: Vasco Urrutia, Joaquín Agurto e Ignacio Mora.

| Criterio | Nota | Observación |
|---|---|---|
| Resolución parcial problema ODS | 4.5 | El prototipo mide corriente RMS en 4 canales con SCT-013, la muestra en web y guarda CSV en microSD, y apunta al ODS 7. No convierte a kWh ni a costo, no hay uso en un hogar real y `testing/` está vacío. |
| Proceso de iteración | 4.0 | La iteración 1 documenta problemas reales (la pinza no mide con fase y neutro juntos, el ruido se confunde con corriente) y un plan v2. Las iteraciones 2 y 3 son plantilla. La tabla de métricas de mejora parece de plantilla y no de datos medidos, así que no cuenta como evidencia. |
| Código documentado | 6.5 | `main.ino` (unas 1250 líneas) tiene cabecera, mapa de conectores, `#include` comentados, constantes explicadas y limitaciones declaradas con honestidad. Faltan versiones de librerías y comentarios en el HTML embebido. |
| Diagramas de circuito | 5.5 | Hay un esquema KiCad completo (ESP32, 2 ADS1115, 4 jacks de pinza y microSD) y `v1_esquema.png`. Faltan valores de componentes, alimentación y direcciones I2C. El cableado es enredado. |
| Nota Sección 4 antes de penalización | 4.3 | |
| Nota Sección 5 antes de penalización | 6.0 | |
| Penalización por entrega tardía | -0.5 | Se descuenta 0.5 puntos a cada sección (1.0 punto en total). |
| Nota Sección 4 | 3.8 | |
| Nota Sección 5 | 5.5 | |

Fortalezas: código completo con limitaciones declaradas, esquema KiCad e identificación honesta de un problema técnico real.

Mejorar para Avance 3: llenar las iteraciones 2 y 3 con datos medidos y código por versión. Resolver y calibrar la medición con pinza, pasar de corriente a kWh y $, y probar con usuarios. Exportar el esquema con rótulos y repartir mejor los commits (Ignacio Mora no tiene ninguno).

## Comentarios

El código es uno de los más completos y declara con honestidad lo que aún no está implementado. El esquema KiCad también está bien armado. Queda pendiente pasar de corriente a kWh y a pesos para conectar el prototipo con el ODS 7, y probarlo en un hogar real. Las iteraciones 2 y 3 siguen vacías y la tabla de métricas de la iteración 1 no tiene datos medidos, así que no la pude contar como evidencia. Ignacio Mora no tiene commits propios, conviene que todos aporten al repositorio. Se descontaron 0.5 puntos en cada sección (1.0 punto en total) por entrega tardía. Esto se debe a que entregaron fuera de plazo.
