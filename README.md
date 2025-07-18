# Income Prediction Project

## Overview
This project uses a Random Forest Classifier to predict whether an individual's income exceeds $50K per year based on demographic and employment data. The dataset is analyzed and processed using Python, with key libraries including Pandas, Seaborn, Matplotlib, and Scikit-learn. The project involves data exploration, preprocessing, and model training with hyperparameter tuning using GridSearchCV.

## Dataset
The dataset (`income.csv`) contains features such as age, workclass, education, occupation, gender, capital gains/losses, hours worked per week, and native country, with the target variable being income (`<=50K` or `>50K`). The dataset has 48,842 rows and 15 columns.

## Features
- **Data Exploration**: Analyzes distributions of categorical variables like education, workclass, and occupation.
- **Data Preprocessing**: Converts categorical variables into dummy variables for model compatibility.
- **Model Training**: Uses a Random Forest Classifier with hyperparameter tuning via GridSearchCV.
- **Feature Importance**: Identifies key features influencing income prediction, such as age, capital-gain, and educational-num.

## Installation
To run this project, ensure you have Python 3.10+ installed. Follow these steps:

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/your-repo-name.git
   cd your-repo-name
   ```

2. **Install Dependencies**:
   Create a virtual environment and install the required packages:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   pip install -r requirements.txt
   ```

3. **Requirements**:
   The following Python libraries are required:
   - pandas
   - seaborn
   - matplotlib
   - scikit-learn

   Install them using:
   ```bash
   pip install pandas seaborn matplotlib scikit-learn
   ```

## Usage
1. **Prepare the Dataset**:
   Ensure `income.csv` is in the project directory. The dataset should contain the columns as shown in the notebook (e.g., age, workclass, education, etc.).

2. **Run the Notebook**:
   Open the Jupyter notebook (`main.ipynb`) in JupyterLab or Jupyter Notebook:
   ```bash
   jupyter notebook main.ipynb
   ```
   Execute the cells sequentially to:
   - Load and explore the dataset
   - Preprocess the data (e.g., convert categorical variables to dummy variables)
   - Train the Random Forest model with GridSearchCV
   - Evaluate the model and view feature importance

3. **Model Details**:
   - The best model from GridSearchCV uses `max_depth=30`, `min_samples_split=4`, with a test accuracy of approximately 86.19%.
   - Feature importance is calculated to highlight the most influential features.

## Project Structure
```
your-repo-name/
├── income.csv           # Dataset file
├── main.ipynb           # Jupyter notebook with analysis and model training
├── requirements.txt     # Python dependencies
├── README.md            # This file
```

## Results
- **Model Performance**: The Random Forest Classifier achieves an accuracy of ~86.19% on the test set.
- **Key Features**:
  - `age`: 15.07%
  - `capital-gain`: 14.08%
  - `educational-num`: 12.75%
  - `hours-per-week`: 9.49%
  - `marital-status_Married-civ-spouse`: 8.30%

## Contributing
Contributions are welcome! Please fork the repository and submit a pull request with your changes. Ensure your code follows PEP 8 style guidelines and includes appropriate documentation.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contact
For questions or feedback, please open an issue on GitHub or contact [your-email@example.com].