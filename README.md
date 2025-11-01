# Medical Disease Prediction using Machine Learning

## Project Overview

This project is a symptom-based disease prediction system that utilizes three different supervised Machine Learning algorithms: Decision Tree, Random Forest, and Gaussian Naive Bayes. The system provides predictions through a simple Graphical User Interface (GUI), allowing users to select symptoms and compare the output from each model.

Key Features:
- **Multi-Model Prediction**: Predicts disease simultaneously using three different classification algorithms for robust result comparison.

- **Tkinter GUI**: Provides a user-friendly interface for inputting up to 5 symptoms via dropdown menus.

- **Performance Visualization**: The "Show Graphs" feature displays the model accuracy comparison (on the validation set) and a disease distribution pie chart using matplotlib.

- **Modular Architecture**: The codebase is structured into three self-contained Jupyter Notebooks (.ipynb) for clean data handling, prediction logic, and GUI implementation.

---

## Tech Stack & Algorithms

- **Language**:	Python - Core programming language.
- **Framework (GUI)**: Tkinter (and ttk) - Creating the desktop application interface.
- **ML Libraries**:	Scikit-learn - Implementing the classification algorithms.
- **Data Handling**: Pandas, Numpy	- Data loading, preprocessing, and vector creation.
- **Visualization**: Matplotlib -	Generating model performance and data distribution graphs.
- **Models Used**: 1. Decision Tree Classifier, 2. Random Forest Classifier, 3. Gaussian Naive Bayes.

---

## Getting Started

1. Clone the repository:
   ```bash
   git clone https://github.com/GaganMS004/Medical-Disease-Prediction-Using-Machine-Learning.git
   ```
2. Install Python libraries:
   ```bash
   pip install pandas numpy scikit-learn matplotlib jupyter import-ipynb
   ```
3. Data Setup: Ensure you have your training and testing data files named Training_Data.csv and Testing_Data.csv in the project's root directory.

---

## How to Run the Application

The project is structured across three Jupyter Notebooks that must be run in sequence.

**1. Execute data_setup.ipynb**:
- This notebook performs Data Loading, Preprocessing (mapping disease names to numerical indices), and Model Training for the Decision Tree, Random Forest, and Naive Bayes classifiers.

**2. Execute predictor_model.ipynb**:
- This notebook defines the core utility functions:
- predict_disease(model, input_symptoms): Converts the list of symptoms into the required one-hot encoded input vector and returns the predicted disease name.
- show_graphs(): Calculates model accuracies and generates comparison plots.

**3. Execute gui_app.ipynb**
- This notebook sets up the Tkinter GUI. Running the code cell will launch the application window.

---

## Using the GUI
Once the window opens:
1. Select up to 5 symptoms from the dropdown menus.
2. Click the Prediction Buttons (Decision Tree, Random Forest, or Naive Bayes) to see the predicted disease in the corresponding white text box.
3. Click "Show Graphs" to view the accuracy comparison and data statistics.
4. Click "Reset" to clear the selected symptoms and prediction boxes.

---

## Future Enhancements
- Integrate a web framework (like Flask or Streamlit) for online access.
- Add a feature to suggest a specialist or nearest hospital based on the predicted disease.
- Implement a cross-validation strategy during training for more robust model evaluation.
- Incorporate feature importance analysis (e.g., from Random Forest) to highlight the most critical symptoms.
