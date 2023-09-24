# Customer Segmentation and Pattern Mining

## Overview
This repository contains Python code for customer segmentation and pattern mining using unsupervised machine learning techniques. The primary objective is to identify distinct customer groups based on purchasing behavior and visualize these groups using clustering methods. 

## Table of Contents
- [Introduction](#introduction)
- [Dataset](#dataset)
- [Data Preprocessing](#data-preprocessing)
- [Feature Engineering](#feature-engineering)
- [K-Means Clustering](#k-means-clustering)
- [Hierarchical Clustering (Dendrogram)](#hierarchical-clustering-dendrogram)
- [Results](#results)
- [How to Use](#how-to-use)

## Introduction
Customer segmentation is a fundamental task in customer relationship management, allowing businesses to tailor their strategies to different customer groups. This repository demonstrates how to apply clustering techniques to a retail dataset, effectively grouping customers based on their purchasing habits.

## Dataset
The dataset utilized in this project is the "Online Retail" dataset, which contains valuable customer purchase information, including CustomerID, Amount, Frequency, and Recency.

## Data Preprocessing
Data preprocessing is crucial for ensuring data quality and consistency. Key steps include:
- Loading the dataset from an Excel file.
- Handling missing values.
- Adjusting data types.
- Creating a new feature, "Amount," by multiplying Quantity and UnitPrice.
- Converting InvoiceDate to a datetime format.
- Calculating Recency by measuring the time since the customer's last purchase.

## Feature Engineering
The project focuses on three essential customer features:
- **Amount**: The total purchase amount for each customer.
- **Frequency**: The number of purchases made by each customer.
- **Recency**: The number of days since the customer's most recent purchase.

## K-Means Clustering
K-Means clustering is applied to the feature-engineered dataset. This technique automatically identifies optimal customer clusters by utilizing the Elbow Method and Silhouette Score. Scaling is performed to ensure all features are equally weighted during clustering.

## Hierarchical Clustering (Dendrogram)
Hierarchical clustering is utilized with different linkage methods (single, complete, and average) to create dendrograms. Dendrograms offer valuable insights into the hierarchical structure of customer data.

## Results
- The K-Means clustering technique successfully segments customers into distinct clusters.
- Dendrograms are generated to visualize hierarchical clustering and hierarchy within customer groups.

## How to Use
1. Clone this repository to your local environment.
2. Install the required Python libraries specified at the start of the code, including numpy, pandas, seaborn, matplotlib, sklearn, and scipy.
3. Download the dataset and provide the accurate file path in the code.
4. Execute the Python script.
5. Review the results, including identified customer clusters and dendrograms.

Feel free to utilize this code as a foundation for your customer segmentation and pattern mining tasks on your datasets.
