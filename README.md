# ETL en Azure: Data Factory + SQL Database

Proyecto de pipeline en **Azure Data Factory** para ingerir datos de COVID desde Data Lake y 
persistirlos en **Azure SQL Database**.  

---

## 🎯 Objetivo
Implementar un pipeline en Azure que:
- Ingesta datos desde archivos CSV.
- Valida la presencia de los archivos en Data Lake.
- Copia y persiste los datos en una tabla de Azure SQL Database (`covid_population`).

---

## 🚀 Pipeline en Data Factory
Pipeline orquestado que incluye:
- Validación de archivos.
- Obtención de metadatos.
- Actividad **Copy Data** para cargar información en SQL.

📸 Ejemplo de actividad *Copy Data* en el pipeline:
![Copy Data Pipeline](pictures/copy_data_pipeline.PNG)

---

## 🛢️ Persistencia en SQL Database
Los datos se almacenan en una tabla relacional dentro de **Azure SQL Database**, accesible vía editor de consultas.  

📸 Vista de la tabla con los datos cargados:
![SQL Database](pictures/sql_database.PNG)

---

## 📊 Resultados esperados
- Carga exitosa de datos en SQL Database.
- Preparación para su futura visualización en Power BI.

---

## 🔧 Tecnologías utilizadas
- **Azure Data Factory**
- **Azure Data Lake Storage**
- **Azure SQL Database**


