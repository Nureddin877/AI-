# Task 3: CIFAR-10 Animals (4 Classes)

**Student:** Nuraddin Qasimov  
**ID:** 3  
**Seed:** 20240103  

## Presentation
[View Presentation Slides.(https://drive.google.com/file/d/1aKQGAqMrf05xZMDvl13if1D2mBMcBeja/view?usp=drivesdk)

## Dataset
- **Name:** CIFAR-10 filtered  
- **Classes:** 4 (cat, dog, horse, deer)  
- **Training samples:** 20,000 (approx.)  
- **Test samples:** 5,000 (approx.)  

## Model Architecture
- **Type:** CNN  
- **Convolutional layers:** 3 (32 → 64 → 128 filters)  
- **Fully connected layers:** 2 (128 units → 4 output)  
- **Total parameters:** ~1.2 million  

## Training Comparison

### Version 1
- **Learning rate:** 0.001  
- **Batch size:** 64  
- **Optimizer:** Adam  
- **Test accuracy:** 74.12%  

### Version 2
- **Learning rate:** 0.01  
- **Batch size:** 128  
- **Optimizer:** SGD with momentum 0.9  
- **Test accuracy:** 87.34%  

### Best Result
- **Best version:** Version 2  
- **Final test accuracy:** 87.34%  
- **Target accuracy:** 85%  
- **Status:** ✓ Achieved  

## Analysis
- **Best performing class:** horse  
- **Worst performing class:** cat  
- **Key observations:**  
  - Using SGD with momentum and a larger batch size improved generalization and convergence.  
  - Cat images were often confused with dog, likely due to similar textures and colors.  
  - Overall, the model achieved the target accuracy after 20 epochs.

