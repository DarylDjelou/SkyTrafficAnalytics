# Sky Traffic Data Analysis

## Project Overview
This project performs an in-depth data analysis of international aviation traffic crossing US borders. Utilizing massive, industry-scale datasets of international flight departures and passengers, the analysis explores seasonal trends, top operational hubs, and historical trajectories. Furthermore, it employs Machine Learning architectures to predict future flight volumes and classify high-traffic routes based on historical characteristics.

This project was developed by **Group 5 - Data Analysis**.

## Datasets
The analysis uses the following primary datasets (expected to be placed in the project root directory):
- `International_Report_Departures.csv`: Contains structured categorical and numerical variables including Year, Month, Carrier Group, Origin Airport, Destination Airport, and Total Departures.
- `International_Report_Passengers.csv`: Contains similar structured data regarding passenger volumes.

*Note: The datasets are extremely large (close to 1 million observations) and must be downloaded separately.*

## Project Structure
The core of the analysis is contained within the Quarto markdown document `SkyTraffic.qmd`, which intertwines executable R code with narrative text. The document is structured sequentially into the following phases:

1. **Pre-Week: Team Forming & Data Acquisition:** Selection of data and definition of the primary research question.
2. **Week 1: Defining the Scope and Understanding the Data:** Data loading, verification, and cleaning (handling missing values and outliers).
3. **Week 2-3: Exploratory Data Analysis (EDA) and Visualization:** Identifying macroeconomic trends, top origin hubs, and seasonality using visualizations (line plots, heatmaps).
4. **Week 4: Baseline Modeling:** Establishing baseline performance using Linear Regression and Logistic Regression to predict flight volumes and classify routes as "High Traffic."
5. **Week 5: Advanced Modeling:** Implementing non-linear tree-based models, including simple Decision Trees and a powerful Random Forest ensemble, to capture complex interactions in the data.
6. **Week 6: Model Evaluation:** Assessing model performance via Feature Importance plots, ROC curves, and comprehensive accuracy/Kappa comparisons.
7. **Week 7: Final Conclusion and Real-World Reporting:** Summarizing findings and proposing real-world business applications for logistics and infrastructure planning.

## Key Findings
- **Seasonality:** Summer months (July/August) heavily dominate international travel volumes.
- **Hubs:** Coastal airports like MIA, JFK, and LAX handle the vast majority of international traffic.
- **Predictive Modeling:** Advanced ensemble methods (Random Forest) significantly outperformed linear baselines in predicting high-traffic routes, proving the complex, non-linear nature of aviation behavior driven heavily by carrier groups and seasons.

## Requirements
To execute the analysis, you will need **R** and the following packages installed:
- `readr`
- `dplyr`
- `ggplot2`
- `patchwork`
- `tidyr`
- `caret`
- `rpart`
- `rpart.plot`
- `ranger`
- `pROC`
- `tidyverse`
- `ggcorrplot`

## Usage
1. Ensure both CSV datasets are placed in the same directory as the `.qmd` file.
2. Open `SkyTrafficAnalytics.Rproj` in RStudio.
3. Render the `SkyTraffic.qmd` file to generate the final HTML report (`SkyTraffic.html`) containing all code output and visualizations.
