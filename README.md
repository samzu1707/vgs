# Data Visualization Project

## Project Overview
This project focuses on analyzing and visualizing the video game sales dataset (`vgsales new.csv`). The primary objective is to clean, preprocess, and augment the data, followed by creating insightful visualizations. The final outputs include a cleaned dataset and a detailed analysis of the data.

## Key Steps

### 1️⃣ Data Loading
- The dataset is loaded using **pandas** for efficient data manipulation.

### 2️⃣ Data Cleaning
- Identified and handled missing values:
  - `Year` column: Missing values were filled with `unknown`.
  - `Publisher` and `Genre` columns: Missing values were replaced with `Unknown`.
- Removed duplicate rows to ensure data integrity.

### 3️⃣ Data Preprocessing
- Standardized column names for consistency.
- Converted the `Year` column to numeric format.
- Renamed columns for better readability, e.g.,
  - `NA_Sales` → `NorthAmerica($)`
  - `EU_Sales` → `EuropeUnion(€)`
  - `JP_Sales` → `Japan(¥)`

### 4️⃣ Data Augmentation
- Added a new column `Total_Sales`, which is the sum of regional sales:
  ```
  Total_Sales = NorthAmerica($) + EuropeUnion(€) + Japan(¥) + Other_Sales
  ```

### 5️⃣ Data Visualization
Created visualizations to uncover patterns and insights:
- **Bar Chart**: Distribution of `Global_Sales`.
- **Pie Chart**: Proportion of `EuropeUnion(€)` sales.
- **Density Plot**: Distribution of `Other_Sales`.
- **Top Games by Sales**: Visualized the top 10 games by total sales.

### 6️⃣ Data Saving
- Saved the cleaned and processed dataset as `cleaned_vgsales new.csv`.

## Tools and Technologies
- **Python Libraries**: pandas, numpy
- **IDE**: Jupyter Notebook

## Files in the Repository
- `vgsales new.csv`: Original dataset
- `cleaned_vgsales new.csv`: Cleaned and processed dataset
- `vgs_dp.ipynb`: Jupyter Notebook containing all the code
- `README.md`: Documentation for the project

## Installation Instructions
1. Clone the repository:
   ```bash
   git clone https://github.com/samzu1707/vgs.git
   ```
2. Navigate to the project directory:
   ```bash
   cd vgs-project
   ```
3. Open the Jupyter Notebook:
   ```bash
   jupyter notebook vgs_dp.ipynb
   ```

## Future Scope
- Explore additional datasets for comparative analysis.
- Enhance visualizations with interactive libraries like Plotly or Dash.
- Implement advanced data analysis techniques, such as regression or clustering.

## Contributors
- **Samra Zulfiqar**

## Contact
- **Email**: samrazulfiqar0@gmail.com
- **GitHub**: [samzu1707](https://github.com/samzu1707)

---
**Good luck with your project! 🚀**
