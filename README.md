# finetuning-transformers

- `bert-base-uncased` : part of feedback prize 3.0 kaggle competition
  - huggingface pretrained autoModel and autoTokenizer
  - from scratch pytorch trainer
  - optimizer with weight decay as recommended by huggingface
  - unfreezed encoder block: full finetuning
  - multiple scheduler support: CosineAnnealingWarmRestarts, StepLR, ReduceLROnPlateau
  - GPU Memory consumption on average (with dataset): 12.6 GB
