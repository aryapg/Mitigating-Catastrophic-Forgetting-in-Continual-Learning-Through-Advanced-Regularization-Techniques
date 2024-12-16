# Mitigating-Catastrophic-Forgetting-in-Continual-Learning-Through-Advanced-Regularization-Techniques

# Continual Learning with PyTorch

This repository contains an implementation of **Continual Learning** experiments using PyTorch. The primary focus is on mitigating **catastrophic forgetting** in neural networks through various regularization techniques.

## Features

- **Implementation**:
  - Custom neural network models using PyTorch.
  - Experiments with multiple continual learning methods, including:
    - **Elastic Weight Consolidation (EWC)**.
    - **Synaptic Intelligence (SI)**.
    - **L1 and L2 Regularization**.
  - Comprehensive support for tracking model performance across tasks.
- **Dependencies**:
  - Libraries: `torch`, `torchvision`, `matplotlib`, `tqdm`.
  - GPU support via CUDA for efficient computation.
- **Visualization**:
  - Loss and accuracy trends across tasks.
  - Plots to compare the effectiveness of different regularization methods.

## Experiment Details

- **Tasks**: The notebook runs experiments across `3` distinct tasks, demonstrating the application and effectiveness of regularization in overcoming catastrophic forgetting.
- **Methods Explored**:
  - **Elastic Weight Consolidation (EWC)**: Penalizes changes to parameters critical to previously learned tasks.
  - **Synaptic Intelligence (SI)**: Tracks parameter importance during training and minimizes changes to critical weights.
  - **L1/L2 Regularization**: Penalizes large parameter values to encourage generalization and prevent overfitting.
- **Hyperparameters**:
  - Epochs: `150`
  - Learning Rate: `0.0001`
  - Batch Size: `128`
  - Hidden Layer Size: `512`

## How to Use

1. Install the required dependencies:
   ```bash
   pip install torch torchvision torchsummary matplotlib tqdm
2. Open and run the Jupyter Notebook to train and evaluate the models with different regularization techniques.

## Results
- Compares the effectiveness of EWC, SI, and L1/L2 regularization in mitigating catastrophic forgetting.
- Includes visualizations to analyze the model's performance on each task.
- Provides insights into the trade-offs and benefits of each regularization method.

## Acknowledgments
This project explores techniques to overcome catastrophic forgetting in neural networks as part of research in Continual Learning. The methods implemented are inspired by widely studied approaches such as EWC and Synaptic Intelligence, alongside traditional L1/L2 Regularization.









