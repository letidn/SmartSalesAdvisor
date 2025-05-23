# SmartSalesAdvisor

**An intelligent decision-support system for microentrepreneurs, based on Business Economics and Decision Tree inference.**

## Description

SmartSalesAdvisor is a Java-based tool designed to support microentrepreneurs with limited financial knowledge in evaluating their business conditions and receiving scenario-based recommendations. The system uses theoretical foundations from Business Economics and a rule-based decision tree to diagnose conditions and propose strategic actions.

## Features

- Break-even analysis using business logic
- Inference engine based on deterministic decision tree
- Generation of actionable recommendations (alerts, suggestions, confirmations)
- Designed for service-oriented microenterprises
- High model accuracy (0.9978 with synthetic data)

## Requirements

- Java 11 or higher
- NetBeans or IntelliJ (recommended for execution)
- Python 3.10+ (for validation script)
- scikit-learn, pandas, numpy

## Installation

1. Clone or download the repository:
   ```bash
   git clone https://github.com/yourusername/SmartSalesAdvisor.git
   ```
2. Open the Java project in your preferred IDE and run `sistemaexperto.java`.

## Usage

1. The user answers a guided set of business-related questions.
2. The system evaluates inputs using a decision tree derived from inference rules.
3. A final message (M1–M11) is displayed, along with recommendations.

Example output:
```
Message: M4 - "The company needs to conduct a price review."
```

## Folder structure

- `/src` – Java source files  
- `sistemaexperto.java` – Main application entry point  
- `accuracy_calculation2_ing.py` – Python script for decision tree validation  
- `/data` – Synthetic dataset (generated in Python)  
- `/figures` – Diagram of decision tree and use case

## Reproducibility

To reproduce the accuracy results of the decision tree model:

1. Run the script `accuracy_calculation2_ing.py`, which:
   - Generates a synthetic dataset based on the system’s inference rules
   - Trains a decision tree classifier
   - Evaluates the model using accuracy, confusion matrix, precision, recall, and F1-score
   - Performs 10-fold cross-validation for robustness

Example output includes:
```
Accuracy: 0.9978  
Cross-validation scores: [0.9967, 1.0000, ..., 1.0000]  
```

This confirms the reliability of the model's structure before deployment in the main application.

To interact with the full decision-support system, execute the main program `sistemaexperto.java`, which provides a guided interface for microentrepreneurs and outputs diagnostic messages (M1–M11) with recommendations.

## License

MIT License

## Authors

- Leticia Dávila Nicanor  
- Juan Carlos Baltazar Escalona  
- Víctor Landassuri Moreno  
- Asdrubal López Chau
- Alejandro Moreno Martínez

## How to cite

If you use SmartSalesAdvisor in your research, please cite:

> Dávila-Nicanor, L., Baltazar Escalona, J.C., Landassuri Moreno, V., López Chau, A., & Moreno Martínez, A. (2024). SmartSalesAdvisor: A Decision-Support Tool for Microentrepreneurs Using Business Economics and Inference Trees.
