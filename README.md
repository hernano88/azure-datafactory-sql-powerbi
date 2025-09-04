# ETL en Azure: Data Factory + Databricks + SQL + Power BI
Proyecto de pipeline en Azure Data Factory con integración a Databricks, SQL Database y visualización en Power BI

## 🚀 Objetivo
Implementar un pipeline de datos en Azure para procesar información de COVID y generar visualizaciones en Power BI.

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

## Dataset
Se utilizó un dataset de COVID (casos confirmados, muertes, población) en formato CSV para simular un escenario real de ingesta y transformación de datos.

## Resultados
Los datos procesados fueron visualizados en Power BI, generando dashboards con métricas como:
- Casos confirmados por cada 100k habitantes.
- Tasa de mortalidad.
- Evolución temporal de la pandemia por región.
