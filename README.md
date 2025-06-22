# Forest Cover Type Prediction

This project explores the use of different classification algorithms to predict forest cover types based on cartographic and ecological data. The data includes a mix of topographic features (like elevation, slope, and distance to water bodies) and categorical indicators (such as soil type and wilderness area).

### Project Overview

The goal was to train and compare the performance of three popular classification models:

- **Logistic Regression**
- **Random Forest Classifier**
- **XGBoost Classifier**

Instead of pre-processing the dataset by selecting only the most important features, all available columns were used directly to see how the models handle the raw input. The idea was to observe whether letting the models work with the full dataset would affect performance positively or negatively.

### Key Steps

- Loaded and explored the dataset
- Visualized feature relationships using correlation heatmaps and pair plots
- Trained and evaluated each model using accuracy and classification reports
- Compared model performance and discussed strengths and weaknesses

### Dataset

The dataset used in this project is publicly available and can be downloaded here:

https://www.kaggle.com/datasets/uciml/forest-cover-type-dataset

It contains data on over 500,000 observations, each representing a 30x30 meter cell of forest with features like elevation, aspect, soil type, and distance to fire points.

### How to Run

1. Clone this repository  
   ```bash
   git clone https://github.com/yourusername/forest-cover-prediction.git
   cd forest-cover-prediction
   ```

2. Install required libraries  
   (Recommended: Use a virtual environment)
   ```bash
   pip install -r requirements.txt
   ```

3. Run the notebook  
   Open `forest_cover_classification.ipynb` in Jupyter or VS Code.

### Results

Model performance was evaluated based on accuracy. Here’s a brief summary:

| Model                | Accuracy (Sample) |
|---------------------|-------------------|
| Logistic Regression | 72%               |
| Random Forest       | 95%               |
| XGBoost             | 87%               |


### Conclusion

This project demonstrates how different classification models perform when given a full, unfiltered dataset. Random Forest and XGBoost handled the high-dimensional data well, while Logistic Regression struggled with the complexity. It highlights the value of model choice and the trade-offs between simplicity and performance.

---

