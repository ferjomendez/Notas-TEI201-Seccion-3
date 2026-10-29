# Grupo 9: Avance 2

Repo: cjquera237/AquaSafe-TEI201. Proyecto: AquaSafe, monitor de calidad del agua con semáforo de LEDs. Integrantes: Oscar Fuentes, Clemente Quera, María Francisca Rayo y Nicolás Weinlaub. Todo el repositorio se subió el 27 de octubre.

| Criterio | Nota | Observación |
|---|---|---|
| Resolución parcial problema ODS | 4.5 | Hay un prototipo armado en protoboard con ESP32, sensor de temperatura DS18B20, módulo de pH y sensor de turbidez, más un semáforo de LEDs. Las lecturas llegan al Monitor Serie. Los sensores de pH y turbidez no están calibrados, el sensor TDS no está integrado y la pantalla que se pidió sigue pendiente. Tampoco hay pruebas con usuarios. |
| Proceso de iteración | 4.5 | `iteraciones/01_desarrollo_inicial.md` cuenta las etapas (simulación en Wokwi, montaje y programación), los problemas con su solución (falta de OneWire, DS18B20 no detectado, GND sin unir) y las limitaciones. Es una sola iteración y sin fechas por versión. Las carpetas `iteracion_1`, `iteracion_2` e `iteracion_3` siguen como plantilla y `testing/` no tiene datos ni evidencias. |
| Código documentado | 5.5 | `AquaSafe_ESP32.ino` tiene cabecera, pines definidos y funciones de calibración comentadas. `FUENTES.md` lista las librerías y declara el uso de IA. Queda por mejorar que la calibración no está validada y que el sensor TDS no aparece en el código. |
| Diagramas de circuito | 4.5 | Existe un circuito real en Wokwi (wokwi.com/projects/476425182391699457), con potenciómetros en lugar de los sensores, el DS18B20 y los tres LEDs con resistencias. Eso se acepta como simulación. Aun así el diagrama no está bien por tres razones. Primero, usa una ESP32-S3 y los pines 1, 2, 4, 5, 6, 15, 16 y 17, mientras que el código y `hardware/README.md` usan una ESP32 Dev Module con los pines 21 (DS18B20), 32 (pH), 34 (turbidez), 33 (TDS) y 16, 17 y 18 (LEDs). Segundo, incluye una entrada de batería que el prototipo real no tiene. Tercero, el diagrama no está dentro del repo: `hardware/esquemas/` sigue como plantilla y el Wokwi solo aparece como enlace en `FUENTES.md`, sin captura ni archivo exportado. Por eso no sirve como documentación del montaje real. |
| Nota Sección 4 antes de penalización | 4.5 | |
| Nota Sección 5 antes de penalización | 5.0 | |
| Penalización por entrega tardía | -0.5 | Se descuenta 0.5 puntos a cada sección (1.0 punto en total). |
| Nota Sección 4 | 4.0 | |
| Nota Sección 5 | 4.5 | |

Fortalezas: prototipo físico con tres sensores leyendo y semáforo funcionando, registro fotográfico del montaje, código comentado y declaración honesta del uso de IA.

Mejorar para Avance 3: integrar el sensor TDS y la pantalla, calibrar pH y turbidez contra una referencia, hacer pruebas con usuarios y subir sus datos a `testing/`, documentar cada iteración en su carpeta con fechas, y dejar el diagrama en el repo (captura o archivo exportado) con la misma placa y los mismos pines que el código.

## Comentarios

El grupo tiene un prototipo físico que lee tres sensores y enciende el semáforo, con fotos del montaje y un código bien comentado. Lo que más baja la nota es el diagrama: el Wokwi existe y es una simulación válida, pero usa otra placa (ESP32-S3) y otros pines que el código y el README de hardware, además de una entrada de batería que el prototipo no tiene, y no está guardado en el repositorio. Quien revise el repo no puede saber cómo está armado el circuito real. También faltan la calibración, el sensor TDS, la pantalla y las pruebas con usuarios. Para el Avance 3 suban el diagrama al repo con los pines del código, y documenten cada iteración en su carpeta. Se descontaron 0.5 puntos en cada sección (1.0 punto en total) por entrega tardía. Esto se debe a que subieron el repositorio el 27 de octubre, fuera de plazo.
