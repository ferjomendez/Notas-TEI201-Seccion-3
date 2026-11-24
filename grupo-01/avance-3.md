# Grupo 1: Avance 3

Repo: ClementeAbarzua/camara_detecta_basura_TEI201_2026. Integrantes: Clemente Abarzúa, Matías Armijo, José Tomás De la Cuadra y Santiago León.

| Criterio | Nota | Observación |
|---|---|---|
| Captura de datos | 7.0 | La XIAO manda las fotos por HTTPS con token y reintentos, y hay 2.488 fotos reales entre el 14 y el 22 de noviembre. La frecuencia está justificada (5 s en modo demo y entre 15 y 19 s en modo estable). |
| Repositorio de datos | 7.0 | PostgreSQL en Aiven con el esquema versionado en `schema.sql`, exportación CSV y JSON desde `/admin` y la exportación real en `testing/datos/`. |
| Dashboard y visualización | 7.0 | El dashboard en Railway está arriba y muestra el estado actual, gráficos, historial y tendencias por hora, además del panel `/admin`. |
| Generación de información | 7.0 | Juntan las tres clases de basura, promedian las últimas fotos y usan un umbral de 80 % con confirmación para decidir entre "Hay basura", "Sin basura" y "No seguro". El resumen por hora responde justo a cuándo aparece la basura. Les faltó la matriz de confusión, pero ustedes mismos lo dicen. |
| Calidad del código | 7.0 | El servidor está ordenado en carpetas y tiene 26 archivos de test, cosa que casi nadie hizo. El firmware tiene docblocks y las librerías con su licencia. Algunas líneas del .ino están muy apretadas. |
| Nota Software (30%) | 7.0 | |
| Esquemático y BOM (Hardware) | 5.0 | El BOM está completo, con cantidades, precios, fuentes y un total de 26,68 USD. El esquemático es el mismo PDF del Avance 2, sin pines, sin valores y sin el interruptor, y `hardware/esquemas/README.md` todavía dice [PENDIENTE]. |
| Estructura del repositorio | 7.0 | Carpetas claras con README en cada una y un README principal completo, con equipo, problema, componentes, instrucciones y link al dashboard. Además corrigieron la arquitectura con Raspberry Pi que estaba mal en el Avance 2. |
| Respaldo completo | 6.5 | Está todo (firmware, servidor, .f3z, .stl, planos, renders, fotos, BOM y testing con datos). Lo que baja son los mensajes de commit, porque hay muchos "cambios" y "Add files via upload". |
| Nota GitHub (5%) | 6.8 | |

Fortalezas: sistema funcionando de punta a punta (cámara, servidor, base de datos y dashboard), pruebas con datos reales y tests en el servidor.

Mejorar para la entrega final: hacer el esquemático en Fritzing, Wokwi o EasyEDA con pines, valores y el interruptor, y escribir mensajes de commit que digan qué cambió.

## Comentarios

Muy buen trabajo. El sistema funciona de punta a punta y se nota que lo probaron harto con datos reales. Lo único que de verdad baja la nota es el esquemático, que sigue siendo el mismo del Avance 2. Se los había pedido formal y con el interruptor, así que para la entrega final háganlo en Fritzing, Wokwi o EasyEDA. Y pongan mensajes de commit que digan algo, porque "cambios" no me dice nada.
