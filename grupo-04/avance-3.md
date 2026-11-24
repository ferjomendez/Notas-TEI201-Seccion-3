# Grupo 4: Avance 3

Repo: sophifuenzalidaa13/TEI201_Bitacora. Integrantes: Sophia Fuenzalida, Sofía Lagos, Rafaela Montero y Sofía Campos.

| Criterio | Nota | Observación |
|---|---|---|
| Captura de datos | 5.5 | `cardiaco_nube.ino` lee el MAX30102, calibra 30 s y manda cada 5 s o cuando cambia el estado, con cola y reintentos. Hay caídas (un `HTTP -1` y un error TLS en las capturas) y la configuración de 400 sps que describe `software/README.md` no se aplica en el código. |
| Repositorio de datos | 6.5 | PostgreSQL en Aiven con un servidor Express en Railway y el historial por período, con capturas que muestran que los datos se guardan. El servidor y el esquema están en un repo privado, así que no los pude revisar. |
| Dashboard y visualización | 6.0 | El dashboard en Railway muestra el BPM, la referencia, la banda de ±20 %, el historial y las rutas, y el video lo muestra funcionando. El código no está en el repo y no hay una cuenta para que yo entre. |
| Generación de información | 6.0 | Calculan una referencia personal y una banda de ±20 % con tres estados, y la alarma suena después de tres lecturas fuera de banda. El informe reconoce que no lo probaron con conductores y no mide precisión ni latencia. |
| Calidad del código | 5.5 | El firmware tiene funciones, una máquina de estados y una tarea de red aparte, pero pocos comentarios y muchas variables globales. Además `software/config.h` quedó subido con la clave del WiFi y el token del dispositivo. |
| Nota Software (30%) | 5.9 | |
| Esquemático y BOM (Hardware) | 5.5 | `cableado_real.png` tiene el ESP32-S3, el MAX30102 y el buzzer, y los pines (SDA 4, SCL 5 y buzzer 6) coinciden con el código. Esta vez está el sensor real. Es una imagen de cableado con etiquetas poco legibles, y la batería y el interruptor solo están descritos en texto. El BOM tiene un total de 20.500 CLP, pero la protoboard, los cables y el USB no tienen precio. |
| Estructura del repositorio | 6.0 | Carpetas claras y README con integrantes, problema, materiales, pines, instrucciones y link al dashboard. Hay un `README (2).md` duplicado, fotos sin extensión en `hardware/` y carpetas que siguen como plantilla. |
| Respaldo completo | 6.5 | Están el firmware, el .f3d, los planos, el esquema, el BOM, el informe de pruebas, los CSV, las capturas y el video. Faltan el código del servidor y del dashboard, los renders y la presentación en PDF (solo hay un link a Google Slides). |
| Nota GitHub (5%) | 6.3 | |

Fortalezas: flujo completo con el sensor real, la nube y el dashboard, y documentación honesta sobre lo que falta validar.

Mejorar para la entrega final: sacar la clave y el token del repo y cambiarlos, subir el código del servidor o dar una cuenta de prueba, y comentar más el firmware.

## Comentarios

Lograron el flujo completo con el sensor real, la nube y el dashboard, y la documentación es muy honesta sobre lo que todavía no está validado. Ojo con algo importante. En `software/config.h` quedaron subidos la contraseña del WiFi y el token del dispositivo. Aunque borren el archivo, siguen en el historial de git, así que cambien la contraseña del WiFi, generen un token nuevo y dejen en el repo solo `config.example.h` (con `config.h` en el `.gitignore`). Para la entrega final suban el código del servidor o denme una cuenta de prueba, y agreguen comentarios al firmware. Vi que hubo commits pasada la medianoche del 24 de noviembre, entre ellos uno que borró el sketch del panel local y dejó enlaces rotos. Me di cuenta, pero no les voy a descontar. Sé que trabajaron harto durante el semestre y valoro el esfuerzo que le pusieron. Eso sí, recuperen ese archivo o arreglen los enlaces.
