**Peptide–HLA Binding Toy Classifier**

This project is a small, end-to-end machine-learning example that predicts whether a 9-mer peptide binds to the human HLA-A*02:01 allele.
It is designed for learning and demonstration, not for clinical use.

**Key Features**

Dataset: 60 peptides (30 binders, 30 non-binders) generated for educational purposes.

Encoding: Each amino acid in a peptide is one-hot encoded at every position, including a padding symbol to handle sequences shorter or longer than nine residues.

Models: Two supervised classifiers—Logistic Regression and Random Forest—are trained and compared.

Evaluation: Accuracy, ROC-AUC, precision, recall, F1-score, and a confusion matrix are reported.

**Workflow**

Data Preparation – Peptide sequences are padded or trimmed to nine residues, then converted to position-specific one-hot feature vectors.

Training & Testing – Data is split into training and test sets (75/25).

Modeling – Logistic Regression and Random Forest classifiers are fit to the training data.

Performance Analysis – Metrics and a confusion matrix are generated to visualize prediction quality.

**Results**

On the small test set, the Random Forest model achieved about 80 % accuracy with a ROC-AUC of 0.79, showing balanced precision and recall for both binders and non-binders.
These numbers are for demonstration only and highlight how limited data affects statistical confidence.

**Purpose**

The notebook illustrates how to:

Transform biological sequence data into machine-learning features.

Train, evaluate, and compare multiple models.

Visualize classifier performance with clear metrics and plots.

This repository provides a quick, reproducible example for students or researchers who want to learn the basics of bioinformatics-oriented machine learning without needing a large dataset or complex infrastructure.
