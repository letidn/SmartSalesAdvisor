# SmartSalesAdvisor

**An intelligent decision-support system for microentrepreneurs, based on Business Economics and Decision Tree inference.**

## Description

SmartSalesAdvisor is a Java-based decision-support tool aimed at microentrepreneurs with limited financial literacy. The system evaluates business conditions and provides scenario-driven recommendations using principles from Business Economics and a rule-based decision tree model.

## Features

- Break-even point analysis grounded in economic theory  
- Inference engine based on a deterministic decision tree  
- Generation of actionable recommendations (alerts, suggestions, confirmations)  
- Targeted at service-oriented microenterprises  
- High accuracy (0.9978 with synthetic data)

## Requirements

- Java 11 or higher  
- Java™ SE Runtime Environment (build 23.0.2+7-58)  
- Python 3.10+ (for model validation)  
- Python libraries: scikit-learn, pandas, numpy

## Installation

Clone the repository:

```bash
git clone https://github.com/yourusername/SmartSalesAdvisor.git
```

Open the project in your preferred IDE and run `SmartSalesAdvisor.java`.

## Usage

1. The user answers a series of guided questions related to their business.  
2. The system evaluates the input using a decision tree derived from encoded business rules.  
3. The system displays a message (M1–M11) along with tailored recommendations.

Example output:

```text
Message: M4 – "The company needs to conduct a price review."
```

## Folder Structure

```
/src                      # Java source files  
SmartSalesAdvisor.java   # Main application file   
accuracy_calculation2_ing.py # Python validation script  
/data                    # Synthetic dataset  
/figures                 # Decision tree and use case diagrams  
```

## Reproducibility

To reproduce the model’s accuracy:

1. Run the script `accuracy_calculation2_ing.py`, which:  
   - Generates a synthetic dataset based on inference rules  
   - Trains a decision tree classifier  
   - Evaluates the model using metrics (accuracy, precision, recall, F1-score)  
   - Performs 10-fold cross-validation

Example output:

```yaml
Accuracy: 0.9978  
Cross-validation scores: [0.9967, 1.0000, ..., 1.0000]
```

This confirms the consistency and robustness of the decision logic before system deployment.

## License

MIT License

## Authors

- Dra. Leticia Dávila Nicanor – Project Lead  
- Dr. Asdrubal López Chau  
- Dr. Víctor Landassuri Moreno  
- Mtro. Alejandro Moreno Martínez  
- Dra. Marisela Quintana López  
- Dr. Saturnino Job Morales Escobar

## How to cite

If you use SmartSalesAdvisor in your research, please cite:

> Dávila-Nicanor, L., Baltazar Escalona, J.C., Landassuri Moreno, V., López Chau, A., & Moreno Martínez, A. (2024). SmartSalesAdvisor: A Decision-Support Tool for Microentrepreneurs Using Business Economics and Inference Trees.
