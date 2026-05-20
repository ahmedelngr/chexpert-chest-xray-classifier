# CheXpert Chest X-Ray Classifier

Multi-label chest X-ray classification using DenseNet-121 trained on the 
Stanford CheXpert dataset. Mean AUC: 0.8649

## Results

**Mean AUC-ROC: 0.8649** across 13 pathology conditions

| Condition | AUC-ROC |
|---|---|
| Pleural Other | 0.9742 |
| Support Devices | 0.9380 |
| Pleural Effusion | 0.9391 |
| Edema | 0.9186 |
| Lung Lesion | 0.9270 |
| Lung Opacity | 0.9059 |
| Consolidation | 0.8936 |
| Pneumothorax | 0.8789 |
| No Finding | 0.8716 |
| Cardiomegaly | 0.8148 |
| Atelectasis | 0.8060 |
| Pneumonia | 0.7113 |
| Enlarged Cardiomediastinum | 0.6647 |

## Dataset

Stanford CheXpert v1.0-small — 223,414 chest X-rays labeled for 14 conditions.

## Model

- Architecture: DenseNet-121 pretrained on ImageNet
- Fine-tuned for multi-label classification (14 conditions)
- Loss function: Binary Cross Entropy with Logits
- Optimizer: Adam (lr=1e-4)
- Epochs: 3
- Framework: PyTorch

## Training Environment

- Platform: Kaggle Notebooks
- GPU: T4 x2
- Training time: ~2 hours
