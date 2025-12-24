# DL-Exam-Task12-Nargiz-Abiyeva

# Task 12: Fashion-MNIST with Data Augmentation

**Student:** Nargiz Abiyeva  
**ID:** nabiyeva.52969  
**Seed:** 20240312

## Presentation
[View Presentation Slides](https://docs.google.com/presentation/d/1sHAuPO_l7eVp35eiD1pfb9GNc3_WDNoj4Fz3FYv-ufI/edit?usp=drive_link)

## Dataset
- **Name:** Fashion-MNIST
- **Classes:** 10
- **Training samples:** 60,000
- **Test samples:** 10,000

## Model Architecture
- **Type:** Convolutional Neural Network (CNN)
- **Convolutional layers:** 2
- **Fully connected layers:** 2
- **Total parameters:** 421,642

## Training Comparison

### Version 1 No Augmentation
- **Learning rate:** 0.001
- **Batch size:** 64
- **Optimizer:** Adam
- **Test accuracy:** 91.86%

### Version 2 With Augmentation
- **Learning rate:** 0.001
- **Batch size:** 64
- **Optimizer:** Adam
- **Test accuracy:** 90.98%

### Best Result
- **Best version:** Version 1
- **Final test accuracy:** 91.86%
- **Target accuracy:** 90%
- **Status:** ✓ Achieved

## Analysis
- **Best performing class:** Bag (98.90%)
- **Worst performing class:** Shirt (78.70%)
- **Key observations:**  
  The model without augmentation achieved higher accuracy due to faster convergence with a larger learning rate within the fixed 10-epoch limit.  
  The augmented model improved robustness but converged more slowly, resulting in slightly lower accuracy under the same training budget.

## Files
- `notebook.ipynb`: Complete implementation with both training runs
- `results/training_comparison.png`: Comparison of Version 1 vs Version 2
- `results/confusion_matrix.png`: Confusion matrix from best model
- `results/predictions.png`: Sample predictions
