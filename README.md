# YouTube Ad Placement Analytics AWS
An end-to-end cloud-based platform for optimizing YouTube ad placements using AWS. The project extracts and analyzes viewer data via the YouTube API, automates ETL with Lambda, Glue, and S3, and visualizes insights through QuickSight, helping businesses maximize ad campaign ROI.

## Introduction
YouTube, the second most visited website globally, presents vast opportunities for businesses to connect with their audiences. However, identifying optimal channels or videos for ad placements remains a challenge. This project aims to develop a **data-driven analytics platform** leveraging AWS services to extract, transform, and analyze YouTube data, enabling smarter ad placement decisions.

## Objectives
- **Data Management**: Extract raw data from the YouTube API and store it in AWS S3.
- **ETL Automation**: Automate data transformation using AWS Glue and Lambda.
- **Dashboard Development**: Design an interactive dashboard using AWS QuickSight to visualize trends and optimize ad placements.

## System Design and Architecture
The architecture follows a streamlined data pipeline:

1. **Data Ingestion**: Raw YouTube API data is uploaded to S3 in JSON/CSV format.
2. **Data Transformation**: AWS Lambda functions convert raw data into Parquet format for efficient querying.
3. **ETL Automation**: AWS Glue automates schema creation, data cataloging, and data joining.
4. **Data Analysis**: AWS Athena executes queries on transformed data.
5. **Visualization**: AWS QuickSight builds interactive dashboards providing actionable insights.

### Architecture Diagram
![Architecture Detailed](https://github.com/user-attachments/assets/eb173aac-6791-4023-90e8-b3a8085ea8eb)

## Technologies Used
- **YouTube API**: Fetches real-time YouTube data.
- **AWS S3**: Stores raw and processed data.
- **AWS Glue**: Automates ETL processes and data cataloging.
- **AWS Lambda**: Handles data transformation (JSON to Parquet).
- **AWS Athena**: Enables SQL querying on transformed data.
- **AWS QuickSight**: Creates interactive dashboards for insights.
- **AWS CLI**: Manages AWS resources via the command line.
- **Python 3.8**: Used in Lambda functions and ETL scripts.

## Implementation Steps
### 1. Data Collection
- Extract data from the YouTube API in JSON/CSV formats.
- Store raw data in an S3 bucket.

### 2. Data Transformation
- Convert JSON/CSV files into Parquet format using Lambda functions.
- Optimize data types for efficient storage and querying.

### 3. ETL Pipeline
- Use AWS Glue to create a data catalog.
- Join datasets and partition data to enhance query performance.

### 4. Querying
- Execute SQL queries using AWS Athena to extract insights from transformed data.

### 5. Visualization
- Connect Athena to AWS QuickSight for dashboard development.
- Visualize trends, engagement metrics, and insights for ad placement optimization.

## Key Features
- **Interactive Dashboard**: Provides insights into:
  - Top viewed content categories (e.g., "Entertainment," "Music").
  - Best-performing ad placement opportunities.
  - Regional trends in content removal and viewership.
- **Automated ETL Process**: Ensures seamless data preparation and transformation.
- **Scalable Cloud Infrastructure**: Built entirely on AWS for high availability and scalability.

## Conclusion
This project delivers a robust analytics solution for YouTube ad placements by integrating AWS services. The automated ETL pipeline and interactive dashboards empower businesses with data-driven insights, improving ad targeting and engagement.
