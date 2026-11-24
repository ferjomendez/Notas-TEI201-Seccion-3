# Grupo 3: Avance 3

Repo: JoacoAgurto/Monitoreo-electrico-eficiente-IOT-TEI201-GRUPO-03-. Integrantes: Vasco Urrutia, Joaquín Agurto e Ignacio Mora.

| Criterio | Nota | Observación |
|---|---|---|
| Captura de datos | 6.5 | `main.ino` mide los 4 canales con dos ADS1115 (128 muestras RMS cada 1 s), guarda en la microSD y tiene una cola para reenviar si se cae el WiFi. No justifican la frecuencia y el CSV de testing casi siempre marca 0. |
| Repositorio de datos | 7.0 | Supabase con el SQL de creación, índice, RLS y restricción única, más el respaldo en la microSD. El CSV de testing tiene 2.160 registros. |
| Dashboard y visualización | 6.5 | El dashboard en Netlify tiene gráficas por conector, consumo diario, comparación mensual, filtros por fecha y exportación CSV, y el ESP32 además sirve su propia página con 4 gráficos en vivo. El link al dashboard está solo en `testing/README.md`. |
| Generación de información | 7.0 | Pasaron de corriente a kWh y a pesos con tarifa editable, que era lo que les pedí en el Avance 2. Muestran el promedio diario, los días de mayor y menor consumo y el consumo por conector. No hay alertas y asumen 220 V con factor de potencia 1, pero lo dicen en pantalla. |
| Calidad del código | 6.5 | `main.ino` tiene cabecera, secciones, constantes con nombre y manejo de errores. El HTML del dashboard está minificado y casi sin comentarios, y `software/README.md` sigue con la plantilla. |
| Nota Software (30%) | 6.7 | |
| Esquemático y BOM (Hardware) | 6.0 | El esquema en KiCad tiene el ESP32, los dos ADS1115, los 4 conectores, la microSD, el LED y las resistencias. En el esquema las resistencias son de 10 kΩ y en el BOM de 100 kΩ, y en el BOM los dos ADS1115 a $5.990 suman $16.970 en vez de $11.980. |
| Estructura del repositorio | 6.0 | Las carpetas están bien y el README tiene equipo, problema y resultados. Le faltan el link al dashboard y las instrucciones para cargar el firmware y configurar Supabase, y quedan READMEs con la plantilla. |
| Respaldo completo | 5.5 | Están el firmware, la web, el SQL, el KiCad, el BOM, renders, planos, fotos y la presentación. Los modelos 3D están en .step y no hay .f3d, y la presentación PDF se llama "Avance N°2". |
| Nota GitHub (5%) | 5.8 | |

Fortalezas: sistema completo con Supabase y cola cuando se cae el WiFi, y el paso a kWh y pesos que conecta el proyecto con el problema.

Mejorar para la entrega final: poner en el README el link del dashboard y los pasos del firmware, subir el .f3d, y revisar las resistencias y las sumas del BOM.

## Comentarios

Se pasaron con lo de kWh y pesos, era justo lo que faltaba para conectar el proyecto con el problema. El sistema con Supabase y la cola cuando se cae el WiFi está muy bien pensado. Lo que más baja es GitHub. Pongan el link del dashboard y los pasos para cargar el firmware en el README principal, suban el .f3d y cámbienle el nombre a la presentación. Revisen también los valores de las resistencias y las sumas del BOM. Me gustó ver commits de los tres esta vez.
