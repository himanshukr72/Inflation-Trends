Inflation-Trends
This project provides a comprehensive analysis of inflation trends using Consumer Price Index (CPI) data from the Ministry of Statistics and Programme Implementation (MoSPI) of India. The repository contains a series of interconnected artifacts: a Jupyter Notebook for data processing, SQL scripts for database operations, and a Power BI dashboard for dynamic data visualization.

Project Recognition
This project was awarded a consolation prize in a Data Visualization Hackathon conducted by the Government of India in collaboration with MoSPI.

Project Contents
MoSPI_final.ipynb: A Jupyter Notebook that serves as the core data processing and exploratory data analysis (EDA) tool. It uses Python libraries such as pandas and numpy to clean the raw cpi Group data.csv, handle missing values (represented as "*"), and prepare the data for further analysis.

SQL_COMMAND.sql: This file contains a series of SQL scripts designed to create and manage the project's relational database. These scripts are used to create tables, load the cleaned data, and perform aggregated calculations, such as the mean of inflation by group and sector.

CPI_Dashboard_MoSPI_GOI.pbix and CPI_Dashboard_MoSPI_GOI.pbit: These Power BI files contain the final, interactive dashboard for visualizing the inflation trends.

README.md: The current file, which you can update with further details about the project.

Data Overview
The primary dataset is cpi Group data.csv, which is sourced from the Ministry of Statistics and Programme Implementation (MoSPI), Government of India. This dataset offers granular, time-series data on the CPI, a key economic indicator. The data includes the following key columns:

BaseYear: The reference year for CPI calculations.

Year & Month: Provides the temporal resolution for the data.

State & Sector: Allows for a more granular analysis of inflation across different regions and economic sectors (Combined, Rural, Urban).

Group & SubGroup: Categorizes consumer goods and services, enabling a detailed look at inflation drivers.

Index: The CPI value itself.

Inflation (%): The final annual inflation metric.

Note that the raw data contains null values represented by *, which are handled and cleaned in the Jupyter Notebook.

Analysis and Visualization
This project employs a robust three-part strategy for data analysis and visualization, ensuring data integrity and real-time insights.

Python-based Analysis: The MoSPI_final.ipynb notebook is used for initial data cleaning and exploratory analysis, providing a foundation for understanding the dataset's characteristics.

SQL Database Integration: The SQL_COMMAND.sql scripts create a structured database environment. This approach is highly scalable and efficient for storing and querying large datasets.

Real-Time Power BI Dashboard: The Power BI dashboard (.pbix file) is a key feature of this project. It utilizes a direct query connection to the SQL database, which means:

No Data Storage: Data is not imported or stored on the Power BI server, keeping the file size small and reducing storage overhead.

Real-Time Insights: All visuals and reports are directly connected to the live database, ensuring that the dashboard always displays the most up-to-date information.

Getting Started
To get started with this project, follow these simple steps:

Clone the Repository:
Open your terminal or command prompt and run the following command to download the project files:
git clone [repository URL]

Run the Analysis:

Open MoSPI_final.ipynb in your preferred Jupyter environment (e.g., Jupyter Notebook, JupyterLab) to execute the data cleaning and analysis steps.

Use the scripts in SQL_COMMAND.sql to set up and populate your PostgreSQL database.

Launch the Dashboard:

Ensure you have Power BI Desktop installed on your machine.

Open the CPI_Dashboard_MoSPI_GOI.pbix file to view the interactive dashboard.

The dashboard will automatically connect to your SQL database to pull the latest data.

Conclusion
This project successfully demonstrates an end-to-end data pipeline, starting from raw, unstructured data and culminating in a dynamic, real-time business intelligence dashboard. By leveraging Python for data preparation, SQL for robust data management, and Power BI for interactive visualization with a direct query connection, the project delivers a scalable and efficient solution for monitoring and analyzing inflation trends. It provides a clear, actionable example of how different technologies can be integrated to transform raw data into valuable business insights.
