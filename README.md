# Predictive-Analysis-with-Decision-Trees

🫀 Predictive Analysis with Decision Trees
📌 Project Overview

This project focuses on building a predictive analytics model using Decision Trees to classify the presence of heart disease in patients. Decision Trees are intuitive and powerful supervised learning algorithms but are prone to overfitting. To address this, the project implements both pre-pruning and post-pruning techniques to improve model generalization.

The project is implemented using Python and scikit-learn in Google Colab, with clear visualizations and feature importance analysis to enhance interpretability.

🎯 Objectives

Implement a Decision Tree Classifier for heart disease prediction

Understand and apply Gini Index and Entropy for node splitting

Demonstrate overfitting using an unpruned decision tree

Apply pre-pruning and post-pruning (cost complexity pruning) techniques

Visualize decision tree structures

Analyze feature importance based on tree splits

📊 Dataset Description

Dataset Name: Heart Disease Cleveland Dataset

Source: Kaggle (UCI Heart Disease dataset)

Records: 303 patients

Features: 13 medical attributes (age, cholesterol, chest pain type, etc.)

Target Variable:

0 → No Heart Disease

1 → Presence of Heart Disease

The dataset contains no missing values, making it suitable for direct modeling.

⚙️ Methodology
1. Data Preprocessing

Loaded dataset using Pandas

Identified categorical features

Applied one-hot encoding

Split data into training (70%) and testing (30%) sets

2. Decision Tree Construction

Built an initial unpruned Decision Tree to observe overfitting

Evaluated using:

Accuracy

Precision

Recall

F1-score

Confusion Matrix

3. Pre-Pruning

Controlled tree growth using:

max_depth

min_samples_split

min_samples_leaf

Reduced model complexity to improve generalization

4. Post-Pruning

Applied Cost Complexity Pruning (ccp_alpha)

Trained multiple trees for different alpha values

Selected optimal alpha based on test accuracy

5. Visualization

Visualized:

Unpruned Decision Tree

Post-pruned Decision Tree

Used plot_tree from scikit-learn for interpretability

6. Feature Importance

Extracted feature importance from the post-pruned model

Identified top contributing medical features affecting prediction

📈 Results Summary
Model Type	Accuracy
Unpruned Decision Tree	~74.7%
Pre-Pruned Decision Tree	~69.2%
Post-Pruned Decision Tree	~78.0%

🔹 Post-pruning produced the best generalization performance
🔹 Chest pain type (cp), thalassemia (thal), and exercise-induced angina (exang) were the most influential features

🛠️ Technologies Used

Python

Google Colab

Pandas, NumPy

Scikit-learn

Matplotlib

▶️ How to Run the Project
Option 1: Run in Google Colab (Recommended)

Open Google Colab

Upload the notebook file

Upload the dataset file:

Heart_disease_cleveland_new.csv


Run all cells sequentially

Option 2: Run Locally
pip install pandas numpy matplotlib scikit-learn


Then run the notebook using Jupyter Notebook or Jupyter Lab.

📂 Project Structure
├── Predictive_Analysis_with_Decision_Trees.ipynb
├── Heart_disease_cleveland_new.csv
├── unpruned_decision_tree.png
├── post_pruned_decision_tree.png
├── README.md

✅ Conclusion

This project demonstrates how Decision Trees can be effectively used for predictive analysis while addressing overfitting through pruning techniques. The combination of visualization, pruning, and feature importance analysis makes the model both accurate and interpretable, which is crucial in healthcare-related applications.

👤 Author

Mukesh

