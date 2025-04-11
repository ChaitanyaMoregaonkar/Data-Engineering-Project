
# Tokyo Olympics Data Analytics Pipeline 🌏🥇📊

This project demonstrates a complete modern data engineering and analytics pipeline using Azure services to process, analyze, and visualize Tokyo Olympics data. The objective was to ingest raw Olympic datasets, perform transformations, and generate insightful dashboards to explore medal counts, athlete performance, and country-wise statistics.

## 🔧 Tech Stack & Tools

- **Azure Data Factory**: Data ingestion and orchestration
- **Azure Data Lake Gen 2**: Storage for raw and transformed data
- **Azure Databricks**: Data transformation using PySpark
- **Azure Synapse Analytics**: Data modeling and advanced analytics
- **Power BI / Looker Studio / Tableau**: Interactive dashboards

---

## 🔄 Architecture Overview

The pipeline is structured as follows:

![image](https://github.com/user-attachments/assets/4bb1cb09-acb8-432e-b0bf-eecfcd8f4066)

1. **Data Source**: Olympic data from public datasets (CSV, JSON).
2. **Ingestion**: Azure Data Factory is used to ingest data into a **Raw Data Store** in Data Lake Gen 2.
3. **Transformation**: Azure Databricks reads raw data, performs cleaning, feature engineering, and stores the transformed data back in Data Lake Gen 2.
4. **Analytics**: Azure Synapse Analytics queries the transformed data for aggregated insights.
5. **Visualization**: Dashboards are built using Power BI, Looker Studio, and Tableau to present the final insights.

---

## 📁 Folder Structure

```
📦tokyo-olympics-analytics
 ┣ 📁data
 ┃ ┣ raw/                   # Raw Olympic data files
 ┃ ┗ transformed/           # Processed/cleaned data
 ┣ 📁notebooks
 ┃ ┗ data_transformation.ipynb
 ┣ 📄README.md
 ┗ 📄requirements.txt
```

---

## 📊 Dashboards

The dashboards provide the following insights:
- Medal tally by country and sport
- Gender-based participation over the years
- Top-performing athletes and countries
- Interactive filters by sport, year, and country

---

## 🚀 Getting Started

1. Clone this repo:
   ```bash
   git clone https://github.com/yourusername/tokyo-olympics-analytics.git
   cd tokyo-olympics-analytics
   ```

2. Open `notebooks/data_transformation.ipynb` in Azure Databricks to process raw data.

3. Deploy the pipeline in Azure Data Factory using the JSON template in `/pipeline`.

4. Use Power BI or Tableau to connect to your Synapse endpoint and import visuals.

---

## 📌 Future Improvements

- Add streaming capability for real-time Olympic updates (simulated)
- MLOps pipeline for predicting medal winners
- Integrate Azure Purview for metadata governance

---

## 📬 Contact

For questions, suggestions, or collaboration:
**Chaitanya Moregaonkar**  
✉️ moregaonkar.chaitanya@utdallas.edu  
🔗 [LinkedIn](https://linkedin.com/in/chaitanyamoregaonkar)

---

## 📄 License

This project is licensed under the MIT License.
