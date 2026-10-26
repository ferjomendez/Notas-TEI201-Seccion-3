# Grupo 6: Avance 2

Repo: mkind06/sensor_fugas_TEI201-. Autores en git: mkind06 y andresgarcia-ing (el README no lista integrantes).

| Criterio | Nota | Observación |
|---|---|---|
| Resolución parcial problema ODS | 5.5 | Comparan el caudal antes y después de un tramo (2 sensores FS400A y 3 LED) y lo vinculan a los ODS 6 y 2. Reconocen que no midieron ahorro de agua ni usuarios. La demo con 3 estados es solo informada, con 2 fotos del montaje. |
| Proceso de iteración | 5.0 | Hay una tabla de problemas y soluciones (LED invertido, conteos espurios de la bomba, ventana de 3 s a 10 s) y un ajuste de K2 con datos (de 275 a 229, con 7 lecturas reales). Se conserva una versión previa del código. Faltan el CSV físico final, la corrida de 5 min y una comparación cuantitativa. El `testeo_verde.csv` es sintético y el README lo declara. |
| Código documentado | 6.5 | `PruebaSensor.ino` tiene cabecera (placa, sensores, lógica y pines), constantes con unidades y no usa librerías externas. Además hay un panel web y un manual. Algunos comentarios son metadatos del proceso y no explican el código. |
| Diagramas de circuito | 4.8 | Hay solo un diagrama Mermaid, comprensible (GPIO, divisor 10k/20k, 330 Ω, bomba con fuente aparte) y una tabla de coordenadas de protoboard. No hay esquema con símbolos y el divisor no se verificó con multímetro. |
| Nota Sección 4 | 5.3 | |
| Nota Sección 5 | 5.7 | |

Fortalezas: documentación honesta que separa lo medido de lo supuesto, código sin dependencias y bien comentado, y fallas de hardware diagnosticadas con registro.

Comentario del profesor: no se ve bien dejar a Claude como contributor del repositorio.

Mejorar para Avance 3: guardar el registro físico continuo y evidencia de los 3 estados, y calibrar con volumen conocido. Entregar un esquema eléctrico real, identificar integrantes y roles, repartir los commits en el tiempo (81 en 2 días) y probar en terreno.
