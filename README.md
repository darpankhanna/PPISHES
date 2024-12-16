# PPISHES: An Enhanced Physicochemical Approach For Predicting Protein Interaction Sites Using Graph Neural Networks

Accurate prediction of protein interaction sites is key to understanding the underlying mechanisms of many biological processes. The current state-of-the-art method for site prediction, Residual Graph Convolutional Network for Protein-Protein Interaction Site Prediction (RGCNPPIS), is top-ranked by leveraging sequence features and incorporating spatial neighborhood information; however, there is still room for improvement in both accuracy and performance. RGCNPPIS captures local and global structural, evolutionary, and sequence-based features; however, it overlooks physicochemical properties important for protein interactions and struggles with feature redundancy, which limits its overall performance. 

By addressing these gaps, we aim to enhance the predictive power of RGCNPPIS and introduce new feature sets that improve overall model performance. We propose an enhanced model, PPISHES (Prediction of Protein Interactions based on Solvent Accessible Surface Area, Hydrogen-Bonding Propensity, and Electrostatic Potential Sites), which is built upon incorporating three critical physicochemical features—electrostatic potential, hydrogen-bonding propensity, and solvent-accessible-surface-area—to enrich the feature representation of protein structure thereby improving site prediction for both obligate and non-obligate complexes. To enhance interpretability and feature selection, we use feature ablation analysis, systematically masking individual features and identifying the most important features of the model. 

We evaluated PPISHES on widely recognized benchmark datasets, achieving a substantial improvement in the Area Under the Precision-Recall Curve, with increases of up to 42.8\%. PPISHES was also evaluated on key metrics like accuracy, precision, recall, area under the curve, and Matthews correlation coefficient), confirming its superior overall performance and surpassing current state-of-the-art.


## System Requirements

To run PPISHES, you need the following dependencies:

- **Python** 3.10.13
- **NumPy** 1.26.4
- **Pandas** 1.1.0
- **PyTorch** 1.12.1 (GPU required)
- **Scikit-learn** 1.4.2

## Dataset

Before running the code, please follow these steps:

1. Unzip the compressed files located in the `Feature` folder.
2. Place the files `distance_map(part1).rar`, `distance_map(part2).rar`, and `distance_map(part3).rar` into a folder named `distance_map`.

## Usage

To train or evaluate the model, use the following commands:

- **Training the Model:**
  ```bash
  python train.py
  ```

- **Evaluating the Model:**
  ```bash
  python test.py
  ```

## Citation

If you find this work useful in your research, please cite our paper:

```

```

---
