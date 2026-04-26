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
