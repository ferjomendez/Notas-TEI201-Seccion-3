# Grupo 12: Avance 3

Repo: mcandela123/esp32-railway-estanque (en el Avance 2 era dpoupinr/proyecto_final_TEI201). Integrantes: Mateo Candela, Claudio Martínez y Diego Poupin.

| Criterio | Nota | Observación |
|---|---|---|
| Captura de datos | 7.0 | El ESP32 lee el flotador con antirrebote y manda el nivel, la bomba y el estado por HTTPS cuando cambian y cada 60 s, con cola y reintentos. La frecuencia está justificada y hay 34 lecturas reales en `testing/datos/`. |
| Repositorio de datos | 7.0 | PostgreSQL en Aiven con la tabla `lecturas`, consulta por API y clave para escribir, más un respaldo en CSV y JSON. |
| Dashboard y visualización | 6.5 | El dashboard en Railway tiene tarjetas de nivel, bomba y estado, un gráfico escalonado, una tabla y el aviso de sin señal. Solo muestra las últimas 300 lecturas, sin selector de rango ni estadísticas por día. |
| Generación de información | 6.5 | El aviso de sin señal y el estado de descanso son útiles, y la página local cuenta los llenados, su duración y el tiempo de bomba. En el dashboard de la nube esos cálculos no están, y los hicieron a mano en `captura_y_datos.md`. |
| Calidad del código | 7.0 | `esp32_railway.ino` tiene una cabecera larga, secciones numeradas, pines como constantes y funciones separadas. `server.js` es corto y está comentado. |
| Nota Software (30%) | 6.8 | |
| Esquemático y BOM (Hardware) | 6.5 | El diagrama SVG muestra todo el circuito y los pines coinciden con el código (flotador en GPIO 27, relé en GPIO 13 y LED en GPIO 2). Está dibujado a mano y no en Fritzing, KiCad o Wokwi. El BOM tiene cantidades, costos y un total de 12.000 CLP. |
| Estructura del repositorio | 7.0 | Carpetas claras, `.env.example`, licencia y un README completo con equipo, roles, ODS, el problema en Culiprán y San Pedro, arquitectura, link e inicio rápido. |
| Respaldo completo | 6.5 | Está todo (código, .f3d, STL, planos, renders, fotos, BOM, testing, iteraciones, reporte y presentación). Casi todo se subió en las últimas 48 horas y hay un solo autor en git. |
| Nota GitHub (5%) | 6.8 | |

Fortalezas: sistema completo y bien documentado, con captura confiable y datos reales.

Mejorar para la entrega final: hacer el esquemático en Fritzing, KiCad o Wokwi, llevar los cálculos de la página local al dashboard y que cada integrante suba su parte con su cuenta.

## Comentarios

Gran salto desde el Avance 2. Pasaron de tener el código pegado en un README a un sistema completo y bien documentado. Para la entrega final hagan el esquemático en Fritzing, KiCad o Wokwi y agreguen al dashboard los cálculos que ya tienen en la página local, como los llenados y los minutos de bomba por día. Todos los commits salen de una sola persona y con un correo que no está vinculado a GitHub, por eso el repo no muestra contribuidores. Traten de que cada uno suba su parte con su cuenta. Sobre la IA, les recomiendo que no dejen que Claude quede como co-autor en los commits (el `Co-Authored-By`), porque se ve mal. Como el uso de IA está declarado en FUENTES.md, no tienen ningún problema.
