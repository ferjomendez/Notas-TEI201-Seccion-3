# Grupo 7: Avance 3

Repo: Macarena2026/proyecto_final_TEI201. Integrantes: Macarena Aldana, Sofía Godoy y Daniela Oñate.

| Criterio | Nota | Observación |
|---|---|---|
| Captura de datos | 6.0 | El firmware lee el VL53L0X en modo continuo cada 50 ms y avisa si hay timeout, lo que tiene sentido para unos lentes de alerta. No justifican la frecuencia elegida. |
| Repositorio de datos | 6.0 | No hay base de datos ni nube porque los lentes funcionan solos, y eso ya lo conversamos. Los datos de las 5 pruebas con usuarios están ordenados en `Archivo pruebas practicas.xlsx`. |
| Dashboard y visualización | 6.0 | No hay dashboard, solo el monitor serial con la distancia y el PWM, lo que calza con unos lentes autónomos. Hay dos gráficos con los resultados de las pruebas. Déjenlo explicado en el README. |
| Generación de información | 6.0 | El sistema convierte la distancia en intensidad de vibración (de 500 a 1500 mm y PWM de 90 a 255), que es lo que responde al problema. De las pruebas sacaron tasas de éxito y una nota promedio de 6,4 con 5 usuarios. |
| Calidad del código | 5.5 | La versión modular (`main_estesisi.ino` con config, sensores y actuadores) está bien comentada. Los archivos quedaron con "(1)" en el nombre, así que los `#include` no funcionan, y hay dos .ino en `software/src`. |
| Nota Software (30%) | 5.9 | |
| Esquemático y BOM (Hardware) | 5.5 | Sigue siendo el dibujo a mano del Avance 2. Los pines coinciden con el código (SDA 4, SCL 5 y el motor en 6 con 1 kΩ y 2N2222) y están todos los componentes, pero la leyenda marca B+ como 5 V. El BOM tiene cantidades, SKU, proveedor y precios, aunque el total está mezclado (36.850 y 29.626). |
| Estructura del repositorio | 5.5 | Las carpetas están bien y cada una tiene README. El README principal todavía tiene "[Fecha]", "[Otras herramientas necesarias]" y el checklist sin marcar, y `software/README.md` sigue con la plantilla. |
| Respaldo completo | 6.5 | Están el código, los esquemas, el BOM, el .f3z, los .stl, los renders, el plano, el informe final, la presentación, las fotos, los datos y las 3 iteraciones. Faltan el video y el enlace al reporte de testing. |
| Nota GitHub (5%) | 6.0 | |

Fortalezas: iteraciones documentadas, pruebas con 5 usuarios y firmware modular bien comentado.

Mejorar para la entrega final: arreglar los nombres con "(1)" para que compile, limpiar las plantillas del README y completar FUENTES.md.

## Comentarios

Hicieron lo que les pedí en el Avance 2, con iteraciones, pruebas con 5 usuarios y el código comentado. Lo de no tener almacenamiento ni dashboard ya lo conversamos, y como los lentes funcionan solos lo tomé en cuenta en la nota. Si alcanzan, un registro simple de las distancias igual les sumaría. Para la entrega final renombren los archivos con "(1)" para que compile, dejen un solo .ino y limpien los textos de plantilla del README. Completen también FUENTES.md, que tiene las tablas vacías y la IA en una sola línea. Pongan qué herramienta usaron y para qué.
