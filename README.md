## 📝 Project Overview

This project focuses on detecting network intrusions using the CIC-IDS2017 dataset. The dataset simulates realistic network traffic with normal activity and seven different attack scenarios. The project involves:
- Cleaning and preprocessing the dataset to handle duplicates, missing values, and imbalances.
- Conducting exploratory data analysis to identify patterns and correlations.
- Using dimensionality reduction techniques like PCA to optimize computational efficiency.
- Training multiple machine learning models for binary and multi-class intrusion detection.
- Evaluating model performance to identify the most effective classifiers.

---

## 📂 Dataset Details

The **CIC-IDS2017 dataset** is a benchmark dataset for evaluating intrusion detection systems. It contains network traffic data, including normal activity and seven different attack scenarios:

- **Attack Scenarios**: Brute-force, Heartbleed, Botnet, DoS, DDoS, Web attacks, and inside infiltration.
- **Rows**: 2,830,743
- **Columns**: 79 (78 features and 1 label)

The dataset is highly imbalanced, with the majority of records classified as "Normal." It is available at [CIC-IDS2017 Dataset](https://www.unb.ca/cic/datasets/ids-2017.html).

---

## 📂 Project Structure

```plaintext
├── Intrusion_Detection.ipynb         # Main notebook
├── README.md                         # Project documentation
├── requirements.txt                  # Python dependencies
├── LICENSE                           # Liecense inforamtion
```

---

## 🚀 Features

1. **Comprehensive Preprocessing**:
   - Removes duplicates and fills missing values efficiently.
   - Optimizes memory usage for large datasets.

2. **Exploratory Analysis**:
   - Insightful visualizations to explore relationships and distributions.
   - Identifies multicollinearity issues to improve model robustness.

3. **Dimensionality Reduction**:
   - Applies PCA to reduce dimensions while retaining maximum information.

4. **Flexible Classification**:
   - Supports both binary and multi-class intrusion detection.
   - Trains multiple machine learning models and compares their performance.

5. **Balanced Training Dataset**:
   - Creates a balanced dataset for robust model training.

---

## 🛠️ Dependencies

Install the required libraries with:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn missingno
```

---

## 🔍 How to Use

1. Clone the repository:
   ```bash
   git clone https://github.com/f-a-tonmoy/intrusion-detection-system.git
   cd intrusion-detection-system
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Run the notebook:
   ```bash
   jupyter notebook Intrusion_Detection.ipynb
   ```

---

## 🧪 Results

### Binary Classification Algorithms
1. **Logistic Regression**:
   - **Strengths**: Efficient with large datasets and quick training time.
   - **Weaknesses**: Lower accuracy compared to SVM.
   - **Insights**:
     - Performance improved with parameter tuning and cross-validation to prevent overfitting.
     - Standardizing the dataset with a scaler significantly enhanced accuracy and other performance metrics.

2. **Support Vector Machine (SVM)**:
   - **Strengths**: Higher accuracy than Logistic Regression, especially after tuning kernel type and regularization parameters.
   - **Weaknesses**: Computationally expensive and time-intensive to train.

**Best Performing Model**: SVM outperformed Logistic Regression, achieving higher accuracy and precision for binary classification tasks.

---

### Multi-Class Classification Algorithms
1. **Random Forest**:
   - **Strengths**: Best performance in precision, recall, and F1-score. Handles complex relationships effectively.
   - **Insights**: Significant improvements achieved through hyperparameter tuning, including feature selection and increasing the number of estimators.

2. **K-Nearest Neighbors (KNN)**:
   - **Strengths**: Simple, interpretable, and performed well across most metrics.
   - **Weaknesses**: Slightly less effective than Random Forest in handling imbalanced data.

3. **Decision Trees**:
   - **Strengths**: Quick to train and computationally efficient.
   - **Weaknesses**: Struggled to capture complex relationships, leading to lower performance metrics compared to Random Forest and KNN.

**Best Performing Model**: Random Forest demonstrated superior performance, followed by KNN and Decision Trees.

---

**Key Insights**:
- SMOTE (Synthetic Minority Over-sampling Technique) was applied to address dataset imbalance, resulting in balanced training data and improved model performance.
- Standardization had minimal impact on multi-class classification models, with only slight improvements observed when using a standard scaler.

---

## 🤝 Contributing

Contributions are welcome! Feel free to open issues or create pull requests.

---

## 📜 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## 💬 Contact

For inquiries or feedback:
- **Fahim Ahamed (Tonmoy)**: [f.a.tonmoy00@gmail.com](mailto:f.a.tonmoy00@gmail.com)
- GitHub: [f-a-tonmoy](https://github.com/f-a-tonmoy)
```
