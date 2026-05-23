
## Conclusión

El análisis del dataset de infracciones por exceso de velocidad permitió
identificar múltiples inconsistencias provenientes del sistema heredado,
tales como errores en los formatos de fecha y hora, valores faltantes y
registros inválidos en campos clave como patentes y ubicaciones.

A través del proceso de limpieza y normalización, se logró estandarizar
los datos, eliminar registros incompletos y depurar valores atípicos,
obteniendo un conjunto de datos consistente y confiable. Asimismo, la
generación de nuevas variables, como el exceso de velocidad real y el
exceso de velocidad considerando el margen permitido, permitió
identificar con mayor precisión las infracciones efectivas.

El análisis exploratorio y las visualizaciones realizadas evidenciaron
patrones relevantes, como la existencia de patentes reincidentes, la
concentración de infracciones en determinados horarios y su distribución
a lo largo del tiempo. Además, se detectó la presencia de valores por
defecto, como la fecha 1932-01-01 y la hora 00:00, lo que confirma la
existencia de errores en los registros originales y resalta la
importancia del proceso de depuración.

En conclusión, el dataset resultante se encuentra preparado para su uso
en análisis más avanzados y para su integración en un nuevo sistema,
permitiendo obtener información confiable que puede contribuir a la toma
de decisiones y a la mejora de los sistemas de control de infracciones.


# Sprint 2 - Conclusiones

Durante este Sprint se trabajó sobre el procesamiento de imágenes asociado a multas por exceso de velocidad. Se realizó la clasificación de imágenes, el procesamiento mediante OpenCV y la extracción de texto utilizando OCR.

Los resultados obtenidos permiten observar que no todas las imágenes pudieron relacionarse correctamente con una multa, ya sea por errores del OCR, calidad de imagen o ausencia de coincidencias en el dataset original.

También se pudo comprobar que una parte importante de las multas impagas sí posee evidencia visual asociada, lo cual podría resultar útil para procesos de validación o auditoría.

La utilización de técnicas simples de procesamiento de imágenes como escala de grises, suavizado y detección de bordes permitió mejorar parcialmente la detección de texto. Sin embargo, existen técnicas más avanzadas que podrían mejorar aún más los resultados, como filtrado morfológico, detección de contornos o segmentación específica de patentes.

Finalmente, este Sprint permitió integrar procesamiento de imágenes, OCR y análisis de datos dentro de un mismo flujo de trabajo utilizando Python, OpenCV y herramientas de versionado con Git.
