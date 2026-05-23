
# Sprint_2

## Objetivo
Desarrollar un sistema capaz de relacionar las multas por exceso de
velocidad con evidencia visual obtenida mediante imágenes de cámaras
urbanas, utilizando técnicas básicas de procesamiento de imágenes y OCR.

## Introducción y contexto del sprint
Los radares urbanos generan registros administrativos de multas de forma
automática y las cámaras asociadas registran la evidencia visual que
acompaña y valida cada infracción.

Sin embargo, existen distintos problemas a considerar:
- No todas las multas poseen una imagen asociada.
- No todas las imágenes corresponden a una infracción válida.
- Puede haber errores en la detección de texto mediante OCR.
- Algunas imágenes presentan baja calidad o ruido visual.

En este sprint se trabajó sobre técnicas básicas de procesamiento de
imágenes utilizando OpenCV para realizar transformaciones como escala de
grises, suavizado y detección de bordes.

Posteriormente, se utilizó OCR mediante EasyOCR para detectar patentes
vehiculares y relacionarlas con el dataset tratado en el Sprint 1,
permitiendo determinar qué multas poseen evidencia visual válida.
