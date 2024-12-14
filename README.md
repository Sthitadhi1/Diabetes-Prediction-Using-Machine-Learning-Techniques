# Diabetes Prediction Using Machine Learning

This repository contains a machine learning project aimed at predicting diabetes using various machine learning techniques. The project involves preprocessing the dataset, training multiple models, evaluating their performance using cross-validation, and visualizing results for algorithm comparison.

## Project Overview

The goal of this project is to accurately classify whether a patient has diabetes based on certain diagnostic measurements. The project includes:

- Exploratory Data Analysis (EDA) and visualization
- Data preprocessing and feature engineering
- Training multiple machine learning models
- Cross-validation for performance evaluation
- Algorithm comparison using visualization

## Dataset

The dataset used in this project includes features such as:
- Pregnancies
- Glucose
- Blood Pressure
- Skin Thickness
- Insulin
- BMI
- Diabetes Pedigree Function
- Age
- Outcome (target variable)

## Requirements

Install the required Python packages using:

```bash
pip install -r requirements.txt
```

### Key Libraries Used
- pandas
- numpy
- scikit-learn
- seaborn
- matplotlib

## Project Structure

```
├── diabetes-prediction-using-ml-techniques.ipynb # Jupyter notebook for the project
├── README.md                                     # Project description and instructions
└── diabetesml.csv                                # Dataset File
```

## Steps in the Project

1. **Data Loading and Exploration**
   - Load the dataset and explore its structure, including missing values and data types.

2. **Data Visualization**
   - Visualize the target distribution using pie charts and bar plots.
   - Explore feature distributions and relationships.

3. **Model Training and Evaluation**
   - Train multiple machine learning models (e.g., Logistic Regression, Decision Trees, Random Forests).
   - Evaluate models using 10-fold cross-validation.

4. **Algorithm Comparison**
   - Compare the performance of different models using boxplots for accuracy.

## Results

Model performance metrics are evaluated using accuracy. The boxplot visualization summarizes the comparison between algorithms.

## Usage

To run the project:

1. Clone this repository:

   ```bash
   git clone https://github.com/yourusername/diabetes-prediction.git
   cd diabetes-prediction
   ```

2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Run the Jupyter notebook:

   ```bash
   jupyter notebook diabetes-prediction-using-ml-techniques.ipynb
   ```

## Visualization Example

### Target Distribution

The target variable (`Outcome`) distribution is visualized using pie charts and count plots:

```python
f, ax = plt.subplots(1, 2, figsize=(18, 8))
df['Outcome'].value_counts().plot.pie(explode=[0, 0.1], autopct='%1.1f%%', ax=ax[0], shadow=True)
ax[0].set_title('Target Distribution')
ax[0].set_ylabel('')
sns.countplot(x='Outcome', data=df, ax=ax[1])
ax[1].set_title('Outcome Count')
plt.show()
```

## Contributing

Contributions are welcome! Feel free to fork this repository and submit a pull request with your improvements or new features.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- The dataset source (if applicable).
- Scikit-learn documentation for model training and evaluation methods.
- Matplotlib and Seaborn for data visualization.

---

Happy coding! 🚀
