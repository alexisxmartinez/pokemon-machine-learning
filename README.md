# Pokémon Type Prediction: A Machine Learning Project

## 1. Introduction

This project explores the Pokémon dataset from Kaggle to build a robust multi-class classification model capable of predicting a Pokémon's primary type (`Type_1`) based on its various characteristics. We will build a full end-to-end data science project, starting from data loading, cleaning, feature engineering, and then moving onto a model building and evaluation step.

This report enhances previous work on the dataset by implementing several state-of-the-art tree based algorithms, hyperparameter tunning, more complex feature engineering techniques, and analyzing feature importances, and by focusing on interpretability.

## 2. Project Goals

*   **Primary Objective:** To accurately predict a Pokémon's primary type (`Type_1`) using machine learning.
*   **Enhancements:** This project aims to improve existing models using:
    *   Advanced feature engineering techniques.
    *   A robust data preprocessing technique with Pandas, and exploration of different tree based and neural network architectures for classification models.
    *  Hyperparameter tunning of the final selected model to improve performance.
    *   Interpretability analysis, using feature importances.
    *   A discussion about the data, the decisions that were taken and comparing it with previous work.
* **End to End Project:** To create a reproducible, well documented project that shows your skills in all the phases of a data science project.

## 3. Dataset

*   **Source:** The dataset was obtained from Kaggle ([https://www.kaggle.com/alopez247/pokemon](https://www.kaggle.com/alopez247/pokemon)).
*   **Description:** It contains information about 721 Pokémon from the first six generations, including their names, types, base stats, and other characteristics.
*  **Additional Information:** The original author of this dataset provides a detailed report on his analysis, and that was used as a starting point for this project.
  
## 4. Technical Documentation Standards

This section outlines the standards followed in this technical document to ensure clarity, reproducibility, and a professional presentation.

### 4.1. Document Structure

*   **Clear Sections:** The document is divided into logical sections (e.g., Introduction, Data Cleaning, Modeling, etc.), using clear titles, headers and sub-headers.
*   **Sequential Flow:** Information is presented in a logical order, following the typical data science workflow.
*   **Context:** Each section begins with a brief overview of what is covered.
*   **Justifications:** Decisions are backed with an explanation of why each step is important, and when applicable, the theoretical background of that approach is also provided.

### 4.2. Code Documentation

*   **Comments:** Code is well-commented to explain what each part does, especially complex operations or logical steps.
*   **Meaningful Variable Names:** The code uses clear, descriptive variable names.
*   **Modularity:** The code is written to be modular, by grouping operations in functions, and using smaller blocks for different stages of the data process.
*   **Reproducibility:** The code uses a random seed to make sure that every step is reproducible.

### 4.3. Reporting

*  **Results and Metrics:** When describing model results, you should include common metrics (like accuracy, precision, recall, F1-score), and use visualisations when possible.
*   **Interpretability:** Explain your decisions and how they relate with the final output, as well as what the results mean.
*   **Comparisons:** You should explicitly compare your work with previous work, showcasing how you are improving on it.
*   **Insights:** Communicate data-driven insights and what you have learned.
*   **Limitations:** Acknowledge any limitations or issues that you may have found.
*  **Visualizations:** The report should use visualizations to highlight results, and should be used to improve the understanding of the process.

### 4.4. Version Control

*   **Git:** This project uses Git for version control.
*   **Commits:** Changes are saved with descriptive commit messages.
*   **Workflow:** You should perform commits in small logical changes, and should push them to the main branch of your repository.

## 5. Project Workflow

1.  **Data Loading:** Load the CSV dataset using pandas.
2.  **Data Cleaning:**
    *   Remove extra spaces and set lowercase on the categorical features.
    *   Remove duplicate rows.
3.  **Feature Engineering:**
    *   Encode categorical features using Label Encoding.
    *   Scale numerical features using StandardScaler.
    *   Create a combination of `Type_1` and `Type_2` features.
4.  **Data Splitting:**
    *   Divide the data into training, testing, and validation sets, using a stratified sampling for training, and a non-stratified sampling for the rest.
5. **Impute Missing Values:**
    *  Fill any NaN value using the mean of the column.
6.  **Modeling:**
    *   Train several models, including Random Forest, XGBoost, LightGBM, Catboost, and a basic Neural Network.
    *   Evaluate each model using the test dataset, and document the results.
    *   Select the best performing model for further analysis.
    *   Use Hyperparameter tunning techniques to improve the model that you have selected.
7.  **Feature Importance and Analysis:**
    *   Use the chosen model to analyze the feature importances.
    *   Use a confusion matrix to study the errors made by your model.
8.  **Documentation:**
    *   Document all your decisions, your process, and your results, and explain what you have done differently from the previous report.
9.   **Report and Visualization:** The results should be properly documented in this `README.md` file, and it should include code, data analysis, and images if they are useful.
10. **Presentation:** This report should be used to create your presentation, following the same structure.

## 6. Deliverables
The project will deliver:

1.  **A Cleaned and Processed Dataset:** Ready for use with machine learning models, and documented in this `README.md` file.
2.  **A Trained Machine Learning Model:** Trained with the techniques described here and with all the steps followed documented.
3.  **Model Evaluation Metrics:** A complete report of the performance of different machine learning models.
4.  **Feature Importance Results:** A list of the most important features for the model and how were they obtained.
5.  **Code Repository:** A well organized and documented code repository hosted on GitHub, with a clear log of your commits.
6.  **Presentation:** A clear presentation of your project.

## 7. License
(Optional) If you want to add any type of license