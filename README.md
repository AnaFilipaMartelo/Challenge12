# Credit Risk Analysis with Imbalanced Classes

This project focuses on building a predictive model to assess credit risk in peer-to-peer lending services. The dataset contains historical lending activity, with healthy loans far outnumbering risky loans, resulting in an imbalanced class distribution. Leveraging the imbalanced-learn library, we'll use a logistic regression model and compare two datasets: the original and a resampled version. Through balanced accuracy, confusion matrices, and classification reports, we'll evaluate the model's performance in identifying creditworthy borrowers, providing valuable insights for financial decision-making.

---

## Technologies

The technologies used in this project include:

   * Python 3.7
   * JupyterLab 3.4.4
   * Pandas 1.3.5
   * Scikit-Learn 1.0.2 
   * Imbalanced-Learn 0.11.0
   * PyDotPlus 2.0.2
---

## Installation Guide

Open your terminal and run the command:

```python
  pip install -r requirements.txt
```

---

## Usage

Clone the repository and Launch Jupyter Notebook by executing the following command in your terminal:

```python
  jupyter lab
```

In the Jupyter Notebook interface, navigate to the project directory and open the credit_risk_resampling.ipynb file.

Run each cell in the notebook sequentially to generate the two logistic regression models and compare the two models. It will calculate  the balanced accuracy score, generate a confusion matrix, and generate a classification report for both models.

Read the comments and text documentation within the notebook to understand the analysis and findings.

---


## Contributors

* Ana Martelo (anafilipamartelo@gmail.com)

---

## License

MIT
