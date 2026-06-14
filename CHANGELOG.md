# CHANGELOG

## Día 1 - Ejercicio 01
- Se creó la estructura base del proyecto urban_flow.
- Se inicializó el repositorio Git.
- Se creó la rama Sprint_1.
- Se agregó la documentación inicial del proyecto.

## Día 2 - Ejercicio 02
- Se descargó el dataset speeding_fines.csv en data/raw.
- Se realizó la carga del dataset en un DataFrame.
- Se visualizaron las primeras filas.
- Se analizaron los tipos de datos.
- Se contabilizaron los valores nulos.

## Día 3 - Ejercicio 03
- Se normalizaron las fechas al formato YYYY-MM-DD.
- Se normalizaron las horas al formato de 24 hs.
- Se normalizaron las ubicaciones eliminando caracteres especiales.
- Se limpiaron y validaron las patentes.
- Se eliminaron filas con valores vacíos en columnas relevantes.
- Se detectaron y eliminaron outliers.
- Se creó la columna exceso_velocidad_real.
- Se creó la columna exceso_velocidad.
- Se eliminaron filas sin infracción.

## Dia 4 - Ejercicio 04.

- Se creo la función FineAnalyzer.
- Se crearon los 4 metodos de analisis
  - Top de patentes
  - Ranking por horas
  - Exceso medio de velocidad
  - Multas por ubicacion.
- Se analizo el csv speeding_fines con los metodos creados.

## Día 5 - Ejercicio 05
- Se implementó la librería Matplotlib para la visualización de datos.
- Se generó un gráfico de barras con el ranking de las 10 patentes más reincidentes (fines.jpg).
- Se creó un gráfico de torta agrupado por franja horaria para analizar el porcentaje de infracciones por hora (hours.jpg).
- Se generó un gráfico de barras horizontales mostrando la cantidad de infracciones agrupadas por mes (months.jpg).
- Se implementaron gráficos de líneas para evaluar la evolución de los excesos de velocidad en los registros anómalos de las 00:00 y de la fecha 1932-01-01 (hour.jpg, date.jpg).
- Se exportaron todas las visualizaciones a la ruta urban_flow/data/interim/plots/.

## Día 6 - Ejercicio 06
- Se analizo el porcentaje de infracción que se produjeron en la fecha 1932-01-01.
- Se analizo el porcentaje de infracción que se produjeron en la hora 00:00.

## Día 7 - Ejercicio 07
- Se redacto una conclusión acerca de los datos que contiene el dataset.
# Sprint 2

## Día 1 - Ejercicio 01
- Configuración del repositorio Git.
- Creación de la rama Sprint_2.
- Descarga y descompresión del dataset de imágenes.

## Día 2 - Ejercicio 02
- Clasificación de imágenes en plates y completes.
- Construcción del diccionario group_images.
- Visualización aleatoria de imágenes.

## Dia 3 - Ejercicio 03
- Conversión de imágenes a escala de grises.
- Aplicación de suavizado Gaussian Blur.
- Detección de bordes mediante Canny.

## Día 4 - Ejercicio 04
- Extracción de patentes utilizando EasyOCR.
- Relación entre imágenes y dataset de multas.
- Generación del dataset final speeding_fines_image.csv.

## Día 5 - Ejercicio 05
- Obtención de métricas sobre multas e imágenes.
- Análisis de imágenes sin match y multas impagas.

## Día 6 - Ejercicio 06
- Elaboración de conclusiones generales del Sprint 2.
# Sprint 3

### Día 1 - Ejercicio 01

- Se creó la rama `Sprint_3` a partir de `Sprint_2`.
- Se preparó el entorno de trabajo para el nuevo sprint.
- Se incorporó el archivo README.md con el objetivo, introducción y contexto del sprint.

### Día 2 - Ejercicio 02

- Se creó el directorio `/content/remote_dvc` para simular un repositorio remoto de DVC.
- Se inicializó DVC en el proyecto.
- Se configuró el remote local de DVC.
- Se removió el seguimiento de archivos binarios por Git.
- Se migraron las imágenes originales a DVC.
- Se migraron las imágenes procesadas a DVC.
- Se migraron los gráficos generados a DVC.
- Se migraron los datasets procesados a DVC.
- Se realizó la sincronización de los datos mediante `dvc push`.

### Día 3 - Ejercicio 03

- Se diseñaron las entidades lógicas Vehiculo, Multa, Radar y Evidencia.
- Se definieron claves principales y atributos relevantes para cada entidad.
- Se documentaron las relaciones uno a muchos entre Vehiculo y Multa, y entre Radar y Multa.
- Se documentó la relación opcional uno a uno entre Multa y Evidencia.

### Día 4 - Ejercicio 04

- Se definieron las clases simples Vehiculo, Radar, Multa y Evidencia.
- Se implementó la función procesar_fila_csv para transformar una fila del CSV en una instancia de Multa.
- Se asociaron los objetos Vehiculo, Radar y Evidencia dentro de la multa generada.
- Se validó la función con una fila de ejemplo.

### Día 5 - Ejercicio 05

- Se implementaron los modelos ORM Vehiculo, Radar, Multa y Evidencia.
- Se definieron claves primarias y claves foráneas para representar las relaciones.
- Se incorporaron relaciones con relationship y back_populates.
- Se sobrescribió el método __repr__ en cada modelo para mejorar la legibilidad.

### Día 6 - Ejercicio 06

- Se creó la base de datos SQLite transito mediante SQLAlchemy.
- Se generaron automáticamente las tablas a partir de los modelos ORM.
- Se migraron los datos del archivo data/processed/speeding_fines_image.csv.
- Se controlaron valores faltantes de radar_id generando identificadores auxiliares.
- Se validó la cantidad de registros insertados por entidad.

### Día 7 - Ejercicio 07

- Se consultaron las diez patentes con mayor cantidad de multas.
- Se identificaron multas sin evidencia asociada y se calcularon sus totales.
- Se listaron los radares con mayor volumen de infracciones.
- Se consultaron las patentes más reincidentes dentro de un período determinado.
- Se calculó el porcentaje de multas confirmadas visualmente.
