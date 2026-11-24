# Grupo 9: Avance 3

Repo: cjquera237/AquaSafe-TEI201. Integrantes: Oscar Fuentes, Clemente Quera, María Francisca Rayo y Nicolás Weinlaub.

| Criterio | Nota | Observación |
|---|---|---|
| Captura de datos | 5.5 | `AquaSafe_Final.ino` lee temperatura, pH, turbidez y TDS y manda a Railway cada 30 s con reintento de WiFi y cola. En la base hay datos reales del 23 de noviembre de los cuatro sensores. El último commit dejó un ternario incompleto en la línea 145, así que el código no compila. |
| Repositorio de datos | 7.0 | PostgreSQL en Aiven con la API de `server.js`, clave, validación de unidades y endpoint de histórico. Consulté `/api/lecturas` y devolvió 500 registros reales. |
| Dashboard y visualización | 6.0 | El dashboard en Railway tiene tarjetas por sensor, un gráfico con selector, tabla y actualización cada 5 s. No tiene umbrales ni semáforo, y el pH, la turbidez y el TDS salen en voltios. |
| Generación de información | 4.5 | El dashboard muestra los valores casi en bruto, sin estadísticas ni alertas. El estado del agua solo se calcula para la OLED y no llega a la web. |
| Calidad del código | 5.5 | El firmware tiene cabecera, pines como constantes y funciones separadas, y `server.js` está bien comentado. Baja por el error de compilación del último commit. |
| Nota Software (30%) | 5.7 | |
| Esquemático y BOM (Hardware) | 6.0 | El Fritzing incluye los cuatro sensores, la OLED y los divisores, y los pines coinciden con el código y con el Wokwi. Las resistencias R1 a R4 no tienen valor y el DS18B20 tiene VDD a 5 V con el pull-up a 3,3 V. El BOM tiene cantidades y proveedores, pero varios ítems no tienen precio. |
| Estructura del repositorio | 5.5 | Las carpetas están ordenadas, pero el README está desactualizado. Manda a abrir `AquaSafe_ESP32.ino`, que ya no existe, y dice que falta conectar el ESP32. `software/README.md` cita una carpeta que se borró. |
| Respaldo completo | 5.5 | Están el .f3d, los planos, los renders, las fotos, el informe final, la presentación, el código y el BOM. `testing/` y las iteraciones siguen como plantilla, y casi todos los commits dicen "Update README.md". |
| Nota GitHub (5%) | 5.5 | |

Fortalezas: sistema funcionando de punta a punta con datos reales en la base, y esquemático, 3D y planos coherentes con el código.

Mejorar para la entrega final: calibrar los sensores para que no salgan en voltios, llevar el semáforo al dashboard con alertas, arreglar la línea 145 y actualizar el README.

## Comentarios

El sistema funciona de punta a punta y vi datos reales en la base, eso está muy bien. Ahora hay que convertir esos datos en información. Calibren el pH, la turbidez y el TDS para que no salgan en voltios, y lleven el semáforo del agua al dashboard con umbrales y alertas. Revisen la línea 145 de `AquaSafe_Final.ino`, porque con el último commit el código no compila. Actualicen el README y llenen `testing/` y las iteraciones. Sobre la IA, les recomiendo que no dejen que Claude quede como co-autor en los commits (el `Co-Authored-By`), porque se ve mal. Como el uso de IA está declarado en FUENTES.md, no tienen ningún problema.
