
# Sprint_3

## Objetivo

Profesionalizar la solución desarrollada incorporando mecanismos de versionado de datos, persistencia en bases de datos relacionales y almacenamiento vectorial de imágenes. El objetivo es mejorar la organización, escalabilidad y capacidad de consulta de la información relacionada con las infracciones de tránsito, permitiendo integrar tanto datos estructurados como evidencia visual en una misma solución.

## Introducción y contexto del sprint

A medida que el sistema Urban Flow crece en volumen de datos y complejidad, el uso exclusivo de archivos CSV deja de ser una alternativa adecuada para almacenar y consultar la información procesada.

Por este motivo, en este sprint se incorpora una base de datos relacional utilizando SQLAlchemy para modelar y persistir entidades clave del dominio, como vehículos, multas, radares y evidencias. Además, se implementa DVC para el control de versiones de archivos binarios, permitiendo gestionar imágenes y datasets de forma más eficiente que utilizando únicamente Git.

Como complemento, se incorpora una base de datos vectorial basada en OpenCLIP para almacenar representaciones vectoriales de las imágenes asociadas a las infracciones. Esto permite realizar búsquedas por similitud visual e identificar vehículos a partir de evidencia fotográfica, integrando información visual con los datos almacenados en la base relacional.

Estas mejoras permiten construir una solución más robusta, escalable y preparada para escenarios reales, combinando tecnologías de gestión de datos estructurados y no estructurados dentro de un mismo flujo de trabajo.

# Conclusión

Durante el desarrollo de este sprint se avanzó en la profesionalización de la solución implementada para el análisis de infracciones de tránsito. En primer lugar, se incorporó DVC para el versionado de archivos binarios, permitiendo gestionar imágenes, gráficos y datasets de manera más eficiente y escalable que utilizando únicamente Git.

Posteriormente, se diseñó un modelo lógico y un modelo relacional que permitieron estructurar la información del dominio mediante las entidades Vehículo, Multa, Radar y Evidencia. A través de SQLAlchemy se implementó una base de datos relacional capaz de almacenar y consultar la información procesada de forma organizada, garantizando la integridad de las relaciones entre las distintas entidades.

Una vez creada la base de datos, se realizó la migración de los datos provenientes del archivo `speeding_fines_image.csv` y se desarrollaron diversas consultas analíticas que permitieron identificar patrones relevantes, como los vehículos con mayor cantidad de infracciones, los radares más activos y el porcentaje de multas que cuentan con evidencia visual.

Finalmente, se incorporó una base de datos vectorial utilizando OpenCLIP para generar representaciones vectoriales de las imágenes asociadas a las multas. Esto permitió vincular la información visual con la base de datos relacional y realizar búsquedas por similitud de imágenes, obteniendo de manera aproximada la patente y los datos del vehículo asociado.

En conjunto, este sprint permitió integrar tecnologías de versionado de datos, bases de datos relacionales y bases de datos vectoriales, construyendo una solución más robusta, escalable y preparada para escenarios reales donde es necesario combinar información estructurada con información visual para facilitar el análisis y la toma de decisiones.

