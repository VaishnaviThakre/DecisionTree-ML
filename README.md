# DecisionTree-ML Repository

Welcome to the **DecisionTree-ML** repository! This project demonstrates the application of Decision Tree Classifiers to the Iris dataset, showcasing various aspects of data loading, preprocessing, model training, evaluation, and hyperparameter tuning. The results are visualized through tree plots and evaluated using metrics like accuracy, precision, recall, and F1-score.

## Table of Contents
1. [Introduction](#introduction)
2. [Dataset](#dataset)
3. [Setup](#setup)
4. [Code Overview](#code-overview)
5. [Results](#results)
7. [Hyperparameter Tuning](#hyperparameter-tuning)
8. [Conclusion](#conclusion)
9. [Contributing](#contributing)
10. [License](#license)

## Introduction
This project aims to explore the capabilities of Decision Tree Classifiers using the classic Iris dataset. The Iris dataset is widely used for demonstrating machine learning techniques due to its simplicity and well-defined features.

## Dataset
The dataset used in this project is the Iris dataset, which includes 150 samples of iris flowers, each described by four features:
- Sepal Length
- Sepal Width
- Petal Length
- Petal Width

Each sample belongs to one of three species:
- Setosa
- Versicolor
- Virginica

## Setup
To get started with this project, follow these steps:

1. **Clone the repository:**
   ```bash
   git clone git@github.com:VaishnaviThakre/DecisionTree-ML.git
   cd DecisionTree-ML
   ```

2. **Install the required dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

## Code Overview
The code in this repository performs the following steps:

1. **Data Loading and Preprocessing:**
   - Loads the Iris dataset.
   - Converts the dataset to a Pandas DataFrame.
   - Creates a new column "Species" with target values mapped to species names.

2. **Data Inspection:**
   - Checks for missing values.
   - Displays data types and descriptive statistics.

3. **Data Splitting:**
   - Splits the dataset into training and testing sets.

4. **Model Training:**
   - Trains a Decision Tree Classifier on the training set.

5. **Model Evaluation:**
   - Evaluates the model using metrics like accuracy, precision, recall, and F1-score.
   - Visualizes the Decision Tree.

6. **Hyperparameter Tuning:**
   - Performs Grid Search with Cross-Validation to find the best hyperparameters.
   - Evaluates the best model.

## Results
- **Initial Model:**
  - Achieved 100% accuracy on the test set.
  - Perfect precision, recall, and F1-score for all species.

- **Best Model after Hyperparameter Tuning:**
  - Best Parameters: `{'criterion': 'gini', 'max_depth': 3, 'min_samples_leaf': 4, 'min_samples_split': 2}`
  - Best Cross-Validation Score: `0.983`
  - Achieved 100% accuracy on the test set.


## Hyperparameter Tuning
The hyperparameter tuning was performed using Grid Search with the following parameter grid:
- `criterion`: ['gini', 'entropy']
- `max_depth`: [2, 3, 4, 5, 6, 7, 8]
- `min_samples_split`: [2, 5, 10]
- `min_samples_leaf`: [1, 2, 4]

The best parameters were found to be:
- `criterion`: 'gini'
- `max_depth`: 3
- `min_samples_leaf`: 4
- `min_samples_split`: 2

## Conclusion
This project demonstrates the effectiveness of Decision Tree Classifiers on the Iris dataset. The model achieved perfect classification accuracy, and hyperparameter tuning further optimized its performance. The visualizations provide insights into the decision-making process of the classifier.

## Contributing
Contributions are welcome! If you have any improvements or new features to suggest, feel free to open an issue or submit a pull request.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

Thank you for checking out the **DecisionTree-ML** repository! 

Happy coding! 🌟

---

![Iris Flower](images/iris_flower.png)
