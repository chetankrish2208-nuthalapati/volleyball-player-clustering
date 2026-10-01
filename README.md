# Volleyball Player Clustering Using K-Means

## Project Overview

This project uses K-Means clustering to group men's volleyball attackers based on their attacking performance statistics.

The analysis was completed using Orange Data Mining without writing code.

## Objective

The objective of this project is to identify groups of volleyball attackers with similar statistical characteristics and explore patterns in attacking performance.

## Dataset

The project uses the **VNL 2024 - Men's Volleyball Stats** dataset obtained from Kaggle.

The attackers dataset includes variables such as:

* Attack points
* Attack errors
* Unsuccessful attacks
* Average attacks per match
* Attack success percentage
* Total attacks

Player name and team were retained as identification information.

## Tools Used

* Orange Data Mining
* K-Means Clustering
* Scatter Plot
* Data Table

## Methodology

The analysis followed these steps:

1. Imported the VNL 2024 men's attackers dataset into Orange.
2. Selected numerical attacking statistics as features.
3. Used player name and team as identifying information.
4. Applied K-Means clustering.
5. Compared different numbers of clusters.
6. Used Scatter Plot to visualize the resulting groups.
7. Examined the characteristics of the clusters based on the attacking statistics.

## Orange Workflow

The workflow used for the analysis is provided in:

`VNL2024_Attacker_Clustering.ows`

The workflow follows the general structure:

`File → Select Columns → K-Means → Data Table / Scatter Plot`





## Results

K-Means clustering was tested using different numbers of clusters to explore how the volleyball attackers could be grouped.

The cluster sizes obtained were:

| Number of Clusters | Cluster Sizes  |
| ------------------ | -------------- |
| K = 2              | 44, 188        |
| K = 3              | 72, 44, 116    |
| K = 4              | 83, 26, 62, 61 |

The K = 4 configuration was visualized using Scatter Plot to examine relationships between attack points, total attacks, and attack success percentage.

The resulting clusters represent groups of players with similar attacking statistical characteristics. The cluster numbers are algorithm-generated labels and do not represent predefined player roles.

The analysis demonstrates how K-Means clustering can be used to identify patterns and group players based on their attacking performance statistics.



## Key Learning

Through this project, I learned how an unsupervised machine learning method can be used to explore patterns in sports performance data.

I also learned how to prepare numerical features, apply K-Means clustering, and visualize clusters using Orange Data Mining.

## Project Files

* `VNL2024Men_Attackers.csv` — Dataset used for analysis
* `VNL2024_Attacker_Clustering.ows` — Orange workflow
* `Images/` — Screenshots of the workflow and visualizations

## Limitations

The clusters are based only on the attacking statistics included in the dataset. Other factors such as position, height, playing style, opposition strength, and defensive performance were not included in this analysis.

## Dataset Source



**VNL 2024 - Men's Volleyball Stats** — Kaggle.

The dataset was obtained from Kaggle and contains men's Volleyball Nations League statistics from 2024.

[Original Kaggle dataset](https://www.kaggle.com/datasets/jonathanpmoyer/vnl-2024-mens-stats)



