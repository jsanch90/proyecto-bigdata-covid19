# Proyecto Big Data COVID-19

- [Proyecto Big Data COVID-19](#proyecto-big-data-covid-19)
  * [Desarrolladores](#desarrolladores)
- [¿Cual es la problemática que quiere resolver?](#-cual-es-la-problem-tica-que-quiere-resolver-)
- [Tecnologías de desarrollo](#tecnolog-as-de-desarrollo)
  * [Ingesta, procesamiento y análisis de los datos](#ingesta--procesamiento-y-an-lisis-de-los-datos)
  * [Visualización](#visualizaci-n)


## Desarrolladores

- Joshua Sánchez Álvarez - jsanch90@eafit.edu.co - Universidad EAFIT
- Juan Pablo Zapata Raigoza - jzapat90@eafit.edu.co - Universidad EAFIT

# ¿Cual es la problemática que quiere resolver?

acumulado - casos vs fechas
Se tienen unos datasets con información sobre el nuevo Coronavirus COVID-19 y se espera con ellos realizar un análisis para obtener información de como el virus se esta desarrollando a nivel nacional e internacional, finalmente se desarrollaran varios dashboard para visualizar y tener un mejor entendimiento de los datos obtenidos durante el análisis.

# Tecnologías de desarrollo

## Ingesta, procesamiento y análisis de los datos
Para esta tarea hicimos uso del framework [Apache Spark](https://spark.apache.org/) adaptado para el lenguaje Python (PySpark) cargamos los datos que venian en formato CSV en dataframes de Spark y realizamos el respectivo procesamiento, finalmente los resultados los almacenamos en ficheros CSV en un Bucket de S3. Todo el procesmienro se realizo en un Jupyter notebook sobre un cluster EMR de Amazon.
![](https://www.bigdata.uma.es/wp-content/uploads/2020/02/apache-spark-825x460.jpg)

## Visualización
Para la visualización utilizamos [Power BI](https://powerbi.microsoft.com/es-es/), cargamos los archivos de salida de Spark que teníamos en el Bucket de S3 y realizamos diferentes gráficos, como mapas de calor, diagramas de barras, diagramas circulares, etc.
![](https://businessdataschool.com/wp-content/uploads/2019/02/power-bi-2-0-logo.png)
