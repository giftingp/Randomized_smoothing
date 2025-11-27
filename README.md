We train a very simple convolutional neural network on MNIST and assess the standard accuracy. Additionally, in order to provide certifiable robust adversarial perturbations we also implement randomized smoothing by Cohen et al [1].

## Results

### Training Progress
| Epoch | Loss | Test Accuracy |
|-------|------|---------------|
| 1/3 | 0.255 | 97.6% |
| 2/3 | 0.063 | 98.2% |
| 3/3 | 0.045 | **98.9%** |

### Final Performance
| Model | Accuracy | Notes |
|-------|----------|-------|
| Base Classifier (f) | **98.9%** | - |
| Smoothed Classifier (g) | **97.6%** | 100 majority votes |

### Certified Robustness
| Radius | Certified Accuracy |
|--------|-------------------|
| 0.0 | 97.54% |
| 0.5 | 80.3% |
| 1.0 | 80.3% |

# References

[1] Cohen, J., Rosenfeld, E., & Kolter, Z. (2019). Certified Adversarial Robustness via Randomized Smoothing. In *International Conference on Machine Learning* (ICML).
