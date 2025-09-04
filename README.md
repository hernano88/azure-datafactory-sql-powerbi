# ETL en Azure: Data Factory + Databricks + SQL + Power BI
Proyecto de pipeline en Azure Data Factory con integración a Databricks, SQL Database y visualización en Power BI

## 🚀 Objetivo
Implementar un pipeline de datos en Azure para procesar información de COVID y generar visualizaciones en Power BI.

## Dataset
Se utilizó un dataset de COVID (casos confirmados, muertes, población) en formato CSV para simular un escenario real de ingesta y transformación de datos.

## Arquitectura
1. **Azure Data Factory** → Orquesta pipelines.
2. **Azure Databricks** → Limpieza, transformación y forecasting.
3. **Azure SQL Database** → Persistencia de datos.
4. **Power BI** → Dashboards de análisis.

## 🛠️ Tecnologías
- Azure Data Factory
- Azure Databricks (PySpark, Prophet, SQL)
- Azure SQL Database
- Power BI
- Python

## Resultados
Los datos procesados fueron visualizados en Power BI, generando dashboards con métricas como:
- Casos confirmados por cada 100k habitantes.
- Tasa de mortalidad.
- Evolución temporal de la pandemia por región.

- ## Cómo usar este proyecto
1. Clonar este repositorio.
2. Cargar el dataset de COVID en Azure Data Lake Storage (CSV).
3. Ejecutar el pipeline en Azure Data Factory para orquestar la ingesta.
4. Procesar los datos con notebooks de Databricks en PySpark/SQL.
5. Persistir resultados en Azure SQL Database.
6. Conectar Power BI al SQL Database para visualizar dashboards.

## Persistencia en SQL Database
Esta captura muestra la tabla `covid_population` creada en **Azure SQL Database** y consultada con un `SELECT TOP 1000`.

![SQL Database](pictures/sql_database.PNG)


## Pipeline de persistencia en Azure Data Factory
Aquí se ve el pipeline `data_persist` en **Azure Data Factory**, que utiliza la actividad *Copy Data* para copiar datos transformados hacia la base de datos SQL.

![Pipeline Copy Data](pictures/copy_data_pipeline.PNG)



