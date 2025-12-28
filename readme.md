
# ResNet-34 

Re-implemented ResNet-34 from scratch with PyTorch
and re-training it on CIFAR-10 dataset (multiclass classification)
 
## Workflow

1. Data preprocessing
- Applied RandomRotation, RandomHorizontalFlip to data
- Applied StratifiedShuffleSplit for train/valid/test sets

2. Training
- Optimizer: NAdam
- Metric: Accuracy
- Loss Fn: CrossEntropyLoss
- Did Regular Cross Validation,including learning rate scheduler,warm up scheduler and early call back function. Used Optuna (with pruning) for hyperparameter tuning of learning rate 

3. Results
- 90% Accuracy on test set

<img width="829" height="328" alt="image" src="https://github.com/user-attachments/assets/95047cfc-61bb-4058-a66e-1f95fdf8cabd" />



