# Neural Style Transfer

## Project Description

This project implements a Neural Style Transfer system using a pretrained VGG19 network to generate artistic images while preserving the structural content of the original image. The system extracts content and style representations from different convolutional layers and optimizes a generated image by minimizing content and style losses.

Beyond the baseline implementation, multiple optimization techniques and architectural improvements were explored to analyze their impact on image quality, convergence speed, and training stability.

---

## Technologies Used

- Python
- PyTorch
- TorchVision
- NumPy
- Matplotlib
- PIL (Python Imaging Library)

---

## Deep Learning Model

- Pretrained VGG19 (Transfer Learning)

---

## Optimization Techniques

- Adam Optimizer
- LBFGS Optimizer
- Learning Rate Scheduler (StepLR)
- Total Variation (TV) Loss
- Weighted Style Layers
- Multi-Style Blending
- Hyperparameter Tuning
- Content Layer Selection
- Learning Rate Adjustment

---

## Methodology

The project follows the following pipeline:

1. Load content and style images.
2. Preprocess images using resizing, normalization, and tensor conversion.
3. Extract content and style features using pretrained VGG19.
4. Compute Gram Matrices for style representation.
5. Optimize the generated image by minimizing:
   - Content Loss
   - Style Loss
   - Total Variation Loss (when enabled)
6. Compare multiple optimization strategies and model configurations.
7. Evaluate generated images using convergence analysis, loss curves, and qualitative visual comparison.

---

## Results

- Successfully generated high-quality artistic images while preserving the original scene structure.
- LBFGS achieved the fastest convergence and the lowest final loss.
- Weighted Style Layers produced the best visual balance between artistic style and content preservation.
- Total Variation Loss effectively reduced image noise and artifacts.
- Multi-Style blending generated visually diverse artistic outputs.
- Multiple optimization strategies were systematically compared to identify the most effective configuration.

---

## Tools

- Google Colab
- Jupyter Notebook
- Kaggle Dataset

---

## Project Structure

```
├── Dataset
├── Image Preprocessing
├── VGG19 Feature Extraction
├── Neural Style Transfer
├── Optimization
├── Evaluation
├── Generated Results
└── Final Report
```

---

## My Contribution

My primary contribution to this project focused on the **Optimization** stage. I implemented and evaluated different optimization strategies, including optimizer tuning, learning rate adjustments, and optimization-related experiments to improve convergence behavior, training stability, and the overall quality of the generated stylized images.

---

## Note

This project was developed as part of a university group project for the **Deep Learning** course at Umm Al-Qura University.
