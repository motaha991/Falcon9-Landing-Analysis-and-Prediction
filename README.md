# SpaceX Falcon 9 Data Analysis and Landing Prediction

This project is focused on analyzing SpaceX's Falcon 9 launch data to predict the success of booster landings. The primary goal is to build a model that can predict whether a Falcon 9 booster will successfully land, which is critical for SpaceX's reusability strategy and cost-saving measures.

## Project Overview

### 1. **Data Collection**
   - **Data Source**: The data used in this project includes details about Falcon 9 launches, such as launch site, payload, orbit type, booster version, and more.
   - **Data Cleaning**: Unwanted columns like `Date`, `Outcome`, `Year`, `LandingPad`, and `BoosterVersion` (since it contains the same value for all rows) were removed to streamline the dataset.
   - **Feature Engineering**:
     - Dummy variables were created for categorical columns such as `Orbit` and `LaunchSite`.
     - Boolean columns (`ridFins`, `Reused`, `Legs`) were mapped to binary values (0 and 1).

### 2. **Exploratory Data Analysis (EDA)**
   - **Visualizations**: Various plots were created to explore the relationships between features and the target variable (`Landing Outcome`).
   - **Correlations**: The correlations between different features were analyzed to understand their impact on the landing outcome.

### 3. **Model Building**
   - **Feature Selection**: Key features that influence the landing outcome were selected for modeling.
   - **Modeling Techniques**: Different machine learning models were trained and evaluated to predict the landing outcome.
   - **Model Evaluation**: Metrics like accuracy, precision, and recall were used to evaluate model performance.

### 4. **Results and Conclusions**
   - The final model provides a reasonable prediction of whether a Falcon 9 booster will successfully land, with potential applications in future SpaceX missions and cost-saving measures.

## Repository Structure

- `SpaceX_Falcon_9_Data_Analysis_and_Landing_Prediction.ipynb`: Jupyter Notebook containing the full analysis, model building, and evaluation process.
- `README.md`: Overview of the project, including objectives, methods, and results.

## Acknowledgments

- **Data Source**: SpaceX launch data from various sources.
- **Inspiration**: Inspired by the reusability goals of SpaceX and the potential for machine learning to predict mission outcomes.
