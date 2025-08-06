
# 🎓 Chance of Admission Prediction

This project aims to build a machine learning model that predicts the **probability of a student being admitted** to a graduate program based on academic performance and profile features.

## 📂 Dataset

- **Source**: [YBI Foundation](https://github.com/ybifoundation/Dataset/raw/main/Admission%20Chance.csv)
- **Records**: 400 student applications
- **Features**:
  - GRE Score
  - TOEFL Score
  - University Rating
  - SOP (Statement of Purpose strength)
  - LOR (Letter of Recommendation quality)
  - CGPA
  - Research (0 or 1)
  - Chance of Admit (Target variable)

## 🛠️ Technologies Used

- Python
- pandas, NumPy – for data manipulation
- matplotlib, seaborn – for visualization
- scikit-learn – for model building and evaluation

## 🧹 Data Preprocessing

- Cleaned column names and dropped unnamed columns
- Verified no missing values
- Defined X (features) and y (target)

## 📊 Exploratory Data Analysis

- Plotted a correlation heatmap to analyze feature importance
- Found CGPA, GRE, and TOEFL to be highly correlated with the target

## 🤖 Model Training

- Split data using 80-20 train-test split
- Trained a **Linear Regression** model on training data

## 📏 Evaluation Metrics

- **R² Score**: 0.8212
- **Mean Squared Error (MSE)**: 0.0046
- Plotted actual vs predicted values for visualization

## 🔮 Sample Prediction

For a student profile with:
- GRE: 325, TOEFL: 112, CGPA: 9.1, Research: 1  
- University Rating: 4, SOP: 4.5, LOR: 4  

📌 **Predicted Chance of Admission**: `0.80`

## 📘 Conclusion

The model effectively uses academic and profile features to estimate admission chances. Features like CGPA, GRE, and TOEFL scores are strong indicators of admission probability.

## 🚀 Future Improvements

- Try advanced models (e.g., Ridge, Lasso, Random Forest)
- Hyperparameter tuning
- Cross-validation
- Deploy as a web app using Streamlit or Flask
