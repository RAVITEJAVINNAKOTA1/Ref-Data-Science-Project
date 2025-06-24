
# NASA Turbofan Engine RUL Prediction

This project uses predictive modeling to estimate the Remaining Useful Life (RUL) of aircraft engines using the NASA C-MAPSS dataset.

## 📂 Project Structure

- **Data Source**: NASA C-MAPSS Turbofan Engine Degradation Simulation Dataset. https://www.nasa.gov/intelligent-systems-division/discovery-and-systems-health/pcoe/pcoe-data-set-repository/
- **File**: `NasaTurbofanModel.ipynb` (Google Colab Notebook)

## 📌 Key Features

- Data loading and preprocessing from multiple file types
- Feature engineering to compute RUL
- Exploratory Data Analysis (EDA) with visualizations
- Model training using:
  - Linear Regression
  - Random Forest
  - Gradient Boosting
- Model evaluation using MAE, RMSE, R²
- Hyperparameter tuning with RandomizedSearchCV
- Feature importance analysis for tree-based models

## 📊 Visualization Highlights

- RUL distribution
- Sensor data trends
- Correlation heatmap
- Feature importance bar plots

## 🚀 Getting Started

### Prerequisites

- Python 3.x
- `pandas`, `numpy`, `matplotlib`, `seaborn`
- `scikit-learn`

### Running the Notebook

1. Upload the dataset folder `CMaps` containing:
   - `train_FD001.txt`
   - `test_FD001.txt`
   - `RUL_FD001.txt`

2. Open `NasaTurbofanModel.ipynb` in Colab or Jupyter.

3. Run all cells.

## ⚙️ Model Performance (Baseline)

| Model                    | MAE   | RMSE  | R² Score |
|--------------------------|-------|--------|----------|
| Baseline Linear Regression | 34.05 | 44.34 | 0.570    |
| Baseline Random Forest     | 29.63 | 41.46 | 0.624    |
| Baseline Gradient Boosting | 29.88 | 41.37 | 0.625    |
| Tuned Random Forest        | 29.25 | 40.93 | 0.633    |
| Tuned Gradient Boosting    | 29.55 | 41.39 | 0.625    |

(Tuned model performance metrics are printed in the notebook output.)

## 📁 Data Columns

- **Operational Settings**: operational_set_1 to operational_set_3
- **Sensor Measurements**: T2, T24, T30, ..., W32
- **Target**: RUL (Remaining Useful Life)

## 📈 License

This project is for academic and research purposes only.

## 📬 Contact

For any inquiries, please open an issue or reach out via GitHub.

---


