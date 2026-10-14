# crime-data-k-means-clustering
Regional safety and crime rate analysis using K-Means clustering to categorize states/cities, identify safety clusters, and evaluate patterns for resource allocation.

# Regional Crime Data Clustering & Analysis

## 1. Business Problem
* **1.1. Business Objective:** Group states based on crime rates (Murder, Assault, Rape) and urban population metrics to identify public safety clusters and assist law enforcement resource allocation.
* **1.2. Constraints:** Disparate units and scaling across crimes per capita versus percentage metrics.

## 2. Data Dictionary
| Feature | Data Type | Description |
| :--- | :--- | :--- |
| `State` | Object | Name of the US State. |
| `Murder` | Float | Murder arrests per 100,000 residents. |
| `Assault` | Integer | Assault arrests per 100,000 residents. |
| `UrbanPop` | Integer | Percentage of the population living in urban areas. |
| `Rape` | Float | Rape arrests per 100,000 residents. |

## 3. Exploratory Data Analysis (EDA)
* **3.1. Summary:** Evaluated central tendencies and spreads for all four crime and demographic indicators.
* **3.2. Univariate Analysis:** Inspected distributions of violent crime statistics.
* **3.3. Bivariate Analysis:** Scatter plots mapping Assault versus Murder rates and Urban Population metrics.

## 4. Data Pre-processing
* **4.1. Data Cleaning & Feature Engineering:** Checked for missing records, encoded state names as index labels, and normalized features to give equal weight during distance calculations.

## 5. Model Building
* **5.1. Model Execution:** Built K-Means models on standardized dataset arrays.
* **5.2. Scree Plot:** Utilized Elbow graphs to verify the optimal number of clusters.
* **5.3. Validation & Insights:** Compared cluster configurations, labeled groups into safety tiers (e.g., High-Crime vs. Low-Crime regions), and derived key demographic insights.

## 6. Business Benefits & Impact
* Provides government bodies and policymakers with objective groupings to distribute safety funding, police personnel, and preventative social programs efficiently.
