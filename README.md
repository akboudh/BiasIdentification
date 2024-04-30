<h1>Data Science: Bias Identification and Mitigation</h1>

<h2>Description</h2>

This project investigates bias identification and mitigation in machine learning models using the Adult Census Income dataset from the UCI Machine Learning Repository. The goal is to predict whether an individual's income is above or below $50,000 based on various demographic features, with a particular focus on gender as the protected variable.

<h2>Dataset</h2>

- **Dataset**: [Adult Census Income dataset](https://archive.ics.uci.edu/ml/datasets/adult) from the UCI Machine Learning Repository.

<h2>Methods Used</h2>

- Two machine learning models were employed:
  1. Decision Forest Model
  2. Neural Network Model

- The dataset was divided into training and test sets using stratified sampling to ensure similar distribution of the protected variable across subsets.

<h2>Results</h2>

### Overall Test Set Results:

- **Decision Forest Model**:
  - Overall Accuracy: 85.69%
  - Male Accuracy: 84.18%
  - Female Accuracy: 87.09%

- **Neural Network Model**:
  - Overall Accuracy: 85.25%
  - Male Accuracy: 83.46%
  - Female Accuracy: 86.06%

### Test Set Results Partitioned by Gender:

| Model              | Male   | Female |
|--------------------|--------|--------|
| Decision Forest    | 84.18% | 87.09% |
| Neural Network    | 83.46% | 86.06% |

### Bias Mitigation Strategy:

- Attempted to mitigate bias by sampling differently from the training sets based on the protected variable (gender).
- Increased the number of samples for males in the training set by 50%.

### Test Set Results after Bias Mitigation:

| Model              | Male   | Female |
|--------------------|--------|--------|
| Decision Forest    | 84.20% | 87.09% |
| Neural Network    | 83.39% | 86.06% |

<h2>Comments and Conclusions</h2>

- Identified potential bias in machine learning models based on gender.
- Proposed bias mitigation strategy somewhat reduced bias but did not eliminate it entirely.
- Emphasized the importance of continual efforts to remove bias in machine learning models to promote fairness and equity.

<h2>References</h2>

1. [Fairness through Awareness](https://dl.acm.org/doi/10.1145/2090236.2090255)
2. [Certifying and Removing Disparate Impact](https://dl.acm.org/doi/10.1145/2783258.2783311)
3. [Data Preprocessing Techniques for Classification without Discrimination](https://link.springer.com/article/10.1007/s10115-011-0463-8)
4. [Inherent Trade-offs in the Fair Determination of Risk Scores](https://dl.acm.org/doi/10.1145/2840728.2840734)
5. [A Survey on Measuring Indirect Discrimination in Machine Learning](https://arxiv.org/abs/1511.00148)
6. [Learning Fair Representations](https://dl.acm.org/doi/10.5555/3042817.3043059)

