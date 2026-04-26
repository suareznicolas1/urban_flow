
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
