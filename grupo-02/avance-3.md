# Grupo 2: Avance 3

Repo: joaco-eng/Proyecto-tei, con el código en JoaquinZavalaM/Monitor-Sumidero. Integrantes: Olivia Betinyani, Joaquín Calderón, Joaquín Zavala y Antonia Uribe.

| Criterio | Nota | Observación |
|---|---|---|
| Captura de datos | 5.5 | El firmware toma la mediana de 5 lecturas, filtra entre 20 y 600 cm, reintenta el WiFi y manda cada 10 s. Está bien hecho, pero no hay evidencia de una captura continua de punta a punta y el mismo README reconoce un error `ENOTFOUND` con la base. |
| Repositorio de datos | 5.0 | La tabla `mediciones` en Aiven está bien diseñada, pero cuando la revisé `/api/salud` respondía `ENOTFOUND` hacia Aiven y no pude ver el histórico. Tampoco hay datos de ejemplo ni una exportación en el repo. |
| Dashboard y visualización | 5.5 | El dashboard en Railway carga y tiene un gráfico con Chart.js y una tabla de las últimas 30 mediciones. Es básico, sin el umbral dibujado ni estadísticas, y sin la base no muestra datos. |
| Generación de información | 4.5 | El servidor calcula el nivel del agua y lo grafica, pero no hay umbral ni alerta. Se perdió la alerta con confirmación de 5 s que tenían en `versiones-anteriores/sumidero_wifi.ino`, y era justo lo que respondía al problema del nivel anormal. |
| Calidad del código | 6.5 | El firmware y `server.js` están comentados, con funciones separadas, consultas parametrizadas y las credenciales en `secrets.h`. El detalle es que el código vive en otro repo. |
| Nota Software (30%) | 5.4 | |
| Esquemático y BOM (Hardware) | 5.5 | `hardware/esquematico.png` tiene los pines correctos (TRIG en 5 y ECHO en 4), pero es un diagrama de bloques y no un esquemático. El comentario del .ino dice que ECHO lleva divisor y el README dice que va directo. El BOM tiene precios y total, aunque el sensor sale a $9.990 unitario y a $14.980 en total para una sola unidad. |
| Estructura del repositorio | 6.5 | Carpetas claras y un README completo con integrantes, ODS, problema, pines, instrucciones y link al dashboard. Quedan varios "COMPLETAR" en testing e iteraciones, y `software/` y `diseno-3d/` solo enlazan al otro repo. |
| Respaldo completo | 6.0 | Hay documentación, pruebas de precisión con datos reales, iteraciones, fotos y presentación. El firmware, el servidor y el .f3d están en Monitor-Sumidero y no en este repo. |
| Nota GitHub (5%) | 6.3 | |

Fortalezas: documentación completa y honesta, pruebas de precisión con error y desviación estándar, y firmware y servidor bien comentados.

Mejorar para la entrega final: volver a poner el umbral con la alerta, dejar la base de datos funcionando y juntar el código, el .f3d y el esquemático en un solo repo.

## Comentarios

La documentación está muy completa y honesta, sobre todo las pruebas de precisión con error y desviación estándar. Lo que más les baja la nota es que el sistema no genera información útil, porque se perdió la alerta que sí tenían antes y el dashboard solo grafica el nivel. Cuando lo revisé, la base de datos tampoco respondía. Para la entrega final vuelvan a poner el umbral con la alerta y junten todo en un solo repo. Vi que la presentación se subió el 24 de noviembre, después del plazo. Me di cuenta, pero no les voy a descontar. Sé que trabajaron harto durante el semestre y valoro el esfuerzo que le pusieron. Sobre la IA, les recomiendo que no dejen que Claude quede como co-autor en los commits (el `Co-Authored-By`), porque se ve mal. Como el uso de IA está declarado en FUENTES.md, no tienen ningún problema.
