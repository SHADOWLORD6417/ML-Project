# Instagram Profile Real vs Fake Predictor

This project aims to determine whether an Instagram profile is real or fake based on a dataset containing specific attributes of the profiles. The project is implemented in a Jupyter Notebook (`.ipynb`) format and employs various machine learning models for prediction and comparison.

## Dataset Attributes

The dataset includes the following features for each Instagram profile:

- **profile pic**: Indicates if the profile has a profile picture.
- **nums/length username**: Ratio of numbers to the total length of the username.
- **fullname words**: Number of words in the full name.
- **nums/length fullname**: Ratio of numbers to the total length of the full name.
- **name==username**: Boolean indicating if the full name matches the username.
- **description length**: Length of the profile description.
- **external URL**: Indicates if the profile has an external URL.
- **private**: Indicates if the profile is private.
- **#posts**: Number of posts by the profile.
- **#followers**: Number of followers.
- **#follows**: Number of accounts the profile follows.

## Workflow

1. **Data Preparation**:
   - The dataset is split into training (80%) and testing (20%) subsets.
   - Preprocessing techniques are applied to ensure the data is ready for model training.

2. **Model Implementation**:
   - **K-Nearest Neighbors (KNN)**: Used to classify profiles based on feature similarity.
   - **Decision Tree**: A tree-based approach to classify profiles.
   - **Random Forest**: An ensemble method combining multiple decision trees for improved accuracy.
   - **Manual Gradient Boosting**: Custom implementation of boosting to improve Decision Tree performance.
   - **Simple Support Vector Machine (SVM)**: Used to plot data and classify profiles.

3. **Evaluation**:
   - Each model's performance is evaluated on the testing dataset.
   - Accuracy scores are compared to identify the best-performing model.

4. **User Input for Prediction**:
   - A form accepts user input for all profile attributes.
   - The entered data is used to predict the likelihood of a profile being real or fake using the trained models: Random Forest, Simple SVM, Decision Tree, and KNN.

## Key Features

- Comparison of different machine learning models for classification accuracy.
- Visualization of data and decision boundaries using SVM.
- Real-time prediction based on user input.

## Results

The project provides insights into the performance of various machine learning models in detecting fake Instagram profiles and highlights the most effective model(s) for this task.

## Prerequisites

- Python 3.x
- Jupyter Notebook
- Required Python libraries: `pandas`, `numpy`, `scikit-learn`, `matplotlib`, and `seaborn`.

## How to Run

1. Clone the repository and navigate to the project directory.
2. Install the necessary dependencies using `pip install -r requirements.txt`.
3. Open the `.ipynb` file in Jupyter Notebook.
4. Run all cells sequentially to execute the project workflow.

## Future Enhancements

- Expand the dataset with additional features to improve model accuracy.
- Deploy the solution as a web application for broader accessibility.
- Experiment with advanced models such as deep learning techniques for improved predictions. 

Feel free to contribute or share your feedback!
