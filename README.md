
# Sprint_3

## Objetivo

Profesionalizar la solución desarrollada incorporando mecanismos de versionado de datos, persistencia en bases de datos relacionales y almacenamiento vectorial de imágenes. El objetivo es mejorar la organización, escalabilidad y capacidad de consulta de la información relacionada con las infracciones de tránsito, permitiendo integrar tanto datos estructurados como evidencia visual en una misma solución.

## Introducción y contexto del sprint

A medida que el sistema Urban Flow crece en volumen de datos y complejidad, el uso exclusivo de archivos CSV deja de ser una alternativa adecuada para almacenar y consultar la información procesada.

Por este motivo, en este sprint se incorpora una base de datos relacional utilizando SQLAlchemy para modelar y persistir entidades clave del dominio, como vehículos, multas, radares y evidencias. Además, se implementa DVC para el control de versiones de archivos binarios, permitiendo gestionar imágenes y datasets de forma más eficiente que utilizando únicamente Git.

Como complemento, se incorpora una base de datos vectorial basada en OpenCLIP para almacenar representaciones vectoriales de las imágenes asociadas a las infracciones. Esto permite realizar búsquedas por similitud visual e identificar vehículos a partir de evidencia fotográfica, integrando información visual con los datos almacenados en la base relacional.

Estas mejoras permiten construir una solución más robusta, escalable y preparada para escenarios reales, combinando tecnologías de gestión de datos estructurados y no estructurados dentro de un mismo flujo de trabajo.
